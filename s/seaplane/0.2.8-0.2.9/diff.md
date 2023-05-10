# Comparing `tmp/seaplane-0.2.8.tar.gz` & `tmp/seaplane-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.2.8.tar", max compression
+gzip compressed data, was "seaplane-0.2.9.tar", max compression
```

## Comparing `seaplane-0.2.8.tar` & `seaplane-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,58 @@
--rw-r--r--   0        0        0     1538 2023-03-15 11:58:02.676710 seaplane-0.2.8/README.md
--rw-r--r--   0        0        0     2452 2023-04-21 13:58:45.731596 seaplane-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      925 2023-04-14 09:20:58.225652 seaplane-0.2.8/src/seaplane/__init__.py
--rw-r--r--   0        0        0       84 2023-03-15 11:58:02.678488 seaplane-0.2.8/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-03-15 11:58:02.678632 seaplane-0.2.8/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2018 2023-04-07 11:43:45.946207 seaplane-0.2.8/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     2987 2023-04-07 11:43:45.946514 seaplane-0.2.8/src/seaplane/api/compute_api.py
--rw-r--r--   0        0        0     3158 2023-03-15 11:58:02.679076 seaplane-0.2.8/src/seaplane/api/formation_configuration_api.py
--rw-r--r--   0        0        0     7410 2023-03-15 11:58:02.679237 seaplane-0.2.8/src/seaplane/api/lock_api.py
--rw-r--r--   0        0        0     5806 2023-03-15 11:58:02.679378 seaplane-0.2.8/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     7724 2023-03-15 11:58:02.679515 seaplane-0.2.8/src/seaplane/api/restrict_api.py
--rw-r--r--   0        0        0     1552 2023-04-13 14:15:21.673019 seaplane-0.2.8/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3141 2023-04-06 16:37:27.622223 seaplane-0.2.8/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0     5458 2023-04-07 11:43:45.947048 seaplane-0.2.8/src/seaplane/configuration.py
--rw-r--r--   0        0        0     1830 2023-03-15 11:58:02.680173 seaplane-0.2.8/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      213 2023-04-07 11:43:45.947356 seaplane-0.2.8/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0     1310 2023-04-07 11:43:45.947582 seaplane-0.2.8/src/seaplane/model/compute/__init__.py
--rw-r--r--   0        0        0     1539 2023-03-15 11:58:02.680692 seaplane-0.2.8/src/seaplane/model/compute/formation_configuration.py
--rw-r--r--   0        0        0      129 2023-03-15 11:58:02.680816 seaplane-0.2.8/src/seaplane/model/compute/formation_metadata.py
--rw-r--r--   0        0        0      436 2023-03-15 11:58:02.680940 seaplane-0.2.8/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3077 2023-03-15 11:58:02.681149 seaplane-0.2.8/src/seaplane/model/locks/__init__.py
--rw-r--r--   0        0        0     3560 2023-03-15 11:58:02.681329 seaplane-0.2.8/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      422 2023-03-15 11:58:02.681451 seaplane-0.2.8/src/seaplane/model/provider.py
--rw-r--r--   0        0        0      478 2023-03-15 11:58:02.681578 seaplane-0.2.8/src/seaplane/model/region.py
--rw-r--r--   0        0        0     4221 2023-03-15 11:58:02.681752 seaplane-0.2.8/src/seaplane/model/restrict/__init__.py
--rw-r--r--   0        0        0      530 2023-04-13 14:15:21.673341 seaplane-0.2.8/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0     4111 2023-04-14 15:58:02.667462 seaplane-0.2.8/src/seaplane/smartpipes/__init__.py
--rw-r--r--   0        0        0      424 2023-03-15 11:58:02.681905 seaplane-0.2.8/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-03-15 11:58:02.682026 seaplane-0.2.8/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0     2906 2023-04-21 13:59:45.298425 seaplane-0.2.8/setup.py
--rw-r--r--   0        0        0     2897 2023-04-21 13:59:45.298665 seaplane-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.2.9/README.md
+-rw-r--r--   0        0        0     2501 2023-05-10 15:57:48.922253 seaplane-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      925 2023-05-10 16:07:33.886849 seaplane-0.2.9/src/seaplane/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-10 16:07:33.887055 seaplane-0.2.9/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.2.9/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2558 2023-05-10 16:07:33.887328 seaplane-0.2.9/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     2987 2023-05-10 16:07:33.887468 seaplane-0.2.9/src/seaplane/api/compute_api.py
+-rw-r--r--   0        0        0     3158 2023-05-10 16:07:33.887602 seaplane-0.2.9/src/seaplane/api/formation_configuration_api.py
+-rw-r--r--   0        0        0     7410 2023-05-10 16:07:33.887749 seaplane-0.2.9/src/seaplane/api/lock_api.py
+-rw-r--r--   0        0        0     5806 2023-05-10 16:07:33.887880 seaplane-0.2.9/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     7724 2023-05-10 16:07:33.888017 seaplane-0.2.9/src/seaplane/api/restrict_api.py
+-rw-r--r--   0        0        0     1552 2023-05-10 16:07:33.888145 seaplane-0.2.9/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.2.9/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0     6542 2023-05-10 17:22:48.324154 seaplane-0.2.9/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     1818 2023-05-10 16:07:33.888625 seaplane-0.2.9/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-10 16:07:33.888776 seaplane-0.2.9/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.2.9/src/seaplane/model/compute/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.2.9/src/seaplane/model/compute/formation_configuration.py
+-rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.2.9/src/seaplane/model/compute/formation_metadata.py
+-rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.2.9/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3077 2023-05-10 16:07:33.889518 seaplane-0.2.9/src/seaplane/model/locks/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-10 16:07:33.889686 seaplane-0.2.9/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.2.9/src/seaplane/model/provider.py
+-rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.2.9/src/seaplane/model/region.py
+-rw-r--r--   0        0        0     4221 2023-05-10 16:07:33.890085 seaplane-0.2.9/src/seaplane/model/restrict/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.2.9/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 16:07:33.890455 seaplane-0.2.9/src/seaplane/smartpipes/__init__.py
+-rw-r--r--   0        0        0     6189 2023-05-10 16:07:33.890622 seaplane-0.2.9/src/seaplane/smartpipes/coprocessor.py
+-rw-r--r--   0        0        0     7464 2023-05-10 16:07:33.890798 seaplane-0.2.9/src/seaplane/smartpipes/decorators.py
+-rw-r--r--   0        0        0     1336 2023-05-10 16:07:33.890932 seaplane-0.2.9/src/seaplane/smartpipes/smartapi.py
+-rw-r--r--   0        0        0     1420 2023-05-10 16:07:33.891062 seaplane-0.2.9/src/seaplane/smartpipes/smartpipe.py
+-rw-r--r--   0        0        0       18 2023-05-10 16:07:33.891248 seaplane-0.2.9/src/seaplane/smartpipes/website/.gitignore
+-rw-r--r--   0        0        0     1750 2023-05-10 16:07:33.891373 seaplane-0.2.9/src/seaplane/smartpipes/website/README.md
+-rw-r--r--   0        0        0       77 2023-05-10 16:07:33.891483 seaplane-0.2.9/src/seaplane/smartpipes/website/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-05-10 16:07:33.891598 seaplane-0.2.9/src/seaplane/smartpipes/website/next.config.js
+-rw-r--r--   0        0        0      534 2023-05-10 16:07:33.891723 seaplane-0.2.9/src/seaplane/smartpipes/website/package.json
+-rw-r--r--   0        0        0       82 2023-05-10 16:07:33.891848 seaplane-0.2.9/src/seaplane/smartpipes/website/postcss.config.js
+-rw-r--r--   0        0        0      717 2023-05-10 16:07:33.892035 seaplane-0.2.9/src/seaplane/smartpipes/website/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-05-10 16:07:33.892164 seaplane-0.2.9/src/seaplane/smartpipes/website/public/next.svg
+-rw-r--r--   0        0        0    39147 2023-05-10 16:07:33.892577 seaplane-0.2.9/src/seaplane/smartpipes/website/public/openai.png
+-rw-r--r--   0        0        0    11580 2023-05-10 16:07:33.892822 seaplane-0.2.9/src/seaplane/smartpipes/website/public/seaplane_logo.svg
+-rw-r--r--   0        0        0     2296 2023-05-10 16:07:33.892979 seaplane-0.2.9/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
+-rw-r--r--   0        0        0   195272 2023-05-10 16:07:33.894399 seaplane-0.2.9/src/seaplane/smartpipes/website/public/stabilityai.png
+-rw-r--r--   0        0        0      629 2023-05-10 16:07:33.894546 seaplane-0.2.9/src/seaplane/smartpipes/website/public/vercel.svg
+-rw-r--r--   0        0        0     3691 2023-05-10 16:07:33.894773 seaplane-0.2.9/src/seaplane/smartpipes/website/src/components/Header.jsx
+-rw-r--r--   0        0        0    10990 2023-05-10 16:07:33.894919 seaplane-0.2.9/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
+-rw-r--r--   0        0        0     3400 2023-05-10 16:07:33.895038 seaplane-0.2.9/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
+-rw-r--r--   0        0        0      127 2023-05-10 16:07:33.895187 seaplane-0.2.9/src/seaplane/smartpipes/website/src/pages/_app.js
+-rw-r--r--   0        0        0      231 2023-05-10 16:07:33.895300 seaplane-0.2.9/src/seaplane/smartpipes/website/src/pages/_document.js
+-rw-r--r--   0        0        0     2042 2023-05-10 16:07:33.895412 seaplane-0.2.9/src/seaplane/smartpipes/website/src/pages/index.js
+-rw-r--r--   0        0        0      228 2023-05-10 16:07:33.895550 seaplane-0.2.9/src/seaplane/smartpipes/website/src/styles/globals.css
+-rw-r--r--   0        0        0      480 2023-05-10 16:07:33.895656 seaplane-0.2.9/src/seaplane/smartpipes/website/tailwind.config.js
+-rw-r--r--   0        0        0     1762 2023-05-10 16:07:33.895787 seaplane-0.2.9/src/seaplane/smartpipes/website/yarn-error.log
+-rw-r--r--   0        0        0   110530 2023-05-10 16:07:33.896390 seaplane-0.2.9/src/seaplane/smartpipes/website/yarn.lock
+-rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.2.9/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.2.9/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0     3203 2023-05-10 17:23:47.784655 seaplane-0.2.9/setup.py
+-rw-r--r--   0        0        0     2988 2023-05-10 17:23:47.785200 seaplane-0.2.9/PKG-INFO
```

### Comparing `seaplane-0.2.8/README.md` & `seaplane-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/pyproject.toml` & `seaplane-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.2.8"
+version = "0.2.9"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 
@@ -24,14 +24,16 @@
 tomli = "2.0.1"
 urllib3 = "1.26.9"
 types-requests = "^2.28.0"
 returns = "^0.19.0"
 requests-mock = "^1.9.3"
 simplejson = "^3.17.6"
 types-simplejson = "^3.17.7"
