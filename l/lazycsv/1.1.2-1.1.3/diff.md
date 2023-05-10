# Comparing `tmp/lazycsv-1.1.2.tar.gz` & `tmp/lazycsv-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.1.2.tar", last modified: Sun May  7 19:56:48 2023, max compression
+gzip compressed data, was "lazycsv-1.1.3.tar", last modified: Wed May 10 14:34:35 2023, max compression
```

## Comparing `lazycsv-1.1.2.tar` & `lazycsv-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.2/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     9408 2023-05-07 19:56:48.041865 lazycsv-1.1.2/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     8357 2023-05-07 19:55:27.000000 lazycsv-1.1.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-07 19:56:48.041865 lazycsv-1.1.2/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-05-07 19:56:34.000000 lazycsv-1.1.2/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.2/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39603 2023-05-07 19:55:27.000000 lazycsv-1.1.2/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     9408 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-07 19:56:48.000000 lazycsv-1.1.2/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-07 19:56:48.041865 lazycsv-1.1.2/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    23765 2023-05-03 15:13:07.000000 lazycsv-1.1.2/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.3/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     9944 2023-05-10 14:34:35.581540 lazycsv-1.1.3/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     8893 2023-05-10 14:32:51.000000 lazycsv-1.1.3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-10 14:34:35.581540 lazycsv-1.1.3/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-05-10 14:34:21.000000 lazycsv-1.1.3/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.3/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39709 2023-05-10 14:16:18.000000 lazycsv-1.1.3/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     9944 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-10 14:34:35.000000 lazycsv-1.1.3/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-10 14:34:35.581540 lazycsv-1.1.3/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    24486 2023-05-10 14:24:35.000000 lazycsv-1.1.3/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.1.2/LICENSE` & `lazycsv-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.1.2/PKG-INFO` & `lazycsv-1.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: lazycsv
-Version: 1.1.2
-Summary: an fast, memory efficient csv parser
-Author: Michael Green, Chris Perkins
-Author-email: dev@crunch.io
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: benchmark
-License-File: LICENSE
-
 # lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
 parser is to provide for fast extraction of sequences of data from a CSV file
 in a memory-efficient manner, with zero dependencies.
@@ -160,14 +133,33 @@
 >>> lazy = lazycsv.LazyCSV(
 ...     "tests/fixtures/file_crlf2.csv", unquote=False
 ... )
 >>> lazy.headers
 (b'', b'"This,that"', b'"Fizz,Buzz"')
 ```
 
+LazyCSV also provides the option to specify a delimiter and a quote character.
+Pass the keywords `delimiter=` and `quotechar=` to the object contstructor to
+use custom values. By default, `delimiter` defaults to `,` and `quotechar`
+defaults to `"`.
+
+```python
+>>> lazy = lazycsv.LazyCSV(
+...     "tests/fixtures/file_delimiter_and_quotechar.csv",
+...     quotechar="|",
+...     delimiter="\t",
+...     unquote=False,
+... )
+...
+>>> open(lazy.name, "rb").read()
+b'INDEX\tATTR\n0\t|A|\n1\t|B|\n'
+>>> list(lazy[:, 1])
+[b'|A|', b'|B|']
+```
+
 ### Numpy
 
 Optional, opt-in numpy support is built into the module. Access to this
 extended feature set can be had by building the extension from source while
 setting a `LAZYCSV_INCLUDE_NUMPY` environment variable to `1`. This adds a
 `to_numpy()` method to the iterator, which allows iterators to materialize in a
 1-dimensional numpy array without creating intermediary PyObject*'s for each
```

### Comparing `lazycsv-1.1.2/README.md` & `lazycsv-1.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: lazycsv
+Version: 1.1.3
+Summary: an fast, memory efficient csv parser
+Author: Michael Green, Chris Perkins
+Author-email: dev@crunch.io
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: benchmark
+License-File: LICENSE
+
 # lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
 parser is to provide for fast extraction of sequences of data from a CSV file
 in a memory-efficient manner, with zero dependencies.
