# Comparing `tmp/aiosow-0.1.2.tar.gz` & `tmp/aiosow-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.2.tar", last modified: Tue May  2 11:13:50 2023, max compression
+gzip compressed data, was "aiosow-0.1.3.tar", last modified: Wed May 10 14:55:49 2023, max compression
```

## Comparing `aiosow-0.1.2.tar` & `aiosow-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8293 2023-05-02 11:13:50.315181 aiosow-0.1.2/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8115 2023-04-27 12:46:26.000000 aiosow-0.1.2/README.md
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/aiosow/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       34 2023-03-22 07:46:41.000000 aiosow-0.1.2/aiosow/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4471 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/autofill.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13356 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/bindings.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2898 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/command.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1974 2023-03-24 08:23:50.000000 aiosow-0.1.2/aiosow/http.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      827 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/options.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4014 2023-05-02 11:11:02.000000 aiosow-0.1.2/aiosow/perpetuate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3629 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/routines.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1427 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      373 2023-04-26 12:14:34.000000 aiosow-0.1.2/aiosow/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/aiosow.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8293 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      555 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       46 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/entry_points.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       69 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/top_level.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-02 11:13:50.315181 aiosow-0.1.2/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      688 2023-05-02 11:12:19.000000 aiosow-0.1.2/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/tests/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3253 2023-03-25 11:26:27.000000 aiosow-0.1.2/tests/test_autofill.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7291 2023-04-27 12:46:26.000000 aiosow-0.1.2/tests/test_bindings.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-03-22 07:46:41.000000 aiosow-0.1.2/tests/test_command.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      185 2023-03-22 07:46:41.000000 aiosow-0.1.2/tests/test_http.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      864 2023-03-25 11:37:11.000000 aiosow-0.1.2/tests/test_perpetuate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1938 2023-04-27 12:46:26.000000 aiosow-0.1.2/tests/test_routines.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      653 2023-03-25 11:26:15.000000 aiosow-0.1.2/tests/test_setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      725 2023-03-22 07:46:41.000000 aiosow-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.790653 aiosow-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-10 14:55:49.790653 aiosow-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-10 14:55:38.000000 aiosow-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.786653 aiosow-0.1.3/aiosow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-10 14:55:38.000000 aiosow-0.1.3/aiosow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.790653 aiosow-0.1.3/aiosow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 14:55:49.000000 aiosow-0.1.3/aiosow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:55:49.790653 aiosow-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-10 14:55:38.000000 aiosow-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:49.790653 aiosow-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 14:55:38.000000 aiosow-0.1.3/tests/test_setup.py
```

### Comparing `aiosow-0.1.2/aiosow/autofill.py` & `aiosow-0.1.3/aiosow/autofill.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 await function(*args, **memory) -> this doesn't work because :
     - it is not generic and will break whenever a function doesn't take **kwargs
     - kwargs itself is a copy and will break reference
 """
 from typing import Any, Callable, List
+from types import LambdaType
 
-import inspect, logging
+import inspect, logging, asyncio
 
 ALIASES = {}
 
 
 def get_aliases():  # pragma: no cover
     global ALIASES
     return ALIASES
@@ -44,15 +45,15 @@
     def decorator(function: Callable):
         ALIASES[name] = function
         return function
 
     return decorator
 
 
-async def autofill(function: Callable, args: Any = [], **kwargs) -> Any:
+async def fill_prototype(function: Callable, args: Any = [], **kwargs) -> Any:
     """
     The autofill function takes a callable function, args, and memory as input
     arguments, and returns the result of calling the function with autofilled
     arguments.
 
     **Args**:
     - function (Callable): The function to be called with autofilled arguments.
@@ -110,17 +111,51 @@
         ]
         given_args = [arg for arg in given_args if arg != Sentinel]
         has_varargs = any(
             param.kind == inspect.Parameter.VAR_POSITIONAL
             for param in inspect.signature(function).parameters.values()
         )
         given_args = given_args if not has_varargs else given_args + list(argscopy)
+    return (name, given_args, kws)
+
+
+async def autofill(function: Callable, args: Any = [], **kwargs) -> Any:
+    name, given_args, kws = await fill_prototype(function, args=args, **kwargs)
     try:
