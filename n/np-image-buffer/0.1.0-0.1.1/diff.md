# Comparing `tmp/np_image_buffer-0.1.0.tar.gz` & `tmp/np_image_buffer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_image_buffer-0.1.0.tar", last modified: Mon Sep 26 13:55:15 2022, max compression
+gzip compressed data, was "np_image_buffer-0.1.1.tar", last modified: Wed May 10 12:56:57 2023, max compression
```

## Comparing `np_image_buffer-0.1.0.tar` & `np_image_buffer-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:55:15.596941 np_image_buffer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-09-26 13:55:15.596941 np_image_buffer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:55:15.596941 np_image_buffer-0.1.0/np_image_buffer/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/np_image_buffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12524 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/np_image_buffer/np_image_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:55:15.596941 np_image_buffer-0.1.0/np_image_buffer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-09-26 13:55:15.000000 np_image_buffer-0.1.0/np_image_buffer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-26 13:55:15.000000 np_image_buffer-0.1.0/np_image_buffer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 13:55:15.000000 np_image_buffer-0.1.0/np_image_buffer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 13:55:15.000000 np_image_buffer-0.1.0/np_image_buffer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-26 13:55:15.000000 np_image_buffer-0.1.0/np_image_buffer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-26 13:55:15.000000 np_image_buffer-0.1.0/np_image_buffer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-26 13:55:15.596941 np_image_buffer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 13:55:15.596941 np_image_buffer-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-26 13:54:53.000000 np_image_buffer-0.1.0/tests/test_np_image_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:56:57.009304 np_image_buffer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-10 12:56:57.009304 np_image_buffer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:56:57.005304 np_image_buffer-0.1.1/np_image_buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/np_image_buffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/np_image_buffer/np_image_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:56:57.009304 np_image_buffer-0.1.1/np_image_buffer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-10 12:56:56.000000 np_image_buffer-0.1.1/np_image_buffer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-10 12:56:57.000000 np_image_buffer-0.1.1/np_image_buffer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:56:56.000000 np_image_buffer-0.1.1/np_image_buffer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:56:56.000000 np_image_buffer-0.1.1/np_image_buffer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:56:56.000000 np_image_buffer-0.1.1/np_image_buffer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 12:56:56.000000 np_image_buffer-0.1.1/np_image_buffer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 12:56:57.009304 np_image_buffer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:56:57.009304 np_image_buffer-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 12:56:33.000000 np_image_buffer-0.1.1/tests/test_np_image_buffer.py
```

### Comparing `np_image_buffer-0.1.0/CONTRIBUTING.rst` & `np_image_buffer-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `np_image_buffer-0.1.0/LICENSE` & `np_image_buffer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `np_image_buffer-0.1.0/PKG-INFO` & `np_image_buffer-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 Metadata-Version: 2.1
 Name: np_image_buffer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A NumPy circular buffer for fast image storing and indexing.
 Home-page: https://github.com/jacopoabramo/np_image_buffer
 Author: Jacopo Abramo
 Author-email: jacopo.abramo@gmail.com
 License: GNU General Public License v3
 Keywords: np_image_buffer
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =================================
 NumPy image circular buffer
 =================================
 
 
 .. image:: https://img.shields.io/pypi/v/np_image_buffer.svg
         :target: https://pypi.python.org/pypi/np_image_buffer
 
-.. image:: https://img.shields.io/travis/jacopoabramo/np_image_buffer.svg
-        :target: https://travis-ci.com/jacopoabramo/np_image_buffer
-
-.. image:: https://readthedocs.org/projects/np_image_buffer/badge/?version=latest
-        :target: https://np_image_buffer.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
 
 .. image:: https://pyup.io/repos/github/jacopoabramo/np_image_buffer/shield.svg
      :target: https://pyup.io/repos/github/jacopoabramo/np_image_buffer/
      :alt: Updates
```

### Comparing `np_image_buffer-0.1.0/README.rst` & `np_image_buffer-0.1.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,14 @@
 NumPy image circular buffer
 =================================
 
 
 .. image:: https://img.shields.io/pypi/v/np_image_buffer.svg
         :target: https://pypi.python.org/pypi/np_image_buffer
 