@@ -133,14 +160,33 @@
 >>> lazy = lazycsv.LazyCSV(
 ...     "tests/fixtures/file_crlf2.csv", unquote=False
 ... )
 >>> lazy.headers
 (b'', b'"This,that"', b'"Fizz,Buzz"')
 ```
 
+LazyCSV also provides the option to specify a delimiter and a quote character.
+Pass the keywords `delimiter=` and `quotechar=` to the object contstructor to
+use custom values. By default, `delimiter` defaults to `,` and `quotechar`
+defaults to `"`.
+
+```python
+>>> lazy = lazycsv.LazyCSV(
+...     "tests/fixtures/file_delimiter_and_quotechar.csv",
+...     quotechar="|",
+...     delimiter="\t",
+...     unquote=False,
+... )
+...
+>>> open(lazy.name, "rb").read()
+b'INDEX\tATTR\n0\t|A|\n1\t|B|\n'
+>>> list(lazy[:, 1])
+[b'|A|', b'|B|']
+```
+
 ### Numpy
 
 Optional, opt-in numpy support is built into the module. Access to this
 extended feature set can be had by building the extension from source while
 setting a `LAZYCSV_INCLUDE_NUMPY` environment variable to `1`. This adds a
 `to_numpy()` method to the iterator, which allows iterators to materialize in a
 1-dimensional numpy array without creating intermediary PyObject*'s for each
```

### Comparing `lazycsv-1.1.2/setup.py` & `lazycsv-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.1.2",
+    version="1.1.3",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
     description="an fast, memory efficient csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
```

### Comparing `lazycsv-1.1.2/src/lazycsv/lazycsv.c` & `lazycsv-1.1.3/src/lazycsv/lazycsv.c`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #include <sys/stat.h>
 #include <unistd.h>
 #include <limits.h>
 
 #include <Python.h>
 #include "structmember.h"
 
-#define DOUBLE_QUOTE 34
-#define COMMA 44
 #define LINE_FEED 10
 #define CARRIAGE_RETURN 13
 
 // users can set this macro using the env variable LAZYCSV_INDEX_DTYPE if you
 // want to be more aggressive with minimizing index disk usage (i.e. define
 // INDEX_DTYPE as uint8_t) but at a cost to performance.
 
@@ -100,14 +98,15 @@
     PyObject_HEAD
     PyObject* headers;
     PyObject* name;
     size_t rows;
     size_t cols;
     int _skip_headers;
     int _unquote;
+    char _quotechar;
     char _newline;
     LazyCSV_Index* _index;
     LazyCSV_File* _data;
     LazyCSV_Cache* _cache;
 } LazyCSV;
 
 
@@ -303,16 +302,16 @@
         Py_INCREF(result);
         break;
     default:
         addr = lazy->_data->data + offset;
 
         char strip_quotes = (
             lazy->_unquote
-            && addr[0] == DOUBLE_QUOTE
-            && addr[len-1] == DOUBLE_QUOTE
+            && addr[0] == lazy->_quotechar
+            && addr[len-1] == lazy->_quotechar
         );
 
         if (strip_quotes) {
             addr = addr+1;
             len = len-2;
         }
 
@@ -600,24 +599,23 @@
 static PyObject *LazyCSV_New(PyTypeObject *type, PyObject *args,
                              PyObject *kwargs) {
 
     PyObject* name;
     int skip_headers = 0;
     int unquote = 1;
     Py_ssize_t buffer_capacity = 2097152; // 2**21
-    char* dirname;
+    char *dirname, *delimiter = ",", *quotechar = "\"";
 
     static char* kwlist[] = {
-        "", "skip_headers", "unquote", "buffer_size", "index_dir", NULL
+        "", "delimiter", "quotechar", "skip_headers", "unquote", "buffer_size", "index_dir", NULL
     };
 
     char ok = PyArg_ParseTupleAndKeywords(
-        args, kwargs, "O|ppns", kwlist, &name,
-        &skip_headers, &unquote, &buffer_capacity, &dirname
-    );
+        args, kwargs, "O|ssppns", kwlist, &name, &delimiter, &quotechar,
+        &skip_headers, &unquote, &buffer_capacity, &dirname);
 
     if (!ok) {
         PyErr_SetString(
             PyExc_ValueError,
             "unable to parse function arguments"
         );
         return NULL;
@@ -746,19 +744,19 @@
             ridx.index += ridx.count*sizeof(LazyCSV_AnchorPoint);
             ridx.count = 1;
 
             _Value_ToDisk(val, &ridx, &apnt, col_index, comma_file,
                           &comma_buffer, anchor_file, &anchor_buffer);
         }
 
-        if (c == DOUBLE_QUOTE) {
+        if (c == *quotechar) {
             quoted = !quoted;
         }
 
-        else if (!quoted && c == COMMA) {
+        else if (!quoted && c == *delimiter) {
             size_t val = i + 1;
             _Value_ToDisk(val, &ridx, &apnt, col_index, comma_file,
                           &comma_buffer, anchor_file, &anchor_buffer);
             if (cols == SIZE_MAX || col_index < cols) {
                 col_index += 1;
             }
             else {
@@ -919,16 +917,16 @@
                 PyTuple_SET_ITEM(headers, i, PyBytes_FromString(""));
             }
             else {
                 addr = file + cs;
 
                 len = ce - cs - 1;
                 if (unquote
-                        && addr[0] == DOUBLE_QUOTE
-                        && addr[len-1] == DOUBLE_QUOTE) {
+                        && addr[0] == *quotechar
+                        && addr[len-1] == *quotechar) {
                     addr = addr+1;
                     len = len-2;
                 }
                 PyTuple_SET_ITEM(
                     headers, i, PyBytes_FromStringAndSize(addr, len)
                 );
             }
@@ -987,14 +985,15 @@
 
     self->rows = rows;
     self->cols = cols;
     self->name = fullname_obj;
     self->headers = headers;
     self->_skip_headers = skip_headers;
     self->_unquote = unquote;
+    self->_quotechar = *quotechar;
     self->_newline = newline;
     self->_index = _index;
     self->_data = _data;
     self->_cache = _cache;
 
     return (PyObject*)self;
```