+        if kwargs.get("memory", {}).get("log_autofill", False):
+            if name == "<lambda>":
+                name = (
+                    inspect.getsource(function)
+                    .replace("\n", "")
+                    .replace("\t", "")
+                    .replace("    ", "")
+                )
+            logging.info(f" -> {name}")
         result = function(*given_args, **kws)
         return await result if inspect.iscoroutine(result) else result
     except Exception as err:  # pragma: no cover
         logging.error(f"{name} : {err}")
         logging.debug(f" > error generated by calling {name}({given_args})")
         raise (err)  # `debug` needs `autofill` to raise
 
 
-__all__ = ["alias", "autofill"]
+def make_async(function: Callable) -> Callable:
+    """
+    Make a synchronous function run in it's own thread
+    using `run_in_executor`.
+
+    **args**:
+    - function: Callable
+
+    **returns**:
+    - Async Callable
+    """
+
+    async def wrapper(*args, **kwargs):
+        loop = asyncio.get_event_loop()
+        __name__, given_args, kws = await fill_prototype(function, args=args, **kwargs)
+        return await loop.run_in_executor(None, function, *given_args, **kws)
+
+    return wrapper
+
+
+__all__ = ["alias", "autofill", "make_async"]
```

### Comparing `aiosow-0.1.2/aiosow/bindings.py` & `aiosow-0.1.3/aiosow/bindings.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pdb as _pdb
 import asyncio
 import time
 import inspect
 
 from functools import wraps
 
-from aiosow.autofill import autofill, alias
+from aiosow.autofill import autofill, alias, make_async
 from aiosow.options import option
 from aiosow.perpetuate import on, perpetuate
 from aiosow.setup import setup
 
 
 def chain(*functions):
     """Applies functions iteratively and pass each result to next function"""
@@ -48,15 +48,15 @@
                     await asyncio.sleep(delay)
 
         return call
 
     return retry_until_success
 
 
-def wire(perpetual=False, pass_args=True) -> Tuple[Callable, Callable]:
+def wire(condition=None, perpetual=False, pass_args=True) -> Tuple[Callable, Callable]:
     """
     Returns a tuple of two decorators: `trigger_decorator` and `listen_decorator`.
 
     The `trigger_decorator` decorator wraps an async function and triggers it,
     calling any functions registered  with the `listen_decorator` decorator. The
     `listen_decorator` decorator registers a function to be called whenever a
     function decorated with `trigger_decorator` is called.
@@ -114,15 +114,17 @@
     caster = autofill if not perpetual else perpetuate
 
     def trigger_decorator(triggerer):
         @wraps(triggerer)
         async def call(*args, **kwargs):
             result = await autofill(triggerer, args=args, **kwargs)
             # if triggerer is a generator we need to iterate over it
-            if result:
+            if result and (
+                await autofill(condition, args=[], **kwargs) if condition else True
+            ):
                 if inspect.isgenerator(result):
                     tasks = []
                     for val in result:
                         tasks += [
                             asyncio.create_task(
                                 caster(func, args=[val] if pass_args else [], **kwargs)
                             )
@@ -453,33 +455,14 @@
     ```
     function_to_debug = debug(pdb)(function_to_debug)
     ```
     """
     _pdb.set_trace()
 
 
-def make_async(function: Callable) -> Callable:
-    """
-    Make a synchronous function run in it's own thread
-    using `run_in_executor`.
-
-    **args**:
-    - function: Callable
-
-    **returns**:
-    - Async Callable
-    """
-
-    async def wrapper(*args, **kwargs):
-        loop = asyncio.get_event_loop()
-        return await loop.run_in_executor(None, function, (args, kwargs))
-
-    return wrapper
-
-
 __all__ = [
     "alias",
     "accumulator",
     "autofill",
     "delay",
     "debug",
     "each",
```

### Comparing `aiosow-0.1.2/aiosow/command.py` & `aiosow-0.1.3/aiosow/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,26 @@
             level=logging.DEBUG if debug else logging.INFO,
             format="[%(asctime)s][%(levelname)s] \t%(message)s",
             datefmt="%H:%M:%S",
         )
     parser = argparse.ArgumentParser()
     if not composition:
         parser.add_argument("composition", help="composition to run")
