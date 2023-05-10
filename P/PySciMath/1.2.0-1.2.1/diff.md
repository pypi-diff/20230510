# Comparing `tmp/PySciMath-1.2.0.tar.gz` & `tmp/PySciMath-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.2.0.tar", last modified: Wed May 10 10:41:19 2023, max compression
+gzip compressed data, was "PySciMath-1.2.1.tar", last modified: Wed May 10 13:27:39 2023, max compression
```

## Comparing `PySciMath-1.2.0.tar` & `PySciMath-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:41:19.284534 PySciMath-1.2.0/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2664 2023-05-10 10:41:19.283537 PySciMath-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 10:41:19.270572 PySciMath-1.2.0/PySciMath/
--rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.2.0/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0      591 2023-05-10 10:37:49.000000 PySciMath-1.2.0/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4281 2023-05-10 10:38:03.000000 PySciMath-1.2.0/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0     2818 2023-05-10 09:50:00.000000 PySciMath-1.2.0/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0     1475 2023-05-10 10:22:01.000000 PySciMath-1.2.0/PySciMath/Numbers.py
--rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.2.0/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.2.0/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.2.0/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0      637 2023-05-10 09:41:19.000000 PySciMath-1.2.0/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:41:19.280545 PySciMath-1.2.0/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2664 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2149 2023-05-10 10:40:03.000000 PySciMath-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 10:41:19.284534 PySciMath-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-10 10:37:16.000000 PySciMath-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:27:39.878052 PySciMath-1.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2649 2023-05-10 13:27:39.877056 PySciMath-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 13:27:39.850127 PySciMath-1.2.1/PySciMath/
+-rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.2.1/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0      591 2023-05-10 10:37:49.000000 PySciMath-1.2.1/PySciMath/ComplexNumbers.py
+-rw-rw-rw-   0        0        0     4281 2023-05-10 10:38:03.000000 PySciMath-1.2.1/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0     2818 2023-05-10 09:50:00.000000 PySciMath-1.2.1/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0     1350 2023-05-10 13:24:34.000000 PySciMath-1.2.1/PySciMath/Numbers.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.2.1/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.2.1/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.2.1/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0      637 2023-05-10 09:41:19.000000 PySciMath-1.2.1/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:27:39.873066 PySciMath-1.2.1/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2649 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 13:27:39.000000 PySciMath-1.2.1/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2134 2023-05-10 13:24:03.000000 PySciMath-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:27:39.879048 PySciMath-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-10 13:23:30.000000 PySciMath-1.2.1/setup.py
```

### Comparing `PySciMath-1.2.0/LICENSE.txt` & `PySciMath-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PKG-INFO` & `PySciMath-1.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,50 @@
-Metadata-Version: 2.1
-Name: PySciMath
-Version: 1.2.0
-Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
-Home-page: https://github.com/Anikethc/PySciMath
-Download-URL: https://pypi.org/project/pyscimath
-Author: Aniketh Chavare
-Author-email: anikethchavare@outlook.com
-License: MIT
-Keywords: Math,Calculations
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PySciMath
-
-## Introduction
-
-PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
-
-Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
-
-## Module Information
-
-**Name** - PySciMath </br>
-**Version** - 1.2.0 </br>
-**Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
-**Author** - Aniketh Chavare </br>
-**Author's Email** - anikethchavare@gmail.com </br>
-**GitHub URL** - [https://github.com/Anikethc/PyMathSolver](https://github.com/Anikethc/PyMathSolver). </br>
-**Pypi.org URL** - [https://pypi.org/project/pymathsolver](https://pypi.org/project/pymathsolver). </br>
-**Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs).
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Aniketh Chavare
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-## Issues & Bugs
-
-If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
-
-## Conclusion
-
-I hope you liked this module. Thank you!
+# PySciMath
+
+## Introduction
+
+PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
+
+Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
+
+## Module Information
+
+**Name** - PySciMath </br>
+**Version** - 1.2.1 </br>
+**Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
+**Author** - Aniketh Chavare </br>
+**Author's Email** - anikethchavare@gmail.com </br>
+**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath) </br>
+**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath) </br>
+**Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Aniketh Chavare
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+## Issues & Bugs
+
+If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
+
+## Conclusion
+
+I hope you liked this module. Thank you!
```

### Comparing `PySciMath-1.2.0/PySciMath/ComplexNumbers.py` & `PySciMath-1.2.1/PySciMath/ComplexNumbers.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath/CoordinateGeometry.py` & `PySciMath-1.2.1/PySciMath/CoordinateGeometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath/Geometry.py` & `PySciMath-1.2.1/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath/Numbers.py` & `PySciMath-1.2.1/PySciMath/Numbers.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,10 @@
 
 # Functions - Squares and Cubes
 def square(number): return power(number, 2)
 def cube(number): return power(number, 3)
 def squareRoot(number): return number ** 0.5
 def cubeRoot(number): return number ** (1/3)
 
-# Functions - Positive and Negative
-def isPositive(number): return number > 0
-def isNegative(number): return number < 0
-
 # Functions - Odd and Even
 def isOdd(number): return number % 2 == 1
 def isEven(number): return number % 2 == 0
```

### Comparing `PySciMath-1.2.0/PySciMath/Quadratic.py` & `PySciMath-1.2.1/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath/Statistics.py` & `PySciMath-1.2.1/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath/Trigonometry.py` & `PySciMath-1.2.1/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath/__init__.py` & `PySciMath-1.2.1/PySciMath/__init__.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.2.0/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.2.0
+Version: 1.2.1
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,21 +18,21 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath </br>
-**Version** - 1.2.0 </br>
+**Version** - 1.2.1 </br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare </br>
 **Author's Email** - anikethchavare@gmail.com </br>
-**GitHub URL** - [https://github.com/Anikethc/PyMathSolver](https://github.com/Anikethc/PyMathSolver). </br>
-**Pypi.org URL** - [https://pypi.org/project/pymathsolver](https://pypi.org/project/pymathsolver). </br>
-**Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs).
+**GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath) </br>
+**Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath) </br>
+**Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
 MIT License
 
 Copyright (c) 2023 Aniketh Chavare
```

### Comparing `PySciMath-1.2.0/setup.py` & `PySciMath-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.2.0",
+    version="1.2.1",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

