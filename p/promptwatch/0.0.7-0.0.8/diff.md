# Comparing `tmp/promptwatch-0.0.7.tar.gz` & `tmp/promptwatch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.7.tar", last modified: Sun May  7 09:56:19 2023, max compression
+gzip compressed data, was "promptwatch-0.0.8.tar", last modified: Wed May 10 08:33:26 2023, max compression
```

## Comparing `promptwatch-0.0.7.tar` & `promptwatch-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.950408 promptwatch-0.0.7/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-07 09:56:19.950230 promptwatch-0.0.7/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.7/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.7/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-07 09:56:19.950457 promptwatch-0.0.7/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.7/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.945527 promptwatch-0.0.7/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.948462 promptwatch-0.0.7/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-07 09:54:30.000000 promptwatch-0.0.7/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 21:26:09.000000 promptwatch-0.0.7/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.7/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.7/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-07 09:39:06.000000 promptwatch-0.0.7/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.949971 promptwatch-0.0.7/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.7/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    34257 2023-05-07 09:37:59.000000 promptwatch-0.0.7/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    14375 2023-05-06 13:44:12.000000 promptwatch-0.0.7/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.7/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.949491 promptwatch-0.0.7/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.7/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.401004 promptwatch-0.0.8/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-10 08:33:26.400827 promptwatch-0.0.8/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.8/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.8/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-10 08:33:26.401050 promptwatch-0.0.8/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.8/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.395406 promptwatch-0.0.8/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.397796 promptwatch-0.0.8/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-10 08:33:10.000000 promptwatch-0.0.8/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11922 2023-05-10 08:27:00.000000 promptwatch-0.0.8/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.8/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.8/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-07 09:39:06.000000 promptwatch-0.0.8/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.400402 promptwatch-0.0.8/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.8/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    34257 2023-05-10 08:30:37.000000 promptwatch-0.0.8/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    14278 2023-05-08 08:14:57.000000 promptwatch-0.0.8/src/promptwatch/promptwatch_context.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.8/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-10 08:33:26.399787 promptwatch-0.0.8/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.8/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-10 08:33:26.000000 promptwatch-0.0.8/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.7/PKG-INFO` & `promptwatch-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.7
+Version: 0.0.8
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.7/README.md` & `promptwatch-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/setup.py` & `promptwatch-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/src/promptwatch/caching.py` & `promptwatch-0.0.8/src/promptwatch/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         raise NotImplementedError()
     
     @property
     def should_include_token_usage(self)->bool:
         return False
 
     @abstractmethod
-    def __call__(self, prompt:str, include_token_usage:bool=False) -> Union[List[float], tuple[List[float],int]]:
+    def __call__(self, prompt:str, include_token_usage:bool=False) -> Union[List[float], Tuple[List[float],int]]:
         pass
         
 
 class OpenAIEmbeddingProviderBase(EmbeddingProviderBase):
     def __init__(self, model_name="text-embedding-ada-002", token_limit=8191):
         self._token_limit = token_limit
         self.model_name = model_name
@@ -174,19 +174,21 @@
             token_limit=512
 
         if local:
             self.caches[cache_namespace_key] = PromptWatchCache(cache_namespace_key, LocalImpl(self.promptwatch_context,cache_namespace_key, embed_func), embed_func, token_limit=token_limit, similarity_limit=similarity_limit)
         else:
             self.caches[cache_namespace_key] = PromptWatchCache(cache_namespace_key, RemoteImpl(self.promptwatch_context, cache_namespace_key, embed_func), embed_func, token_limit=token_limit, similarity_limit=similarity_limit)
 
+    
     def get_cache(self, cache_namespace_key=None)->PromptWatchCache:
-        cache_namespace_key=cache_namespace_key or DEFAULT_CACHE_KEY
-        if not cache_namespace_key in self.caches:
-            raise Exception(f"Cache {cache_namespace_key} not initialized")
-        return self.caches[cache_namespace_key]
+        return self.get_or_init_cache(cache_namespace_key=cache_namespace_key)
+        # cache_namespace_key=cache_namespace_key or DEFAULT_CACHE_KEY
+        # if not cache_namespace_key in self.caches:
+        #     raise Exception(f"Cache {cache_namespace_key} not initialized")
+        # return self.caches[cache_namespace_key]
     
     def get_or_init_cache(self, cache_namespace_key:str=None,  embed_func:Callable[[str],List[float]]=None, token_limit=None, similarity_limit=0.97, local:bool=False)->PromptWatchCache:
         cache_namespace_key=cache_namespace_key or DEFAULT_CACHE_KEY
         if not cache_namespace_key in self.caches:
             self.init_cache(cache_namespace_key=cache_namespace_key,  embed_func=embed_func, token_limit=token_limit,  similarity_limit=similarity_limit, local=local)
         return self.caches[cache_namespace_key]
```

### Comparing `promptwatch-0.0.7/src/promptwatch/client.py` & `promptwatch-0.0.8/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/src/promptwatch/data_model.py` & `promptwatch-0.0.8/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/src/promptwatch/decorators.py` & `promptwatch-0.0.8/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.0.8/src/promptwatch/langchain/langchain_support.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/src/promptwatch/promptwatch_context.py` & `promptwatch-0.0.8/src/promptwatch/promptwatch_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
     _thread_local = threading.local()
 
     def __call__(cls, *args, **kwargs):
         """Call method for the singleton metaclass."""
         if not hasattr(ContextTrackerSingleton._thread_local, "_instance"):
             ContextTrackerSingleton._thread_local._instance = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
-        else:
-            ContextTrackerSingleton._thread_local._instance._cached_init_(*args, **kwargs)
+       
         return ContextTrackerSingleton._thread_local._instance 
         
     def get_current():
         if hasattr(ContextTrackerSingleton._thread_local, "_instance"):
             return ContextTrackerSingleton._thread_local._instance
         else:
             return None
```

### Comparing `promptwatch-0.0.7/src/promptwatch/utils.py` & `promptwatch-0.0.8/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.7/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.0.8/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.7
+Version: 0.0.8
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.7/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.0.8/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

