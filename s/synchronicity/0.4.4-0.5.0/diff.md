# Comparing `tmp/synchronicity-0.4.4-py3-none-any.whl.zip` & `tmp/synchronicity-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19907 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       72 b- defN 22-Mar-21 08:08 synchronicity/__init__.py
--rw-rw-r--  2.0 unx     2547 b- defN 23-Apr-24 07:29 synchronicity/async_wrap.py
+Zip file size: 21786 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx      100 b- defN 23-May-10 19:02 synchronicity/__init__.py
+-rw-rw-r--  2.0 unx     2581 b- defN 23-May-10 19:02 synchronicity/async_wrap.py
 -rw-rw-r--  2.0 unx     1485 b- defN 23-Mar-23 14:53 synchronicity/callback.py
 -rw-rw-r--  2.0 unx     1303 b- defN 23-Mar-20 08:05 synchronicity/exceptions.py
--rw-rw-r--  2.0 unx      136 b- defN 23-Mar-29 14:29 synchronicity/interface.py
--rw-rw-r--  2.0 unx     1694 b- defN 23-May-03 14:36 synchronicity/overload_tracking.py
--rw-rw-r--  2.0 unx    25602 b- defN 23-May-03 19:40 synchronicity/synchronizer.py
--rw-rw-r--  2.0 unx    22482 b- defN 23-Apr-24 07:29 synchronicity/type_stubs.py
--rw-rw-r--  2.0 unx     7736 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      997 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/RECORD
-12 files, 64160 bytes uncompressed, 18229 bytes compressed:  71.6%
+-rw-rw-r--  2.0 unx      331 b- defN 23-May-10 19:02 synchronicity/interface.py
+-rw-rw-r--  2.0 unx     1792 b- defN 23-May-10 19:02 synchronicity/overload_tracking.py
+-rw-rw-r--  2.0 unx    30174 b- defN 23-May-10 19:02 synchronicity/synchronizer.py
+-rw-rw-r--  2.0 unx    24842 b- defN 23-May-10 19:02 synchronicity/type_stubs.py
+-rw-rw-r--  2.0 unx     7736 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      998 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/RECORD
+12 files, 71448 bytes uncompressed, 20108 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: synchronicity/synchronizer.py
 Comment: 
 
 Filename: synchronicity/type_stubs.py
 Comment: 
 
-Filename: synchronicity-0.4.4.dist-info/METADATA
+Filename: synchronicity-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: synchronicity-0.4.4.dist-info/WHEEL
+Filename: synchronicity-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: synchronicity-0.4.4.dist-info/top_level.txt
+Filename: synchronicity-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: synchronicity-0.4.4.dist-info/RECORD
+Filename: synchronicity-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synchronicity/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .interface import Interface
-from .synchronizer import Synchronizer
+from .interface import Interface  # noqa: F401
+from .synchronizer import Synchronizer  # noqa: F401
```

## synchronicity/async_wrap.py

```diff
@@ -14,15 +14,18 @@
 
     Use this when the wrapper function is non-async but returns the coroutine resulting
     from calling the underlying wrapped `func`. This will make sure that the wrapper
     is still an async function in that case, and can be inspected as such.
 
     Note: Does not forward async generator information other than explicit annotations
     """
-    if inspect.iscoroutinefunction(func) and interface == Interface.ASYNC:
+    if inspect.iscoroutinefunction(func) and interface in (
+        Interface.ASYNC,
+        Interface._ASYNC_WITH_BLOCKING_TYPES,
+    ):
 
         def asyncfunc_deco(user_wrapper):
             @functools.wraps(func)
             async def wrapper(*args, **kwargs):
                 try:
                     return await user_wrapper(*args, **kwargs)
                 except UserCodeException as uc_exc:
@@ -42,30 +45,27 @@
 def asynccontextmanager(
     f: typing.Callable[..., typing.AsyncGenerator[YIELD_TYPE, SEND_TYPE]]
 ) -> typing.Callable[[], typing.AsyncContextManager[YIELD_TYPE]]:
     """Wrapper around contextlib.asynccontextmanager that sets correct type annotations
 
     The standard library one doesn't
     """
-    acm_factory: typing.Callable[
-        ..., typing.AsyncContextManager[YIELD_TYPE]
-    ] = _asynccontextmanager(f)
+    acm_factory: typing.Callable[..., typing.AsyncContextManager[YIELD_TYPE]] = _asynccontextmanager(f)
 
     old_ret = acm_factory.__annotations__.pop("return", None)
     if old_ret is not None:
         if old_ret.__origin__ in [
             collections.abc.AsyncGenerator,
             collections.abc.AsyncIterator,
             collections.abc.AsyncIterator,
         ]:
-            acm_factory.__annotations__["return"] = typing.AsyncContextManager[
-                old_ret.__args__[0]  # type: ignore
-            ]
+            acm_factory.__annotations__["return"] = typing.AsyncContextManager[old_ret.__args__[0]]  # type: ignore
         elif old_ret.__origin__ == contextlib.AbstractAsyncContextManager:
             # if the standard lib fixes the annotations in the future, lets not break it...
             return acm_factory
     else:
         raise ValueError(
-            "To use the fixed @asynccontextmanager, make sure to properly annotate your wrapped function as an AsyncGenerator"
+            "To use the fixed @asynccontextmanager, make sure to properly"
+            " annotate your wrapped function as an AsyncGenerator"
         )
 
     return acm_factory
```

## synchronicity/interface.py

```diff
@@ -1,7 +1,10 @@
 import enum
 
 
 class Interface(enum.Enum):
     BLOCKING = enum.auto()
     ASYNC = enum.auto()
+    # temporary internal type until we deprecate the old ASYNC type,
+    # used for `function.aio` async callables accepting/returning BLOCKING types
+    _ASYNC_WITH_BLOCKING_TYPES = enum.auto()
     AUTODETECT = enum.auto()  # DEPRECATED
```

## synchronicity/overload_tracking.py

```diff
@@ -11,29 +11,34 @@
         ...
 
     def foo(a: typing.Union[bool, int]) -> typing.Union[bool, float]:
         if isinstance(a, bool):
             return a
         return float(a)
 
-foo_overloads = get_overloads(foo)  # returns reference to the overloads of foo (the int -> float one in this case) in the order they are declared
+# returns reference to the overloads of foo (the int -> float one in this case)
+# in the order they are declared
+foo_overloads = get_overloads(foo)
 """
 import contextlib
 import typing
 from unittest import mock
 
 overloads: typing.Dict[typing.Tuple[str, str], typing.List] = {}
 original_overload = typing.overload
 
 
 class Untrackable(Exception):
     pass
 
 
 def _function_locator(f):
+    if isinstance(f, (staticmethod, classmethod)):
+        return _function_locator(f.__func__)
+
     try:
         return (f.__module__, f.__qualname__)
     except AttributeError:
         raise Untrackable()  # TODO(elias): handle descriptors like classmethod
 
 
 def _tracking_overload(f):