-    parser.add_argument(
-        "-c", "--config", help="Path to configuration file", default="", type=str
-    )
+    # parser.add_argument(
+    #    "-c", "--config", help="Path to configuration file", default="", type=str
+    # )
     parser.add_argument(
         "-d", "--debug", default=False, action="store_true", help="Debug mode"
     )
     parser.add_argument(
         "-la",
         "--log_autofill",
         default=False,
         action="store_true",
-        help="Log.debug every autofill arguments",
+        help="Log.info autofilled functions",
     )
     parser.add_argument(
         "--raise",
         default=False,
         action="store_true",
         help="Routines will raise errors and stop the execution",
     )
@@ -63,14 +63,15 @@
 
 def run(composition=None):
     memory = load_composition(composition=composition)
     logging.debug(memory)
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     tasks = loop.run_until_complete(initialize(memory))
+    memory["running"] = True
     logging.info("--------------------------------")
     logging.info("----------SETUP--DONE-----------")
     logging.info("--------------------------------")
     consumer = loop.run_until_complete(spawn_routine_consumer(memory))
     tasks = tasks + [consumer]
     # setups can return a task which is ran here
     # this allows setups to start tasks and still have them complete
```

### Comparing `aiosow-0.1.2/aiosow/options.py` & `aiosow-0.1.3/aiosow/options.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.2/aiosow/perpetuate.py` & `aiosow-0.1.3/aiosow/perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.2/aiosow/routines.py` & `aiosow-0.1.3/aiosow/routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             try:
                 if await autofill(condition, args=[], memory=memory):
                     if routine["perpetuate"]:
                         await perpetuate(function, args=[], memory=memory)
                     else:
                         await autofill(function, args=[], memory=memory)
             except Exception as err:
+                logging.error(err)
                 if memory.get("raise", False):
                     raise (err)
             # Update the timeout value based on the frequency
             if routine["frequency"] > 0:
                 routine["timeout"] = routine["frequency"]
             else:
                 routines.remove(routine)
```

### Comparing `aiosow-0.1.2/aiosow/setup.py` & `aiosow-0.1.3/aiosow/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 
     **Args**:
     - func (Callable): Function to add to the list of initialization functions.
 
     **Returns**:
     - func (Callable): The same function, unchanged.
     """
-    logging.info("+ setup %s", func.__name__)
-    SETUP_FUNCTIONS.append(func)
+    if func in SETUP_FUNCTIONS:
+        logging.debug("duplicate setup declaration of %s is ignored", func.__name__)
+    else:
+        logging.info("+ setup %s", func.__name__)
+        SETUP_FUNCTIONS.append(func)
     return func
 
 
 async def initialize(memory: Dict) -> List[asyncio.Task]:
     """
     Function that runs all initialization functions added to the list.
```

### Comparing `aiosow-0.1.2/setup.py` & `aiosow-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="aiosow",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(include=["aiosow"]),
     description="An event-based framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     entry_points={
         "console_scripts": [
```

### Comparing `aiosow-0.1.2/tests/test_autofill.py` & `aiosow-0.1.3/tests/test_autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.2/tests/test_bindings.py` & `aiosow-0.1.3/tests/test_bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time
+import time, asyncio
 import pytest
 from aiosow.bindings import (
     expect,
     do_raise,
     dont_raise,
     return_true,
     return_false,
@@ -170,17 +170,14 @@
     async def raises():
         raise Exception("error")
 
     await raises()
     assert mock_listener.call_count == 1
 
 
-import time, asyncio
-
-
 @pytest.mark.asyncio
 async def test_make_async():
     @make_async
     def wait(*__args__):
         time.sleep(0.2)
         return "foo"
 
@@ -188,14 +185,24 @@
     results = await asyncio.gather(wait(), wait(), wait())
     end_time = time.monotonic()
     assert results == ["foo", "foo", "foo"]
     assert end_time - start_time < (0.3)
 
 
 @pytest.mark.asyncio
+async def test_make_async_parameters():
+    @make_async
+    def wait(arg):
+        return arg * 2
+
+    results = await asyncio.gather(wait(2, memory={}))
+    assert results == [4]
+
+
+@pytest.mark.asyncio
 async def test_chain():
     def add(x):
         return x + 1
 
     def mul(x):
         return x * 2
```

### Comparing `aiosow-0.1.2/tests/test_perpetuate.py` & `aiosow-0.1.3/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.2/tests/test_routines.py` & `aiosow-0.1.3/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.2/tests/test_setup.py` & `aiosow-0.1.3/tests/test_setup.py`

 * *Files identical despite different names*