### Comparing `lazycsv-1.1.2/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.1.3/src/lazycsv.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.2
+Version: 1.1.3
 Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -160,14 +160,33 @@
 >>> lazy = lazycsv.LazyCSV(
 ...     "tests/fixtures/file_crlf2.csv", unquote=False
 ... )
 >>> lazy.headers
 (b'', b'"This,that"', b'"Fizz,Buzz"')
 ```
 
+LazyCSV also provides the option to specify a delimiter and a quote character.
+Pass the keywords `delimiter=` and `quotechar=` to the object contstructor to
+use custom values. By default, `delimiter` defaults to `,` and `quotechar`
+defaults to `"`.
+
+```python
+>>> lazy = lazycsv.LazyCSV(
+...     "tests/fixtures/file_delimiter_and_quotechar.csv",
+...     quotechar="|",
+...     delimiter="\t",
+...     unquote=False,
+... )
+...
+>>> open(lazy.name, "rb").read()
+b'INDEX\tATTR\n0\t|A|\n1\t|B|\n'
+>>> list(lazy[:, 1])
+[b'|A|', b'|B|']
+```
+
 ### Numpy
 
 Optional, opt-in numpy support is built into the module. Access to this
 extended feature set can be had by building the extension from source while
 setting a `LAZYCSV_INCLUDE_NUMPY` environment variable to `1`. This adds a
 `to_numpy()` method to the iterator, which allows iterators to materialize in a
 1-dimensional numpy array without creating intermediary PyObject*'s for each
```

### Comparing `lazycsv-1.1.2/tests/test_lazycsv.py` & `lazycsv-1.1.3/tests/test_lazycsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,28 @@
                     "test suite did not test numpy, recompile while setting"
                     " LAZYCSV_INCLUDE_NUMPY=1 as an env variable to compile"
                     " extension with numpy support."
                 )
 
 
 class TestLazyCSVOptions:
+    def test_custom_quotechar_and_delimiter(self):
+        lazy = lazycsv.LazyCSV("tests/fixtures/file_delimiter_and_quotechar.csv", quotechar="|", delimiter="\t")
+        actual = list(list(lazy.sequence(row=i)) for i in range(lazy.rows))
+        expected = [[b'0', b'A'], [b'1', b'B']]
+        assert actual == expected
+
+    def test_custom_quotechar_unquote_false(self):
+        data = "INDEX,ATTR\n0,|A|\n1,|B|\n"
+        with prepped_file(data.encode()) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name, unquote=False, quotechar="|")
+            actual = list(list(lazy.sequence(row=i)) for i in range(lazy.rows))
+            expected = [[b'0', b'|A|'], [b'1', b'|B|']]
+            assert actual == expected
+
     def test_get_skipped_header_column(self):
         lazy = lazycsv.LazyCSV(FPATH, skip_headers=True)
         actual = list(lazy.sequence(col=0))
         assert actual == [b"", b"0", b"1"]
         actual = list(lazy.sequence(col=1))
         assert actual == [b"ALPHA", b"a0", b"a1"]
         actual = list(lazy.sequence(col=2))
```