-.. image:: https://img.shields.io/travis/jacopoabramo/np_image_buffer.svg
-        :target: https://travis-ci.com/jacopoabramo/np_image_buffer
-
-.. image:: https://readthedocs.org/projects/np_image_buffer/badge/?version=latest
-        :target: https://np_image_buffer.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
 
 .. image:: https://pyup.io/repos/github/jacopoabramo/np_image_buffer/shield.svg
      :target: https://pyup.io/repos/github/jacopoabramo/np_image_buffer/
      :alt: Updates
```

### Comparing `np_image_buffer-0.1.0/np_image_buffer/np_image_buffer.py` & `np_image_buffer-0.1.1/np_image_buffer/np_image_buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     
     def append(self, value: np.ndarray) -> None:
         """Append an image to the buffer.
         """
         if self.full:
             if not self.__allow_overwrite:
                 raise IndexError(
-                    "Append to a full RingBuffer with overwrite disabled."
+                    "Append to a full ImageBuffer with overwrite disabled."
                 )
             if self.__full_capacity == 0:
                 return  # Mimick behavior of deque(maxlen=0)
             self.__tail += 1
 
         self.__unwrap_buffer_is_dirty = True
         self.__array[self.__head % self.__full_capacity] = value
@@ -65,15 +65,15 @@
 
     def appendleft(self, value) -> None:
         """Append an image to the buffer's tail.
         """
         if self.full:
             if not self.__allow_overwrite:
                 raise IndexError(
-                    "Append to a full RingBuffer with overwrite disabled."
+                    "Append to a full ImageBuffer with overwrite disabled."
                 )
             if self.__full_capacity == 0:
                 return  # Mimick behavior of deque(maxlen=0)
             self.__head -= 1
 
         self.__unwrap_buffer_is_dirty = True
         self.__tail -= 1
@@ -87,15 +87,15 @@
     def extend(self, values: np.ndarray) -> None:
         """Extend the buffer with a list of images.
         """
         lv = len(values)
         if len(self) + lv > self.__full_capacity:
             if not self.__allow_overwrite:
                 raise IndexError(
-                    "RingBuffer overflows, because overwrite is disabled."
+                    "ImageBuffer overflows, because overwrite is disabled."
                 )
             if self.__full_capacity == 0:
                 return  # Mimick behavior of deque(maxlen=0)
 
         self.__unwrap_buffer_is_dirty = True
         if lv >= self.__full_capacity:
             self.__array[...] = values[-self.__full_capacity :]
@@ -117,15 +117,15 @@
     def extendleft(self, values) -> None:
         """Extend the ring buffer with a list of values from the left side.
         """
         lv = len(values)
         if len(self) + lv > self.__full_capacity:
             if not self.__allow_overwrite:
                 raise IndexError(
-                    "RingBuffer overflows, because overwrite is disabled."
+                    "ImageBuffer overflows, because overwrite is disabled."
                 )
             if self.__full_capacity == 0:
                 return  # Mimick behavior of deque(maxlen=0)
 
         self.__unwrap_buffer_is_dirty = True
         if lv >= self.__full_capacity:
             self.__array[...] = values[: self.__full_capacity]
@@ -146,23 +146,31 @@
 
     # --------------------------------------------------------------------------
     #   pop
     # --------------------------------------------------------------------------
 
     def pop(self):
         if len(self) == 0:
-            raise IndexError("Pop from an empty RingBuffer.")
+            raise IndexError("Pop from an empty ImageBuffer.")
         self.__unwrap_buffer_is_dirty = True
         self.__head -= 1
         self._fix_indices()
         return self.__array[self.__head % self.__full_capacity]
+    
+    def popall(self):
+        if len(self) == 0:
+            raise IndexError("Pop from an empty ImageBuffer.")
+        self.__unwrap_buffer_is_dirty = True
+        self.__head -= len(self)
+        self._fix_indices()
+        return self.__array
 
     def popleft(self):
         if len(self) == 0:
-            raise IndexError("Pop from an empty RingBuffer.")
+            raise IndexError("Pop from an empty ImageBuffer.")
         self.__unwrap_buffer_is_dirty = True
         res = self.__array[self.__tail]
         self.__tail += 1
         self._fix_indices()
         return res
 
     # --------------------------------------------------------------------------
