# Comparing `tmp/megamock-0.1.0b2.tar.gz` & `tmp/megamock-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megamock-0.1.0b2.tar", max compression
+gzip compressed data, was "megamock-0.1.0b3.tar", max compression
```

## Comparing `megamock-0.1.0b2.tar` & `megamock-0.1.0b3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-02-23 18:15:29.866540 megamock-0.1.0b2/LICENSE
--rw-r--r--   0        0        0    10248 2023-04-05 21:01:46.160410 megamock-0.1.0b2/README.md
--rw-r--r--   0        0        0      282 2023-04-11 18:50:21.187235 megamock-0.1.0b2/megamock/__init__.py
--rw-r--r--   0        0        0     5689 2023-05-02 21:35:31.007772 megamock-0.1.0b2/megamock/import_machinery.py
--rw-r--r--   0        0        0     3881 2023-05-02 18:35:25.379981 megamock-0.1.0b2/megamock/import_references.py
--rw-r--r--   0        0        0    32321 2023-05-02 21:35:31.007772 megamock-0.1.0b2/megamock/megamocks.py
--rw-r--r--   0        0        0    14787 2023-05-02 21:41:48.474942 megamock-0.1.0b2/megamock/megapatches.py
--rw-r--r--   0        0        0     3672 2023-04-11 18:50:21.187235 megamock-0.1.0b2/megamock/megas.py
--rw-r--r--   0        0        0     3066 2023-04-05 19:30:52.816855 megamock-0.1.0b2/megamock/name_words.py
--rw-r--r--   0        0        0        0 2023-03-15 05:28:12.131080 megamock-0.1.0b2/megamock/plugins/__init__.py
--rw-r--r--   0        0        0      949 2023-03-27 18:29:48.174052 megamock-0.1.0b2/megamock/plugins/pytest.py
--rw-r--r--   0        0        0      303 2023-04-11 18:50:21.187235 megamock-0.1.0b2/megamock/type_util.py
--rw-r--r--   0        0        0     1179 2023-05-02 21:35:55.857772 megamock-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0    11352 1970-01-01 00:00:00.000000 megamock-0.1.0b2/setup.py
--rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b2/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 08:50:11.430853 megamock-0.1.0b3/LICENSE
+-rwxr-xr-x   0        0        0    10248 2023-05-10 08:50:11.431855 megamock-0.1.0b3/README.md
+-rwxr-xr-x   0        0        0      282 2023-05-10 08:50:11.445853 megamock-0.1.0b3/megamock/__init__.py
+-rwxr-xr-x   0        0        0     5689 2023-05-10 08:50:11.445853 megamock-0.1.0b3/megamock/import_machinery.py
+-rwxr-xr-x   0        0        0     3881 2023-05-10 08:50:11.446853 megamock-0.1.0b3/megamock/import_references.py
+-rwxr-xr-x   0        0        0    32748 2023-05-10 10:26:15.062755 megamock-0.1.0b3/megamock/megamocks.py
+-rwxr-xr-x   0        0        0    14787 2023-05-10 08:50:11.448853 megamock-0.1.0b3/megamock/megapatches.py
+-rwxr-xr-x   0        0        0     3672 2023-05-10 08:50:11.448853 megamock-0.1.0b3/megamock/megas.py
+-rwxr-xr-x   0        0        0     3066 2023-05-10 08:50:11.449852 megamock-0.1.0b3/megamock/name_words.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 08:50:11.449852 megamock-0.1.0b3/megamock/plugins/__init__.py
+-rwxr-xr-x   0        0        0      949 2023-05-10 08:50:11.450861 megamock-0.1.0b3/megamock/plugins/pytest.py
+-rwxr-xr-x   0        0        0      303 2023-05-10 08:50:11.450861 megamock-0.1.0b3/megamock/type_util.py
+-rwxr-xr-x   0        0        0     1199 2023-05-10 10:24:17.344905 megamock-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b3/PKG-INFO
```

### Comparing `megamock-0.1.0b2/LICENSE` & `megamock-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/README.md` & `megamock-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/megamock/import_machinery.py` & `megamock-0.1.0b3/megamock/import_machinery.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/megamock/import_references.py` & `megamock-0.1.0b3/megamock/import_references.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/megamock/megamocks.py` & `megamock-0.1.0b3/megamock/megamocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,30 +384,44 @@
             try:
                 setattr(wrapped, key, value)
             except AttributeError:
                 # mock won't allow assignment of values assigned in __init__ or
                 # elsewhere when spec_set is set. Check spec annotations and if the
                 # value exists, allow assignment
                 if key in self.megamock.spec.__annotations__:
-                    # do not check type if assigning a mock object
-                    # note that MegaMock is a subclass of NonCallableMagicMock
-                    if not isinstance(
-                        value, mock.NonCallableMock | mock.NonCallableMagicMock
-                    ):
-                        allowed_values = self.megamock.spec.__annotations__[key]
-                        if not isinstance(value, allowed_values):
-                            raise TypeError(
-                                f"{value!r} is not an instance of {allowed_values}"
-                            )
+                    self._set_attr_annotations_check(key, value)
                     wrapped.__dict__[key] = value
                 else:
                     raise
         else:
             self.__dict__[key] = value
 
+    def _set_attr_annotations_check(self, key: str, value: Any) -> None:
+        # do not check type if assigning a mock object
+        # note that MegaMock is a subclass of NonCallableMagicMock
+        if not isinstance(
+            value, mock.NonCallableMock | mock.NonCallableMagicMock
+        ):
+            allowed_values = self.megamock.spec.__annotations__[key]
+
+            def raise_type_error() -> None:
+                raise TypeError(
+                    f"{value!r} is not an instance of {allowed_values}"
+                )
+
+            # handle:
+            # "from __future__ import annotations" converting type to str
+            if isinstance(allowed_values, str):
+                if str(value.__class__.__name__) not in [
+                    x.strip() for x in allowed_values.split("|")
+                ]:
+                    raise_type_error()
+            elif not isinstance(value, allowed_values):
+                raise_type_error()
+
     def _get_spec_from_parents(
         self, _parent_stack: list[_MegaMockMixin] | None = None
     ) -> Any:
         """
         The built-in generate autospec function creates a few issues because
         it bypasses some of the tooling, so the whole tree of mocks are created
         without hitting MegaMock anywhere.
```

### Comparing `megamock-0.1.0b2/megamock/megapatches.py` & `megamock-0.1.0b3/megamock/megapatches.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/megamock/megas.py` & `megamock-0.1.0b3/megamock/megas.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/megamock/name_words.py` & `megamock-0.1.0b3/megamock/name_words.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/megamock/plugins/pytest.py` & `megamock-0.1.0b3/megamock/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0b2/pyproject.toml` & `megamock-0.1.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "megamock"
-version = "0.1.0-beta.2"
+version = "0.1.0-beta.3"
 description = "Mega mocking capabilities - stop using dot-notated paths!"
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/JamesHutchison/megamock"
 repository = "https://github.com/JamesHutchison/megamock"
 keywords = ["mock", "test"]
@@ -24,14 +24,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 mypy = "^1.1.1"
+pydantic = "1.10.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-p megamock.plugins.pytest"
```

### Comparing `megamock-0.1.0b2/setup.py` & `megamock-0.1.0b3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,360 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: megamock
+Version: 0.1.0b3
+Summary: Mega mocking capabilities - stop using dot-notated paths!
+Home-page: https://github.com/JamesHutchison/megamock
+License: MIT
+Keywords: mock,test
+Author: James Hutchison
+Author-email: jamesghutchison@proton.me
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Mocking
+Requires-Dist: asttokens (>=2.2.1,<2.3.0)
+Requires-Dist: varname[asttokens] (>=0.10.0,<0.11.0)
+Project-URL: Repository, https://github.com/JamesHutchison/megamock
+Description-Content-Type: text/markdown
 
-packages = \
-['megamock', 'megamock.plugins']
+# **MegaMock** - _The Developer Experience Upgrade for Python Mocking_
 
-package_data = \
-{'': ['*']}
+Pew pew! Sane defaults for mocking behavior! Patch objects, variables, attributes, etc by passing in the thing in question, rather than passing in dot-delimited path strings! Create tests faster than ever!
 
-install_requires = \
-['asttokens>=2.2.1,<2.3.0', 'varname[asttokens]>=0.10.0,<0.11.0']
-
-setup_kwargs = {
-    'name': 'megamock',
-    'version': '0.1.0b2',
-    'description': 'Mega mocking capabilities - stop using dot-notated paths!',
-    'long_description': '# **MegaMock** - _The Developer Experience Upgrade for Python Mocking_\n\nPew pew! Sane defaults for mocking behavior! Patch objects, variables, attributes, etc by passing in the thing in question, rather than passing in dot-delimited path strings! Create tests faster than ever!\n\nSupported Python Versions: 3.10+\n### Installation\n\nPip installation:\n```\npip install megamock\n```\n\n[poetry](https://python-poetry.org/) (as a development dependency):\n```\npoetry add megamock --group=dev\n```\n\n# Why Use MegaMock? (short version)\nMegaMock is a library that provides a better interface for mocking and patching in Python. Its version\nof patch doesn\'t have any gotchas based on how you import something, and it also automatically\ncreates mocks using best practices. Additionally, the generated mock types are unions of the mocked object\nand `MegaMock`, allowing you to better leverage your IDE\'s autocomplete.\n\n![Sample MegaMock vs Mock Comparison](docs/img/megamock-example.gif)\n\nMock:\n\n```python\nclass_mock = mock.create_autospec(ClassICareAbout, instance=True)\n# cmd / alt clicking on "method_call" doesn\'t direct you to the definition\nclass_mock.method_call.return_value = "some value"\n\n# can\'t simply cmd / alt click and go to ClassICareAbout\nwith mock.patch("some.hard.to.remember.and.long.dot.path.ClassICareAbout", class_mock) as mock_instance:\n    do_something()\n```\n\nMegaMock:\n\n```python\n# cmd / alt clicking on ClassICareAbout takes you to the definition\npatch = MegaPatch.it(ClassICareAbout)\nmock_instance = patch.megainstance\n# cmd / alt clicking on "method_call" directs you to the definition\nmock_instance.method_call.return_value = "some value"\n\ndo_something()\n```\n\n# Why Use MegaMock? (long version)\nMegaMock was created to address some shortcomings in the built-in Python library:\n- Legacy code holds back "best practice" defaults, so many developers write sub-optimal mocks\n  that allow things that should not be allowed. Likewise, writing better mocks are more work,\n  so there\'s a tendency to write simpler code because, at that point in time, the developer\n  felt that is all that was needed. MegaMock\'s simple interface provides sane defaults.\n- `mock.patch` is very commonly used, and can work well when `autospec=True`, but has the drawback that\n  you need to pass in a string to the thing that is being patched. Most (all?) IDEs do not properly\n  recognize these strings as references to the objects that are being patched, and thus automated\n  refactoring and reference finding skips them. Likewise, automatically getting a dot referenced path\n  to an object is also commonly missing functionality. This all adds additional burden to the developer.\n  With `MegaPatch`, you can import an object as you normally would into the test, then pass in thing\n  itself you want to patch. This even works for methods, attributes, and nested classes! Additionally, your IDE\'s autocomplete for attributes\n  will work in many situations as well!\n- `mock.patch` has a gotcha where the string you provide must match where the reference lives.\n  So, for example, if you have in `my_module.py`: `from other_module import Thing`, then doing\n  `mock.patch("other_module.Thing")` won\'t actually work, because the reference in `my_module` still\n  points to the original. You can work around this by doing `import other_module` and referencing `Thing`\n  by `other_module.Thing`. MegaMock does not have this problem, and it doesn\'t matter how you import.\n\n## Features\n\nSee the [full features list](FEATURES.md).\n## Example Usage\n\n### Production Code\n```python\nfrom module.submodule import MyClassToMock\n\n\ndef my_method(...):\n    ...\n    a_thing = MyClassToMock(...)\n    do_something_with_a_thing(a_thing)\n    ...\n\n\ndef do_something_with_a_thing(a_thing: MyClassToMock) -> None:\n    result = a_thing.some_method(...)\n    if result == "a value":\n        ...\n```\n\n### Test Code\n```python\nfrom megamock import MegaPatch\nfrom module.submodule import MyClassToMock\n\n\ndef test_something(...):\n    patch = MegaPatch.it(MyClassToMock.some_method)\n    patch.return_value = "a value"\n\n    my_method(...)\n```\n\n## Documentation\n\n### Usage (pytest)\n\nWith [pytest](https://pytest.org), MegaMock is easily leveraged by using the included pytest plugin. You can use it by adding `-p megamock.plugins.pytest`\nto the command line.\n\nCommand line example:\n```\npytest -p megamock.plugins.pytest\n```\n\n`pyproject.toml` example:\n```toml\n[tool.pytest.ini_options]\naddopts = "-p megamock.plugins.pytest"\n```\n\nThe pytest plugin also automatically stops `MegaPatch`es after each test. To disable this behavior, pass in the `--do_not_autostop_megapatches`\ncommand line argument. If `pytest-mock` is installed, the default mocker will be switched to the `pytest-mock` `mocker`.\n\n### Usage (other test frameworks)\n\nIf you\'re not using the pytest plugin, import and execution order is important for MegaMock. When running tests, you will need to execute the `start_import_mod`\nfunction prior to importing any production or test code. You will also want it so the loader is not used in production.\n\n-------------------\n\n**Core Classes**\n\n`MegaMock` - the primary class for a mocked object. This is similar to `MagicMock`. Use `MegaMock.it(MyObject)` to make `MyObject` the [spec](https://docs.python.org/3/library/unittest.mock.html#unittest.mock.create_autospec).\n\n`MegaPatch` - the class for patching. This is similar to `patch`. Use `MegaPath.it(MyObject)` to replace new instances of the `MyObject` class.\n\n`Mega` - helper class for accessing mock attributes without having to memorize the due to lost type inference. Use `Mega(some_megamock)`.\nNote that the `assert_` methods, such as `assert_called_once`, is now `called_once` and returns a boolean. The assertion error\nis stored in `Mega.last_assertion_error`.\n\n--------------------\n\nDependency injection example:\n```python\n\nfrom megamock import MegaMock\n\ndef test_something(...):\n    manager = MegaMock.it(MyManagerClass)\n    service = SomeService(manager)\n    ...\n```\n\nMegaPatch example:\n```python\nfrom elsewhere import Service\n\nfrom megamock import MegaPatch\n\ndef test_something(...):\n    patched = MegaPatch.it(Service.make_external_call)\n    patched.return_value = SomeValue(...)\n    service = SomeService(...)\n\n    code_under_test(service)\n    ...\n```\n\n`MegaMock` objects have the same attributes as regular `MagicMock`s plus `megamock` and `megainstance`\nFor example, `my_mega_mock.megamock.spy` is the object being spied, if set. `my_class_mock.megainstance` is the instance returned when the class is instantiated.\n\nThe [guidance document](GUIDANCE.md) is available to provide in-depth information on using mocking and MegaMock. Continuing reading to\nquickly jump in to examples.\n\n-----------------------\n\n### Learning By Example\n\nAll examples below have the following imports:\n\n```python\nfrom my_module import MyClass\nfrom megamock import Mega, MegaMock, MegaPatch\n```\n\nCreating a mock instance of a class:\n\n```python\nmock_instance = MegaMock.it(MyClass)\n```\n\nCreating a mock class itself:\n\n```python\nmock_class = MegaMock.it(MyClass, instance=False)\n```\n\nSpying an object:\n\n```python\nmy_thing = MyClass()\nspied_class = MegaMock(spy=my_thing)\n\n# ... do stuff with spied_class...\n\nMega(spied_class.some_method).call_args_list  # same as wraps\n\n# check whether a value was accessed\n# if things aren\'t as expected, you can pull up the debugger and see the stack traces\nassert len(spied_class.megamock.spied_access["some_attribute"]) == 1\n\nspy_access_list = spied_class.megamock.spied_access["some_attribute"]\nspy_access: SpyAccess = spy_access_list[0]\nspy_access.attr_value  # shallow copy of what was returned\nspy_access.stacktrace  # where the access happened\nspy_access.time  # when it happened (from time.time())\nspy_access.top_of_stacktrace  # a shorthand property intended to be used when debugging in the IDE\nspy_access.format_stacktrace()  # return a list of strings for the stacktrace\nspy_access.print_stacktrace()  # display the stacktrace to the console\n```\n\n\nPatching a class:\n\n```python\nmock_patch = MegaPatch.it(MyClass)\n\n# the class itself\nmock_patch.new_value\n\n# the class instance\nmock_patch.megainstance\n\n# the return value of the __call__ method on the class\nmock_patch.megainstance.return_value\n```\n\nPatching a class attribute:\n\n```python\n# temporarily update the max retries to 0\nmega_patch = MegaPatch.it(MyClass.max_retries, new=0)\n```\n\nPatching a class method:\n\n```python\nmega_patch = MegaPatch.it(MyClass.my_method, return_value=...)\n```\n\nAlternatively:\n```python\nmega_patch = MegaPatch.it(MyClass.my_method)\nmega_patch.mock.return_value = ...\n```\n\n```python\nmega_patch = MegaPatch.it(MyClass.my_method)\nmega_patch.new_value.return_value = ...\n```\n\nYou can also alter the return value of your mock without creating a separate mock object first.\n\n```python\nmega_patch.return_value.user = SomeUser()\n```\n\nWorking with `MegaPatch` and classes:\n\n`mega_patch.new_value` is the class _type_ itself\n\n```python\nmega_patch = MegaPatch.it(MyClass)\n\nmega_patch.new_value.x is MyClass.x\n```\n\n`mega_patch.return_value` is the class _instance_ returned. However, there is the property\n`megainstance` which is preferred because it has better type hinting.\n\n```python\nmega_patch = MegaPatch.it(MyClass)\n\n# instead of this, for which the static type is Any:\nmega_patch.return_value is MyClass()\n\n# use this, which has a static type of MegaMock | MyClass:\nmega_patch.megainstance is MyClass()\n```\n\nPatching a module attribute:\n\n```python\nimport my_module\n\nMegaPatch.it(my_module.some_attribute, new=...)\n```\n\nPatching a method of a nested class:\n\n```python\nimport my_module\n\nMegaPatch.it(\n    my_module.MyClass.MyNestedClass.some_method,\n    return_value=...\n)\n```\n\nSetting the return value:\n\n```python\nmy_mock.my_method.return_value = "foo"\n```\n\nTurning on real logic:\n\n```python\nimport my_module\nfrom mega_mock import UseRealLogic\n\nmega_patch = MegaPatch.it(my_module.SomeClass)\nMega(mega_patch.megainstance.some_pure_logic_method).use_real_logic()\n\ndo_something_that_invokes_that_function(...)\n```\n\n# Congrats on Reading This Far! Here\'s an Art Gallery!\n\n![MegaMock](docs/img/megamock-v2-cropped.png)\n\nNobody said it was a big art gallery. Feel free to submit a PR that helps fix that. No artistic skill required.\n',
-    'author': 'James Hutchison',
-    'author_email': 'jamesghutchison@proton.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/JamesHutchison/megamock',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+Supported Python Versions: 3.10+
+### Installation
 
+Pip installation:
+```
+pip install megamock
+```
+
+[poetry](https://python-poetry.org/) (as a development dependency):
+```
+poetry add megamock --group=dev
+```
+
+# Why Use MegaMock? (short version)
+MegaMock is a library that provides a better interface for mocking and patching in Python. Its version
+of patch doesn't have any gotchas based on how you import something, and it also automatically
+creates mocks using best practices. Additionally, the generated mock types are unions of the mocked object
+and `MegaMock`, allowing you to better leverage your IDE's autocomplete.
+
+![Sample MegaMock vs Mock Comparison](docs/img/megamock-example.gif)
+
+Mock:
+
+```python
+class_mock = mock.create_autospec(ClassICareAbout, instance=True)
+# cmd / alt clicking on "method_call" doesn't direct you to the definition
+class_mock.method_call.return_value = "some value"
+
+# can't simply cmd / alt click and go to ClassICareAbout
+with mock.patch("some.hard.to.remember.and.long.dot.path.ClassICareAbout", class_mock) as mock_instance:
+    do_something()
+```
+
+MegaMock:
+
+```python
+# cmd / alt clicking on ClassICareAbout takes you to the definition
+patch = MegaPatch.it(ClassICareAbout)
+mock_instance = patch.megainstance
+# cmd / alt clicking on "method_call" directs you to the definition
+mock_instance.method_call.return_value = "some value"
+
+do_something()
+```
+
+# Why Use MegaMock? (long version)
+MegaMock was created to address some shortcomings in the built-in Python library:
+- Legacy code holds back "best practice" defaults, so many developers write sub-optimal mocks
+  that allow things that should not be allowed. Likewise, writing better mocks are more work,
+  so there's a tendency to write simpler code because, at that point in time, the developer
+  felt that is all that was needed. MegaMock's simple interface provides sane defaults.
+- `mock.patch` is very commonly used, and can work well when `autospec=True`, but has the drawback that
+  you need to pass in a string to the thing that is being patched. Most (all?) IDEs do not properly
+  recognize these strings as references to the objects that are being patched, and thus automated
+  refactoring and reference finding skips them. Likewise, automatically getting a dot referenced path
+  to an object is also commonly missing functionality. This all adds additional burden to the developer.
+  With `MegaPatch`, you can import an object as you normally would into the test, then pass in thing
+  itself you want to patch. This even works for methods, attributes, and nested classes! Additionally, your IDE's autocomplete for attributes
+  will work in many situations as well!
+- `mock.patch` has a gotcha where the string you provide must match where the reference lives.
+  So, for example, if you have in `my_module.py`: `from other_module import Thing`, then doing
+  `mock.patch("other_module.Thing")` won't actually work, because the reference in `my_module` still
+  points to the original. You can work around this by doing `import other_module` and referencing `Thing`
+  by `other_module.Thing`. MegaMock does not have this problem, and it doesn't matter how you import.
+
+## Features
+
+See the [full features list](FEATURES.md).
+## Example Usage
+
+### Production Code
+```python
+from module.submodule import MyClassToMock
+
+
+def my_method(...):
+    ...
+    a_thing = MyClassToMock(...)
+    do_something_with_a_thing(a_thing)
+    ...
+
+
+def do_something_with_a_thing(a_thing: MyClassToMock) -> None:
+    result = a_thing.some_method(...)
+    if result == "a value":
+        ...
+```
+
+### Test Code
+```python
+from megamock import MegaPatch
+from module.submodule import MyClassToMock
+
+
+def test_something(...):
+    patch = MegaPatch.it(MyClassToMock.some_method)
+    patch.return_value = "a value"
+
+    my_method(...)
+```
+
+## Documentation
+
+### Usage (pytest)
+
+With [pytest](https://pytest.org), MegaMock is easily leveraged by using the included pytest plugin. You can use it by adding `-p megamock.plugins.pytest`
+to the command line.
+
+Command line example:
+```
+pytest -p megamock.plugins.pytest
+```
+
+`pyproject.toml` example:
+```toml
+[tool.pytest.ini_options]
+addopts = "-p megamock.plugins.pytest"
+```
+
+The pytest plugin also automatically stops `MegaPatch`es after each test. To disable this behavior, pass in the `--do_not_autostop_megapatches`
+command line argument. If `pytest-mock` is installed, the default mocker will be switched to the `pytest-mock` `mocker`.
+
+### Usage (other test frameworks)
+
+If you're not using the pytest plugin, import and execution order is important for MegaMock. When running tests, you will need to execute the `start_import_mod`
+function prior to importing any production or test code. You will also want it so the loader is not used in production.
+
+-------------------
+
+**Core Classes**
+
+`MegaMock` - the primary class for a mocked object. This is similar to `MagicMock`. Use `MegaMock.it(MyObject)` to make `MyObject` the [spec](https://docs.python.org/3/library/unittest.mock.html#unittest.mock.create_autospec).
+
+`MegaPatch` - the class for patching. This is similar to `patch`. Use `MegaPath.it(MyObject)` to replace new instances of the `MyObject` class.
+
+`Mega` - helper class for accessing mock attributes without having to memorize the due to lost type inference. Use `Mega(some_megamock)`.
+Note that the `assert_` methods, such as `assert_called_once`, is now `called_once` and returns a boolean. The assertion error
+is stored in `Mega.last_assertion_error`.
+
+--------------------
+
+Dependency injection example:
+```python
+
+from megamock import MegaMock
+
+def test_something(...):
+    manager = MegaMock.it(MyManagerClass)
+    service = SomeService(manager)
+    ...
+```
+
+MegaPatch example:
+```python
+from elsewhere import Service
+
+from megamock import MegaPatch
+
+def test_something(...):
+    patched = MegaPatch.it(Service.make_external_call)
+    patched.return_value = SomeValue(...)
+    service = SomeService(...)
+
+    code_under_test(service)
+    ...
+```
+
+`MegaMock` objects have the same attributes as regular `MagicMock`s plus `megamock` and `megainstance`
+For example, `my_mega_mock.megamock.spy` is the object being spied, if set. `my_class_mock.megainstance` is the instance returned when the class is instantiated.
+
+The [guidance document](GUIDANCE.md) is available to provide in-depth information on using mocking and MegaMock. Continuing reading to
+quickly jump in to examples.
+
+-----------------------
+
+### Learning By Example
+
+All examples below have the following imports:
+
+```python
+from my_module import MyClass
+from megamock import Mega, MegaMock, MegaPatch
+```
+
+Creating a mock instance of a class:
+
+```python
+mock_instance = MegaMock.it(MyClass)
+```
+
+Creating a mock class itself:
+
+```python
+mock_class = MegaMock.it(MyClass, instance=False)
+```
+
+Spying an object:
+
+```python
+my_thing = MyClass()
+spied_class = MegaMock(spy=my_thing)
+
+# ... do stuff with spied_class...
+
+Mega(spied_class.some_method).call_args_list  # same as wraps
+
+# check whether a value was accessed
+# if things aren't as expected, you can pull up the debugger and see the stack traces
+assert len(spied_class.megamock.spied_access["some_attribute"]) == 1
+
+spy_access_list = spied_class.megamock.spied_access["some_attribute"]
+spy_access: SpyAccess = spy_access_list[0]
+spy_access.attr_value  # shallow copy of what was returned
+spy_access.stacktrace  # where the access happened
+spy_access.time  # when it happened (from time.time())
+spy_access.top_of_stacktrace  # a shorthand property intended to be used when debugging in the IDE
+spy_access.format_stacktrace()  # return a list of strings for the stacktrace
+spy_access.print_stacktrace()  # display the stacktrace to the console
+```
+
+
+Patching a class:
+
+```python
+mock_patch = MegaPatch.it(MyClass)
+
+# the class itself
+mock_patch.new_value
+
+# the class instance
+mock_patch.megainstance
+
+# the return value of the __call__ method on the class
+mock_patch.megainstance.return_value
+```
+
+Patching a class attribute:
+
+```python
+# temporarily update the max retries to 0
+mega_patch = MegaPatch.it(MyClass.max_retries, new=0)
+```
+
+Patching a class method:
+
+```python
+mega_patch = MegaPatch.it(MyClass.my_method, return_value=...)
+```
+
+Alternatively:
+```python
+mega_patch = MegaPatch.it(MyClass.my_method)
+mega_patch.mock.return_value = ...
+```
+
+```python
+mega_patch = MegaPatch.it(MyClass.my_method)
+mega_patch.new_value.return_value = ...
+```
+
+You can also alter the return value of your mock without creating a separate mock object first.
+
+```python
+mega_patch.return_value.user = SomeUser()
+```
+
+Working with `MegaPatch` and classes:
+
+`mega_patch.new_value` is the class _type_ itself
+
+```python
+mega_patch = MegaPatch.it(MyClass)
+
+mega_patch.new_value.x is MyClass.x
+```
+
+`mega_patch.return_value` is the class _instance_ returned. However, there is the property
+`megainstance` which is preferred because it has better type hinting.
+
+```python
+mega_patch = MegaPatch.it(MyClass)
+
+# instead of this, for which the static type is Any:
+mega_patch.return_value is MyClass()
+
+# use this, which has a static type of MegaMock | MyClass:
+mega_patch.megainstance is MyClass()
+```
+
+Patching a module attribute:
+
+```python
+import my_module
+
+MegaPatch.it(my_module.some_attribute, new=...)
+```
+
+Patching a method of a nested class:
+
+```python
+import my_module
+
+MegaPatch.it(
+    my_module.MyClass.MyNestedClass.some_method,
+    return_value=...
+)
+```
+
+Setting the return value:
+
+```python
+my_mock.my_method.return_value = "foo"
+```
+
+Turning on real logic:
+
+```python
+import my_module
+from mega_mock import UseRealLogic
+
+mega_patch = MegaPatch.it(my_module.SomeClass)
+Mega(mega_patch.megainstance.some_pure_logic_method).use_real_logic()
+
+do_something_that_invokes_that_function(...)
+```
+
+# Congrats on Reading This Far! Here's an Art Gallery!
+
+![MegaMock](docs/img/megamock-v2-cropped.png)
+
+Nobody said it was a big art gallery. Feel free to submit a PR that helps fix that. No artistic skill required.
 
-setup(**setup_kwargs)
```

