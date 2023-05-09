# Comparing `tmp/azure-core-tracing-opencensus-1.0.0b8.zip` & `tmp/azure-core-tracing-opencensus-1.0.0b9.zip`

## zipinfo {}

```diff
@@ -1,31 +1,34 @@
-Zip file size: 18820 bytes, number of entries: 29
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure/
--rw-rw-r--  2.0 unx      596 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/CHANGELOG.md
--rw-rw-r--  2.0 unx     2482 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/setup.py
--rw-rw-r--  2.0 unx     2648 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/README.md
--rw-rw-r--  2.0 unx      214 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/MANIFEST.in
--rw-rw-r--  2.0 unx       67 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/setup.cfg
--rw-rw-r--  2.0 unx     4948 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/PKG-INFO
--rw-rw-r--  2.0 unx     2552 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/tests/tracing_common.py
--rw-rw-r--  2.0 unx    10814 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/tests/test_tracing_implementations.py
--rw-rw-r--  2.0 unx      887 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/tests/test_threading.py
--rw-rw-r--  2.0 unx        1 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx      129 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      664 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     4948 b- defN 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure/core/
--rw-rw-r--  2.0 unx       81 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/
--rw-rw-r--  2.0 unx       81 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/azure/core/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/
--rw-rw-r--  2.0 unx       81 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-01 17:21 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/
--rw-rw-r--  2.0 unx       81 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/__init__.py
--rw-rw-r--  2.0 unx    11186 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/__init__.py
--rw-rw-r--  2.0 unx      172 b- defN 21-Jul-01 17:19 azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/_version.py
-29 files, 42639 bytes uncompressed, 12798 bytes compressed:  70.0%
+Zip file size: 20384 bytes, number of entries: 32
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/tests/
+-rw-rw-r--  2.0 unx     4425 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/PKG-INFO
+-rw-rw-r--  2.0 unx     2468 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/setup.py
+-rw-rw-r--  2.0 unx      285 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/MANIFEST.in
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/LICENSE
+-rw-rw-r--  2.0 unx     2649 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/README.md
+-rw-rw-r--  2.0 unx      850 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/CHANGELOG.md
+-rw-rw-r--  2.0 unx       98 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/pyproject.toml
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/setup.cfg
+-rw-rw-r--  2.0 unx     4425 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       97 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/requires.txt
+-rw-rw-r--  2.0 unx      725 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/top_level.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure/core/
+-rw-rw-r--  2.0 unx       81 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/
+-rw-rw-r--  2.0 unx       81 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/core/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/
+-rw-rw-r--  2.0 unx       81 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-09 20:40 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/
+-rw-rw-r--  2.0 unx       81 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/__init__.py
+-rw-rw-r--  2.0 unx    11124 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/py.typed
+-rw-rw-r--  2.0 unx      172 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/_version.py
+-rw-rw-r--  2.0 unx      855 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/tests/test_threading.py
+-rw-rw-r--  2.0 unx     2550 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/tests/tracing_common.py
+-rw-rw-r--  2.0 unx    10783 b- defN 23-May-09 20:39 azure-core-tracing-opencensus-1.0.0b9/tests/test_tracing_implementations.py
+32 files, 42949 bytes uncompressed, 13770 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -1,88 +1,97 @@
-Filename: azure-core-tracing-opencensus-1.0.0b8/
+Filename: azure-core-tracing-opencensus-1.0.0b9/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/tests/
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/
+Filename: azure-core-tracing-opencensus-1.0.0b9/tests/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/CHANGELOG.md
+Filename: azure-core-tracing-opencensus-1.0.0b9/PKG-INFO
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/setup.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/setup.py
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/README.md
+Filename: azure-core-tracing-opencensus-1.0.0b9/MANIFEST.in
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/MANIFEST.in
+Filename: azure-core-tracing-opencensus-1.0.0b9/LICENSE
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/setup.cfg
+Filename: azure-core-tracing-opencensus-1.0.0b9/README.md
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/PKG-INFO
+Filename: azure-core-tracing-opencensus-1.0.0b9/CHANGELOG.md
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/tests/tracing_common.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/pyproject.toml
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/tests/test_tracing_implementations.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/setup.cfg
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/tests/test_threading.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/not-zip-safe
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/requires.txt
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/top_level.txt
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/requires.txt
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/SOURCES.txt
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/dependency_links.txt
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/PKG-INFO
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/__init__.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/__init__.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/__init__.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/__init__.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/__init__.py
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/__init__.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/py.typed
 Comment: 
 
-Filename: azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/_version.py
+Filename: azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/_version.py
+Comment: 
+
+Filename: azure-core-tracing-opencensus-1.0.0b9/tests/test_threading.py
+Comment: 
+
+Filename: azure-core-tracing-opencensus-1.0.0b9/tests/tracing_common.py
+Comment: 
+
+Filename: azure-core-tracing-opencensus-1.0.0b9/tests/test_tracing_implementations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/README.md` & `azure-core-tracing-opencensus-1.0.0b9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 exporter = AzureExporter(
     instrumentation_key="uuid of the instrumentation key (see your Azure Monitor account)"
 )
 
 tracer = Tracer(exporter=exporter, sampler=AlwaysOnSampler())
 with tracer.span(name="MyApplication") as span:
     client = BlobServiceClient.from_connection_string('connectionstring')
-    client.delete_container('mycontainer')  # Call will be traced
+    client.delete_container('my_container')  # Call will be traced
 ```
 
 
 ## Troubleshooting
 
 This client raises exceptions defined in [Azure Core](https://docs.microsoft.com/python/api/azure-core/azure.core.exceptions?view=azure-python).
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/PKG-INFO` & `azure-core-tracing-opencensus-1.0.0b9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,125 @@
 Metadata-Version: 2.1
 Name: azure-core-tracing-opencensus
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Microsoft Azure Azure Core Opencensus plugin Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opencensus
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: 
-        
-        # Azure Core Tracing OpenCensus client library for Python
-        
-        ## Getting started
-        
-        Install the opencensus python for Python with [pip](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install azure-core-tracing-opencensus --pre
-        ```
-        
-        Now you can use opencensus for Python as usual with any SDKs that is compatible
-        with azure-core tracing. This includes (not exhaustive list), azure-storage-blob, azure-keyvault-secrets, azure-eventhub, etc.
-        
-        ## Key concepts
-        
-        * You don't need to pass any context, SDK will get it for you
-        * The opencensus threading plugin is installed with this package
-        
-        ## Examples
-        
-        There is no explicit context to pass, you just create your usual opencensus and tracer and
-        call any SDK code that is compatible with azure-core tracing. This is an example
-        using Azure Monitor exporter, but you can use any exporter (Zipkin, etc.).
-        
-        ```python
-        from opencensus.ext.azure.trace_exporter import AzureExporter
-        
-        from opencensus.trace.tracer import Tracer
-        from opencensus.trace.samplers import AlwaysOnSampler
-        
-        from azure.storage.blob import BlobServiceClient
-        
-        exporter = AzureExporter(
-            instrumentation_key="uuid of the instrumentation key (see your Azure Monitor account)"
-        )
-        
-        tracer = Tracer(exporter=exporter, sampler=AlwaysOnSampler())
-        with tracer.span(name="MyApplication") as span:
-            client = BlobServiceClient.from_connection_string('connectionstring')
-            client.delete_container('mycontainer')  # Call will be traced
-        ```
-        
-        
-        ## Troubleshooting
-        
-        This client raises exceptions defined in [Azure Core](https://docs.microsoft.com/python/api/azure-core/azure.core.exceptions?view=azure-python).
-        
-        
-        ## Next steps
-        
-        More documentation on OpenCensus configuration can be found on the [OpenCensus website](https://opencensus.io)
-        
-        
-        ## Contributing
-        This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.
-        
-        When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
-        
-        This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
-        
-        
-        
-        # Release History
-        
-        ## 1.0.0b8 (2021-07-01)
-        
-        - Fix for supporting `kind` keyword while instantiating the span.
-        
-        ## 1.0.0b7 (2021-04-08)
-        
-        - `Link` and `SpanKind` can now be added while creating the span instance.
-        
-        ## 1.0.0b6 (2020-05-04)
-        
-        - `link` and `link_from_headers` now accept attributes.
-        
-        ## 1.0.0b5 (2019-01-14)
-        
-        ### Bugfix
-        
-        - Fix context passing for multi-threading
-        - Don't fail on unknown span type, but maps to PRODUCER or UNSPECIFIED
-        
-        ### Features
-        
-        - Implement new "change_context" API
-        
-        ## 1.0.0b4 (2019-10-07)
-        
-        ### Features
-        
-        - Opencensus implementation of azure-core tracing protocol
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+# Azure Core Tracing OpenCensus client library for Python
+
+## Getting started
+
+Install the opencensus python for Python with [pip](https://pypi.org/project/pip/):
+
+```bash
+pip install azure-core-tracing-opencensus --pre
+```
+
+Now you can use opencensus for Python as usual with any SDKs that is compatible
+with azure-core tracing. This includes (not exhaustive list), azure-storage-blob, azure-keyvault-secrets, azure-eventhub, etc.
+
+## Key concepts
+
+* You don't need to pass any context, SDK will get it for you
+* The opencensus threading plugin is installed with this package
+
+## Examples
+
+There is no explicit context to pass, you just create your usual opencensus and tracer and
+call any SDK code that is compatible with azure-core tracing. This is an example
+using Azure Monitor exporter, but you can use any exporter (Zipkin, etc.).
+
+```python
+from opencensus.ext.azure.trace_exporter import AzureExporter
+
+from opencensus.trace.tracer import Tracer
+from opencensus.trace.samplers import AlwaysOnSampler
+
+from azure.storage.blob import BlobServiceClient
+
+exporter = AzureExporter(
+    instrumentation_key="uuid of the instrumentation key (see your Azure Monitor account)"
+)
+
+tracer = Tracer(exporter=exporter, sampler=AlwaysOnSampler())
+with tracer.span(name="MyApplication") as span:
+    client = BlobServiceClient.from_connection_string('connectionstring')
+    client.delete_container('my_container')  # Call will be traced
+```
+
+
+## Troubleshooting
+
+This client raises exceptions defined in [Azure Core](https://docs.microsoft.com/python/api/azure-core/azure.core.exceptions?view=azure-python).
+
+
+## Next steps
+
+More documentation on OpenCensus configuration can be found on the [OpenCensus website](https://opencensus.io)
+
+
+## Contributing
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.
+
+When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+
+
+# Release History
+
+## 1.0.0b9 (2023-05-09)
+
+### Bugs Fixed
+
+- Fixed a bug where starting a span would fail if an unexpected keyword argument was passed in to `OpenCensusSpan`.
+
+### Other Changes
+
+- Python 2.7 is no longer supported. Please use Python version 3.7 or later.
+
+## 1.0.0b8 (2021-07-01)
+
+- Fix for supporting `kind` keyword while instantiating the span.
+
+## 1.0.0b7 (2021-04-08)
+
+- `Link` and `SpanKind` can now be added while creating the span instance.
+
+## 1.0.0b6 (2020-05-04)
+
+- `link` and `link_from_headers` now accept attributes.
+
+## 1.0.0b5 (2020-01-14)
+
+### Bugfix
+
+- Fix context passing for multi-threading
+- Don't fail on unknown span type, but maps to PRODUCER or UNSPECIFIED
+
+### Features
+
+- Implement new "change_context" API
+
+## 1.0.0b4 (2019-10-07)
+
+### Features
+
+- Opencensus implementation of azure-core tracing protocol
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/tests/tracing_common.py` & `azure-core-tracing-opencensus-1.0.0b9/tests/tracing_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 
 class MockExporter(Exporter):
     def __init__(self):
         self.root = None  # type: SpanData
         self._all_nodes = []
         self.parent_dict = defaultdict(list)
 
-    def export(self, span_datas):
+    def export(self, span_data):
         # type: (List[SpanData]) -> None
-        sp = span_datas[0]  # type: SpanData
+        sp = span_data[0]  # type: SpanData
         node = Node(sp)
         if not node.span_data.parent_span_id:
             self.root = node
         parent_span_id = node.span_data.parent_span_id
         self.parent_dict[parent_span_id].append(node)
         self._all_nodes.append(node)
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/tests/test_tracing_implementations.py` & `azure-core-tracing-opencensus-1.0.0b9/tests/test_tracing_implementations.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from opencensus.trace.samplers import AlwaysOnSampler
 from opencensus.trace.base_exporter import Exporter
 from tracing_common import MockExporter, ContextHelper
 import os
 
 import pytest
 
+
 class TestOpencensusWrapper(unittest.TestCase):
     def test_span_passed_in(self):
         with ContextHelper():
             tracer = tracer_module.Tracer(sampler=AlwaysOnSampler())
             with tracer.start_span(name="parent") as parent:
                 wrapped_span = OpenCensusSpan(parent)
             assert wrapped_span.span_instance.name == "parent"
@@ -137,43 +138,40 @@
             assert wrapped_class.kind == SpanKind.CLIENT
 
     def test_passing_links_in_ctor(self):
         with ContextHelper() as ctx:
             trace = tracer_module.Tracer(sampler=AlwaysOnSampler())
             parent = trace.start_span()
             wrapped_class = OpenCensusSpan(
-                links=[Link(
-                    headers= {"traceparent": "00-2578531519ed94423ceae67588eff2c9-231ebdc614cb9ddd-01"}
-                    )
-                ]
+                links=[Link(headers={"traceparent": "00-2578531519ed94423ceae67588eff2c9-231ebdc614cb9ddd-01"})]
             )
             assert len(wrapped_class.span_instance.links) == 1
             link = wrapped_class.span_instance.links[0]
             assert link.trace_id == "2578531519ed94423ceae67588eff2c9"
             assert link.span_id == "231ebdc614cb9ddd"
 
     def test_passing_links_in_ctor_with_attr(self):
         attributes = {"attr1": 1}
         with ContextHelper() as ctx:
             trace = tracer_module.Tracer(sampler=AlwaysOnSampler())
             parent = trace.start_span()
             wrapped_class = OpenCensusSpan(
-                links=[Link(
-                    headers= {"traceparent": "00-2578531519ed94423ceae67588eff2c9-231ebdc614cb9ddd-01"},
-                    attributes=attributes
+                links=[
+                    Link(
+                        headers={"traceparent": "00-2578531519ed94423ceae67588eff2c9-231ebdc614cb9ddd-01"},
+                        attributes=attributes,
                     )
                 ]
             )
             assert len(wrapped_class.span_instance.links) == 1
             link = wrapped_class.span_instance.links[0]
             assert link.attributes is not None
             assert link.trace_id == "2578531519ed94423ceae67588eff2c9"
             assert link.span_id == "231ebdc614cb9ddd"
 
-
     def test_set_http_attributes(self):
         with ContextHelper():
             trace = tracer_module.Tracer(sampler=AlwaysOnSampler())
             parent = trace.start_span()
             wrapped_class = OpenCensusSpan(span=parent)
             request = mock.Mock()
             setattr(request, "method", "GET")
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/tests/test_threading.py` & `azure-core-tracing-opencensus-1.0.0b9/tests/test_threading.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 
 from azure.core.tracing.ext.opencensus_span import OpenCensusSpan
 
 
 def test_get_span_from_thread():
 
     result = []
+
     def get_span_from_thread(output):
         current_span = OpenCensusSpan.get_current_span()
         output.append(current_span)
 
     tracer = Tracer(sampler=AlwaysOnSampler())
     with tracer.span(name="TestSpan") as span:
 
-        thread = threading.Thread(
-            target=get_span_from_thread,
-            args=(result,)
-        )
+        thread = threading.Thread(target=get_span_from_thread, args=(result,))
         thread.start()
         thread.join()
 
         assert span is result[0]
 
-    execution_context.clear()
+    execution_context.clear()
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/SOURCES.txt` & `azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/core/__init__.py
 azure/core/tracing/__init__.py
 azure/core/tracing/ext/__init__.py
 azure/core/tracing/ext/opencensus_span/__init__.py
 azure/core/tracing/ext/opencensus_span/_version.py
+azure/core/tracing/ext/opencensus_span/py.typed
 azure_core_tracing_opencensus.egg-info/PKG-INFO
 azure_core_tracing_opencensus.egg-info/SOURCES.txt
 azure_core_tracing_opencensus.egg-info/dependency_links.txt
 azure_core_tracing_opencensus.egg-info/not-zip-safe
 azure_core_tracing_opencensus.egg-info/requires.txt
 azure_core_tracing_opencensus.egg-info/top_level.txt
 tests/test_threading.py
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/azure_core_tracing_opencensus.egg-info/PKG-INFO` & `azure-core-tracing-opencensus-1.0.0b9/azure_core_tracing_opencensus.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,125 @@
 Metadata-Version: 2.1
 Name: azure-core-tracing-opencensus
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Microsoft Azure Azure Core Opencensus plugin Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opencensus
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: 
-        
-        # Azure Core Tracing OpenCensus client library for Python
-        
-        ## Getting started
-        
-        Install the opencensus python for Python with [pip](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install azure-core-tracing-opencensus --pre
-        ```
-        
-        Now you can use opencensus for Python as usual with any SDKs that is compatible
-        with azure-core tracing. This includes (not exhaustive list), azure-storage-blob, azure-keyvault-secrets, azure-eventhub, etc.
-        
-        ## Key concepts
-        
-        * You don't need to pass any context, SDK will get it for you
-        * The opencensus threading plugin is installed with this package
-        
-        ## Examples
-        
-        There is no explicit context to pass, you just create your usual opencensus and tracer and
-        call any SDK code that is compatible with azure-core tracing. This is an example
-        using Azure Monitor exporter, but you can use any exporter (Zipkin, etc.).
-        
-        ```python
-        from opencensus.ext.azure.trace_exporter import AzureExporter
-        
-        from opencensus.trace.tracer import Tracer
-        from opencensus.trace.samplers import AlwaysOnSampler
-        
-        from azure.storage.blob import BlobServiceClient
-        
-        exporter = AzureExporter(
-            instrumentation_key="uuid of the instrumentation key (see your Azure Monitor account)"
-        )
-        
-        tracer = Tracer(exporter=exporter, sampler=AlwaysOnSampler())
-        with tracer.span(name="MyApplication") as span:
-            client = BlobServiceClient.from_connection_string('connectionstring')
-            client.delete_container('mycontainer')  # Call will be traced
-        ```
-        
-        
-        ## Troubleshooting
-        
-        This client raises exceptions defined in [Azure Core](https://docs.microsoft.com/python/api/azure-core/azure.core.exceptions?view=azure-python).
-        
-        
-        ## Next steps
-        
-        More documentation on OpenCensus configuration can be found on the [OpenCensus website](https://opencensus.io)
-        
-        
-        ## Contributing
-        This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.
-        
-        When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
-        
-        This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
-        
-        
-        
-        # Release History
-        
-        ## 1.0.0b8 (2021-07-01)
-        
-        - Fix for supporting `kind` keyword while instantiating the span.
-        
-        ## 1.0.0b7 (2021-04-08)
-        
-        - `Link` and `SpanKind` can now be added while creating the span instance.
-        
-        ## 1.0.0b6 (2020-05-04)
-        
-        - `link` and `link_from_headers` now accept attributes.
-        
-        ## 1.0.0b5 (2019-01-14)
-        
-        ### Bugfix
-        
-        - Fix context passing for multi-threading
-        - Don't fail on unknown span type, but maps to PRODUCER or UNSPECIFIED
-        
-        ### Features
-        
-        - Implement new "change_context" API
-        
-        ## 1.0.0b4 (2019-10-07)
-        
-        ### Features
-        
-        - Opencensus implementation of azure-core tracing protocol
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+# Azure Core Tracing OpenCensus client library for Python
+
+## Getting started
+
+Install the opencensus python for Python with [pip](https://pypi.org/project/pip/):
+
+```bash
+pip install azure-core-tracing-opencensus --pre
+```
+
+Now you can use opencensus for Python as usual with any SDKs that is compatible
+with azure-core tracing. This includes (not exhaustive list), azure-storage-blob, azure-keyvault-secrets, azure-eventhub, etc.
+
+## Key concepts
+
+* You don't need to pass any context, SDK will get it for you
+* The opencensus threading plugin is installed with this package
+
+## Examples
+
+There is no explicit context to pass, you just create your usual opencensus and tracer and
+call any SDK code that is compatible with azure-core tracing. This is an example
+using Azure Monitor exporter, but you can use any exporter (Zipkin, etc.).
+
+```python
+from opencensus.ext.azure.trace_exporter import AzureExporter
+
+from opencensus.trace.tracer import Tracer
+from opencensus.trace.samplers import AlwaysOnSampler
+
+from azure.storage.blob import BlobServiceClient
+
+exporter = AzureExporter(
+    instrumentation_key="uuid of the instrumentation key (see your Azure Monitor account)"
+)
+
+tracer = Tracer(exporter=exporter, sampler=AlwaysOnSampler())
+with tracer.span(name="MyApplication") as span:
+    client = BlobServiceClient.from_connection_string('connectionstring')
+    client.delete_container('my_container')  # Call will be traced
+```
+
+
+## Troubleshooting
+
+This client raises exceptions defined in [Azure Core](https://docs.microsoft.com/python/api/azure-core/azure.core.exceptions?view=azure-python).
+
+
+## Next steps
+
+More documentation on OpenCensus configuration can be found on the [OpenCensus website](https://opencensus.io)
+
+
+## Contributing
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.
+
+When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+
+
+# Release History
+
+## 1.0.0b9 (2023-05-09)
+
+### Bugs Fixed
+
+- Fixed a bug where starting a span would fail if an unexpected keyword argument was passed in to `OpenCensusSpan`.
+
+### Other Changes
+
+- Python 2.7 is no longer supported. Please use Python version 3.7 or later.
+
+## 1.0.0b8 (2021-07-01)
+
+- Fix for supporting `kind` keyword while instantiating the span.
+
+## 1.0.0b7 (2021-04-08)
+
+- `Link` and `SpanKind` can now be added while creating the span instance.
+
+## 1.0.0b6 (2020-05-04)
+
+- `link` and `link_from_headers` now accept attributes.
+
+## 1.0.0b5 (2020-01-14)
+
+### Bugfix
+
+- Fix context passing for multi-threading
+- Don't fail on unknown span type, but maps to PRODUCER or UNSPECIFIED
+
+### Features
+
+- Implement new "change_context" API
+
+## 1.0.0b4 (2019-10-07)
+
+### Features
+
+- Opencensus implementation of azure-core tracing protocol
```

## Comparing `azure-core-tracing-opencensus-1.0.0b8/azure/core/tracing/ext/opencensus_span/__init__.py` & `azure-core-tracing-opencensus-1.0.0b9/azure/core/tracing/ext/opencensus_span/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 except ImportError:
     TYPE_CHECKING = False
 
 if TYPE_CHECKING:
     from typing import Dict, Optional, Union, Callable, Sequence, Any
 
     from azure.core.pipeline.transport import HttpRequest, HttpResponse
+
     AttributeValue = Union[
         str,
         bool,
         int,
         float,
         Sequence[str],
         Sequence[bool],
@@ -36,15 +37,15 @@
         Sequence[float],
     ]
     Attributes = Optional[Dict[str, AttributeValue]]
 
 
 __version__ = VERSION
 
-_config_integration.trace_integrations(['threading'])
+_config_integration.trace_integrations(["threading"])
 
 
 class OpenCensusSpan(HttpSpanMixin, object):
     """Wraps a given OpenCensus Span so that it implements azure.core.tracing.AbstractSpan"""
 
     def __init__(self, span=None, name="span", **kwargs):
         # type: (Optional[Span], Optional[str], Any) -> None
@@ -57,42 +58,45 @@
         :param name: The name of the OpenCensus span to create if a new span is needed
         :type name: str
         :keyword SpanKind kind: The span kind of this span.
         :keyword links: The list of links to be added to the span.
         :paramtype links: list[~azure.core.tracing.Link]
         """
         tracer = self.get_current_tracer()
-        value = kwargs.pop('kind', None)
+        value = kwargs.pop("kind", None)
         kind = (
-            OpenCensusSpanKind.CLIENT if value == SpanKind.CLIENT else
-            OpenCensusSpanKind.CLIENT if value == SpanKind.PRODUCER else # No producer in opencensus
-            OpenCensusSpanKind.SERVER if value == SpanKind.SERVER else
-            OpenCensusSpanKind.CLIENT if value == SpanKind.CONSUMER else # No consumer in opencensus
-            OpenCensusSpanKind.UNSPECIFIED if value == SpanKind.INTERNAL else # No internal in opencensus
-            OpenCensusSpanKind.UNSPECIFIED if value == SpanKind.UNSPECIFIED else
-            None
-        ) # type: SpanKind
+            OpenCensusSpanKind.CLIENT
+            if value == SpanKind.CLIENT
+            else OpenCensusSpanKind.CLIENT
+            if value == SpanKind.PRODUCER
+            else OpenCensusSpanKind.SERVER  # No producer in opencensus
+            if value == SpanKind.SERVER
+            else OpenCensusSpanKind.CLIENT
+            if value == SpanKind.CONSUMER
+            else OpenCensusSpanKind.UNSPECIFIED  # No consumer in opencensus
+            if value == SpanKind.INTERNAL
+            else OpenCensusSpanKind.UNSPECIFIED  # No internal in opencensus
+            if value == SpanKind.UNSPECIFIED
+            else None
+        )  # type: SpanKind
         if value and kind is None:
             raise ValueError("Kind {} is not supported in OpenCensus".format(value))
 
-        links = kwargs.pop('links', None)
-        self._span_instance = span or tracer.start_span(name=name, **kwargs)
+        links = kwargs.pop("links", None)
+        self._span_instance = span or tracer.start_span(name=name)
         if kind is not None:
             self._span_instance.span_kind = kind
 
         if links:
             try:
                 for link in links:
                     ctx = trace_context_http_header_format.TraceContextPropagator().from_headers(link.headers)
                     self._span_instance.add_link(
-                        Link(
-                            trace_id=ctx.trace_id,
-                            span_id=ctx.span_id,
-                            attributes=link.attributes
-                        ))
+                        Link(trace_id=ctx.trace_id, span_id=ctx.span_id, attributes=link.attributes)
+                    )
             except AttributeError:
                 # we will just send the links as is if it's not ~azure.core.tracing.Link without any validation
                 # assuming user knows what they are doing.
                 self._span_instance.links = links
 
     @property
     def span_instance(self):
@@ -117,18 +121,21 @@
 
     @property
     def kind(self):
         # type: () -> Optional[SpanKind]
         """Get the span kind of this span."""
         value = self.span_instance.span_kind
         return (
-            SpanKind.CLIENT if value == OpenCensusSpanKind.CLIENT else
-            SpanKind.SERVER if value == OpenCensusSpanKind.SERVER else
-            SpanKind.UNSPECIFIED if value == OpenCensusSpanKind.UNSPECIFIED else
-            None
+            SpanKind.CLIENT
+            if value == OpenCensusSpanKind.CLIENT
+            else SpanKind.SERVER
+            if value == OpenCensusSpanKind.SERVER
+            else SpanKind.UNSPECIFIED
+            if value == OpenCensusSpanKind.UNSPECIFIED
+            else None
         )
 
     _KIND_MAPPING = {
         SpanKind.CLIENT: OpenCensusSpanKind.CLIENT,
         SpanKind.PRODUCER: OpenCensusSpanKind.CLIENT,  # No producer in opencensus
         SpanKind.SERVER: OpenCensusSpanKind.SERVER,
         SpanKind.CONSUMER: OpenCensusSpanKind.CLIENT,  # No consumer in opencensus
@@ -167,15 +174,15 @@
     def to_header(self):
         # type: () -> Dict[str, str]
         """
         Returns a dictionary with the header labels and values.
         :return: A key value pair dictionary
         """
         tracer_from_context = self.get_current_tracer()
-        temp_headers = {} # type: Dict[str, str]
+        temp_headers = {}  # type: Dict[str, str]
         if tracer_from_context is not None:
             ctx = tracer_from_context.span_context
             try:
                 temp_headers = tracer_from_context.propagator.to_headers(ctx)
             except AttributeError:
                 pass
         return temp_headers
@@ -201,45 +208,39 @@
         base16(trace-id) = 4bf92f3577b34da6a3ce929d0e0e4736
         base16(parent-id) = 00f067aa0ba902b7
         base16(trace-flags) = 01  // sampled
 
         :return: a traceparent string
         :rtype: str
         """
-        return self.to_header()['traceparent']
+        return self.to_header()["traceparent"]
 
     @classmethod
     def link(cls, traceparent, attributes=None):
         # type: (str, Attributes) -> None
         """
         Links the context to the current tracer.
 
         :param traceparent: A complete traceparent
         :type traceparent: str
         """
-        cls.link_from_headers({
-            'traceparent': traceparent
-        }, attributes)
+        cls.link_from_headers({"traceparent": traceparent}, attributes)
 
     @classmethod
     def link_from_headers(cls, headers, attributes=None):
         # type: (Dict[str, str], Attributes) -> None
         """
         Given a dictionary, extracts the context and links the context to the current tracer.
 
         :param headers: A key value pair dictionary
         :type headers: dict
         """
         ctx = trace_context_http_header_format.TraceContextPropagator().from_headers(headers)
         current_span = cls.get_current_span()
-        current_span.add_link(Link(
-            trace_id=ctx.trace_id,
-            span_id=ctx.span_id,
-            attributes=attributes
-        ))
+        current_span.add_link(Link(trace_id=ctx.trace_id, span_id=ctx.span_id, attributes=attributes))
 
     @classmethod
     def get_current_span(cls):
         # type: () -> Span
         """
         Get the current span from the execution context. Return None otherwise.
         """
@@ -264,16 +265,15 @@
         """
         warnings.warn("set_current_span is deprecated, use change_context instead", DeprecationWarning)
         return execution_context.set_current_span(span)
 
     @classmethod
     def change_context(cls, span):
         # type: (Span) -> ContextManager
-        """Change the context for the life of this context manager.
-        """
+        """Change the context for the life of this context manager."""
         original_span = cls.get_current_span()
         try:
             execution_context.set_current_span(span)
             yield
         finally:
             execution_context.set_current_span(original_span)
```