+Flask-Cors = "^3.0.10"
+Flask-SocketIO = "^5.3.4"
 
 [tool.poetry.dev-dependencies]
 nox-poetry = "*"
 
 # Testing.
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `seaplane-0.2.8/src/seaplane/__init__.py` & `seaplane-0.2.9/src/seaplane/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/api_http.py` & `seaplane-0.2.9/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/api_request.py` & `seaplane-0.2.9/src/seaplane/api/api_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,29 @@
 
 from ..logging import log
 from ..model.errors import HTTPError
 from .api_http import SDK_HTTP_ERROR_CODE
 from .token_api import TokenAPI
 
 
+def handle_request(request: Callable[[], Response]) -> Result[Any, HTTPError]:
+    try:
+        response = request()
+
+        if response.ok:
+            return Success(response.json())
+        else:
+            body_error = response.text
+            log.error(f"Request Error: {body_error}")
+            return Failure(HTTPError(response.status_code, body_error))
+    except requests.exceptions.RequestException as err:
+        log.error(f"Request exception: {str(err)}")
+        return Failure(HTTPError(SDK_HTTP_ERROR_CODE, str(err)))
+
+
 def provision_req(
     token_api: TokenAPI,
 ) -> Callable[[Callable[[str], Response]], Result[Any, HTTPError]]:
     """
     Before every request, we make sure we use a valid access token.
     """
```

