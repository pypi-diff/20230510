# Comparing `tmp/robocorp_log-0.1.0.tar.gz` & `tmp/robocorp_log-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_log-0.1.1.tar", max compression
```

## Comparing `robocorp_log-0.1.0.tar` & `robocorp_log-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10142 2023-05-09 16:31:51.266637 robocorp_log-0.1.0/LICENSE
--rw-r--r--   0        0        0     3195 2023-05-09 16:31:51.266637 robocorp_log-0.1.0/README.md
--rw-r--r--   0        0        0     1199 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    27456 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0    13242 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0     9794 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0     5361 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      572 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0    12420 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0    49216 2023-05-09 16:32:24.722633 robocorp_log-0.1.0/src/robocorp/log/_index.py
--rw-r--r--   0        0        0    61053 2023-05-09 16:32:26.978633 robocorp_log-0.1.0/src/robocorp/log/_index_v2.py
--rw-r--r--   0        0        0     2497 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      385 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0    21836 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     8900 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12453 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0     9706 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    55041 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1436 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_sensitive_variable_names.py
--rw-r--r--   0        0        0     1915 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/_suppress_helper.py
--rw-r--r--   0        0        0     7802 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/console.py
--rw-r--r--   0        0        0     1057 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     7317 2023-05-09 16:31:51.270637 robocorp_log-0.1.0/src/robocorp/log/redirect.py
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 robocorp_log-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-05-10 17:49:39.717459 robocorp_log-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5471 2023-05-10 17:49:39.717459 robocorp_log-0.1.1/README.md
+-rw-r--r--   0        0        0     1137 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    27835 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0    13242 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0     9794 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     5361 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      572 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0    12420 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0    49206 2023-05-10 17:50:31.613837 robocorp_log-0.1.1/src/robocorp/log/_index.py
+-rw-r--r--   0        0        0    61043 2023-05-10 17:50:34.769856 robocorp_log-0.1.1/src/robocorp/log/_index_v2.py
+-rw-r--r--   0        0        0     2497 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      385 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0    21836 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     8900 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12453 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     9706 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    55042 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     7802 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/console.py
+-rw-r--r--   0        0        0     1057 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     7312 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/redirect.py
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 robocorp_log-0.1.1/PKG-INFO
```

### Comparing `robocorp_log-0.1.0/LICENSE` & `robocorp_log-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/README.md` & `robocorp_log-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -70,15 +70,98 @@
 
 3. `async` and `await` are not currently well supported (although it's already in
 the plans).
 
 
 ## Dealing with sensitive data in the logs
 
