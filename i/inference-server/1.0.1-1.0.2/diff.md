# Comparing `tmp/inference-server-1.0.1.tar.gz` & `tmp/inference-server-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-server-1.0.1.tar", last modified: Tue May  9 11:26:38 2023, max compression
+gzip compressed data, was "inference-server-1.0.2.tar", last modified: Wed May 10 12:39:26 2023, max compression
```

## Comparing `inference-server-1.0.1.tar` & `inference-server-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 11:26:23.000000 inference-server-1.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-09 11:26:23.000000 inference-server-1.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.759274 inference-server-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.763274 inference-server-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 11:26:23.000000 inference-server-1.0.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-09 11:26:23.000000 inference-server-1.0.1/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-09 11:26:23.000000 inference-server-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-09 11:26:23.000000 inference-server-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-09 11:26:23.000000 inference-server-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-09 11:26:23.000000 inference-server-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-09 11:26:23.000000 inference-server-1.0.1/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-09 11:26:38.767274 inference-server-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-09 11:26:23.000000 inference-server-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.763274 inference-server-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/inference_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 11:26:23.000000 inference-server-1.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-09 11:26:23.000000 inference-server-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:26:38.767274 inference-server-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.759274 inference-server-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/src/inference_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/default_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-09 11:26:23.000000 inference-server-1.0.1/src/inference_server/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/src/inference_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 11:26:38.000000 inference-server-1.0.1/src/inference_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:26:38.767274 inference-server-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-09 11:26:23.000000 inference-server-1.0.1/tests/test_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-09 11:26:23.000000 inference-server-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 12:39:11.000000 inference-server-1.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-10 12:39:11.000000 inference-server-1.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.048981 inference-server-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.048981 inference-server-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 12:39:11.000000 inference-server-1.0.2/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 12:39:11.000000 inference-server-1.0.2/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-10 12:39:11.000000 inference-server-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-10 12:39:11.000000 inference-server-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 12:39:11.000000 inference-server-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-10 12:39:11.000000 inference-server-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-10 12:39:11.000000 inference-server-1.0.2/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-10 12:39:26.052981 inference-server-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-10 12:39:11.000000 inference-server-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/inference_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/inference_server_testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-10 12:39:11.000000 inference-server-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:39:26.052981 inference-server-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.048981 inference-server-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/src/inference_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/default_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/src/inference_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-10 12:39:11.000000 inference-server-1.0.2/tests/test_inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-10 12:39:11.000000 inference-server-1.0.2/tox.ini
```

### Comparing `inference-server-1.0.1/.flake8` & `inference-server-1.0.2/.flake8`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/.github/workflows/release-package.yml` & `inference-server-1.0.2/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/.github/workflows/test-package.yml` & `inference-server-1.0.2/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/.gitignore` & `inference-server-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/.pre-commit-config.yaml` & `inference-server-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/.readthedocs.yaml` & `inference-server-1.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/LICENSE` & `inference-server-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/LICENSE_HEADER.txt` & `inference-server-1.0.2/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/PKG-INFO` & `inference-server-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.1
+Version: 1.0.2
 Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.0.1/README.md` & `inference-server-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/docs/conf.py` & `inference-server-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/docs/deployment.rst` & `inference-server-1.0.2/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/docs/hooks.rst` & `inference-server-1.0.2/docs/hooks.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. currentmodule:: inference_server._plugin
 
 Implementing server hooks
 =========================
 
-This pages explains how to implement the **inference-server** hooks to deploy a model to Amazon SageMaker.
+This page explains how to implement the **inference-server** hooks to deploy a model to Amazon SageMaker.
 
 
 Hook definitions
 ----------------
 
 **inference-server** defines 4 hooks that can be implemented to deploy a model as a SageMaker Docker container:
```