### Comparing `seaplane-0.2.8/src/seaplane/api/compute_api.py` & `seaplane-0.2.9/src/seaplane/api/compute_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/formation_configuration_api.py` & `seaplane-0.2.9/src/seaplane/api/formation_configuration_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/lock_api.py` & `seaplane-0.2.9/src/seaplane/api/lock_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/metadata_api.py` & `seaplane-0.2.9/src/seaplane/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/restrict_api.py` & `seaplane-0.2.9/src/seaplane/api/restrict_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/sql_api.py` & `seaplane-0.2.9/src/seaplane/api/sql_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/api/token_api.py` & `seaplane-0.2.9/src/seaplane/api/token_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/configuration.py` & `seaplane-0.2.9/src/seaplane/configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 from .api.token_api import TokenAPI
 from .logging import log
+from .model.errors import SeaplaneError
 
 _SEAPLANE_COMPUTE_API_ENDPOINT = "https://compute.cplane.cloud/v2beta"
 _SEAPLANE_COORDINATION_API_ENDPOINT = "https://metadata.cplane.cloud/v1"
 _SEAPLANE_IDENTIFY_API_ENDPOINT = "https://flightdeck.cplane.cloud/v1"
 _SEAPLANE_GLOBAL_SQL_API_ENDPOINT = "https://sql.cplane.cloud/v1"
 
 