-* See: [Handling Sensitive Data](https://github.com/robocorp/robo/tree/master/log/docs/handling_sensitive_data.md)
+By default `Robocorp Log` will show information for all method calls in user
+code as well as some selected libraries automatically.
+
+This is very handy but comes with the drawback that some care must be must be taken 
+in order for sensitive data to be kept out of the logs.
+
+The most common use cases and APIs are explained below:
+
+Usernames and passwords
+------------------------
+
+For usernames and passwords, the preferred approach is that the provider of the sensitive information
+asks for the information and requests `Robocorp Log` to keep such information out of
+the logs.
+
+The usage for the API is:
+
+```python
+
+from robocorp import log
+
+with log.suppress_variables():
+    pwd = request_password()
+    log.hide_from_output(pwd)
+```
+
+By calling the `hide_from_output` method, any further occurrence of the `password` contents will be
+automatically changed to `<redacted>`.
+
+Note that some arguments and variable assigns for some names are automatically redacted.
+
+-- by default `password` and `passwd`, but others may be customized through the 
+`robocorp.log.add_sensitive_variable_name` and `add_sensitive_variable_name_pattern`
+functions.
+
+In the example below, the contents of the `${user password}` variable will be automatically added to
+the list of strings to be hidden from the output.
+
+```python
+
+def check_handling(user_password):
+    ...
+
+check_handling('the password')
+```
+
+
+Sensitive data obtained from APIs
+----------------------------------
+
+When handling sensitive data from APIs (such as private user information obtained from an API, as the SSN
+or medical data) the preferred API is disabling the logging for variables.
+
+This can be done with the `robocorp.log.suppress_variables` API (which is usable as a context manager).
+
+Example using API:
+
+```python
+from robocorp import log
+
+def handle_sensitive_info()
+    with log.suppress_variables():
+        ...
+
+```
+
+
+If even the methods called could be used to compromise some information (or if
+there's too much noise in those calls), it's possible
+to completely stop the logging with the `robocorp.log.suppress` API. 
+
+Note: this may make debugging a failure harder as method calls won't be logged, 
+albeit you may still call `critical / info / warn` to explicitly log something in this case.
+
+Example using API:
+
+```python
+from robocorp import log
+
+def handle_sensitive_info()
+    with log.suppress():
+        ...
+
+```
 
 
 ## Internal structure
 
 * [Format specification](https://github.com/robocorp/robo/tree/master/log/docs/format.md)
 
 ## License: Apache 2.0
```

### Comparing `robocorp_log-0.1.0/pyproject.toml` & `robocorp_log-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-log"
-version = "0.1.0"
+version = "0.1.1"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/log", from = "src"}]
 include = ["**/_index.py", "**/_index_v2.py"]
@@ -13,14 +13,21 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Logging",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
+[tool.poetry.dependencies]
+python = "^3.9"
+tomli = { version = "^2.0.1", python = "<3.11" }
+
+[tool.poetry.group.dev.dependencies]
+robocorp-devutils = {path = "../devutils/", develop = true}
+
 [tool.mypy]
 mypy_path = "src:tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
 
@@ -28,23 +35,10 @@
 module = "pytest_timeout.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "pytest_timeout.*"
 ignore_missing_imports = true
 
-[tool.poetry.dependencies]
-python = "^3.9"
-tomli = { version = "^2.0.1", python = "<3.11" }
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-mypy = "^1.1.1"
-pytest = "^7.2.2"
-pytest-xdist = "^3.2.1"
-pytest-regressions = "1.0.6"
-fire = "^0.5.0"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `robocorp_log-0.1.0/src/robocorp/log/__init__.py` & `robocorp_log-0.1.1/src/robocorp/log/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from .protocols import OptExcInfo, LogHTMLStyle, Status, IReadLines
 from ._suppress_helper import SuppressHelper as _SuppressHelper
 
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 from . import _config
 
 # --- Make these a part of the public API.
 
 Filter = _config.Filter
@@ -297,16 +297,15 @@
 
 
 _suppress_helper = _SuppressHelper(_suppress_contextmanager)
 
 
 def suppress_methods():
     """
-    Can be used as a context manager or decorator so that methods are no
-    longer logged.
+    Can be used as a context manager or decorator so that methods are not logged.
 
     i.e.:
         @suppress_methods
         def method():
             ...
 
         or
@@ -315,16 +314,15 @@
             ...
     """
     return suppress(variables=False, methods=True)
 
 
 def suppress_variables():
     """
-    Can be used as a context manager or decorator so that variables are no
-    longer logged.
+    Can be used as a context manager or decorator so that variables are not logged.
 
     i.e.:
         @suppress_variables
         def method():
             ...
 
         or
@@ -354,16 +352,16 @@
     Suppresses everything except the arguments marked as "False"
     """
 
 
 @overload
 def suppress(func: Callable[[], Any]) -> _AnyCallOrCtxManager:
     """
-    Arguments when used as a decorator without any arguments (where it just
-    receives a function).
+    Arguments when used as a decorator without any arguments
+    -- just receives it as a function.
     """
 
 
 def suppress(*args, **kwargs):
     """
     API to suppress logging to be used as a context manager or decorator.
 
@@ -408,42 +406,47 @@
 )
 
 _sensitive_names = _SensitiveVariableNames(("password", "passwd"))
 
 
 def is_sensitive_variable_name(variable_name: str) -> bool:
     """
+    Returns true if the given variable name should be considered sensitive.
+
     Args:
         variable_name: The variable name to be checked.
 
     Returns:
         True if the given variable name is considered to be sensitive (in which
         case its value should be redacted) and False otherwise.
     """
     return _sensitive_names.is_sensitive_variable_name(variable_name)
 
 
 def add_sensitive_variable_name(variable_name: str) -> None:
     """
-    Marks a given variable name as sensitive (in which case any variable
-    containing the given `variable_name` will be redacted).
+    Marks a given variable name as sensitive
+
+    (in this case any variable containing the given `variable_name` will be
+    redacted).
 
     Note that this will add a patterns where any variable containing the given
     variable name even as a substring will be considered sensitive.
 
     Args:
         variable_name: The variable name to be considered sensitive.
     """
     _sensitive_names.add_sensitive_variable_name(variable_name)
 
 
 def add_sensitive_variable_name_pattern(variable_name_pattern: str) -> None:
     """
-    Adds a given pattern to consider a variable name as sensitive. Any variable
-    name matching the given pattern will have its value redacted.
+    Adds a given pattern to consider a variable name as sensitive.
+
+    Any variable name matching the given pattern will have its value redacted.
 
     Args:
         variable_name_pattern: The variable name pattern to be considered
         sensitive.
     """
     _sensitive_names.add_sensitive_variable_name_pattern(variable_name_pattern)
 
@@ -534,14 +537,16 @@
 
 
 # ---- APIs to decode existing log files
 
 
 def iter_decoded_log_format_from_stream(stream: IReadLines) -> Iterator[dict]:
     """
+    Iterates stream contents and decodes those as dicts.
+
     Args:
         stream: The stream which should be iterated in (anything with a
             `readlines()` method which should provide the messages encoded
             in the internal format).
 
     Returns:
         An iterator which will decode the messages and provides a dictionary for
@@ -561,16 +566,15 @@
     from ._decoder import iter_decoded_log_format
 
     return iter_decoded_log_format(stream)
 
 
 def iter_decoded_log_format_from_log_html(log_html: Path) -> Iterator[dict]:
     """
-    This function will read the data saved in the log html and provide an
-    iterator which will provide the decoded messages which were encoded into it.
+    Reads the data saved in the log html and provides decoded messages (dicts).
 
     Returns:
         An iterator which will decode the messages and provides a dictionary for
         each message found.
 
         Example of messages provided:
 
@@ -622,16 +626,17 @@
 
 def verify_log_messages_from_messages_iterator(
     messages_iterator: Iterator[dict],
     expected: Sequence[dict],
     not_expected: Sequence[dict] = _DEFAULT_NOT_EXPECTED,
 ) -> List[dict]:
     """
-    A helper for checking that the expected messages are found (or not found) in
-    the given messages iterator.
+    Helper for checking that the expected messages are found in the given messages iterator.
+
+    Can also check if a message is not found.
 
     Args:
         messages_iterator: An iterator over the messages found.
         expected: The messages which are expected to be found. If some message
             expected to be found is not found an AssertionError will be raised.
         not_expected: The messages that should not appear.
 
@@ -698,14 +703,16 @@
 
 def verify_log_messages_from_decoded_str(
     s: str,
     expected: Sequence[dict],
     not_expected: Sequence[dict] = _DEFAULT_NOT_EXPECTED,
 ) -> List[dict]:
     """
+    Verifies whether the given messages are available or not in the decoded messages.
+
     Args:
         s: A string with the messages already decoded (where messages are
         separated by lines and each message is a json string to be decoded).
         expected: The messages expected.
         not_expected: The messages that should not appear.
 
     See: `verify_log_messages_from_messages_iterator` for more details on the
@@ -749,14 +756,16 @@
 
 def verify_log_messages_from_log_html(
     log_html: Path,
     expected: Sequence[dict],
     not_expected: Sequence[dict] = _DEFAULT_NOT_EXPECTED,
 ) -> List[dict]:
     """
+    Verifies whether the given messages are available or not in the decoded messages.
+
     Args:
         log_html: The path to the log_html where messages were embedded.
         expected: The messages expected.
         not_expected: The messages that should not appear.
 
     See: `verify_log_messages_from_messages_iterator` for more details on the
         matching of messages.
@@ -767,14 +776,16 @@
 
 def verify_log_messages_from_stream(
     stream: IReadLines,
     expected: Sequence[dict],
     not_expected: Sequence[dict] = _DEFAULT_NOT_EXPECTED,
 ) -> Sequence[dict]:
     """
+    Verifies whether the given messages are available or not in the decoded messages.
+
     Args:
         stream: A stream from where the encoded messages are expected to be read
             from.
         expected: The messages expected.
         not_expected: The messages that should not appear.
 
     See: `verify_log_messages_from_messages_iterator` for more details on the
@@ -823,17 +834,18 @@
     output_dir: Union[str, Path],
     max_file_size: str = "1MB",
     max_files: int = 5,
     log_html: Optional[Union[str, Path]] = None,
     log_html_style: LogHTMLStyle = "standalone",
 ):
     """
-    Adds a log output which will write the contents to the given output
-    directory. Optionally it's possible to collect all the output when the run
-    is finished and put it into a log.html file.
+    Adds a log output which will write the contents to the given output directory.
+
+    Optionally it's possible to collect all the output when the run is finished
+    and put it into a log.html file.
 
     Args:
         output_dir: The output directory where the log contents should be saved.
         max_file_size: The maximum file size for one log file.
         max_files: The maximum amount of files which can be added (if more would
             be needed the oldest one is erased).
         log_html: If given this is the path (file) where the log.html contents
@@ -862,26 +874,28 @@
         logger.close()
 
     return OnExitContextManager(_exit)
 
 
 def close_log_outputs():
     """
-    This method must be called to close loggers (note that some loggers such as
-    the one which outputs html needs to bo closed to actually write the output).
+    This method must be called to close loggers.
+
+    Note that some loggers such as the one which outputs html needs to bo closed
+    to actually write the output.
     """
     while _get_logger_instances():
         logger = next(iter(_get_logger_instances()))
         _get_logger_instances().pop(logger, None)
         logger.close()
 
 
-def add_in_memory_log_output(write):
+def add_in_memory_log_output(write: Callable[[str], Any]):
     """
-    Adds a log output which is in-memory.
+    Adds a log output which is in-memory (receives a callable).
 
     Args:
         write: A callable which will be called as `write(msg)` whenever
         a message is sent from the logging.
 
     Returns:
         A context manager which can be used to automatically remove and
```

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_ast_utils.py` & `robocorp_log-0.1.1/src/robocorp/log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-0.1.1/src/robocorp/log/_auto_logging_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_config.py` & `robocorp_log-0.1.1/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_convert_units.py` & `robocorp_log-0.1.1/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_decoder.py` & `robocorp_log-0.1.1/src/robocorp/log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_index.py` & `robocorp_log-0.1.1/src/robocorp/log/_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
 # Note: autogenerated file.
-# To regenerate this file use: python -m dev build-output-view.
+# To regenerate this file use: inv build-output-view.
 
 # The FILE_CONTENTS contains the contents of the files with
 # html/javascript code which can be used to visualize the contents of the
 # output generated by robocorp-log (i.e.: the .log files).
 
 FILE_CONTENTS = {'index.html': '<!doctype html><html style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%"><head><meta charset="utf-8"/><title>Robot Output</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body class="vscode-dark" style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%; display: flex; flex-direction: column"><div style="display: flex"><div class="summaryField" style="flex-grow: 1; white-space: nowrap" id="summary" class="NOT_RUN">Total:&nbsp;&nbsp;&nbsp;&nbsp;Failures:&nbsp;&nbsp;&nbsp;&nbsp;</div><div class="summaryField" style="flex-grow: 1"><div style="display: flex"><span>Filter:&nbsp;</span> <select name="filterLevel" id="filterLevel" style="flex-grow: 1" onchange="window.onChangedFilterLevel()"><option value="FAIL">FAIL</option><option value="WARN">WARN</option><option value="PASS" selected="selected">PASS</option><option value="NOT RUN">NOT RUN</option></select></div></div><div class="summaryField" id="selectRunContainer" style="flex-grow: 2; display: none"><select name="selectedRun" id="selectedRun" onchange="window.onChangedRun()" style="width: 100%"><option value="NO_RUN" selected="selected">No runs available...</option></select></div></div><div id="mainTree" style="white-space: nowrap; overflow: auto; flex-grow: 1"></div><script>(()=>{"use strict";var e={426:(e,n,t)=>{t.d(n,{Z:()=>o});var s=t(645),a=t.n(s)()((function(e){return e[1]}));a.push([e.id,":root {\\n    --fg-color: var(--vscode-editor-foreground, black);\\n    --bg-color: var(--vscode-editor-background, white);\\n    --font-family: var(--vscode-editor-font-family, monospace, courier);\\n    --font-size: var(--vscode-editor-font-size, 14px);\\n    --font-weight: var(--vscode-font-weight);\\n    --menu-background: var(--vscode-menu-background, rgb(235, 235, 235));\\n    --menu-foreground: var(--vscode-menu-foreground, rgb(0, 0, 0));\\n\\n    /* background-color: var(--vscode-editorError-foreground); */\\n    /* background-color: var(--vscode-inputValidation-errorBorder);  high-contrast doesn\'t have a good color */\\n    /* background-color: var(--vscode-testing-iconErrored);  red and green always (not always ideal...) */\\n    --error-background-color: var(--vscode-terminalCommandDecoration-errorBackground, rgb(201, 28, 28));\\n    --error-color: var(--vscode-button-foreground, white);\\n\\n    --hidden-background-color: var(--vscode-foobarcolornotthere, rgb(243, 152, 16));\\n    --hidden-color: var(--vscode-button-foreground, white);\\n\\n    /* background-color: var(--vscode-inputValidation-infoBorder); */\\n    /* background-color: var(--vscode-testing-iconPassed); */\\n    --pass-background-color: var(--vscode-terminalCommandDecoration-successBackground, rgb(36, 47, 202));\\n    --pass-color: var(--vscode-button-foreground, white);\\n\\n    --warn-background-color: var(--vscode-debugConsole-warningForeground, rgb(190, 159, 20));\\n    --warn-color: var(--vscode-button-foreground, white);\\n\\n    --not-run-background-color: var(--vscode-editor-foreground, rgb(102, 102, 102));\\n    --not-run-color: var(--vscode-editor-background, white);\\n\\n    --summary-hover-background-color: var(--vscode-editor-hoverHighlightBackground, rgb(222, 222, 222));\\n\\n    /* \\n    --fg-color: white;\\n    --bg-color: #4b4a4a;\\n    --font-family: \\"Segoe UI\\", Tahoma, Geneva, Verdana, sans-serif; \\n    */\\n}\\n\\n.summaryField {\\n    margin-left: 3px;\\n    margin-right: 3px;\\n}\\n\\n.summaryFileName {\\n    opacity: 0.6;\\n    margin-left: 1rem;\\n}\\n\\n.timeLabel {\\n    opacity: 0.6;\\n}\\n\\n/* .summaryInput {\\n    opacity: 0.6;\\n} */\\n\\n.summaryInput::before {\\n    margin-left: 3px;\\n    content: \\"(\\";\\n}\\n.summaryInput::after {\\n    margin-right: 3px;\\n    content: \\")\\";\\n}\\n\\n/* nesting level vertical line */\\n.detailInfo {\\n    border-left: 1px solid var(--error-background-color);\\n\\n    /* centering the line with the icon */\\n    margin-left: 1.5rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\nbody {\\n    font-family: var(--font-family);\\n    font-size: var(--font-size);\\n    font-weight: var(--font-weight);\\n    color: var(--fg-color);\\n    background-color: var(--bg-color);\\n}\\n\\n#mainTree {\\n    margin-top: 5px;\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\ndiv ul:not(:first-child) {\\n    border-left: 1px dotted rgb(141, 141, 141);\\n}\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n.tree ul {\\n    margin-left: 10px;\\n    padding-left: 0;\\n}\\n\\n.toolbarButton {\\n    display: inline;\\n    border-radius: 5px;\\n    background: var(--bg-color);\\n    color: var(--fg-color);\\n    margin-left: 3px;\\n    width: 15px;\\n    height: 15px;\\n    border: 0;\\n    padding: 0;\\n    vertical-align: middle;\\n}\\n\\n.toolbarContainer {\\n    display: inline-block;\\n}\\n\\n.summaryDiv {\\n    display: inline;\\n}\\n\\ndetails > summary {\\n    /* Note: couldn\'t get proper color with the svg approach */\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-forward\'><rect width=\'24\' height=\'24\' transform=\'rotate(-90 12 12)\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M10 19a1 1 0 0 1-.64-.23 1 1 0 0 1-.13-1.41L13.71 12 9.39 6.63a1 1 0 0 1 .15-1.41 1 1 0 0 1 1.46.15l4.83 6a1 1 0 0 1 0 1.27l-5 6A1 1 0 0 1 10 19z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮞ \\"; */\\n    /* list-style-type: \\"⏵\\"; */\\n    list-style-type: \\"+ \\";\\n}\\n\\ndetails[open] > summary {\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-downward\'><rect width=\'24\' height=\'24\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M12 16a1 1 0 0 1-.64-.23l-6-5a1 1 0 1 1 1.28-1.54L12 13.71l5.36-4.32a1 1 0 0 1 1.41.15 1 1 0 0 1-.14 1.46l-6 4.83A1 1 0 0 1 12 16z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮟ \\"; */\\n    /* list-style-type: \\"⏷\\"; */\\n    list-style-type: \\"- \\";\\n}\\n\\n.NO_CHILDREN > summary {\\n    list-style-type: \\"\xa0\xa0\\" !important;\\n}\\n\\nselect {\\n    background-color: var(--menu-background);\\n    color: var(--menu-foreground);\\n}\\n\\nsummary {\\n    padding: 3px;\\n}\\n\\na:link {\\n    color: var(--fg-color);\\n}\\n\\na:visited {\\n    color: var(--fg-color);\\n}\\n\\na:hover {\\n    color: var(--fg-color);\\n}\\n\\na:active {\\n    color: var(--fg-color);\\n}\\n\\n.label {\\n    padding: 2px 2px;\\n    font-size: 0.65em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: bold;\\n}\\n\\n.timeLabel {\\n    padding: 2px 2px;\\n    font-size: 0.85em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: lighter;\\n}\\n\\n.label.F,\\n.label.E,\\n.label.FAIL,\\n.label.ERROR {\\n    border-radius: 3px;\\n    background-color: var(--error-background-color);\\n    color: var(--error-color);\\n    font-weight: bolder;\\n}\\n\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n    border-radius: 3px;\\n    background-color: var(--pass-background-color);\\n    color: var(--pass-color);\\n    font-weight: bolder;\\n}\\n\\n.label.W,\\n.label.WARN {\\n    border-radius: 3px;\\n    background-color: var(--warn-background-color);\\n    color: var(--warn-color);\\n    font-weight: bolder;\\n}\\n\\n.label.HIDDEN {\\n    border-radius: 3px;\\n    background-color: var(--hidden-background-color);\\n    color: var(--hidden-color);\\n    font-weight: bolder;\\n}\\n.label.HIDDEN.inline {\\n    margin-left: 5px;\\n}\\n\\nsummary.HIDDEN {\\n    margin-top: 10px;\\n    margin-bottom: 10px;\\n}\\n\\n.label.NOT_RUN {\\n    border-radius: 3px;\\n    background-color: var(--not-run-background-color);\\n    color: var(--not-run-color);\\n    font-weight: bolder;\\n}\\n\\n#summary.FAIL,\\n#summary.ERROR {\\n    border-bottom: 5px solid var(--error-background-color);\\n}\\n\\n#summary.PASS {\\n    border-bottom: 5px solid var(--pass-background-color);\\n}\\n\\n#summary.NOT_RUN {\\n    border-bottom: 5px solid var(--not-run-background-color);\\n}\\n\\n/* .span_link::after {\\n    content: \\" ⮳\\";\\n} */\\n.span_link {\\n    cursor: pointer;\\n    /* text-decoration: underline; */\\n}\\n\\nsummary:hover {\\n    background-color: var(--summary-hover-background-color);\\n}\\n",""]);const o=a},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,s){"string"==typeof e&&(e=[[null,e,""]]);var a={};if(s)for(var o=0;o<this.length;o++){var r=this[o][0];null!=r&&(a[r]=!0)}for(var i=0;i<e.length;i++){var d=[].concat(e[i]);s&&a[d[0]]||(t&&(d[2]?d[2]="".concat(t," and ").concat(d[2]):d[2]=t),n.push(d))}},n}},391:(e,n,t)=>{let s;window.setVSCodeAPI=function(e){s=e};let a={};function o(e){let n;try{n=s}catch(e){}n&&n.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=a[e.request_seq];t&&(delete a[e.request_seq],t(e));break;case"event":let s=r[n.event];s?s(n):console.log("Unhandled event: ",n);break;case"request":let o=i[n.command];o?o(n):console.log("Unhandled request: ",n)}}));let d=0;function l(){return d+=1,d}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=s}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function b(){return document.createElement("div")}function y(e){return e.getAttribute("data-tree-id")}function S(e,n=void 0){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function w(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function C(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&T(e,n);t.open?e.openNodes[y(n)]="open":delete e.openNodes[y(n)]}}function T(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&C(e,t)}const N=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{L()})(...e)}),500)}})();function L(){const e=m();!function(e,n){const t=p("mainTree");let s={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(s=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&T(s,e);e.runIdToTreeState[n]=s;const a=e.runIdLRU.indexOf(n);for(a>-1&&e.runIdLRU.splice(a,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=s}catch(e){}n?n.setState(e):c=e}(e.state)}function _(e,n){if(void 0===e)return;const t=f("selectedRun"),s=new Map;for(let a of t.childNodes)if(a instanceof HTMLOptionElement){const t=a,o=t.value,r=e[o];if(void 0===r)a.remove();else{t.text!==r&&(t.text=r),s.set(o,r);const e=n==o;t.selected=e}}for(const a of Object.keys(e)){if(void 0===a)continue;const o=n==a;if(!s.has(a)){const n=document.createElement("option"),r=e[a];n.value=a,t.appendChild(n),n.selected=o,n.text=r,s.set(a,r)}}}Math.pow(10,8);var x=6e4,I=36e5;var R={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},k=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,M=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function F(e){return e&&parseFloat(e.replace(",","."))||0}var O=[31,null,31,30,31,30,31,31,30,31,30,31];function H(e){return e%400==0||e%4==0&&e%100!=0}function U(e,n){return function(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var s=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==s&&1!==s&&0!==s)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var a,o=function(e){var n,t={},s=e.split(R.dateTimeDelimiter);if(s.length>2)return t;if(/:/.test(s[0])?n=s[0]:(t.date=s[0],n=s[1],R.timeZoneDelimiter.test(t.date)&&(t.date=e.split(R.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var a=R.timezone.exec(n);a?(t.time=n.replace(a[1],""),t.timezone=a[1]):t.time=n}return t}(e);if(o.date){var r=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),s=e.match(t);if(!s)return{year:NaN,restDateString:""};var a=s[1]?parseInt(s[1]):null,o=s[2]?parseInt(s[2]):null;return{year:null===o?a:100*o,restDateString:e.slice((s[1]||s[2]).length)}}(o.date,s);a=function(e,n){if(null===n)return new Date(NaN);var t=e.match(k);if(!t)return new Date(NaN);var s=!!t[4],a=D(t[1]),o=D(t[2])-1,r=D(t[3]),i=D(t[4]),d=D(t[5])-1;if(s)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,d)?function(e,n,t){var s=new Date(0);s.setUTCFullYear(e,0,4);var a=7*(n-1)+t+1-(s.getUTCDay()||7);return s.setUTCDate(s.getUTCDate()+a),s}(n,i,d):new Date(NaN);var l=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(O[n]||(H(e)?29:28))}(n,o,r)&&function(e,n){return n>=1&&n<=(H(e)?366:365)}(n,a)?(l.setUTCFullYear(n,o,Math.max(a,r)),l):new Date(NaN)}(r.restDateString,r.year)}if(!a||isNaN(a.getTime()))return new Date(NaN);var i,d=a.getTime(),l=0;if(o.time&&(l=function(e){var n=e.match(M);if(!n)return NaN;var t=F(n[1]),s=F(n[2]),a=F(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,s,a)?t*I+s*x+1e3*a:NaN}(o.time),isNaN(l)))return new Date(NaN);if(!o.timezone){var c=new Date(d+l),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var n=e.match(A);if(!n)return 0;var t="+"===n[1]?-1:1,s=parseInt(n[2]),a=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,a)?t*(s*I+a*x):NaN}(o.timezone),isNaN(i)?new Date(NaN):new Date(d+l+i)}(n).toString()}function B(e,n){var t,s;const a=J(n,":");if(a){[t,s]=a;try{s=JSON.parse(s)}catch(e){return console.log("Error parsing json: "+s),console.log(e),null}e.memo[t]=s}return null}function P(e,n){const[t,s]=J(n,":"),[a,o,r,i,d]=s.split("|",5);e.location_memo[t]=[e.memo[a],e.memo[o],e.memo[r],e.memo[i],parseInt(d)]}function j(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function $(e,n){return parseFloat(n)}function z(e,n){return parseInt(n)}function Y(e,n){return n}function V(e,n){return JSON.parse(n)}function W(e){if("memorize"===e)return B;if("memorize_path"===e)return P;const n=[],t=new Map;for(let s of e.split(",")){let e;if(s=s.trim(),-1==s.indexOf(":"))throw new Error("Unexpected definition: {message_definition}");if([s,e]=s.split(":",2),n.push(s),"oid"===e)t.set(s,j);else if("int"===e)t.set(s,z);else if("float"===e)t.set(s,$);else if("str"===e)t.set(s,Y);else{if("json.loads"===e)return V;if("dateisoformat"===e)return U;if("loc_id"===e)t.set(s,"loc_id");else{if("loc_and_doc_id"!==e)throw new Error("Unexpected: "+e);t.set(s,"loc_and_doc_id")}}}return function(e,s){const a=s.split("|",n.length),o={};for(let s=0;s<a.length;s++){const r=a[s],i=n[s],d=t.get(i);if("loc_id"===d){const n=e.location_memo[r];o.name=n[0],o.libname=n[1],o.source=n[2],o.lineno=n[4]}else if("loc_and_doc_id"===d){const n=e.location_memo[r];o.name=n[0],o.libname=n[1],o.source=n[2],o.doc=n[3],o.lineno=n[4]}else o[i]=d(e,r)}return o}}const q={};!function(){for(let e of"\\n# Each message should use a single line in the log output where the prefix\\n# is the message type and the arguments is either a message with ids/numbers\\n# separated by \'|\' or json-encoded strings.\\n#\\n# Note that each output log file (even if splitted after the main one) should be\\n# readable in a completely independent way, so, the starting scope should be\\n# replicated as well as the needed names to memorize.\\n#\\n# To keep the format compact, some strings and locations are referenced through ids. \\n# \\n# In the spec \'oid\' are used to reference a message memorized with \'M\' and \\n# \'loc_id\' or \'loc_and_doc_id\' a message memorized with \'P\'.\\n#\\n# There\'s an initial time and other time references are time-deltas from this time.\\n#\\n# The spec for the messages is below:\\n#\\n\\n# Version of the log output\\n# Example: \'V 0.0.1\' - Identifies version 1 of the log\\nV: version:str\\n\\n# Some information message\\n# Example: \'I \\"python=3.7\\"\'\\nI: info:json.loads\\n\\n# The log has an id that may be split into multiple parts.\\n# \'ID: 1|36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2\'     1st part with identifier 36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2.\\n# \'ID: 2|36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2\'     2nd part with identifier 36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2.\\nID: part:int, id:str\\n\\n# Initial time in UTC (all others are based on a delta from this date).\\n# Example: \'T 2022-10-03T11:30:54.927+00:00\'\\nT: time:dateisoformat\\n\\n# Memorize some word (to be used as oid).\\n# i.e.: when the message is something as \'M a:\\"Start\\"\', we memorize \\"Start\\" with key: \\"a\\"\\n# Example: \'M a:\\"Start\\"\'\\nM: memorize\\n\\n# Memorize a path location (name/libname/source/lineno/docstring) to be referenced as loc_id or loc_and_doc_id.\\n# Note: loc_id and loc_and_doc_id use the same info but one unpacks the docstring and the other doesn\'t\\n# Example: \'P a|b|c|d|e\' (where those are references to strings memoized with \'M\').\\nP: memorize_path\\n\\n# Log (raw text)\\n# level_enum is:\\n# - ERROR = \'E\'\\n# - FAIL = \'F\'\\n# - INFO = \'I\'\\n# - WARN = \'W\'\\n#\\n# Example:\\n#\\n# \'L E|a|b|0.123\'\\nL: level:str, message:oid, loc:loc_id, time_delta_in_seconds:float\\n\\n# A message which is intended to be sent to to the console\\n# This can be either a message being sent by the user to stdout/stderr\\n# (if those are being redirected) or some message from the framework\\n# intended to be shown in the console.\\n#\\n# Expected \\"kind\\" values:\\n#\\n# User messages:\\n# \\"stdout\\": Some user message which was being sent to the stdout.\\n# \\"stderr\\": Some user message which was being sent to the stderr.\\n#\\n# Messages from the framework:\\n# \\"regular\\": Some regular message.\\n# \\"important\\": Some message which deserves a bit more attention.\\n# \\"task_name\\": The task name is being written.\\n# \\"error\\": Some error message.\\n# \\"traceback\\": Some traceback message.\\n#\\n# Example:\\n#\\n# \'C a|b|0.123\'\\nC: kind:oid, message:oid, time_delta_in_seconds:float\\n\\n# Log (html) -- same thing as Log but the message must be interpreted as HTML.\\n# So, something as <img alt=\\"screenshot\\" src=\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABAAAAAEgCAIAAACl65ZFAAEAAElEQVR4nOz9d7R...\\"/>\\n# would be interpreted as an image in the final HTML. \\nLH=L\\n\\n# Start Run\\nSR: name:oid, time_delta_in_seconds:float\\n\\n# End Run\\nER: status:oid, time_delta_in_seconds:float\\n\\n# Start Task\\nST: loc:loc_id, time_delta_in_seconds:float\\n\\n# End Task\\n# status may be:\\n# \\"PASS\\": Everything went well.\\n# \\"ERROR\\": There was some detected error while running the task.\\nET: status:oid, message:oid, time_delta_in_seconds:float\\n\\n# Start Element \\n# Should be sent when some element we\'re tracking such as method, for, while, etc. starts.\\n# The \'type\' can be:\\n#\\n# METHOD\\n#\\n# GENERATOR\\n#\\n# UNTRACKED_GENERATOR (untracked generator is a generator in a library, where we\\n# just track the start/end and not what happens inside it).\\nSE: loc:loc_and_doc_id, type:oid, time_delta_in_seconds:float\\n\\n# Yield Resume (coming back to a suspended frame).\\n# Should be sent when a given frame is resumed from a yield.\\nYR: loc:loc_id, time_delta_in_seconds:float\\n\\n# Yield From Resume (coming back to a suspended frame).\\n# Should be sent when a given frame is resumed from a yield from.\\nYFR: loc:loc_id, time_delta_in_seconds:float\\n\\n# End Element\\n# When the element ends, provide its status (\\"PASS\\", \\"ERROR\\") and the time at which it finished.\\nEE: type:oid, status:oid, time_delta_in_seconds:float\\n\\n# Yield Suspend (pausing a frame)\\n# Should be sent when a given frame is suspended in a yield.\\nYS: loc:loc_id, type:oid, value:oid, time_delta_in_seconds:float\\n\\n# Yield From Suspend (pausing a frame)\\n# Should be sent when a given frame is suspended in a yield from.\\nYFS: loc:loc_id, time_delta_in_seconds:float\\n\\n# Assign\\n# Assign some content (type, value) to a variable (target) in the given location (loc). \\nAS: loc:loc_id, target:oid, type:oid, value:oid, time_delta_in_seconds:float\\n\\n# Element/method argument (name and value of the argument).\\n# Adds some argument (name) to the current element (with the given type and value).\\nEA: name:oid, type:oid, value:oid\\n\\n# Set some time for the current scope (usually not needed as the time\\n# is usually given in the element itself).\\nS: start_time_delta:float\\n\\n# --------------------------------------------------------------- Tracebacks\\n# Start traceback with the exception error message.\\n# Note: it should be possible to start a traceback inside another traceback\\n# for cases where the exception has an exception cause.\\n\\n# Start Traceback\\nSTB: message:oid, time_delta_in_seconds:float\\n\\n# Traceback Entry\\nTBE: source:oid, lineno:int, method:oid, line_content:oid\\n\\n# Traceback variable\\nTBV: name:oid, type:oid, value:oid\\n\\n# End Traceback\\nETB: time_delta_in_seconds:float\\n\\n# These messages have the same format (just the message type is different).\\nRR=SR\\nRT=ST\\nRE=SE\\nRTB=STB\\nRYR=YR\\n".split(/\\r?\\n/))if(e=e.trim(),0!==e.length&&!e.startsWith("#"))try{let[n,t]=J(e,":");n=n.trim(),t=t.trim(),q[n]=W(t)}catch(n){let[t,s]=J(e,"=");t=t.trim(),s=s.trim(),q[t]=q[s]}}();class G{constructor(){this.memo={},this.location_memo={}}decode_message_type(e,n){return(0,q[e])(this,n)}}function J(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*Z(e,n){var t,s,a;for(let o of e.split(/\\r?\\n/))if(o=o.trim(),o)try{const e=J(o," ");if(e&&([a,s]=e,t=n.decode_message_type(a,s))){const e={message_type:a,decoded:t};yield e}}catch(e){console.log("Unable to decode message: "+o),console.log(e)}}function K(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function Q(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function X(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class ee{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,s){const a=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:s,variables:a})}pushVar(e,n,t){this.stack.at(-1).variables.set(e,[n,t])}}class ne{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function te(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),s=document.createElement("details");e&&(s.open=e),s.classList.add("NO_CHILDREN"),t.appendChild(s);const a=b();a.classList.add("detailContainer"),s.appendChild(a);const o=document.createElement("summary"),r=b();r.classList.add("summaryDiv"),o.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const d=v();return d.className="summaryInput emptySummaryInput",d.textContent="",r.appendChild(d),s.appendChild(o),{li:t,details:s,summary:o,summaryDiv:r,summaryName:i,summaryInput:d,detailContainer:a}}function se(e,n){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${n}`}function ae(e,n,t,s,a,o,r,i,d,l){const c=e.state.runIdToTreeState[e.runId],u="li_"+l;if(c){const e=c.openNodes;e&&(o=e[u])}const m=te(o,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,b=m.summaryName,y=m.summaryInput;if("LH"===a.message_type){b.textContent="";const e=w(t);b.appendChild(e)}else b.textContent=t;s&&(b.title=s),e.onClickReference&&(b.classList.add("span_link"),b.onclick=n=>{const t=[];let s=d.parent;for(;void 0!==s&&void 0!==s.message;)t.push(s.message),s=s.parent;n.preventDefault(),e.onClickReference({source:r,lineno:i,message:a.decoded,messageType:a.message_type,scope:t})});const S=g("ul_"+l);p.appendChild(S);const C={ul:S,li:h,details:p,detailContainer:f,summary:v,summaryName:b,summaryInput:y,source:r,lineno:i,appendContentChild:void 0,decodedMessage:a,maxLevelFoundInHierarchy:-1,summaryDiv:E};return C.appendContentChild=le.bind(C),n.appendContentChild(C),C}let oe,re;function*ie(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of de(e))yield n;yield n}}function*de(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of ie(n))yield e}function le(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){N()})),m().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===oe){oe=b(),oe.classList.add("toolbarContainer");const e=E();e.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==re){re.details.open=!0;for(let e of de(re.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=E();return n.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==re){re.details.open=!1;for(let e of de(re.ul))e.open=!1}}()},oe.appendChild(n),void oe.appendChild(e)}re=e,e.summaryDiv.appendChild(oe)}(n)})))}var ce=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let ue=0,me=-1;class he{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new ee(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class pe{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new G,this.seenSuiteTaskOrElement=!1,this.tbHandler=new he,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new ne,this.lease=(ue+=1,me=ue,ue),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===me&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return ce(this,null,(function*(){for(const e of Z(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return ce(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of Z(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return ce(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let s,a,o=e.message_type;switch(o){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;o="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;o="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;o="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;o="STB"}switch(this.id+=1,o){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"AS":a=ae(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),se(a,e.decoded.value),this.addAssignCssClass(a);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=ae(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":case"YR":case"YFR":if("SE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){this.messageNode={parent:this.messageNode,message:e};let n=e.decoded.name;"YR"==o&&(n+=" (resumed)"),this.parent=ae(this.opts,this.parent,n,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),"YR"==o&&this.addResumedCSSClass(this.parent),this.argsTarget=this.parent,this.stack.push(this.parent)}else{const n=ae(this.opts,this.parent,`Create Generator: ${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addGeneratorCSSClass(n),this.argsTarget=n}break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),s=this.addDetailsCSSClasses(e.decoded.status,r),s&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":case"YS":case"YFS":if("EE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){if("YS"==o||"YFS"==o){const n=ae(this.opts,this.parent,"Yielded",`Suspending function with yield.\\nYielding an object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addYieldedCSSClass(n),se(n,e.decoded.value),e.decoded.status="PASS"}this.messageNode=this.messageNode.parent;let n=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(n,this.parent,e),this.onEndSetStatusOrRemove(this.opts,n,e.decoded,this.parent,!0),s=this.addDetailsCSSClasses(e.decoded.status,n),s&&(n.details.open=!0)}break;case"S":const i=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":!function(e,n,t,s){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n} = ${s}`,e.summaryInput.title=`Argument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.classList.remove("emptySummaryInput")):(e.summaryInput.title+=`\\n\\nArgument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.textContent+=`, ${n} = ${s}`)}(this.argsTarget,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const d=e.decoded.level,l=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(d);if(l>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=l),Q(this.opts,l)){const n=ae(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=l,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,d),this.addDetailsCSSClasses(l,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const n=c.stack[0],t=c.exceptionMsg.split(":",2);let s,o;t.length>1?(s=t[0],o=t[1]):(s="Error",o=t[0]),a=ae(this.opts,this.parent,s,"",e,!1,n.source,n.lineno,this.messageNode,this.id.toString()),se(a,o),this.addExceptionCssClass(a)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addYieldedCSSClass(e){e.details.classList.add("yiededParent"),e.details.classList.add("leafNode")}addResumedCSSClass(e){e.details.classList.add("resumedParent")}addGeneratorCSSClass(e){e.details.classList.add("generatorParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,n){let t,s=!1;return t="string"==typeof e?X(e):e,t>=2?(n.details.classList.add("errorParent"),s=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),s}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const s=X(t.decoded.status);s>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=s),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,s,a){const o=t.status;if(Q(e,n.maxLevelFoundInHierarchy)){if(a&&n.maxLevelFoundInHierarchy<=0){const e=50;if(s.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=y(n.li);if(n.li.remove(),S(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=te(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const a=v();a.setAttribute("role","button"),a.textContent="...",a.classList.add("label"),a.classList.add("HIDDEN"),a.classList.add("inline"),e.summaryDiv.appendChild(a);const o=v();o.setAttribute("role","button"),o.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(o),K(e,"HIDDEN"),S(e.li,!0),s.ul.appendChild(e.li)}return}}}if(n.summary,K(n,o),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var fe=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let ge;function ve(){return fe(this,null,(function*(){ge=new pe,ge.clearAndInitializeTree(),yield ge.addInitialContents()}))}function Ee(e){let n={type:"event",seq:l(),event:"onClickReference"};n.data=e,o(n)}function be(e){L();const n=m();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==s&&(n.onClickReference=Ee),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,_(n.allRunIdsToLabel,n.runId),ve()}t(320),i.setContents=be,i.appendContents=function(e){const n=m();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==ge&&ge.onAppendedContents())},i.updateLabel=function(e){const n=m();n.allRunIdsToLabel[e.runId]=e.label,_(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:l(),event:"onSetCurrentRunId"};n.data={runId:e},o(n)},window.onChangedFilterLevel=function(){!function(e){const n=m();n.state.filterLevel!==e&&(n.state.filterLevel=e,L(),ve())}(f("filterLevel").value)},window.setContents=be,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},320:(e,n,t)=>{var s=t(379),a=t.n(s),o=t(426),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};a()(o.Z,r),o.Z.locals},379:(e,n,t)=>{var s,a=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),o=[];function r(e){for(var n=-1,t=0;t<o.length;t++)if(o[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},s=[],a=0;a<e.length;a++){var i=e[a],d=n.base?i[0]+n.base:i[0],l=t[d]||0,c="".concat(d," ").concat(l);t[d]=l+1;var u=r(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(o[u].references++,o[u].updater(m)):o.push({identifier:c,updater:f(m,n),references:1}),s.push(c)}return s}function d(e){var n=document.createElement("style"),s=e.attributes||{};if(void 0===s.nonce){var o=t.nc;o&&(s.nonce=o)}if(Object.keys(s).forEach((function(e){n.setAttribute(e,s[e])})),"function"==typeof e.insert)e.insert(n);else{var r=a(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(n)}return n}var l,c=(l=[],function(e,n){return l[e]=n,l.filter(Boolean).join("\\n")});function u(e,n,t,s){var a=t?"":s.media?"@media ".concat(s.media," {").concat(s.css,"}"):s.css;if(e.styleSheet)e.styleSheet.cssText=c(n,a);else{var o=document.createTextNode(a),r=e.childNodes;r[n]&&e.removeChild(r[n]),r.length?e.insertBefore(o,r[n]):e.appendChild(o)}}function m(e,n,t){var s=t.css,a=t.media,o=t.sourceMap;if(a?e.setAttribute("media",a):e.removeAttribute("media"),o&&"undefined"!=typeof btoa&&(s+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o))))," */")),e.styleSheet)e.styleSheet.cssText=s;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(s))}}var h=null,p=0;function f(e,n){var t,s,a;if(n.singleton){var o=p++;t=h||(h=d(n)),s=u.bind(null,t,o,!1),a=u.bind(null,t,o,!0)}else t=d(n),s=m.bind(null,t,n),a=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return s(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;s(e=n)}else a()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===s&&(s=Boolean(window&&document&&document.all&&!window.atob)),s));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var s=0;s<t.length;s++){var a=r(t[s]);o[a].references--}for(var d=i(e,n),l=0;l<t.length;l++){var c=r(t[l]);0===o[c].references&&(o[c].updater(),o.splice(c,1))}t=d}}}}},n={};function t(s){var a=n[s];if(void 0!==a)return a.exports;var o=n[s]={id:s,exports:{}};return e[s](o,o.exports,t),o.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var s in n)t.o(n,s)&&!t.o(e,s)&&Object.defineProperty(e,s,{enumerable:!0,get:n[s]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(391),t(320)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(true);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
```

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_index_v2.py` & `robocorp_log-0.1.1/src/robocorp/log/_index_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
 # Note: autogenerated file.
-# To regenerate this file use: python -m dev build-output-view.
+# To regenerate this file use: inv build-output-view.
 
 # The FILE_CONTENTS contains the contents of the files with
 # html/javascript code which can be used to visualize the contents of the
 # output generated by robocorp-log (i.e.: the .log files).
 
 FILE_CONTENTS = {'index.html': '<!doctype html><html><head><meta charset="utf-8"/><title class="suiteHeader">Robocorp Log</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body><div class="headerTitleSection"><h3 class="suiteHeader">Robocorp Log</h3><span id="suiteResult" class="label" style="display: none;"></span></div><div id="suiteRunStart" class="headerRunDetails"></div><div class="headers"><span class="headerSource"></span> <span class="headerInputs">Details</span></div><div id="mainTree"></div><script>(()=>{"use strict";var e={599:(e,n,t)=>{t.d(n,{Z:()=>o});var s=t(645),a=t.n(s)()((function(e){return e[1]}));a.push([e.id,\'/* ******************************* */\\n/* CONTAINERS ETC */\\n\\n/* box model reset */\\n* {\\n    box-sizing: border-box;\\n}\\n\\nhtml,\\nbody {\\n    margin: 0;\\n    padding: 0;\\n    height: 100%;\\n}\\n\\n:root {\\n    --right-column-width-narrow: 50vw;\\n    --right-column-width-wide: 60vw;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --sans-font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu",\\n        "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", Arial, sans-serif;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --fixed-font-family: ui-monospace, Menlo, Monaco, "Cascadia Mono", "Segoe UI Mono", "Roboto Mono", "Oxygen Mono",\\n        "Ubuntu Monospace", "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New", monospace;\\n}\\n\\n/* ******************************* */\\n/* THEMING SUPPORT */\\n\\n@media (prefers-color-scheme: light) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-variable: #5070b4;\\n\\n        --log-color-warn: #93801c;\\n        --log-color-disabled: #999999;\\n        --log-color-border: #dddddd;\\n\\n        --log-color-text: #000000;\\n        --log-color-text-weaker: #444444;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #ffffff;\\n        --log-color-bg-raised: #f3f3f3;\\n    }\\n}\\n\\n@media (prefers-color-scheme: dark) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-warn: #fff565;\\n        --log-color-variable: #4094c5;\\n\\n        --log-color-disabled: #666666;\\n        --log-color-border: #444444;\\n\\n        --log-color-text: #eeeeee;\\n        --log-color-text-weaker: #bbbbbb;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #222222;\\n        --log-color-bg-raised: #333333;\\n    }\\n}\\n\\nbody {\\n    display: flex;\\n    flex-direction: column;\\n    padding: 1rem;\\n    font-size: 0.8rem;\\n    font-family: var(--sans-font-family);\\n    color: var(--log-color-text);\\n    background-color: var(--log-color-bg);\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\n#mainTree {\\n    white-space: nowrap;\\n    overflow: auto;\\n    flex-grow: 1;\\n}\\n\\n/* ******************************* */\\n/* TREE */\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n/* nesting level vertical line */\\n.tree ul:not(:first-child),\\n.detailContainer {\\n    border-left: 1px solid var(--log-color-border);\\n\\n    /* centering the line with the icon */\\n    margin-left: 0.65rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\ndetails.errorParent .tree ul:not(:first-child),\\ndetails.errorParent .detailContainer {\\n    border-color: var(--log-color-error);\\n}\\n\\n/* ******************************* */\\n/* SUMMARY ROW FOR EACH CODE ROW */\\n\\ndetails.parentNode > summary,\\ndetails.errorParent.leafNode > summary {\\n    cursor: pointer;\\n}\\n\\ndetails > summary {\\n    padding-top: 0.25rem;\\n    padding-bottom: 0.25rem;\\n    padding-left: 0.25rem;\\n\\n    /* chrome needs this, safari doesn\\\'t */\\n    list-style: none;\\n}\\n\\ndetails > summary:hover {\\n    background-color: var(--log-color-bg-raised);\\n    border-radius: 2px;\\n}\\n\\ndetails > summary::-webkit-details-marker {\\n    display: none;\\n}\\n\\ndetails > summary::marker {\\n    display: none;\\n}\\n\\ndetails > summary::before {\\n    background-color: var(--log-color-success);\\n}\\n\\ndetails.errorParent > summary::before {\\n    background-color: var(--log-color-error);\\n}\\n\\ndetails.warnParent > summary::before {\\n    background-color: var(--log-color-warn);\\n}\\n\\n/* icon from: https://github.com/twbs/icons/blob/main/icons/caret-right-square-fill.svg */\\ndetails > summary::before {\\n    position: absolute;\\n    left: 0.25rem;\\n    top: 4px;\\n\\n    /* chrome seems to need the \\\'-webkit\\\' prefix here */\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="black" class="bi bi-caret-right-square-fill" viewBox="0 0 16 16"><path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm5.5 10a.5.5 0 0 0 .832.374l4.5-4a.5.5 0 0 0 0-.748l-4.5-4A.5.5 0 0 0 5.5 4v8z"/></svg>\\\');\\n    width: 1rem;\\n    height: 1rem;\\n    display: inline-block;\\n    content: "";\\n}\\n\\n/* filled icon */\\n/*details.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square-fill" viewBox="0 0 16 16"><path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2zm10.03 4.97a.75.75 0 0 1 .011 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.75.75 0 0 1 1.08-.022z"/></svg>\\\');\\n}*/\\n\\ndetails.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h12zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"/><path d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.235.235 0 0 1 .02-.022z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (debug-pause) */\\ndetails.leafNode.yiededParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M4.5 3H6v10H4.5V3zm7 0v10H10V3h1.5z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (circuit-board) */\\ndetails.leafNode.generatorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14.5 1h-13l-.5.5v13l.5.5h13l.5-.5v-13l-.5-.5zM14 14H5v-2h2.3c.3.6 1 1 1.7 1 1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2H4v3H2V2h2v2.3c-.6.3-1 1-1 1.7 0 1.1.9 2 2 2s2-.9 2-2h2c0 1.1.9 2 2 2s2-.9 2-2-.9-2-2-2c-.7 0-1.4.4-1.7 1H6.7c-.3-.6-1-1-1.7-1V2h9v12zm-6-3c0-.6.4-1 1-1s1 .4 1 1-.4 1-1 1-1-.4-1-1zM5 5c.6 0 1 .4 1 1s-.4 1-1 1-1-.4-1-1 .4-1 1-1zm6 0c.6 0 1 .4 1 1s-.4 1-1 1-1-.4-1-1 .4-1 1-1z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (debug-restart-frame) */\\ndetails.resumedParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M1 10V9h5.207a5.48 5.48 0 0 0-.185 1H1zm6.257-3a5.54 5.54 0 0 1 1.08-1H1v1h6.257zM6.6 13a5.465 5.465 0 0 1-.393-1H1v1h5.6zM15 3v1H1V3h14zm-3.36 10.031a2.531 2.531 0 1 0-2.192-3.797h1.068v.844h-1.97l-.421-.422v-2.25h.844v1.032a3.375 3.375 0 1 1-.423 3.412l.782-.318a2.532 2.532 0 0 0 2.313 1.5z"></path></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (symbol-variable) */\\ndetails.leafNode.variableParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M2 5h2V4H1.5l-.5.5v8l.5.5H4v-1H2V5zm12.5-1H12v1h2v7h-2v1h2.5l.5-.5v-8l-.5-.5zm-2.74 2.57L12 7v2.51l-.3.45-4.5 2h-.46l-2.5-1.5-.24-.43v-2.5l.3-.46 4.5-2h.46l2.5 1.5zM5 9.71l1.5.9V9.28L5 8.38v1.33zm.58-2.15l1.45.87 3.39-1.5-1.45-.87-3.39 1.5zm1.95 3.17l3.5-1.56v-1.4l-3.5 1.55v1.41z"></path></svg>\\\');\\n    background-color: var(--log-color-variable);\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (bracket-error) */\\ndetails.leafNode.exceptionParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M6 2.97184V2.98361H5.91083C5.71113 2.98361 5.5238 3.02427 5.34802 3.10513C5.17461 3.18275 5.02193 3.28942 4.89086 3.42437C4.76421 3.55475 4.66135 3.71034 4.58238 3.89205C4.50833 4.07152 4.47134 4.26019 4.47134 4.45902C4.47134 4.68725 4.4753 4.9134 4.48321 5.13749C4.49125 5.36105 4.49127 5.58262 4.48324 5.80219C4.47914 6.01973 4.46082 6.2333 4.42826 6.44285C4.39513 6.65175 4.33913 6.85263 4.26039 7.04464C4.18091 7.23843 4.07258 7.42254 3.93616 7.59702C3.82345 7.74119 3.68538 7.87538 3.52283 8C3.68538 8.12462 3.82345 8.25881 3.93616 8.40298C4.07258 8.57746 4.18091 8.76157 4.26039 8.95536C4.33921 9.14757 4.39513 9.35024 4.42823 9.56312C4.46084 9.76883 4.47914 9.98246 4.48324 10.2039C4.49127 10.4195 4.49125 10.6411 4.48321 10.8686C4.4753 11.0885 4.47134 11.3127 4.47134 11.541C4.47134 11.744 4.50838 11.9346 4.58223 12.1137C4.66104 12.2911 4.76386 12.4469 4.89086 12.5818C5.02194 12.7126 5.17396 12.8191 5.34763 12.9008C5.52346 12.9777 5.71095 13.0164 5.91083 13.0164H6V13.2V14H5.91083C5.59743 14 5.29407 13.9384 5.00128 13.8153C4.70818 13.692 4.44942 13.5153 4.22578 13.285C4.00311 13.0558 3.83793 12.805 3.73283 12.5323L3.73232 12.531C3.63387 12.265 3.56819 11.9903 3.53535 11.7072L3.53516 11.7055C3.50677 11.4215 3.4987 11.1316 3.51084 10.8357C3.52272 10.5462 3.52866 10.2567 3.52866 9.96721C3.52866 9.76883 3.48986 9.58047 3.41201 9.40108L3.41129 9.39942C3.33659 9.21871 3.23428 9.0637 3.10412 8.93352L3.10221 8.93161C2.97577 8.79762 2.82457 8.69157 2.64742 8.61396L2.64601 8.61334C2.47001 8.53238 2.28465 8.4918 2.08917 8.4918H2V8.4V7.6V7.5082H2.08917C2.28497 7.5082 2.4706 7.46954 2.64672 7.3925C2.82466 7.31055 2.97644 7.20405 3.10317 7.07359C3.23423 6.93866 3.33687 6.78296 3.4116 6.60601L3.412 6.60507C3.48974 6.42594 3.52866 6.23556 3.52866 6.03279C3.52866 5.74329 3.52272 5.45379 3.51084 5.16428C3.4987 4.86844 3.50678 4.5805 3.53519 4.30053L3.53533 4.29917C3.56814 4.01201 3.63382 3.7352 3.73233 3.46898L3.73282 3.46766C3.83792 3.19498 4.00311 2.94422 4.22578 2.71498C4.44942 2.48474 4.70818 2.30798 5.00128 2.18473C5.29407 2.06161 5.59743 2 5.91083 2H6V2.97184ZM13.9232 8.4918H14V8.4V7.6V7.5082H13.9108C13.7153 7.5082 13.53 7.46762 13.354 7.38666L13.3526 7.38604C13.1754 7.30844 13.0242 7.20238 12.8978 7.06839L12.8959 7.06648C12.7657 6.9363 12.6634 6.78129 12.5887 6.60058L12.588 6.59892C12.5101 6.41953 12.4713 6.23117 12.4713 6.03279C12.4713 5.74329 12.4773 5.45379 12.4892 5.16428C12.5013 4.86842 12.4932 4.57848 12.4648 4.29454L12.4646 4.29285C12.4318 4.00971 12.3661 3.73502 12.2677 3.46897L12.2672 3.46766C12.1621 3.19499 11.9969 2.94422 11.7742 2.71498C11.5506 2.48474 11.2918 2.30798 10.9987 2.18473C10.7059 2.06161 10.4026 2 10.0892 2H10V2.8V2.98361H10.0892C10.2891 2.98361 10.4765 3.0223 10.6524 3.09917C10.826 3.18092 10.9781 3.28736 11.1091 3.41823C11.2361 3.55305 11.339 3.70889 11.4178 3.88628C11.4916 4.0654 11.5287 4.25596 11.5287 4.45902C11.5287 4.68727 11.5247 4.91145 11.5168 5.13142C11.5088 5.35894 11.5087 5.58049 11.5168 5.79605C11.5209 6.01754 11.5392 6.23117 11.5718 6.43688C11.6049 6.64976 11.6608 6.85243 11.7396 7.04464C11.8191 7.23843 11.9274 7.42254 12.0638 7.59702C12.1765 7.74119 12.3146 7.87538 12.4772 8L12.4456 8.02455C12.9764 8.08338 13.4758 8.24605 13.9232 8.4918Z"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M10.3333 9.50559C10.8266 9.17595 11.4067 9 12 9C12.7954 9.00098 13.5578 9.31736 14.1202 9.87976C14.6826 10.4422 14.999 11.2047 15 12C15 12.5933 14.8241 13.1734 14.4944 13.6667C14.1648 14.1601 13.6962 14.5446 13.1481 14.7716C12.5999 14.9987 11.9967 15.0581 11.4147 14.9424C10.8328 14.8266 10.2982 14.5409 9.87868 14.1213C9.45912 13.7018 9.1734 13.1672 9.05765 12.5853C8.94189 12.0033 9.0013 11.4001 9.22836 10.8519C9.45543 10.3038 9.83994 9.83524 10.3333 9.50559ZM13.1464 10.1464L12 11.2929L10.8536 10.1464L10.1465 10.8535L11.2929 12L10.1464 13.1464L10.8536 13.8536L12 12.7071L13.1465 13.8535L13.8536 13.1464L12.7071 12L13.8536 10.8536L13.1464 10.1464Z"></path></svg>\\\');\\n    background-color: var(--log-color-error);\\n}\\n.exceptionParent {\\n    font-weight: bold;\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (error) */\\ndetails.leafNode.errorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M8.6 1c1.6.1 3.1.9 4.2 2 1.3 1.4 2 3.1 2 5.1 0 1.6-.6 3.1-1.6 4.4-1 1.2-2.4 2.1-4 2.4-1.6.3-3.2.1-4.6-.7-1.4-.8-2.5-2-3.1-3.5C.9 9.2.8 7.5 1.3 6c.5-1.6 1.4-2.9 2.8-3.8C5.4 1.3 7 .9 8.6 1zm.5 12.9c1.3-.3 2.5-1 3.4-2.1.8-1.1 1.3-2.4 1.2-3.8 0-1.6-.6-3.2-1.7-4.3-1-1-2.2-1.6-3.6-1.7-1.3-.1-2.7.2-3.8 1-1.1.8-1.9 1.9-2.3 3.3-.4 1.3-.4 2.7.2 4 .6 1.3 1.5 2.3 2.7 3 1.2.7 2.6.9 3.9.6zM7.9 7.5L10.3 5l.7.7-2.4 2.5 2.4 2.5-.7.7-2.4-2.5-2.4 2.5-.7-.7 2.4-2.5-2.4-2.5.7-.7 2.4 2.5z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (warn) */\\ndetails.leafNode.warnParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M7.56 1h.88l6.54 12.26-.44.74H1.44L1 13.26 7.56 1zM8 2.28L2.28 13H13.7L8 2.28zM8.625 12v-1h-1.25v1h1.25zm-1.25-2V6h1.25v4h-1.25z"/></svg>\\\');\\n}\\n\\ndetails.parentNode > summary::before,\\ndetails.parentNode.errorParent > summary::before {\\n    transform-origin: 8px 8px;\\n    transform: rotate(0deg);\\n    transition: transform 0.2s ease-out !important;\\n}\\n\\ndetails[open].parentNode > summary::before,\\ndetails[open].parentNode.errorParent > summary::before {\\n    transform: rotate(90deg);\\n}\\n\\ndetails[open] > summary > .summaryDiv > .summaryInput {\\n    /* Display full input parameters when expanded by adjusting the\\n       white-space to wrap the contents. Even nodes that don\\\'t have\\n       children can be expanded in this way, but it is not obvious\\n       since there is no triangle icon next to them. */\\n    white-space: initial;\\n}\\n\\n.summaryDiv {\\n    /* aligns code line correctly with the icon */\\n    display: flex;\\n    margin-left: 1.2rem;\\n}\\n\\n.summaryDiv > .label {\\n    order: 2;\\n}\\n\\n.summaryDiv > .summaryName {\\n    order: 1;\\n\\n    margin-left: 0.5rem;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv > .summaryName,\\n.detailContainer > .detailInfo {\\n    /* this forces the correct column size, see:\\n       https://makandracards.com/makandra/66994-css-flex-and-min-width */\\n    min-width: 0;\\n}\\n\\ndetails.errorParent > summary > .summaryDiv > .summaryName {\\n    font-weight: bold;\\n}\\n\\n.summaryDiv > .summaryInput {\\n    order: 4;\\n    margin-left: auto;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.summaryDiv > .summaryInput.emptySummaryInput {\\n    color: var(--log-color-text-weakest);\\n}\\n\\n.detailContainer {\\n    display: flex;\\n}\\n\\n.detailContainer > .detailInfo {\\n    margin-right: auto;\\n}\\n\\n.summaryDiv > .summaryInput,\\n.detailContainer > .detailInputs {\\n    flex: 0 0 var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv .timeLabel,\\n.summaryDiv .summaryFileName {\\n    order: 3;\\n    color: var(--log-color-text-weakest);\\n    margin-left: 0.5rem;\\n}\\n\\ndetails > summary:hover .timeLabel,\\ndetails > summary:hover .summaryFileName {\\n    color: var(--log-color-text-weaker);\\n}\\n\\ndetails > summary:hover .summaryInput:not(.emptySummaryInput) {\\n    color: var(--log-color-text) !important;\\n}\\n\\n/* ******************************* */\\n/* RESPONSIVE SIZING */\\n\\n@media only screen and (max-width: 840px) {\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs,\\n    .headerInputs {\\n        display: none;\\n    }\\n}\\n\\n@media only screen and (max-width: 960px) {\\n    .headerInputs {\\n        width: var(--right-column-width-narrow) !important;\\n    }\\n\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs {\\n        flex: 0 0 var(--right-column-width-narrow) !important;\\n    }\\n}\\n\\n/* ******************************* */\\n/* ERROR OUTPUT */\\n\\n.detailInfo {\\n    margin: 0.25rem 0;\\n    padding: 0.25rem 0;\\n    border-radius: 3px;\\n    font-size: 0.8rem;\\n}\\n\\n.errorHeader {\\n    font-weight: bold;\\n    margin-bottom: 0.35rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n}\\n\\n.errorDetails {\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* HEADERS */\\n\\n.headers {\\n    display: flex;\\n    border-bottom: 1px solid var(--log-color-border);\\n    padding-bottom: 1rem;\\n    margin-bottom: 1rem;\\n}\\n\\n.headerSource,\\n.headerInputs {\\n    font-weight: 600;\\n    text-transform: uppercase;\\n    font-size: 0.75rem;\\n    letter-spacing: 0.3px;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.headerInputs {\\n    margin-left: auto;\\n    width: var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n}\\n\\n.headerRunDetails {\\n    margin: 0;\\n    margin-bottom: 1.5rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* LABEL IS THE PASS/ERROR BADGE */\\n\\n.label {\\n    display: inline-block;\\n    margin-left: 0.5rem;\\n    color: white;\\n    font-weight: 600;\\n    font-size: 10px;\\n    border-radius: 2px;\\n    padding: 0 4px;\\n    height: 1rem;\\n    line-height: 1rem;\\n    letter-spacing: 0;\\n    display: none;\\n}\\n\\n.errorParent.leafNode .label.F,\\n.errorParent.leafNode .label.E,\\n.errorParent.leafNode .label.FAIL,\\n.errorParent.leafNode .label.ERROR {\\n    display: block;\\n    background-color: var(--log-color-error);\\n}\\n\\n/* hide labels when everything was successful */\\n/*\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n}\\n*/\\n.errorParent.leafNode .label.W,\\n.errorParent.leafNode .label.WARN {\\n    background-color: var(--log-color-warn);\\n}\\n\\n.label.NOT_RUN {\\n    background-color: var(--log-color-disabled);\\n}\\n\\n/* ******************************* */\\n/* HEADER TITLE ROW */\\n\\n.headerTitleSection {\\n    display: flex;\\n    align-items: center;\\n    margin-top: 0.3rem;\\n    margin-bottom: 0.5rem;\\n}\\n\\n.headerTitleSection h3 {\\n    margin: 0;\\n    padding: 0;\\n    font-size: 1.5rem;\\n}\\n\\n#suiteResult {\\n    font-size: 0.82rem;\\n    padding: 0.1rem 0.3rem 0.15rem 0.3rem;\\n    height: auto;\\n    margin-left: 0.75rem;\\n    display: inline-block;\\n}\\n.headerTitleSection .ERROR {\\n    background-color: var(--log-color-error);\\n}\\n.headerTitleSection .PASS {\\n    background-color: var(--log-color-success);\\n}\\n\',""]);const o=a},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,s){"string"==typeof e&&(e=[[null,e,""]]);var a={};if(s)for(var o=0;o<this.length;o++){var r=this[o][0];null!=r&&(a[r]=!0)}for(var i=0;i<e.length;i++){var l=[].concat(e[i]);s&&a[l[0]]||(t&&(l[2]?l[2]="".concat(t," and ").concat(l[2]):l[2]=t),n.push(l))}},n}},457:(e,n,t)=>{let s;window.setVSCodeAPI=function(e){s=e};let a={};function o(e){let n;try{n=s}catch(e){}n&&n.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=a[e.request_seq];t&&(delete a[e.request_seq],t(e));break;case"event":let s=r[n.event];s?s(n):console.log("Unhandled event: ",n);break;case"request":let o=i[n.command];o?o(n):console.log("Unhandled request: ",n)}}));let l=0;function d(){return l+=1,l}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},m={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function u(){return void 0===m.state&&(m.state=function(){let e;try{e=s}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),m}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function b(){return document.createElement("button")}function E(){return document.createElement("div")}function y(e){return e.getAttribute("data-tree-id")}function w(e,n=void 0){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function C(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function S(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&T(e,n);t.open?e.openNodes[y(n)]="open":delete e.openNodes[y(n)]}}function T(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&S(e,t)}const x=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{L()})(...e)}),500)}})();function L(){const e=u();!function(e,n){const t=p("mainTree");let s={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(s=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&T(s,e);e.runIdToTreeState[n]=s;const a=e.runIdLRU.indexOf(n);for(a>-1&&e.runIdLRU.splice(a,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=s}catch(e){}n?n.setState(e):c=e}(e.state)}function N(e,n){if(void 0===e)return;const t=f("selectedRun"),s=new Map;for(let a of t.childNodes)if(a instanceof HTMLOptionElement){const t=a,o=t.value,r=e[o];if(void 0===r)a.remove();else{t.text!==r&&(t.text=r),s.set(o,r);const e=n==o;t.selected=e}}for(const a of Object.keys(e)){if(void 0===a)continue;const o=n==a;if(!s.has(a)){const n=document.createElement("option"),r=e[a];n.value=a,t.appendChild(n),n.selected=o,n.text=r,s.set(a,r)}}}Math.pow(10,8);var I=6e4,M=36e5;var k={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},R=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,_=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function H(e){return e&&parseFloat(e.replace(",","."))||0}var F=[31,null,31,30,31,30,31,31,30,31,30,31];function O(e){return e%400==0||e%4==0&&e%100!=0}function P(e,n){return function(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var s=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==s&&1!==s&&0!==s)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var a,o=function(e){var n,t={},s=e.split(k.dateTimeDelimiter);if(s.length>2)return t;if(/:/.test(s[0])?n=s[0]:(t.date=s[0],n=s[1],k.timeZoneDelimiter.test(t.date)&&(t.date=e.split(k.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var a=k.timezone.exec(n);a?(t.time=n.replace(a[1],""),t.timezone=a[1]):t.time=n}return t}(e);if(o.date){var r=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),s=e.match(t);if(!s)return{year:NaN,restDateString:""};var a=s[1]?parseInt(s[1]):null,o=s[2]?parseInt(s[2]):null;return{year:null===o?a:100*o,restDateString:e.slice((s[1]||s[2]).length)}}(o.date,s);a=function(e,n){if(null===n)return new Date(NaN);var t=e.match(R);if(!t)return new Date(NaN);var s=!!t[4],a=D(t[1]),o=D(t[2])-1,r=D(t[3]),i=D(t[4]),l=D(t[5])-1;if(s)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,l)?function(e,n,t){var s=new Date(0);s.setUTCFullYear(e,0,4);var a=7*(n-1)+t+1-(s.getUTCDay()||7);return s.setUTCDate(s.getUTCDate()+a),s}(n,i,l):new Date(NaN);var d=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(F[n]||(O(e)?29:28))}(n,o,r)&&function(e,n){return n>=1&&n<=(O(e)?366:365)}(n,a)?(d.setUTCFullYear(n,o,Math.max(a,r)),d):new Date(NaN)}(r.restDateString,r.year)}if(!a||isNaN(a.getTime()))return new Date(NaN);var i,l=a.getTime(),d=0;if(o.time&&(d=function(e){var n=e.match(_);if(!n)return NaN;var t=H(n[1]),s=H(n[2]),a=H(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,s,a)?t*M+s*I+1e3*a:NaN}(o.time),isNaN(d)))return new Date(NaN);if(!o.timezone){var c=new Date(l+d),m=new Date(0);return m.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),m.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),m}return i=function(e){if("Z"===e)return 0;var n=e.match(A);if(!n)return 0;var t="+"===n[1]?-1:1,s=parseInt(n[2]),a=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,a)?t*(s*M+a*I):NaN}(o.timezone),isNaN(i)?new Date(NaN):new Date(l+d+i)}(n).toString()}function U(e,n){var t,s;const a=G(n,":");if(a){[t,s]=a;try{s=JSON.parse(s)}catch(e){return console.log("Error parsing json: "+s),console.log(e),null}e.memo[t]=s}return null}function z(e,n){const[t,s]=G(n,":"),[a,o,r,i,l]=s.split("|",5);e.location_memo[t]=[e.memo[a],e.memo[o],e.memo[r],e.memo[i],parseInt(l)]}function B(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function V(e,n){return parseFloat(n)}function j(e,n){return parseInt(n)}function $(e,n){return n}function Y(e,n){return JSON.parse(n)}function q(e){if("memorize"===e)return U;if("memorize_path"===e)return z;const n=[],t=new Map;for(let s of e.split(",")){let e;if(s=s.trim(),-1==s.indexOf(":"))throw new Error("Unexpected definition: {message_definition}");if([s,e]=s.split(":",2),n.push(s),"oid"===e)t.set(s,B);else if("int"===e)t.set(s,j);else if("float"===e)t.set(s,V);else if("str"===e)t.set(s,$);else{if("json.loads"===e)return Y;if("dateisoformat"===e)return P;if("loc_id"===e)t.set(s,"loc_id");else{if("loc_and_doc_id"!==e)throw new Error("Unexpected: "+e);t.set(s,"loc_and_doc_id")}}}return function(e,s){const a=s.split("|",n.length),o={};for(let s=0;s<a.length;s++){const r=a[s],i=n[s],l=t.get(i);if("loc_id"===l){const n=e.location_memo[r];o.name=n[0],o.libname=n[1],o.source=n[2],o.lineno=n[4]}else if("loc_and_doc_id"===l){const n=e.location_memo[r];o.name=n[0],o.libname=n[1],o.source=n[2],o.doc=n[3],o.lineno=n[4]}else o[i]=l(e,r)}return o}}const W={};!function(){for(let e of"\\n# Each message should use a single line in the log output where the prefix\\n# is the message type and the arguments is either a message with ids/numbers\\n# separated by \'|\' or json-encoded strings.\\n#\\n# Note that each output log file (even if splitted after the main one) should be\\n# readable in a completely independent way, so, the starting scope should be\\n# replicated as well as the needed names to memorize.\\n#\\n# To keep the format compact, some strings and locations are referenced through ids. \\n# \\n# In the spec \'oid\' are used to reference a message memorized with \'M\' and \\n# \'loc_id\' or \'loc_and_doc_id\' a message memorized with \'P\'.\\n#\\n# There\'s an initial time and other time references are time-deltas from this time.\\n#\\n# The spec for the messages is below:\\n#\\n\\n# Version of the log output\\n# Example: \'V 0.0.1\' - Identifies version 1 of the log\\nV: version:str\\n\\n# Some information message\\n# Example: \'I \\"python=3.7\\"\'\\nI: info:json.loads\\n\\n# The log has an id that may be split into multiple parts.\\n# \'ID: 1|36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2\'     1st part with identifier 36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2.\\n# \'ID: 2|36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2\'     2nd part with identifier 36ac1f85-6d32-45b0-8ebf-3bbf8d7482f2.\\nID: part:int, id:str\\n\\n# Initial time in UTC (all others are based on a delta from this date).\\n# Example: \'T 2022-10-03T11:30:54.927+00:00\'\\nT: time:dateisoformat\\n\\n# Memorize some word (to be used as oid).\\n# i.e.: when the message is something as \'M a:\\"Start\\"\', we memorize \\"Start\\" with key: \\"a\\"\\n# Example: \'M a:\\"Start\\"\'\\nM: memorize\\n\\n# Memorize a path location (name/libname/source/lineno/docstring) to be referenced as loc_id or loc_and_doc_id.\\n# Note: loc_id and loc_and_doc_id use the same info but one unpacks the docstring and the other doesn\'t\\n# Example: \'P a|b|c|d|e\' (where those are references to strings memoized with \'M\').\\nP: memorize_path\\n\\n# Log (raw text)\\n# level_enum is:\\n# - ERROR = \'E\'\\n# - FAIL = \'F\'\\n# - INFO = \'I\'\\n# - WARN = \'W\'\\n#\\n# Example:\\n#\\n# \'L E|a|b|0.123\'\\nL: level:str, message:oid, loc:loc_id, time_delta_in_seconds:float\\n\\n# A message which is intended to be sent to to the console\\n# This can be either a message being sent by the user to stdout/stderr\\n# (if those are being redirected) or some message from the framework\\n# intended to be shown in the console.\\n#\\n# Expected \\"kind\\" values:\\n#\\n# User messages:\\n# \\"stdout\\": Some user message which was being sent to the stdout.\\n# \\"stderr\\": Some user message which was being sent to the stderr.\\n#\\n# Messages from the framework:\\n# \\"regular\\": Some regular message.\\n# \\"important\\": Some message which deserves a bit more attention.\\n# \\"task_name\\": The task name is being written.\\n# \\"error\\": Some error message.\\n# \\"traceback\\": Some traceback message.\\n#\\n# Example:\\n#\\n# \'C a|b|0.123\'\\nC: kind:oid, message:oid, time_delta_in_seconds:float\\n\\n# Log (html) -- same thing as Log but the message must be interpreted as HTML.\\n# So, something as <img alt=\\"screenshot\\" src=\\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABAAAAAEgCAIAAACl65ZFAAEAAElEQVR4nOz9d7R...\\"/>\\n# would be interpreted as an image in the final HTML. \\nLH=L\\n\\n# Start Run\\nSR: name:oid, time_delta_in_seconds:float\\n\\n# End Run\\nER: status:oid, time_delta_in_seconds:float\\n\\n# Start Task\\nST: loc:loc_id, time_delta_in_seconds:float\\n\\n# End Task\\n# status may be:\\n# \\"PASS\\": Everything went well.\\n# \\"ERROR\\": There was some detected error while running the task.\\nET: status:oid, message:oid, time_delta_in_seconds:float\\n\\n# Start Element \\n# Should be sent when some element we\'re tracking such as method, for, while, etc. starts.\\n# The \'type\' can be:\\n#\\n# METHOD\\n#\\n# GENERATOR\\n#\\n# UNTRACKED_GENERATOR (untracked generator is a generator in a library, where we\\n# just track the start/end and not what happens inside it).\\nSE: loc:loc_and_doc_id, type:oid, time_delta_in_seconds:float\\n\\n# Yield Resume (coming back to a suspended frame).\\n# Should be sent when a given frame is resumed from a yield.\\nYR: loc:loc_id, time_delta_in_seconds:float\\n\\n# Yield From Resume (coming back to a suspended frame).\\n# Should be sent when a given frame is resumed from a yield from.\\nYFR: loc:loc_id, time_delta_in_seconds:float\\n\\n# End Element\\n# When the element ends, provide its status (\\"PASS\\", \\"ERROR\\") and the time at which it finished.\\nEE: type:oid, status:oid, time_delta_in_seconds:float\\n\\n# Yield Suspend (pausing a frame)\\n# Should be sent when a given frame is suspended in a yield.\\nYS: loc:loc_id, type:oid, value:oid, time_delta_in_seconds:float\\n\\n# Yield From Suspend (pausing a frame)\\n# Should be sent when a given frame is suspended in a yield from.\\nYFS: loc:loc_id, time_delta_in_seconds:float\\n\\n# Assign\\n# Assign some content (type, value) to a variable (target) in the given location (loc). \\nAS: loc:loc_id, target:oid, type:oid, value:oid, time_delta_in_seconds:float\\n\\n# Element/method argument (name and value of the argument).\\n# Adds some argument (name) to the current element (with the given type and value).\\nEA: name:oid, type:oid, value:oid\\n\\n# Set some time for the current scope (usually not needed as the time\\n# is usually given in the element itself).\\nS: start_time_delta:float\\n\\n# --------------------------------------------------------------- Tracebacks\\n# Start traceback with the exception error message.\\n# Note: it should be possible to start a traceback inside another traceback\\n# for cases where the exception has an exception cause.\\n\\n# Start Traceback\\nSTB: message:oid, time_delta_in_seconds:float\\n\\n# Traceback Entry\\nTBE: source:oid, lineno:int, method:oid, line_content:oid\\n\\n# Traceback variable\\nTBV: name:oid, type:oid, value:oid\\n\\n# End Traceback\\nETB: time_delta_in_seconds:float\\n\\n# These messages have the same format (just the message type is different).\\nRR=SR\\nRT=ST\\nRE=SE\\nRTB=STB\\nRYR=YR\\n".split(/\\r?\\n/))if(e=e.trim(),0!==e.length&&!e.startsWith("#"))try{let[n,t]=G(e,":");n=n.trim(),t=t.trim(),W[n]=q(t)}catch(n){let[t,s]=G(e,"=");t=t.trim(),s=s.trim(),W[t]=W[s]}}();class Z{constructor(){this.memo={},this.location_memo={}}decode_message_type(e,n){return(0,W[e])(this,n)}}function G(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*J(e,n){var t,s,a;for(let o of e.split(/\\r?\\n/))if(o=o.trim(),o)try{const e=G(o," ");if(e&&([a,s]=e,t=n.decode_message_type(a,s))){const e={message_type:a,decoded:t};yield e}}catch(e){console.log("Unable to decode message: "+o),console.log(e)}}function K(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function Q(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function X(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class ee{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,s){const a=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:s,variables:a})}pushVar(e,n,t){this.stack.at(-1).variables.set(e,[n,t])}}class ne{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function te(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),s=document.createElement("details");e&&(s.open=e),s.classList.add("NO_CHILDREN"),t.appendChild(s);const a=E();a.classList.add("detailContainer"),s.appendChild(a);const o=document.createElement("summary"),r=E();r.classList.add("summaryDiv"),o.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const l=v();return l.className="summaryInput emptySummaryInput",l.textContent="",r.appendChild(l),s.appendChild(o),{li:t,details:s,summary:o,summaryDiv:r,summaryName:i,summaryInput:l,detailContainer:a}}function se(e,n){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${n}`}function ae(e,n,t,s,a,o,r,i,l,d){const c=e.state.runIdToTreeState[e.runId],m="li_"+d;if(c){const e=c.openNodes;e&&(o=e[m])}const u=te(o,m),h=u.li,p=u.details,f=u.detailContainer,v=u.summary,b=u.summaryDiv,E=u.summaryName,y=u.summaryInput;if("LH"===a.message_type){E.textContent="";const e=C(t);E.appendChild(e)}else E.textContent=t;s&&(E.title=s),e.onClickReference&&(E.classList.add("span_link"),E.onclick=n=>{const t=[];let s=l.parent;for(;void 0!==s&&void 0!==s.message;)t.push(s.message),s=s.parent;n.preventDefault(),e.onClickReference({source:r,lineno:i,message:a.decoded,messageType:a.message_type,scope:t})});const w=g("ul_"+d);p.appendChild(w);const S={ul:w,li:h,details:p,detailContainer:f,summary:v,summaryName:E,summaryInput:y,source:r,lineno:i,appendContentChild:void 0,decodedMessage:a,maxLevelFoundInHierarchy:-1,summaryDiv:b};return S.appendContentChild=de.bind(S),n.appendContentChild(S),S}let oe,re;function*ie(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of le(e))yield n;yield n}}function*le(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of ie(n))yield e}function de(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){x()})),u().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===oe){oe=E(),oe.classList.add("toolbarContainer");const e=b();e.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==re){re.details.open=!0;for(let e of le(re.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=b();return n.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==re){re.details.open=!1;for(let e of le(re.ul))e.open=!1}}()},oe.appendChild(n),void oe.appendChild(e)}re=e,e.summaryDiv.appendChild(oe)}(n)})))}var ce=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let me=0,ue=-1;class he{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new ee(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class pe{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new Z,this.seenSuiteTaskOrElement=!1,this.tbHandler=new he,this.suiteErrored=!1,this.opts=u(),this.runId=this.opts.runId,this.summaryBuilder=new ne,this.lease=(me+=1,ue=me,me),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===ue&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return ce(this,null,(function*(){for(const e of J(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return ce(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=u();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of J(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return ce(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let s,a,o=e.message_type;switch(o){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;o="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;o="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;o="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;o="STB"}switch(this.id+=1,o){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"AS":a=ae(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),se(a,e.decoded.value),this.addAssignCssClass(a);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=ae(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":case"YR":case"YFR":if("SE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){this.messageNode={parent:this.messageNode,message:e};let n=e.decoded.name;"YR"==o&&(n+=" (resumed)"),this.parent=ae(this.opts,this.parent,n,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),"YR"==o&&this.addResumedCSSClass(this.parent),this.argsTarget=this.parent,this.stack.push(this.parent)}else{const n=ae(this.opts,this.parent,`Create Generator: ${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addGeneratorCSSClass(n),this.argsTarget=n}break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),s=this.addDetailsCSSClasses(e.decoded.status,r),s&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":case"YS":case"YFS":if("EE"!=o||"UNTRACKED_GENERATOR"!=e.decoded.type){if("YS"==o||"YFS"==o){const n=ae(this.opts,this.parent,"Yielded",`Suspending function with yield.\\nYielding an object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());this.addYieldedCSSClass(n),se(n,e.decoded.value),e.decoded.status="PASS"}this.messageNode=this.messageNode.parent;let n=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(n,this.parent,e),this.onEndSetStatusOrRemove(this.opts,n,e.decoded,this.parent,!0),s=this.addDetailsCSSClasses(e.decoded.status,n),s&&(n.details.open=!0)}break;case"S":const i=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":!function(e,n,t,s){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n} = ${s}`,e.summaryInput.title=`Argument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.classList.remove("emptySummaryInput")):(e.summaryInput.title+=`\\n\\nArgument: ${n}\\nArgument type: ${t}\\nRepresentation:\\n${s}`,e.summaryInput.textContent+=`, ${n} = ${s}`)}(this.argsTarget,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const l=e.decoded.level,d=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(l);if(d>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=d),Q(this.opts,d)){const n=ae(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=d,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,l),this.addDetailsCSSClasses(d,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const n=c.stack[0],t=c.exceptionMsg.split(":",2);let s,o;t.length>1?(s=t[0],o=t[1]):(s="Error",o=t[0]),a=ae(this.opts,this.parent,s,"",e,!1,n.source,n.lineno,this.messageNode,this.id.toString()),se(a,o),this.addExceptionCssClass(a)}break;case"T":const m=p("suiteRunStart");m&&(m.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addYieldedCSSClass(e){e.details.classList.add("yiededParent"),e.details.classList.add("leafNode")}addResumedCSSClass(e){e.details.classList.add("resumedParent")}addGeneratorCSSClass(e){e.details.classList.add("generatorParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,n){let t,s=!1;return t="string"==typeof e?X(e):e,t>=2?(n.details.classList.add("errorParent"),s=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),s}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const s=X(t.decoded.status);s>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=s),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,s,a){const o=t.status;if(Q(e,n.maxLevelFoundInHierarchy)){if(a&&n.maxLevelFoundInHierarchy<=0){const e=50;if(s.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=y(n.li);if(n.li.remove(),w(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=te(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const a=v();a.setAttribute("role","button"),a.textContent="...",a.classList.add("label"),a.classList.add("HIDDEN"),a.classList.add("inline"),e.summaryDiv.appendChild(a);const o=v();o.setAttribute("role","button"),o.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(o),K(e,"HIDDEN"),w(e.li,!0),s.ul.appendChild(e.li)}return}}}if(n.summary,K(n,o),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var fe=(e,n,t)=>new Promise(((s,a)=>{var o=e=>{try{i(t.next(e))}catch(e){a(e)}},r=e=>{try{i(t.throw(e))}catch(e){a(e)}},i=e=>e.done?s(e.value):Promise.resolve(e.value).then(o,r);i((t=t.apply(e,n)).next())}));let ge;function ve(){return fe(this,null,(function*(){ge=new pe,ge.clearAndInitializeTree(),yield ge.addInitialContents()}))}function be(e){let n={type:"event",seq:d(),event:"onClickReference"};n.data=e,o(n)}function Ee(e){L();const n=u();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==s&&(n.onClickReference=be),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,N(n.allRunIdsToLabel,n.runId),ve()}t(739),i.setContents=Ee,i.appendContents=function(e){const n=u();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==ge&&ge.onAppendedContents())},i.updateLabel=function(e){const n=u();n.allRunIdsToLabel[e.runId]=e.label,N(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:d(),event:"onSetCurrentRunId"};n.data={runId:e},o(n)},window.onChangedFilterLevel=function(){!function(e){const n=u();n.state.filterLevel!==e&&(n.state.filterLevel=e,L(),ve())}(f("filterLevel").value)},window.setContents=Ee,window.setShowTime=function(e){u().showTime=e},window.setShowExpand=function(e){u().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},739:(e,n,t)=>{var s=t(379),a=t.n(s),o=t(599),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};a()(o.Z,r),o.Z.locals},379:(e,n,t)=>{var s,a=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),o=[];function r(e){for(var n=-1,t=0;t<o.length;t++)if(o[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},s=[],a=0;a<e.length;a++){var i=e[a],l=n.base?i[0]+n.base:i[0],d=t[l]||0,c="".concat(l," ").concat(d);t[l]=d+1;var m=r(c),u={css:i[1],media:i[2],sourceMap:i[3]};-1!==m?(o[m].references++,o[m].updater(u)):o.push({identifier:c,updater:f(u,n),references:1}),s.push(c)}return s}function l(e){var n=document.createElement("style"),s=e.attributes||{};if(void 0===s.nonce){var o=t.nc;o&&(s.nonce=o)}if(Object.keys(s).forEach((function(e){n.setAttribute(e,s[e])})),"function"==typeof e.insert)e.insert(n);else{var r=a(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(n)}return n}var d,c=(d=[],function(e,n){return d[e]=n,d.filter(Boolean).join("\\n")});function m(e,n,t,s){var a=t?"":s.media?"@media ".concat(s.media," {").concat(s.css,"}"):s.css;if(e.styleSheet)e.styleSheet.cssText=c(n,a);else{var o=document.createTextNode(a),r=e.childNodes;r[n]&&e.removeChild(r[n]),r.length?e.insertBefore(o,r[n]):e.appendChild(o)}}function u(e,n,t){var s=t.css,a=t.media,o=t.sourceMap;if(a?e.setAttribute("media",a):e.removeAttribute("media"),o&&"undefined"!=typeof btoa&&(s+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o))))," */")),e.styleSheet)e.styleSheet.cssText=s;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(s))}}var h=null,p=0;function f(e,n){var t,s,a;if(n.singleton){var o=p++;t=h||(h=l(n)),s=m.bind(null,t,o,!1),a=m.bind(null,t,o,!0)}else t=l(n),s=u.bind(null,t,n),a=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return s(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;s(e=n)}else a()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===s&&(s=Boolean(window&&document&&document.all&&!window.atob)),s));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var s=0;s<t.length;s++){var a=r(t[s]);o[a].references--}for(var l=i(e,n),d=0;d<t.length;d++){var c=r(t[d]);0===o[c].references&&(o[c].updater(),o.splice(c,1))}t=l}}}}},n={};function t(s){var a=n[s];if(void 0!==a)return a.exports;var o=n[s]={id:s,exports:{}};return e[s](o,o.exports,t),o.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var s in n)t.o(n,s)&&!t.o(e,s)&&Object.defineProperty(e,s,{enumerable:!0,get:n[s]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(457),t(739)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(false);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
```

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_lifecycle_hooks.py` & `robocorp_log-0.1.1/src/robocorp/log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_null.py` & `robocorp_log-0.1.1/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-0.1.1/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-0.1.1/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-0.1.1/src/robocorp/log/_rewrite_importhook.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_robo_logger.py` & `robocorp_log-0.1.1/src/robocorp/log/_robo_logger.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-0.1.1/src/robocorp/log/_robo_output_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -913,15 +913,15 @@
 
             if self._config.log_html_style == 1:
                 from robocorp.log import _index as index
             elif self._config.log_html_style == 2:
                 from robocorp.log import _index_v2 as index
             else:
                 raise ValueError(
-                    "Unexpected log html style: {self._config.log_html_style}"
+                    f"Unexpected log html style: {self._config.log_html_style}"
                 )
 
             has_separate_bundle_js = "bundle.js" in index.FILE_CONTENTS
 
             for name, contents in index.FILE_CONTENTS.items():
                 if name == "index.html":
                     if has_separate_bundle_js:
```

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_sensitive_variable_names.py` & `robocorp_log-0.1.1/src/robocorp/log/_sensitive_variable_names.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/_suppress_helper.py` & `robocorp_log-0.1.1/src/robocorp/log/_suppress_helper.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/console.py` & `robocorp_log-0.1.1/src/robocorp/log/console.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/protocols.py` & `robocorp_log-0.1.1/src/robocorp/log/protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.0/src/robocorp/log/redirect.py` & `robocorp_log-0.1.1/src/robocorp/log/redirect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import contextmanager, redirect_stdout, redirect_stderr
 import json
 import os
 import sys
 import traceback
-from typing import Iterator, Any, IO, AnyStr, Iterable
+from typing import Iterator, IO, AnyStr, Iterable
 from threading import RLock
 from robocorp.log import console_message
 
 
 class _IORedirector(IO[str]):
     """
     This class works to wrap a stream (stdout/stderr) with an additional redirect.
```