```

## synchronicity/synchronizer.py

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import atexit
+import collections.abc
 import contextlib
 import functools
 import inspect
 import platform
+import sys
 import threading
 import typing
 import warnings
 from typing import Optional
 
 from .async_wrap import wraps_by_interface
 from .callback import Callback
@@ -18,39 +20,129 @@
     "__aiter__": "__iter__",
     "__aenter__": "__enter__",
     "__aexit__": "__exit__",
     "__anext__": "__next__",
 }
 
 IGNORED_ATTRIBUTES = (
-    "__provides__",  # the "zope" lib monkey patches in some non-introspectable stuff on stdlib abc.ABC. Ignoring __provides__ fixes an incompatibility with `channels[daphne]`, where Synchronizer creation fails when wrapping contextlib._AsyncGeneratorContextManager
+    # the "zope" lib monkey patches in some non-introspectable stuff on stdlib abc.ABC.
+    # Ignoring __provides__ fixes an incompatibility with `channels[daphne]`,
+    # where Synchronizer creation fails when wrapping contextlib._AsyncGeneratorContextManager
+    "__provides__",
 )
 
 _RETURN_FUTURE_KWARG = "_future"
 
 # Default names for classes
 _CLASS_PREFIXES = {
     Interface.BLOCKING: "Blocking",
     Interface.ASYNC: "Async",
 }
 
 # Default names for functions
 _FUNCTION_PREFIXES = {
     Interface.BLOCKING: "blocking_",
-    Interface.ASYNC: "async_",
+    Interface.ASYNC: "async_",  # deprecated, will be removed soon!
+    Interface._ASYNC_WITH_BLOCKING_TYPES: "aio_",
 }
 
 TARGET_INTERFACE_ATTR = "_sync_target_interface"
 SYNCHRONIZER_ATTR = "_sync_synchronizer"
 
 
-def warn_old_modal_client():
-    warnings.warn(
-        "Using latest synchronicity with an old interface - please upgrade to latest modal-client!"
-    )
+ASYNC_GENERIC_ORIGINS = (
+    collections.abc.Awaitable,
+    collections.abc.Coroutine,
+    collections.abc.AsyncIterator,
+    collections.abc.AsyncIterable,
+    collections.abc.AsyncGenerator,
+    contextlib.AbstractAsyncContextManager,
+)
+
+
+def _type_requires_aio_usage(annotation, home_module):
+    if isinstance(annotation, str):
+        # evaluate string annotations...
+        # mod = importlib.import_module(home_module)
+        if home_module in sys.modules:
+            mod = sys.modules[home_module]
+            try:
+                annotation = eval(annotation, mod.__dict__)
+            except NameError:
+                # this could happen with forward annotations,
+                # or imports that aren't available in the namespace when synchronicity wrapping occurs
+                # TODO: support eval of non-imported modules?
+                return False
+        else:
+            return False
+
+    if hasattr(annotation, "__origin__"):
+        if annotation.__origin__ in ASYNC_GENERIC_ORIGINS:
+            return True
+        # recurse
+        for a in getattr(annotation, "__args__", ()):
+            if _type_requires_aio_usage(a, home_module):
+                return True
+    return False
+
+
+def should_have_aio_interface(func):
+    # determines if a blocking function gets an .aio attribute with an async interface to the function or not
+    if inspect.iscoroutinefunction(func) or inspect.isasyncgenfunction(func):
+        return True
+    # check annotations if they contain any async entities that would need an event loop to be translated:
+    # This catches things like vanilla functions returning Coroutines
+    annos = getattr(func, "__annotations__", {})
+    for anno in annos.values():
+        if _type_requires_aio_usage(anno, func.__module__):
+            return True
+    return False
+
+
+class FunctionWithAio:
+    def __init__(self, func, aio_func, synchronizer):
+        self._func = func
+        self._aio_func = self.aio = aio_func
+        self._synchronizer = synchronizer
+
+    def __call__(self, *args, **kwargs):
+        # .__call__ is special - it's being looked up on the class instead of the instance when calling something,
+        # so setting the magic method from the constructor is not possible
+        # https://stackoverflow.com/questions/22390532/object-is-not-callable-after-adding-call-method-to-instance
+        # so we need to use an explicit wrapper function here
+        try:
+            return self._func(*args, **kwargs)
+        except UserCodeException as uc_exc:
+            raise uc_exc.exc from None
+
+
+class MethodWithAio:
+    """Creates a bound method that can have callable child-properties on the method itself.
+
+    Child-properties are also bound to the parent instance.
+    """
+
+    def __init__(self, func, aio_func, synchronizer: "Synchronizer", is_classmethod=False):
+        self._func = func
+        self._aio_func = aio_func
+        self._synchronizer = synchronizer
+        self._is_classmethod = is_classmethod
+
+    def __get__(self, instance, owner=None):
+        bind_var = instance if instance and not self._is_classmethod else owner
+
+        bound_func = functools.wraps(self._func)(functools.partial(self._func, bind_var))  # bound blocking function
+        self._synchronizer._update_wrapper(bound_func, self._func, interface=Interface.BLOCKING)
+
+        bound_aio_func = wraps_by_interface(Interface._ASYNC_WITH_BLOCKING_TYPES, self._aio_func)(
+            functools.partial(self._aio_func, bind_var)
+        )  # bound async function
+        self._synchronizer._update_wrapper(bound_func, self._func, interface=Interface._ASYNC_WITH_BLOCKING_TYPES)
+        bound_func.aio = bound_aio_func
+        return bound_func
 
 
 class Synchronizer:
     """Helps you offer a blocking (synchronous) interface to asynchronous code."""
 
     def __init__(
         self,
@@ -156,21 +248,17 @@
         if not self._async_leakage_warning:
             return coro
 
         async def coro_wrapped():
             value = await coro
             # TODO: we should include the name of the original function here
             if inspect.iscoroutine(value):
-                warnings.warn(
-                    f"Potential async leakage: coroutine returned a coroutine {value}."
-                )
+                warnings.warn(f"Potential async leakage: coroutine returned a coroutine {value}.")
             elif inspect.isasyncgen(value):
-                warnings.warn(
-                    f"Potential async leakage: Coroutine returned an async generator {value}."
-                )
+                warnings.warn(f"Potential async leakage: Coroutine returned an async generator {value}.")
             return value
 
         return coro_wrapped()
 
     def _wrap_instance(self, obj, interface):
         # Takes an object and creates a new proxy object for it
         cls = obj.__class__
@@ -193,14 +281,17 @@
                 return obj.__dict__.get(self._original_attr, obj)
             else:
                 return obj.__dict__.get(self._original_attr, obj)
         else:
             return obj
 
     def _translate_scalar_out(self, obj, interface):
+        if interface == Interface._ASYNC_WITH_BLOCKING_TYPES:
+            interface = Interface.BLOCKING
+
         # If it's an internal object, translate it to the external interface
         if inspect.isclass(obj) or isinstance(obj, typing.TypeVar):  # TODO: functions?
             cls_dct = obj.__dict__
             if self._wrapped_attr in cls_dct:
                 return cls_dct[self._wrapped_attr][interface]
             else:
                 return obj
@@ -214,39 +305,33 @@
 
     def _recurse_map(self, mapper, obj):
         if type(obj) == list:
             return list(self._recurse_map(mapper, item) for item in obj)
         elif type(obj) == tuple:
             return tuple(self._recurse_map(mapper, item) for item in obj)
         elif type(obj) == dict:
-            return dict(
-                (key, self._recurse_map(mapper, item)) for key, item in obj.items()
-            )
+            return dict((key, self._recurse_map(mapper, item)) for key, item in obj.items())
         else:
             return mapper(obj)
 
     def _translate_in(self, obj):
         return self._recurse_map(self._translate_scalar_in, obj)
 
     def _translate_out(self, obj, interface):
-        return self._recurse_map(
-            lambda scalar: self._translate_scalar_out(scalar, interface), obj
-        )
+        return self._recurse_map(lambda scalar: self._translate_scalar_out(scalar, interface), obj)
 
     def _translate_coro_out(self, coro, interface):
         async def unwrap_coro():
             return self._translate_out(await coro, interface)
 
         return unwrap_coro()
 
     def _run_function_sync(self, coro, interface):
         if self._is_inside_loop():
-            raise Exception(
-                "Deadlock detected: calling a sync function from the synchronizer loop"
-            )
+            raise Exception("Deadlock detected: calling a sync function from the synchronizer loop")
 
         coro = wrap_coro_exception(coro)
         coro = self._wrap_check_async_leakage(coro)
         loop = self._get_loop(start=True)
         fut = asyncio.run_coroutine_threadsafe(coro, loop)
         value = fut.result()
         return self._translate_out(value, interface)
@@ -309,17 +394,15 @@
             except BaseException as exc:
                 value = exc
                 is_exc = True
 
     def create_callback(self, f, interface):
         return Callback(self, f, interface)
 
-    def _update_wrapper(
-        self, f_wrapped, f, name=None, interface=None, target_module=None
-    ):
+    def _update_wrapper(self, f_wrapped, f, name=None, interface=None, target_module=None):
         """Very similar to functools.update_wrapper"""
         functools.update_wrapper(f_wrapped, f)
         if name is not None:
             f_wrapped.__name__ = name
             f_wrapped.__qualname__ = name
         if target_module is not None:
             f_wrapped.__module__ = target_module
@@ -330,29 +413,25 @@
         self,
         f,
         interface,
         name=None,
         allow_futures=True,
         unwrap_user_excs=True,
         target_module=None,
+        include_aio_interface=True,
     ):
         if hasattr(f, self._original_attr):
             if self._multiwrap_warning:
-                warnings.warn(
-                    f"Function {f} is already wrapped, but getting wrapped again"
-                )
+                warnings.warn(f"Function {f} is already wrapped, but getting wrapped again")
             return f
 
         if name is None:
-            if hasattr(self, "get_name"):
-                # super dumb backwards compatibility fix
-                warn_old_modal_client()
-                name = self.get_name(f, interface)
-            else:
-                name = _FUNCTION_PREFIXES[interface] + f.__name__
+            _name = _FUNCTION_PREFIXES[interface] + f.__name__
+        else:
+            _name = name
 
         is_coroutinefunction = inspect.iscoroutinefunction(f)
 
         @wraps_by_interface(interface, f)
         def f_wrapped(*args, **kwargs):
             return_future = kwargs.pop(_RETURN_FUTURE_KWARG, False)
 
@@ -374,102 +453,134 @@
                 elif is_coroutine:
                     return self._run_function_sync_future(res, interface)
                 elif is_asyncgen:
                     raise Exception("Can not return futures for generators")
                 else:
                     return res
             elif is_coroutine:
-                if interface == Interface.ASYNC:
+                if interface in (Interface.ASYNC, Interface._ASYNC_WITH_BLOCKING_TYPES):
                     coro = self._run_function_async(res, interface)
                     if not is_coroutinefunction:
                         # If this is a non-async function that returns a coroutine,
                         # then this is the exit point, and we need to unwrap any
                         # wrapped exception here. Otherwise, the exit point is
                         # in async_wrap.py
                         coro = unwrap_coro_exception(coro)
                     return coro
                 elif interface == Interface.BLOCKING:
                     # This is the exit point, so we need to unwrap the exception here
                     try:
                         return self._run_function_sync(res, interface)
                     except UserCodeException as uc_exc:
                         # Used to skip a frame when called from `proxy_method`.
-                        if unwrap_user_excs:
+                        if unwrap_user_excs and not (Interface.BLOCKING and include_aio_interface):
                             raise uc_exc.exc from None
                         else:
                             raise uc_exc
             elif is_asyncgen:
                 # Note that the _run_generator_* functions handle their own
                 # unwrapping of exceptions (this happens during yielding)
-                if interface == Interface.ASYNC:
+                if interface in (Interface.ASYNC, Interface._ASYNC_WITH_BLOCKING_TYPES):
                     return self._run_generator_async(res, interface)
                 elif interface == Interface.BLOCKING:
                     return self._run_generator_sync(res, interface)
             else:
-                if inspect.isfunction(res) or isinstance(
-                    res, functools.partial
-                ):  # TODO: HACKY HACK
+                if inspect.isfunction(res) or isinstance(res, functools.partial):  # TODO: HACKY HACK
                     # TODO: this is needed for decorator wrappers that returns functions
                     # Maybe a bit of a hacky special case that deserves its own decorator
                     @wraps_by_interface(interface, res)
                     def f_wrapped(*args, **kwargs):
                         args = self._translate_in(args)
                         kwargs = self._translate_in(kwargs)
                         f_res = res(*args, **kwargs)
                         return self._translate_out(f_res, interface)
 
                     return f_wrapped
 
                 return self._translate_out(res, interface)
 
-        self._update_wrapper(f_wrapped, f, name, interface, target_module=target_module)
+        self._update_wrapper(f_wrapped, f, _name, interface, target_module=target_module)
         setattr(f_wrapped, self._original_attr, f)
+
+        if interface == Interface.BLOCKING and include_aio_interface and should_have_aio_interface(f):
+            # special async interface
+            # this async interface returns *blocking* instances of wrapped objects, not async ones:
+            async_interface = self._wrap_callable(
+                f,
+                interface=Interface._ASYNC_WITH_BLOCKING_TYPES,
+                name=name,
+                allow_futures=allow_futures,
+                unwrap_user_excs=unwrap_user_excs,
+                target_module=target_module,
+            )
+            f_wrapped = FunctionWithAio(f_wrapped, async_interface, self)
+            self._update_wrapper(f_wrapped, f, _name, interface, target_module=target_module)
+            setattr(f_wrapped, self._original_attr, f)
+
         return f_wrapped
 
-    def _wrap_proxy_method(synchronizer_self, method, interface, allow_futures=True):
+    def _wrap_proxy_method(
+        synchronizer_self,
+        method,
+        interface,
+        allow_futures=True,
+        include_aio_interface=True,
+    ):
         if getattr(method, synchronizer_self._nowrap_attr, None):
             # This method is marked as non-wrappable
             return method
 
-        method = synchronizer_self._wrap_callable(
-            method, interface, allow_futures=allow_futures, unwrap_user_excs=False
+        wrapped_method = synchronizer_self._wrap_callable(
+            method,
+            interface,
+            allow_futures=allow_futures,
+            unwrap_user_excs=False,
         )
 
-        @wraps_by_interface(interface, method)
+        @wraps_by_interface(interface, wrapped_method)
         def proxy_method(self, *args, **kwargs):
             instance = self.__dict__[synchronizer_self._original_attr]
             try:
-                return method(instance, *args, **kwargs)
+                return wrapped_method(instance, *args, **kwargs)
             except UserCodeException as uc_exc:
                 raise uc_exc.exc from None
 
+        if interface == Interface.BLOCKING and include_aio_interface and should_have_aio_interface(method):
+            async_proxy_method = synchronizer_self._wrap_proxy_method(
+                method, Interface._ASYNC_WITH_BLOCKING_TYPES, allow_futures
+            )
+            return MethodWithAio(proxy_method, async_proxy_method, synchronizer_self)
+
         return proxy_method
 
     def _wrap_proxy_staticmethod(self, method, interface):
         orig_function = method.__func__
         method = self._wrap_callable(orig_function, interface)
-        self._update_wrapper(method, orig_function, interface=interface)
+        if isinstance(method, FunctionWithAio):
+            return method  # no need to wrap a FunctionWithAio in a staticmethod, as it won't get bound anyways
         return staticmethod(method)
 
-    def _wrap_proxy_classmethod(self, method, interface):
-        method = self._wrap_callable(method.__func__, interface)
-
-        @wraps_by_interface(interface, method)
-        def proxy_classmethod(cls, *args, **kwargs):
-            return method(cls, *args, **kwargs)
+    def _wrap_proxy_classmethod(self, orig_classmethod, interface):
+        orig_func = orig_classmethod.__func__
+        method = self._wrap_callable(orig_func, interface, include_aio_interface=False)
+
+        if interface == Interface.BLOCKING and should_have_aio_interface(orig_func):
+            async_method = self._wrap_callable(orig_func, Interface._ASYNC_WITH_BLOCKING_TYPES)
+            return MethodWithAio(method, async_method, self, is_classmethod=True)
 
-        self._update_wrapper(proxy_classmethod, method, interface=interface)
-        return classmethod(proxy_classmethod)
+        return classmethod(method)
 
     def _wrap_proxy_property(self, prop, interface):
         kwargs = {}
         for attr in ["fget", "fset", "fdel"]:
             if getattr(prop, attr):
                 func = getattr(prop, attr)
-                kwargs[attr] = self._wrap_proxy_method(func, interface, False)
+                kwargs[attr] = self._wrap_proxy_method(
+                    func, interface, allow_futures=False, include_aio_interface=False
+                )
         return property(**kwargs)
 
     def _wrap_proxy_constructor(synchronizer_self, cls, interface):
         """Returns a custom __init__ for the subclass."""
 
         def my_init(self, *args, **kwargs):
             # Create base instance
@@ -486,34 +597,38 @@
 
         synchronizer_self._update_wrapper(my_init, cls.__init__, interface=interface)
         setattr(my_init, synchronizer_self._original_attr, cls.__init__)
         return my_init
 
     def _wrap_class(self, cls, interface, name, target_module=None):
         bases = tuple(
-            self._wrap(base, interface, require_already_wrapped=(name is not None))
-            if base != object
-            else object
+            self._wrap(base, interface, require_already_wrapped=(name is not None)) if base != object else object
             for base in cls.__bases__
         )
         new_dict = {self._original_attr: cls}
         if cls is not None:
             new_dict["__init__"] = self._wrap_proxy_constructor(cls, interface)
 
         for k, v in cls.__dict__.items():
             if k in _BUILTIN_ASYNC_METHODS:
                 k_sync = _BUILTIN_ASYNC_METHODS[k]
                 if interface == Interface.BLOCKING:
                     new_dict[k_sync] = self._wrap_proxy_method(
-                        v, interface, allow_futures=False
+                        v,
+                        interface,
+                        allow_futures=False,
+                        include_aio_interface=False,
                     )
-                if interface == Interface.ASYNC:
                     new_dict[k] = self._wrap_proxy_method(
-                        v, interface, allow_futures=False
+                        v,
+                        Interface._ASYNC_WITH_BLOCKING_TYPES,
+                        allow_futures=False,
                     )
+                elif interface == Interface.ASYNC:
+                    new_dict[k] = self._wrap_proxy_method(v, interface, allow_futures=False)
             elif k in ("__new__", "__init__"):
                 # Skip custom constructor in the wrapped class
                 # Instead, delegate to the base class constructor and wrap it
                 pass
             elif k in IGNORED_ATTRIBUTES:
                 pass
             elif isinstance(v, staticmethod):
@@ -523,20 +638,15 @@
                 new_dict[k] = self._wrap_proxy_classmethod(v, interface)
             elif isinstance(v, property):
                 new_dict[k] = self._wrap_proxy_property(v, interface)
             elif callable(v):
                 new_dict[k] = self._wrap_proxy_method(v, interface)
 
         if name is None:
-            if hasattr(self, "get_name"):
-                # super dumb backwards compatibility fix
-                warn_old_modal_client()
-                name = self.get_name(cls, interface)
-            else:
-                name = _CLASS_PREFIXES[interface] + cls.__name__
+            name = _CLASS_PREFIXES[interface] + cls.__name__
 
         new_cls = type.__new__(type, name, bases, new_dict)
         new_cls.__module__ = cls.__module__ if target_module is None else target_module
         new_cls.__doc__ = cls.__doc__
         if "__annotations__" in cls.__dict__:
             new_cls.__annotations__ = cls.__annotations__  # transfer annotations
 
@@ -564,34 +674,31 @@
                 # This works for classes & functions
                 setattr(obj, self._wrapped_attr, {})
 
         # If this is already wrapped, return the existing interface
         interfaces = obj.__dict__[self._wrapped_attr]
         if interface in interfaces:
             if self._multiwrap_warning:
-                warnings.warn(
-                    f"Object {obj} is already wrapped, but getting wrapped again"
-                )
+                warnings.warn(f"Object {obj} is already wrapped, but getting wrapped again")
             return interfaces[interface]
 
         if require_already_wrapped:
             # This happens if a class has a custom name but its base class doesn't
-            raise RuntimeError(
-                f"{obj} needs to be serialized explicitly with a custom name"
-            )
+            raise RuntimeError(f"{obj} needs to be serialized explicitly with a custom name")
 
         # Wrap object (different cases based on the type)
         if inspect.isclass(obj):
             new_obj = self._wrap_class(
-                obj, interface, name, target_module=target_module
+                obj,
+                interface,
+                name,
+                target_module=target_module,
             )
         elif inspect.isfunction(obj):
-            new_obj = self._wrap_callable(
-                obj, interface, name, target_module=target_module
-            )
+            new_obj = self._wrap_callable(obj, interface, name, target_module=target_module)
         elif isinstance(obj, typing.TypeVar):
             new_obj = self._wrap_type_var(obj, interface, name, target_module)
         elif self._wrapped_attr in obj.__class__.__dict__:
             new_obj = self._wrap_instance(obj, interface)
         else:
             raise Exception("Argument %s is not a class or a callable" % obj)
 
@@ -618,40 +725,20 @@
         return new_obj
 
     def nowrap(self, obj):
         setattr(obj, self._nowrap_attr, True)
         return obj
 
     # New interface that (almost) doesn't mutate objects
-
-    def create_blocking(
-        self, obj, name: Optional[str] = None, target_module: Optional[str] = None
-    ):
+    def create_blocking(self, obj, name: Optional[str] = None, target_module: Optional[str] = None):
         wrapped = self._wrap(obj, Interface.BLOCKING, name, target_module=target_module)
         return wrapped
 
-    def create_async(
-        self, obj, name: Optional[str] = None, target_module: Optional[str] = None
-    ):
+    def create_async(self, obj, name: Optional[str] = None, target_module: Optional[str] = None):
         wrapped = self._wrap(obj, Interface.ASYNC, name, target_module=target_module)
         return wrapped
 
     def is_synchronized(self, obj):
         if inspect.isclass(obj) or inspect.isfunction(obj):
             return hasattr(obj, self._original_attr)
         else:
             return hasattr(obj.__class__, self._original_attr)
-
-    ### DEPRECATED
-    # Only needed because old modal clients don't pin the synchronicity version,
-    # so we need this for backwards compatibility for a short while
-
-    def create(self, obj):
-        warn_old_modal_client()
-        return {
-            Interface.ASYNC: self.create_async(obj),
-            Interface.BLOCKING: self.create_blocking(obj),
-        }
-
-    def __call__(self, obj):
-        warn_old_modal_client()
-        return self.create_blocking(obj)
```