@@ -21,14 +22,15 @@
         self.seaplane_api_key: Optional[str] = None
         self.identify_endpoint = _SEAPLANE_IDENTIFY_API_ENDPOINT
         self.compute_endpoint = _SEAPLANE_COMPUTE_API_ENDPOINT
         self.coordination_endpoint = _SEAPLANE_COORDINATION_API_ENDPOINT
         self.global_sql_endpoint = _SEAPLANE_GLOBAL_SQL_API_ENDPOINT
         self._current_access_token: Optional[str] = None
         self._token_auto_renew = True
+        self._api_keys: Optional[str] = None
         self._update_token_api()
 
     def set_api_key(self, api_key: str) -> None:
         """Set the Seaplane API Key.
 
         The API Key is needed for the Seaplane Python SDK usage.
 
@@ -36,14 +38,49 @@
         ----------
         api_key : str
             Seaplane API Key.
         """
         self.seaplane_api_key = api_key
         self._update_token_api()
 
+    def set_api_keys(self, api_keys: object) -> None:
+        """Set the Seaplane API Keys for SmartPipes.
+
+        The API Keys is needed for some of the Coprocessors.
+
+        Supported Coprocessors API Keys:
+
+        Seaplane: SEA_API_KEY
+        Open AI: OPENAI_API_KEY
+        Replicate: RE_API_KEY
+
+        For example, for use an OpenAI Coprocessor,
+        you need to provide the Key - Value, of the API Key.
+
+            $ from seaplane import sea
+
+            $ api_keys = {"OPENAI_API_KEY": "sp-api-key-test" }
+            $ sea.config.set_api_keys(api_keys)
+
+        Parameters
+        ----------
+        api_keys : object
+            API Keys and values.
+        """
+        self._api_keys = api_keys
+
+        if api_keys is None:
+            raise SeaplaneError(
+                "api_keys parameters can't be None"
+            )
+        elif api_keys.get("SEA_API_KEY", None) is not None:
+            self.seaplane_api_key = api_keys["SEA_API_KEY"]
+
+        self._update_token_api()
+
     def set_token(self, access_token: Optional[str]) -> None:
         """Set a valid Seaplane Token globally.
 
         The access token will be persisted even if any configuration changes.
 
         Setting the token, will change auto-renew to False
         needing to renew the token manually when the token expires.
```

### Comparing `seaplane-0.2.8/src/seaplane/logging/__init__.py` & `seaplane-0.2.9/src/seaplane/logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class SeaLogger:
     """
     Seaplane Logger container module, which uses Python logger.
     """
 
     PREFIX = "[Seaplane] "
-    FORMAT = "%(asctime)s [Seaplane] %(message)s"
+    FORMAT = "[Seaplane] %(message)s"
 
     CRITICAL = logging.CRITICAL
     FATAL = logging.FATAL
     ERROR = logging.ERROR
     WARNING = logging.WARNING
     WARN = logging.WARN
     INFO = logging.INFO
```

### Comparing `seaplane-0.2.8/src/seaplane/model/compute/__init__.py` & `seaplane-0.2.9/src/seaplane/model/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/model/compute/formation_configuration.py` & `seaplane-0.2.9/src/seaplane/model/compute/formation_configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/model/locks/__init__.py` & `seaplane-0.2.9/src/seaplane/model/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/model/metadata/__init__.py` & `seaplane-0.2.9/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/model/restrict/__init__.py` & `seaplane-0.2.9/src/seaplane/model/restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/src/seaplane/model/sql/__init__.py` & `seaplane-0.2.9/src/seaplane/model/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.2.8/setup.py` & `seaplane-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,18 +14,25 @@
  'seaplane.model.metadata',
  'seaplane.model.restrict',
  'seaplane.model.sql',
  'seaplane.smartpipes',
  'seaplane.util']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'seaplane.smartpipes': ['website/*',
+                         'website/public/*',
+                         'website/src/components/*',
+                         'website/src/pages/*',
+                         'website/src/styles/*']}
 
 install_requires = \
-['attrs==21.4.0',
+['Flask-Cors>=3.0.10,<4.0.0',
+ 'Flask-SocketIO>=5.3.4,<6.0.0',
+ 'attrs==21.4.0',
  'certifi==2022.6.15',
  'charset-normalizer==2.1.0',
  'idna==3.3',
  'iniconfig==1.1.1',
  'packaging==21.3',
  'pluggy==1.0.0',
  'py==1.11.0',
@@ -37,15 +44,15 @@
  'tomli==2.0.1',
  'types-requests>=2.28.0,<3.0.0',
  'types-simplejson>=3.17.7,<4.0.0',
  'urllib3==1.26.9']
 
 setup_kwargs = {
     'name': 'seaplane',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Seaplane Python SDK',
     'long_description': '# Seaplane Python SDK\n[![PyPI](https://badge.fury.io/py/seaplane.svg)](https://badge.fury.io/py/seaplane)\n[![Python](https://img.shields.io/pypi/pyversions/seaplane.svg?style=plastic)](https://badge.fury.io/py/seaplane)\n\nSimple Python library to manage your resources at seaplane.\n\n## What is Seaplane?\n\nSeaplane is the global platform for building and scaling your application stack\nwithout the complexity of managing cloud infrastructure.\n\nIt serves as a reference application for how our APIs can be utilized.\n\nNot sure where to go to quickly run a workload on Seaplane? See our [Getting\nStarted] guide.\n\nTo build and test this software yourself, see the CONTRIBUTING document that is a peer to this one.\n\n## Installation\n\n```shell\npip install seaplane\n```\n\n## Configure your API KEY\n\n* Set `SEAPLANE_API_KEY` environment variable.\n* Use `config` object in order to set the api key.\n\n```python\nfrom seaplane import sea\n\nsea.config.set_api_key("your_api_key")\n```\n\n## License\n\nLicensed under the Apache License, Version 2.0, [LICENSE]. Copyright 2022 Seaplane IO, Inc.\n\n[//]: # (Links)\n\n[Seaplane]: https://seaplane.io/\n[CLI]: https://github.com/seaplane-io/seaplane/tree/main/seaplane-cli\n[SDK]: https://github.com/seaplane-io/seaplane/tree/main/seaplane\n[Getting Started]: https://github.com/seaplane-io/seaplane/blob/main/seaplane-sdk/python/docs/quickstart.md\n[CONTRIBUTING]: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python/CONTRIBUTIONS.md\n[LICENSE]: https://github.com/seaplane-io/seaplane/blob/main/LICENSE\n',
     'author': 'Seaplane IO, Inc.',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python',
```

### Comparing `seaplane-0.2.8/PKG-INFO` & `seaplane-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.2.8
+Version: 0.2.9
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
+Requires-Dist: Flask-SocketIO (>=5.3.4,<6.0.0)
 Requires-Dist: attrs (==21.4.0)
 Requires-Dist: certifi (==2022.6.15)
 Requires-Dist: charset-normalizer (==2.1.0)
 Requires-Dist: idna (==3.3)
 Requires-Dist: iniconfig (==1.1.1)
 Requires-Dist: packaging (==21.3)
 Requires-Dist: pluggy (==1.0.0)
```