### Comparing `inference-server-1.0.1/docs/introduction.rst` & `inference-server-1.0.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/pyproject.toml` & `inference-server-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/src/inference_server/__init__.py` & `inference-server-1.0.2/src/inference_server/__init__.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/src/inference_server/_plugin.py` & `inference-server-1.0.2/src/inference_server/_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/src/inference_server/default_plugin.py` & `inference-server-1.0.2/src/inference_server/default_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/src/inference_server/testing.py` & `inference-server-1.0.2/src/inference_server/testing.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,49 +6,75 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 """
-Public functions for testing plugins
+Functions for testing **inference-server** plugins
 """
 
 from types import ModuleType
 from typing import Callable, Type, Union
 
 import pluggy
 import werkzeug.test
 
 import inference_server
 import inference_server._plugin
 
 
 def client() -> werkzeug.test.Client:
-    """Return an HTTP test client for :mod:`inference_server`"""
+    """
+    Return an HTTP test client for :mod:`inference_server`
+
+    The test client is simply a :class:`werkzeug.test.Client` instance which loads the **inference-server** WSGI app.
+    Consult the :mod:`werkzeug` documentation for details how to use the test client.
+    """
     return werkzeug.test.Client(inference_server.create_app())
 
 
 def post_invocations(**kwargs) -> werkzeug.test.TestResponse:
-    """Send an HTTP POST request to ``/invocations`` using a test HTTP client"""
+    """
+    Send an HTTP POST request to ``/invocations`` using a test HTTP client and return the response
+
+    This function should be used to verify an inference request using the full **inference-server** logic.
+
+    :param kwargs: Keyword arguments passed to :meth:`werkzeug.test.Client.post`
+    """
     response = client().post("/invocations", **kwargs)
     assert response.status_code == 200
     return response
 
 
 def plugin_manager() -> pluggy.PluginManager:
-    """Return the plugin manager"""
+    """Return the plugin manager used by **inference-server**"""
     return inference_server._plugin.manager()
 
 
 def plugin_is_registered(plugin: Union[Type, ModuleType]) -> bool:
-    """Return whether the given plugin is registered with :mod:`inference_server`"""
+    """
+    Return whether the given plugin is registered with :mod:`inference_server`
+
+    This validates whether a plugin entrypoint is defined in :file:`pyproject.toml` like this:
+
+    .. code-block:: toml
+
+       [project.entry-points.inference_server]
+       my_plugin_name = "my_module_name"
+
+    :param plugin: The plugin, typically a module containg the hook functions.
+    """
     return plugin_manager().is_registered(plugin)
 
 
 def hookimpl_is_valid(function: Callable) -> bool:
-    """Return whether the given function is a valid implementation of a :mod:`inference_server` hook"""
+    """
+    Return whether the given function is a valid implementation of an :mod:`inference_server` hook
+
+    :param function: The hook function to validate
+    """
     try:
         hook = getattr(plugin_manager().hook, function.__name__)
     except AttributeError:
         return False
     return function in (impl.function for impl in hook.get_hookimpls())
```

### Comparing `inference-server-1.0.1/src/inference_server.egg-info/PKG-INFO` & `inference-server-1.0.2/src/inference_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.1
+Version: 1.0.2
 Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.0.1/src/inference_server.egg-info/SOURCES.txt` & `inference-server-1.0.2/src/inference_server.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 .github/workflows/release-package.yml
 .github/workflows/test-package.yml
 docs/conf.py
 docs/deployment.rst
 docs/hooks.rst
 docs/index.rst
 docs/inference_server.rst
+docs/inference_server_testing.rst
 docs/introduction.rst
 docs/modules.rst
+docs/testing.rst
 src/inference_server/__init__.py
 src/inference_server/_plugin.py
 src/inference_server/default_plugin.py
 src/inference_server/py.typed
 src/inference_server/testing.py
 src/inference_server.egg-info/PKG-INFO
 src/inference_server.egg-info/SOURCES.txt
```

### Comparing `inference-server-1.0.1/tests/test_inference_server.py` & `inference-server-1.0.2/tests/test_inference_server.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.1/tox.ini` & `inference-server-1.0.2/tox.ini`

 * *Files identical despite different names*