## synchronicity/type_stubs.py

```diff
@@ -1,30 +1,36 @@
 """
 Improvement Ideas:
 * Extract this into its own package, not linked to synchronicity, but with good extension plugs?
-* Don't use the wrapped synchronicity types directly, and instead emit stubs based on the root implementation types directly (but translated to blocking).
+* Don't use the wrapped synchronicity types directly, and instead emit stubs based on the root
+  implementation types directly (but translated to blocking).
 * Let synchronicity emit actual function bodies, to avoid runtime wrapping altogether
 """
 import collections
 import collections.abc
 import contextlib
 import importlib
 import inspect
 import sys
 import typing
 from pathlib import Path
 from typing import TypeVar, Generic
 from unittest import mock
 
 import sigtools.specifiers  # type: ignore
-from sigtools._signatures import EmptyAnnotation, UpgradedAnnotation  # type: ignore
+from sigtools._signatures import EmptyAnnotation, UpgradedAnnotation, UpgradedParameter  # type: ignore
 
 import synchronicity
 from synchronicity import Interface, overload_tracking
-from synchronicity.synchronizer import TARGET_INTERFACE_ATTR, SYNCHRONIZER_ATTR
+from synchronicity.synchronizer import (
+    TARGET_INTERFACE_ATTR,
+    SYNCHRONIZER_ATTR,
+    MethodWithAio,
+    FunctionWithAio,
+)
 
 
 class ReprObj:
     # Hacky repr passthrough object so we can pass verbatim type annotations as partial arguments
     # to generic and have them render correctly through `repr()`, used by inspect.Signature etc.
     def __init__(self, repr: str):
         assert isinstance(repr, str), f"{repr} is not a string!"
@@ -38,14 +44,24 @@
 
     def __call__(self):
         # being a callable gets around some generic's automatic type checking of provided types
         # otherwise we get errors like `provided argument is not a type`
         pass
 
 
+def inject_self(sig: inspect.Signature):
+    parameters = sig.parameters.values()
+    return sig.replace(
+        parameters=[
+            UpgradedParameter("self", inspect.Parameter.POSITIONAL_OR_KEYWORD),
+            *parameters,
+        ]
+    )
+
+
 class StubEmitter:
     def __init__(self, target_module):
         self.target_module = target_module
         self.imports = set()
         self.parts = []
         self._indentation = "    "
         self.global_types = set()
@@ -60,59 +76,59 @@
                 hasattr(entity, "__module__")
                 and entity.__module__ != module.__name__
                 and entity_name not in explicit_members
             ):
                 continue  # skip imported stuff, unless it's explicitly in __all__
             if inspect.isclass(entity):
                 emitter.add_class(entity, entity_name)
-            elif inspect.isfunction(entity):
+            elif inspect.isfunction(entity) or isinstance(entity, FunctionWithAio):
                 emitter.add_function(entity, entity_name, 0)
             elif isinstance(entity, typing.TypeVar):
                 emitter.add_type_var(entity, entity_name)
-            elif (
-                hasattr(entity, "__class__")
-                and getattr(entity.__class__, "__module__", None) == module.__name__
-            ):
+            elif hasattr(entity, "__class__") and getattr(entity.__class__, "__module__", None) == module.__name__:
                 # instances of stuff
                 emitter.add_variable(entity.__class__, entity_name)
 
         for varname, annotation in getattr(module, "__annotations__", {}).items():
             emitter.add_variable(annotation, varname)
 
         return emitter
 
     def add_variable(self, annotation, name):
         # TODO: evaluate string annotations
         self.parts.append(self._get_var_annotation(name, annotation))
 
     def add_function(self, func, name, indentation_level=0):
         # adds function source code to module
-        self.parts.append(
-            self._get_function_source_with_overloads(func, name, indentation_level)
-        )
+        if isinstance(func, FunctionWithAio):
+            # since the original function signature lacks the "self" argument of the "synthetic" Protocol, we inject it
+            self.parts.append(
+                self._get_dual_function_source(func, name, indentation_level, transform_signature=inject_self)
+            )
+        else:
+            self.parts.append(self._get_function_source_with_overloads(func, name, indentation_level))
 
     def _get_translated_class_bases(self, cls):
         # get __orig_bases__ (__bases__ with potential generic args) for any class
         # note that this has to unwrap the class first in case of synchronicity wrappers,
         # since synchronicity classes don't preserve/translate __orig_bases__.
         # (This is due to __init_subclass__ triggering in odd ways for wrapper classes)
 
         if TARGET_INTERFACE_ATTR in cls.__dict__:
-            # get base classes from origin class instead, to preserve potential Generic base classes which are otherwise stripped by synchronicitys wrappers
+            # get base classes from origin class instead, to preserve potential Generic base classes
+            # which are otherwise stripped by synchronicitys wrappers
             synchronizer = cls.__dict__[SYNCHRONIZER_ATTR]
             impl_cls = cls.__dict__[synchronizer._original_attr]
             target_interface = cls.__dict__[TARGET_INTERFACE_ATTR]
             impl_bases = self._get_translated_class_bases(impl_cls)
 
             retranslated_bases = []
             for impl_base in impl_bases:
                 retranslated_bases.append(
-                    self._translate_annotation(
-                        impl_base, synchronizer, target_interface, cls.__module__
-                    )
+                    self._translate_annotation(impl_base, synchronizer, target_interface, cls.__module__)
                 )
 
             return tuple(retranslated_bases)
 
         # the case that the annotation is a Generic base class, but *not* a synchronicity wrapped one
         bases = []
         for b in cls.__dict__.get("__orig_bases__", cls.__bases__):
@@ -128,84 +144,111 @@
 
         bases_str = "" if not bases else "(" + ", ".join(bases) + ")"
         decl = f"class {name}{bases_str}:"
         var_annotations = []
         methods = []
 
         annotations = cls.__dict__.get("__annotations__", {})
-        annotations = {
-            k: self._translate_global_annotation(annotation, cls)
-            for k, annotation in annotations.items()
-        }
+        annotations = {k: self._translate_global_annotation(annotation, cls) for k, annotation in annotations.items()}
 
         body_indent_level = 1
         body_indent = self._indent(body_indent_level)
 
         for varname, annotation in annotations.items():
-            var_annotations.append(
-                f"{body_indent}{self._get_var_annotation(varname, annotation)}"
-            )
+            var_annotations.append(f"{body_indent}{self._get_var_annotation(varname, annotation)}")
         if var_annotations:
-            var_annotations.append(
-                ""
-            )  # formatting ocd - add an extra newline after var annotations
+            var_annotations.append("")  # formatting ocd - add an extra newline after var annotations
 
         for entity_name, entity in cls.__dict__.items():
             if inspect.isfunction(entity):
-                methods.append(
-                    self._get_function_source_with_overloads(
-                        entity, entity_name, body_indent_level
-                    )
-                )
+                methods.append(self._get_function_source_with_overloads(entity, entity_name, body_indent_level))
 
             elif isinstance(entity, classmethod):
-                methods.append(
-                    f"{body_indent}@classmethod\n{self._get_function_source_with_overloads(entity.__func__, entity_name, body_indent_level)}"
-                )
+                fn_source = self._get_function_source_with_overloads(entity.__func__, entity_name, body_indent_level)
+                methods.append(f"{body_indent}@classmethod\n{fn_source}")
 
             elif isinstance(entity, staticmethod):
-                methods.append(
-                    f"{body_indent}@staticmethod\n{self._get_function_source_with_overloads(entity.__func__, entity_name, body_indent_level)}"
-                )
+                fn_source = self._get_function_source_with_overloads(entity.__func__, entity_name, body_indent_level)
+                methods.append(f"{body_indent}@staticmethod\n{fn_source}")
 
             elif isinstance(entity, property):
+                fn_source = self._get_function_source_with_overloads(entity.fget, entity_name, body_indent_level)
+                methods.append(f"{body_indent}@property\n{fn_source}")
+
+            elif isinstance(entity, (FunctionWithAio, MethodWithAio)):
                 methods.append(
-                    f"{body_indent}@property\n{self._get_function_source_with_overloads(entity.fget, entity_name, body_indent_level)}"
+                    self._get_dual_function_source(
+                        entity,
+                        entity_name,
+                        body_indent_level,
+                        transform_signature=inject_self if isinstance(entity, FunctionWithAio) else None,
+                    )
                 )
 
         padding = [] if var_annotations or methods else [f"{body_indent}..."]
         self.parts.append(
             "\n".join(
                 [
                     decl,
                     *var_annotations,
                     *methods,
                     *padding,
                 ]
             )
         )
 
+    def _get_dual_function_source(
+        self,
+        entity: typing.Union[MethodWithAio, FunctionWithAio],
+        entity_name,
+        body_indent_level,
+        transform_signature=None,
+    ):
+        # Emits type stub for a "dual" function that is both callable and has an .aio callable with an async version
+        # Currently this is emitted as a typing.Protocol declaration + instance with a __call__ and aio method
+        self.imports.add("typing_extensions")
+        # Synchronicity specific blocking + async method
+        body_indent = self._indent(body_indent_level)
+        # create an inline protocol type, inlining both the blocking and async interfaces:
+        blocking_func_source = self._get_function_source_with_overloads(
+            entity._func,
+            "__call__",
+            body_indent_level + 1,
+            transform_signature=transform_signature,
+        )
+        aio_func_source = self._get_function_source_with_overloads(
+            entity._aio_func,
+            "aio",
+            body_indent_level + 1,
+            transform_signature=transform_signature,
+        )
+        protocol_attr = f"""\
+{body_indent}class __{entity_name}_spec(typing_extensions.Protocol):
+{blocking_func_source}
+{aio_func_source}
+{body_indent}{entity_name}: __{entity_name}_spec
+"""
+        return protocol_attr
+
     def add_type_var(self, type_var, name):
-        self.imports.add("typing")
+        type_module = type(type_var).__module__
+        self.imports.add(type_module)
         args = [f'"{name}"']
         if type_var.__bound__:
-            translated_bound = self._translate_global_annotation(
-                type_var.__bound__, type_var
-            )
+            translated_bound = self._translate_global_annotation(type_var.__bound__, type_var)
             str_annotation = self._formatannotation(translated_bound)
             args.append(f'bound="{str_annotation}"')
         self.global_types.add(name)
-        self.parts.append(f'{name} = typing.TypeVar({", ".join(args)})')
+        type_name = type(type_var).__name__  # could be both ParamSpec and TypeVar
+        self.parts.append(f'{name} = {type_module}.{type_name}({", ".join(args)})')
 
     def get_source(self):
         missing_types = self.referenced_global_types - self.global_types
         if missing_types:
-            print(
-                f"WARNING: {self.target_module} missing the following referenced types, expected to be in module"
-            )
+            print(f"WARNING: {self.target_module} missing the following referenced types, expected to be in module")
             for t in missing_types:
                 print(t)
         import_src = "\n".join(sorted(f"import {mod}" for mod in self.imports))
         stubs = "\n\n".join(self.parts)
         return f"{import_src}\n\n{stubs}".lstrip()
 
     def _ensure_import(self, typ):
@@ -240,45 +283,38 @@
             self._register_imports(arg)
 
     def _translate_global_annotation(self, annotation, source_class_or_function):
         # convenience wrapper for _translate_annotation when the translated entity itself
         # determines eval scope and synchronizer target
 
         # infers synchronizer, target and home_module from an entity (class, function) containing the annotation
-        synchronicity_target_interface = getattr(
-            source_class_or_function, TARGET_INTERFACE_ATTR, None
-        )
+        synchronicity_target_interface = getattr(source_class_or_function, TARGET_INTERFACE_ATTR, None)
         synchronizer = getattr(source_class_or_function, SYNCHRONIZER_ATTR, None)
         if synchronizer:
-            home_module = getattr(
-                source_class_or_function, synchronizer._original_attr
-            ).__module__
+            home_module = getattr(source_class_or_function, synchronizer._original_attr).__module__
         else:
             home_module = source_class_or_function.__module__
 
-        return self._translate_annotation(
-            annotation, synchronizer, synchronicity_target_interface, home_module
-        )
+        return self._translate_annotation(annotation, synchronizer, synchronicity_target_interface, home_module)
 
     def _translate_annotation(
         self,
         annotation,
         synchronizer: typing.Optional[synchronicity.Synchronizer],
         synchronicity_target_interface: typing.Optional[Interface],
         home_module: typing.Optional[str],
     ):
         """
         Takes an annotation (type, generic, typevar, forward ref) and applies recursively (in case of generics):
         * eval for string annotations (importing `home_module` to be used as namespace)
-        * re-mapping of the annotation to the correct synchronicity target (using synchronizer and synchronicity_target_interface)
+        * re-mapping of the annotation to the correct synchronicity target
+          (using synchronizer and synchronicity_target_interface)
         * registers imports for all referenced modules
         """
-        if isinstance(
-            annotation, typing.ForwardRef
-        ):  # TypeVars wrap their arguments as ForwardRefs (sometimes?)
+        if isinstance(annotation, typing.ForwardRef):  # TypeVars wrap their arguments as ForwardRefs (sometimes?)
             annotation = annotation.__forward_arg__
 
         if isinstance(annotation, str):
             assert home_module is not None
             mod = importlib.import_module(home_module)
             try:
                 annotation = eval(annotation, mod.__dict__)
@@ -311,18 +347,15 @@
 
         if origin is None or args is None:
             # scalar - if type is synchronicity origin type, use the blocking/async version instead
             if synchronizer:
                 return synchronizer._translate_out(type_annotation, interface)
             return type_annotation
 
-        mapped_args = tuple(
-            self._translate_annotation(arg, synchronizer, interface, home_module)
-            for arg in args
-        )
+        mapped_args = tuple(self._translate_annotation(arg, synchronizer, interface, home_module) for arg in args)
         if interface == Interface.BLOCKING:
             # blocking interface special generic translations:
             if origin == collections.abc.AsyncGenerator:
                 return typing.Generator[mapped_args + (None,)]  # type: ignore
 
             if origin == contextlib.AbstractAsyncContextManager:
                 return typing.ContextManager[mapped_args]  # type: ignore
@@ -341,44 +374,40 @@
 
         if origin.__module__ not in (
             "typing",
             "collections.abc",
             "contextlib",
         ):  # don't translate built in generics in type annotations, even if they have been synchronicity wrapped
             # for other hierarchy reasons...
-            translated_origin = self._translate_annotation(
-                origin, synchronizer, interface, home_module
-            )
+            translated_origin = self._translate_annotation(origin, synchronizer, interface, home_module)
             if translated_origin is not origin:
-                # special case for synchronicity-translated generics, due to synchronicitys wrappers not being valid generics
+                # special case for synchronicity-translated generics,
+                # due to synchronicitys wrappers not being valid generics
                 # kind of ugly as it returns a string representation rather than a type...
                 str_args = ", ".join(self._formatannotation(arg) for arg in mapped_args)
-                return ReprObj(
-                    f"{self._formatannotation(translated_origin)}[{str_args}]"
-                )
+                return ReprObj(f"{self._formatannotation(translated_origin)}[{str_args}]")
 
         return type_annotation.copy_with(mapped_args)
 
-    def _custom_signature(self, func) -> str:
+    def _custom_signature(self, func, transform_signature=None) -> str:
         """
         We use this instead o str(inspect.Signature()) due to a few issues:
         * Generics with None args are incorrectly encoded as NoneType in str(signature)
         * Some names for stdlib module object types omit the module qualification (notably typing)
         * We might have to stringify annotations to support forward/self references
         * General flexibility like not being able to maintain *comments* in the arg declarations if we want to
-        * We intentionally do not use follow_wrapped, since it will override runtime-transformed annotations on a wrapper
+        * We intentionally do not use follow_wrapped,
+          since it will override runtime-transformed annotations on a wrapper
         * TypeVars default repr is `~T` instead of `origin_module.T` etc.
         """
         sig = sigtools.specifiers.signature(func)
 
         if sig.upgraded_return_annotation is not EmptyAnnotation:
             return_annotation = sig.upgraded_return_annotation.source_value()
-            return_annotation = self._translate_global_annotation(
-                return_annotation, func
-            )
+            return_annotation = self._translate_global_annotation(return_annotation, func)
             sig = sig.replace(
                 return_annotation=return_annotation,
                 upgraded_return_annotation=UpgradedAnnotation.upgrade(
                     return_annotation, func, None
                 ),  # not sure if needed
             )
 
@@ -395,14 +424,16 @@
                         ),  # not sure if needed...
                     )
                 )
             else:
                 new_parameters.append(param)
 
         sig = sig.replace(parameters=new_parameters)
+        if transform_signature:
+            sig = transform_signature(sig)
 
         # kind of ugly, but this ensures valid formatting of Generics etc, see docstring above
         with mock.patch("inspect.formatannotation", self._formatannotation):
             return str(sig)
 
     def _get_var_annotation(self, name, annotation):
         # TODO: how to translate annotation here - we don't know the
@@ -413,22 +444,18 @@
         """modified version of `inspect.formatannotations`
         * Uses verbatim `None` instead of `NoneType` for None-arguments in generic types
         * Doesn't omit `typing.`-module from qualified imports in type names
         * recurses through generic types using ReprObj wrapper
         * ignores base_module (uses self.target_module instead)
         """
 
-        assert (
-            base_module is None
-        )  # inspect.Signature isn't generally using the base_module arg afaik
+        assert base_module is None  # inspect.Signature isn't generally using the base_module arg afaik
 
         origin = getattr(annotation, "__origin__", None)
-        assert not isinstance(
-            annotation, typing.ForwardRef
-        )  # Forward refs should already have been evaluated!
+        assert not isinstance(annotation, typing.ForwardRef)  # Forward refs should already have been evaluated!
         args = getattr(annotation, "__args__", None)
 
         if origin is None or not args:
             if annotation == Ellipsis:
                 return "..."
             if isinstance(annotation, type) or isinstance(annotation, TypeVar):
                 if annotation == None.__class__:  # check for "NoneType"
@@ -443,80 +470,87 @@
                 return annotation.__module__ + "." + name
             return repr(annotation)
         # generic:
         try:
             formatted_annotation = str(
                 annotation.copy_with(
                     # ellipsis (...) needs to be passed as is, or it will be reformatted
-                    tuple(
-                        ReprObj(self._formatannotation(arg))
-                        if arg != Ellipsis
-                        else Ellipsis
-                        for arg in args
-                    )
+                    tuple(ReprObj(self._formatannotation(arg)) if arg != Ellipsis else Ellipsis for arg in args)
                 )
             )
         except Exception:
-            raise Exception(
-                f"Could not reformat generic {annotation.__origin__} with arguments {args}"
-            )
+            raise Exception(f"Could not reformat generic {annotation.__origin__} with arguments {args}")
 
         # this is a bit ugly, but gets rid of incorrect module qualification of Generic subclasses:
         # TODO: find a better way...
         if formatted_annotation.startswith(self.target_module + "."):
             return formatted_annotation.split(self.target_module + ".", 1)[1]
         return formatted_annotation
 
     def _indent(self, level):
         return level * self._indentation
 
-    def _get_function_source_with_overloads(
-        self, func, name, indentation_level=0
-    ) -> str:
+    def _get_function_source_with_overloads(self, func, name, indentation_level=0, transform_signature=None) -> str:
         signature_indent = self._indent(indentation_level)
         body_indent = self._indent(indentation_level + 1)
         parts = []
 
         interface = func.__dict__.get(TARGET_INTERFACE_ATTR)
         synchronizer = func.__dict__.get(SYNCHRONIZER_ATTR)
         if interface:
             root_func = func.__dict__[SYNCHRONIZER_ATTR]._translate_in(func)
         else:
             root_func = func
 
         overloaded_signatures = overload_tracking.get_overloads(root_func)
         for overload_func in overloaded_signatures:
-            self._ensure_import(typing.overload)
+            self.imports.add("typing")
             parts.append(f"{signature_indent}@typing.overload")
             if interface:
                 overload_func = synchronizer._wrap(overload_func, interface, name=name)
 
             parts.append(
                 self._get_function_source(
-                    overload_func, name, signature_indent, body_indent
+                    overload_func,
+                    name,
+                    signature_indent,
+                    body_indent,
+                    transform_signature=transform_signature,
                 )
             )
 
         if not overloaded_signatures:
             # only add the functions complete signatures if there are no stubs
             parts.append(
-                self._get_function_source(func, name, signature_indent, body_indent)
+                self._get_function_source(
+                    func,
+                    name,
+                    signature_indent,
+                    body_indent,
+                    transform_signature=transform_signature,
+                )
             )
         return "\n".join(parts)
 
     def _get_function_source(
-        self, func, name, signature_indent: str, body_indent: str
+        self,
+        func,
+        name,
+        signature_indent: str,
+        body_indent: str,
+        transform_signature=None,
     ) -> str:
         async_prefix = ""
         if inspect.iscoroutinefunction(func):
-            # note: async prefix should not be used for annotated abstract/stub *async generators*, so we don't check for inspect.isasyncgenfunction
-            # since they contain no yield keyword, and would otherwise indicate an awaitable that returns an async generator to static type checkers
+            # note: async prefix should not be used for annotated abstract/stub *async generators*,
+            # so we don't check for inspect.isasyncgenfunction since they contain no yield keyword,
+            # and would otherwise indicate an awaitable that returns an async generator to static type checkers
             async_prefix = "async "
 
-        signature = self._custom_signature(func)
+        signature = self._custom_signature(func, transform_signature)
 
         return "\n".join(
             [
                 f"{signature_indent}{async_prefix}def {name}{signature}:",
                 f"{body_indent}...",
                 "",
             ]
```