@@ -286,28 +294,28 @@
         #   ringbuffer[int]
         #   ringbuffer[list of ints]
         #   ringbuffer[np.ndarray of ints]
         # ----------------------------------
         item_arr = np.asarray(item)
 
         if not issubclass(item_arr.dtype.type, np.integer):
-            raise TypeError("RingBuffer indices must be integers.")
+            raise TypeError("ImageBuffer indices must be integers.")
 
         if len(self) == 0:
             raise IndexError(
-                "RingBuffer list index out of range. The RingBuffer has "
+                "ImageBuffer list index out of range. The ImageBuffer has "
                 "length 0."
             )
 
         if not hasattr(item, "__len__"):
             # Single element: We can speed up the code
             # Check for `List index out of range`
             if item_arr < -len(self) or item_arr >= len(self):
                 raise IndexError(
-                    "RingBuffer list index %s out of range. The RingBuffer "
+                    "ImageBuffer list index %s out of range. The ImageBuffer "
                     "has length %s." % (item_arr, len(self))
                 )
 
             if item_arr < 0:
                 item_arr = (self.__head + item_arr) % self.__full_capacity
             else:
                 item_arr = (item_arr + self.__tail) % self.__full_capacity
@@ -316,15 +324,15 @@
             # Multiple elements
             # Check for `List index out of range`
             if np.any(item_arr < -len(self)) or np.any(item_arr >= len(self)):
                 idx_under = item_arr[np.where(item_arr < -len(self))]
                 idx_over = item_arr[np.where(item_arr >= len(self))]
                 idx_oor = np.sort(np.concatenate((idx_under, idx_over)))
                 raise IndexError(
-                    "RingBuffer list indices %s out of range. The RingBuffer "
+                    "ImageBuffer list indices %s out of range. The ImageBuffer "
                     "has length %s." % (idx_oor, len(self))
                 )
             idx_neg = np.where(item_arr < 0)
             idx_pos = np.where(item_arr >= 0)
 
             if len(idx_neg) > 0:
                 item_arr[idx_neg] = (self.__head + item_arr[idx_neg]) % self.__full_capacity
@@ -339,8 +347,8 @@
         if self.full:
             self._unwrap_into_buffer()
             return iter(self.__unwrap_buffer)
         else:
             return iter(self._unwrap())
 
     def __repr__(self):
-        return "<RingBuffer of {!r}>".format(np.asarray(self))
+        return "<ImageBuffer of {!r}>".format(np.asarray(self))
```

### Comparing `np_image_buffer-0.1.0/np_image_buffer.egg-info/PKG-INFO` & `np_image_buffer-0.1.1/np_image_buffer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 Metadata-Version: 2.1
 Name: np-image-buffer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A NumPy circular buffer for fast image storing and indexing.
 Home-page: https://github.com/jacopoabramo/np_image_buffer
 Author: Jacopo Abramo
 Author-email: jacopo.abramo@gmail.com
 License: GNU General Public License v3
 Keywords: np_image_buffer
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =================================
 NumPy image circular buffer
 =================================
 
 
 .. image:: https://img.shields.io/pypi/v/np_image_buffer.svg
         :target: https://pypi.python.org/pypi/np_image_buffer
 
-.. image:: https://img.shields.io/travis/jacopoabramo/np_image_buffer.svg
-        :target: https://travis-ci.com/jacopoabramo/np_image_buffer
-
-.. image:: https://readthedocs.org/projects/np_image_buffer/badge/?version=latest
-        :target: https://np_image_buffer.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
 
 .. image:: https://pyup.io/repos/github/jacopoabramo/np_image_buffer/shield.svg
      :target: https://pyup.io/repos/github/jacopoabramo/np_image_buffer/
      :alt: Updates
```

### Comparing `np_image_buffer-0.1.0/setup.py` & `np_image_buffer-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,33 +15,31 @@
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Jacopo Abramo",
     author_email='jacopo.abramo@gmail.com',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     description="A NumPy circular buffer for fast image storing and indexing.",
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='np_image_buffer',
     name='np_image_buffer',
     packages=find_packages(include=['np_image_buffer', 'np_image_buffer.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/jacopoabramo/np_image_buffer',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

