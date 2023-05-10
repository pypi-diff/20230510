# Comparing `tmp/PySciMath-1.1.0.tar.gz` & `tmp/PySciMath-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.1.0.tar", last modified: Wed May 10 10:04:11 2023, max compression
+gzip compressed data, was "PySciMath-1.2.0.tar", last modified: Wed May 10 10:41:19 2023, max compression
```

## Comparing `PySciMath-1.1.0.tar` & `PySciMath-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:04:11.852280 PySciMath-1.1.0/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2667 2023-05-10 10:04:11.851281 PySciMath-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 10:04:11.840312 PySciMath-1.1.0/PySciMath/
--rw-rw-rw-   0        0        0      593 2023-05-10 09:45:35.000000 PySciMath-1.1.0/PySciMath/ComplexNumbers.py
--rw-rw-rw-   0        0        0     4283 2023-05-10 09:46:47.000000 PySciMath-1.1.0/PySciMath/CoordinateGeometry.py
--rw-rw-rw-   0        0        0     2818 2023-05-10 09:50:00.000000 PySciMath-1.1.0/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0     1228 2023-05-10 09:41:32.000000 PySciMath-1.1.0/PySciMath/Numbers.py
--rw-rw-rw-   0        0        0      374 2023-05-10 09:50:41.000000 PySciMath-1.1.0/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.1.0/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.1.0/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0      637 2023-05-10 09:41:19.000000 PySciMath-1.1.0/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:04:11.849287 PySciMath-1.1.0/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2667 2023-05-10 10:04:11.000000 PySciMath-1.1.0/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-05-10 10:04:11.000000 PySciMath-1.1.0/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:04:11.000000 PySciMath-1.1.0/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 10:04:11.000000 PySciMath-1.1.0/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2152 2023-05-10 10:03:44.000000 PySciMath-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 10:04:11.853275 PySciMath-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-10 09:57:57.000000 PySciMath-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:41:19.284534 PySciMath-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2664 2023-05-10 10:41:19.283537 PySciMath-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 10:41:19.270572 PySciMath-1.2.0/PySciMath/
+-rw-rw-rw-   0        0        0      431 2023-05-10 10:33:22.000000 PySciMath-1.2.0/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0      591 2023-05-10 10:37:49.000000 PySciMath-1.2.0/PySciMath/ComplexNumbers.py
+-rw-rw-rw-   0        0        0     4281 2023-05-10 10:38:03.000000 PySciMath-1.2.0/PySciMath/CoordinateGeometry.py
+-rw-rw-rw-   0        0        0     2818 2023-05-10 09:50:00.000000 PySciMath-1.2.0/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0     1475 2023-05-10 10:22:01.000000 PySciMath-1.2.0/PySciMath/Numbers.py
+-rw-rw-rw-   0        0        0      568 2023-05-10 10:26:42.000000 PySciMath-1.2.0/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1392 2023-05-10 09:43:22.000000 PySciMath-1.2.0/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.2.0/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0      637 2023-05-10 09:41:19.000000 PySciMath-1.2.0/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:41:19.280545 PySciMath-1.2.0/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2664 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 10:41:19.000000 PySciMath-1.2.0/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2149 2023-05-10 10:40:03.000000 PySciMath-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:41:19.284534 PySciMath-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-10 10:37:16.000000 PySciMath-1.2.0/setup.py
```

### Comparing `PySciMath-1.1.0/LICENSE.txt` & `PySciMath-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.1.0/PKG-INFO` & `PySciMath-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.1.0
+Version: 1.2.0
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyMathSolver
+# PySciMath
 
 ## Introduction
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath </br>
-**Version** - 1.1.0 </br>
+**Version** - 1.2.0 </br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare </br>
 **Author's Email** - anikethchavare@gmail.com </br>
 **GitHub URL** - [https://github.com/Anikethc/PyMathSolver](https://github.com/Anikethc/PyMathSolver). </br>
 **Pypi.org URL** - [https://pypi.org/project/pymathsolver](https://pypi.org/project/pymathsolver). </br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs).
```

### Comparing `PySciMath-1.1.0/PySciMath/ComplexNumbers.py` & `PySciMath-1.2.0/PySciMath/ComplexNumbers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# PySciMath - Complex Numbers
+# PySciMath - ComplexNumbers
 
-''' This is the "Complex Numbers" sub-module. '''
+''' This is the "ComplexNumbers" sub-module. '''
 
 # Imports
 import math
 import cmath
 
 # Functions - Algebra
 def addition(z1, z2): return z1 + z2
```

### Comparing `PySciMath-1.1.0/PySciMath/CoordinateGeometry.py` & `PySciMath-1.2.0/PySciMath/CoordinateGeometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# PySciMath - Coordinate Geometry
+# PySciMath - CoordinateGeometry
 
-''' This is the "Coordinate Geometry" sub-module. '''
+''' This is the "CoordinateGeometry" sub-module. '''
 
 # Imports
 import math
 
 # Function 1 - Distance
 def distance(point1, point2):
     distance = None
```

### Comparing `PySciMath-1.1.0/PySciMath/Geometry.py` & `PySciMath-1.2.0/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.1.0/PySciMath/Numbers.py` & `PySciMath-1.2.0/PySciMath/Numbers.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             lcm = greater
             break
         greater += 1
 
     return lcm
 
 # Function 3 - Prime
-def prime(number):
+def isPrime(number):
     isPrime = False
 
     if (number < 1):
         isPrime = False
     else:
         for i in range(2, int(number/2) + 1):
             if (number % i == 0):
@@ -48,15 +48,20 @@
     num = 1
 
     for i in range(exponent, 0, -1):
         num *= base
 
     return num
 
-# Function 5 - Square
+# Functions - Squares and Cubes
 def square(number): return power(number, 2)
-
-# Function 6 - Cube
 def cube(number): return power(number, 3)
+def squareRoot(number): return number ** 0.5
+def cubeRoot(number): return number ** (1/3)
 
-# Function 7 - Square Root
-def squareRoot(number): return number ** 0.5
+# Functions - Positive and Negative
+def isPositive(number): return number > 0
+def isNegative(number): return number < 0
+
+# Functions - Odd and Even
+def isOdd(number): return number % 2 == 1
+def isEven(number): return number % 2 == 0
```

### Comparing `PySciMath-1.1.0/PySciMath/Statistics.py` & `PySciMath-1.2.0/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.1.0/PySciMath/Trigonometry.py` & `PySciMath-1.2.0/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.1.0/PySciMath/__init__.py` & `PySciMath-1.2.0/PySciMath/__init__.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.1.0/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.2.0/PySciMath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.1.0
+Version: 1.2.0
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/pyscimath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyMathSolver
+# PySciMath
 
 ## Introduction
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath </br>
-**Version** - 1.1.0 </br>
+**Version** - 1.2.0 </br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare </br>
 **Author's Email** - anikethchavare@gmail.com </br>
 **GitHub URL** - [https://github.com/Anikethc/PyMathSolver](https://github.com/Anikethc/PyMathSolver). </br>
 **Pypi.org URL** - [https://pypi.org/project/pymathsolver](https://pypi.org/project/pymathsolver). </br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs).
```

### Comparing `PySciMath-1.1.0/README.md` & `PySciMath-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# PyMathSolver
+# PySciMath
 
 ## Introduction
 
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath </br>
-**Version** - 1.1.0 </br>
+**Version** - 1.2.0 </br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare </br>
 **Author's Email** - anikethchavare@gmail.com </br>
 **GitHub URL** - [https://github.com/Anikethc/PyMathSolver](https://github.com/Anikethc/PyMathSolver). </br>
 **Pypi.org URL** - [https://pypi.org/project/pymathsolver](https://pypi.org/project/pymathsolver). </br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs).
```

### Comparing `PySciMath-1.1.0/setup.py` & `PySciMath-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.1.0",
+    version="1.2.0",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