## Comparing `synchronicity-0.4.4.dist-info/METADATA` & `synchronicity-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synchronicity
-Version: 0.4.4
+Version: 0.5.0
 Summary: Export blocking and async library versions from a single async implementation
 Requires-Python: >=3.7.9
 Description-Content-Type: text/markdown
 Requires-Dist: sigtools (==4.0.1)
 
 ![CI/CD badge](https://github.com/erikbern/synchronicity/actions/workflows/ci.yml/badge.svg)
 [![pypi badge](https://img.shields.io/pypi/v/synchronicity.svg?style=flat)](https://pypi.python.org/pypi/synchronicity)
```

## Comparing `synchronicity-0.4.4.dist-info/RECORD` & `synchronicity-0.5.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-synchronicity/__init__.py,sha256=Q3dvKSQ-AUXnBfRe-utqSWh6mE9wV1kDoizoVtg_gxI,72
-synchronicity/async_wrap.py,sha256=ejbLikhxeGhL3-0pvCCJ145HU8GhN2UpUMOAbja4wAY,2547
+synchronicity/__init__.py,sha256=iLUYrr2mW166J8mGeL1pwiSRVUUdozDXPN2Y_P9hnBA,100
+synchronicity/async_wrap.py,sha256=4Q_gBFxOOdCjcRpYGCkmv-NHeAYCes763nZqK-8laPc,2581
 synchronicity/callback.py,sha256=ZPCfzrZkaepalwEmvxdfYewHEc059hDKFz_7oXIdIoY,1485
 synchronicity/exceptions.py,sha256=pJw_RhOvRSr-sMhSRLmCzNb1M5W36W4EFfeE0FD27OA,1303
-synchronicity/interface.py,sha256=9SVPl_zRhQs030LfDQ4_d_emsNkmlM-A7DL45P7JzAU,136
-synchronicity/overload_tracking.py,sha256=cfdar8Mc8gRYMY0HPInIIAW2FyH_-d_vCbM8h-x6_90,1694
-synchronicity/synchronizer.py,sha256=TvZ0zUGDHVp6SKAb4ZyYqc1IV7v29Bce1u69RSEfR_4,25602
-synchronicity/type_stubs.py,sha256=hGE23W4ov1bBLB0mH8tZnQsIMd7mDLaHd5z-ZezSjss,22482
-synchronicity-0.4.4.dist-info/METADATA,sha256=c_J9aHdAx8L8jGGxpeSaGc6zBnCrrl-KcNSFfLwLzyQ,7736
-synchronicity-0.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-synchronicity-0.4.4.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
-synchronicity-0.4.4.dist-info/RECORD,,
+synchronicity/interface.py,sha256=OVodgsiXbzr9h_3q0bYc4T7qnbTaWQqorbkhYXdxwo0,331
+synchronicity/overload_tracking.py,sha256=ynM0MhkggMkUe5Dc3Nl2ZpWlbHi_srzT9IKNw21NJdU,1792
+synchronicity/synchronizer.py,sha256=feZjhrwfdyWlZ3E5spw1I7ewIsUVIf8ySBLxTI72DaM,30174
+synchronicity/type_stubs.py,sha256=q0LyI6dG61HlG39_Wt2PWaiPQ_Te4QkjV97Yga1lWIA,24842
+synchronicity-0.5.0.dist-info/METADATA,sha256=tEb0uJxuNp3EGGiabBnkvEL3mK-WN7ZiwkRB7cI59DM,7736
+synchronicity-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+synchronicity-0.5.0.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
+synchronicity-0.5.0.dist-info/RECORD,,
```

