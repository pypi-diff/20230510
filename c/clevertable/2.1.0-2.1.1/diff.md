# Comparing `tmp/clevertable-2.1.0.tar.gz` & `tmp/clevertable-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.1.0.tar", last modified: Tue May  9 06:39:26 2023, max compression
+gzip compressed data, was "clevertable-2.1.1.tar", last modified: Wed May 10 15:58:02 2023, max compression
```

## Comparing `clevertable-2.1.0.tar` & `clevertable-2.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.086484 clevertable-2.1.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    28874 2023-05-09 06:39:26.086484 clevertable-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    27104 2023-05-04 17:35:13.000000 clevertable-2.1.0/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-09 06:34:18.000000 clevertable-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 06:39:26.086484 clevertable-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.023056 clevertable-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.071442 clevertable-2.1.0/src/clevertable/
--rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.1.0/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-01 14:12:57.000000 clevertable-2.1.0/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.1.0/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.1.0/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.1.0/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.1.0/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.1.0/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.1.0/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.1.0/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     3864 2023-05-01 18:32:23.000000 clevertable-2.1.0/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.1.0/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.1.0/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.1.0/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.1.0/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.1.0/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.1.0/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.1.0/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.1.0/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.1.0/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.1.0/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.1.0/src/clevertable/Split.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.1.0/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0      312 2023-05-01 14:33:36.000000 clevertable-2.1.0/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2535 2023-05-04 10:32:03.000000 clevertable-2.1.0/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      672 2023-05-09 06:34:18.000000 clevertable-2.1.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.1.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2731 2023-05-02 18:50:19.000000 clevertable-2.1.0/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:39:26.086484 clevertable-2.1.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    28874 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-05-09 06:39:26.000000 clevertable-2.1.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-09 06:39:25.000000 clevertable-2.1.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.387510 clevertable-2.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0    31025 2023-05-10 15:58:02.386688 clevertable-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29255 2023-05-10 15:55:34.000000 clevertable-2.1.1/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-10 15:57:08.000000 clevertable-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 15:58:02.387510 clevertable-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.297219 clevertable-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.371991 clevertable-2.1.1/src/clevertable/
+-rw-rw-rw-   0        0        0     2761 2023-05-03 09:47:00.000000 clevertable-2.1.1/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-01 14:12:57.000000 clevertable-2.1.1/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     2948 2023-05-04 17:33:19.000000 clevertable-2.1.1/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.1.1/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     3672 2023-05-04 12:32:37.000000 clevertable-2.1.1/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.1.1/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.1.1/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.1.1/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.1.1/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     3864 2023-05-01 18:32:23.000000 clevertable-2.1.1/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.1.1/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.1.1/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.1.1/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      563 2023-05-03 06:07:00.000000 clevertable-2.1.1/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.1.1/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.1.1/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.1.1/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1836 2023-05-03 15:33:14.000000 clevertable-2.1.1/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.1.1/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     6334 2023-05-04 05:34:03.000000 clevertable-2.1.1/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.1.1/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.1.1/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0      312 2023-05-01 14:33:36.000000 clevertable-2.1.1/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.1.1/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      672 2023-05-10 15:57:08.000000 clevertable-2.1.1/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.1.1/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2664 2023-05-09 10:07:13.000000 clevertable-2.1.1/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:58:02.384986 clevertable-2.1.1/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    31025 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 15:58:02.000000 clevertable-2.1.1/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.1.0/LICENSE` & `clevertable-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/PKG-INFO` & `clevertable-2.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,85 @@
-Metadata-Version: 2.1
-Name: clevertable
-Version: 2.1.0
-Summary: Low effort conversion of tabular data into numerical values.
-Author: Tom Mohr
-License: MIT License
-        
-        Copyright (c) 2023 Tom Mohr
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/tom-mohr/clevertable
-Keywords: parser,converter,numerical
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # CleverTable
 
-Consistent and intelligent conversion of tabular data into numerical values.<br>
+Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
 ```bash
 pip install clevertable
 ```
 
 Example:
 
 ```python
 from clevertable import *
 
 profile = ConversionProfile({
-    # optional: specify converters for specific columns
+    # optionally specify converters for specific columns:
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
-    "Hospitalized": Ignore(),
+    "Hospitalized": None,  # ignore column
 }, pre_processing=None)
 
 df = profile.fit_transform("datasets/survey.xlsx")  # transformed pandas.DataFrame
 ```
 
+# Why this Library?
+
+- CleverTable makes it really easy to convert text-based tabular data
+  (optionally mixed with numbers), e.g. a medical survey,
+  into numerical data, e.g. a Pandas DataFrame or a NumPy array.
+- If something is obvious, you should not need to specify it.
+  CleverTable will try to make choices for you if you don't make them.
+- You stay in control: All choices made by CleverTable can be modified and overridden.
+
+This is how CleverTable works:
+
+1. You create a new `profile = ConversionProfile()`.
+   Here, you can specify certain converters, but you don't have to.
+2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
+    - CleverTable chooses the best converter if you don't specify it.
+    - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
+3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
+   which converts the data according to the fixed profile.
+
+Here are some examples on what you can do with CleverTable:
+
+- Chain multiple converters to achieve complex conversions:
+  ```python
+  profile["Column 7"] = [
+      Split(),
+      ForEach(Strip()),
+      Flatten(),
+      Infer()  # Infer() -> CleverTable will choose what to put here
+  ]
+  ```
+- Use the `Infer()` converter where you want CleverTable to figure out the best solution (see above).
+- Concise shorthand writings with Python syntax:
+  ```python
+  profile["Column 1"] = [  # Python lists create pipelines
+    str.lower,             # functions /
+    lambda s: s.strip(),   # lambda expressions are allowed
+  ]
+  profile["Column 2"] = {"Hello": 1, "Bye": 2}
+  profile["Column 3"] = Float(), 1  # tries conversion to float, defaults to 1 on error
+  ```
+- Incremental configuration: If a column already has a correct converter, you can further process the column
+  by adding another converter.
+  This implicitly creates a pipeline.
+  ```python
+  profile["Column 5"] += OneHot()
+  ```
+- After `fit()`, you can access the inferred state of the converters.
+  ```python
+  my_weather_conv = profile["Weather"]            # e.g. OneHot()
+  my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
+  ```
+
 # Tutorial
 
 Suppose you want to convert the following table of survey results into a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
 | China   | 32  | benign    | no           | University      | cough, fever    |
@@ -233,28 +248,30 @@
 
 # CLI
 
 `pip install clevertable` also makes the command `clevertable` available
 in the command line.
 It can convert files with tabular data.
 Execute `clevertable --help` to see what arguments can be passed to the tool:
+
 ```text
 usage: clevertable [-h] [-i IGNORE [IGNORE ...]] src out
 
 Consistent and intelligent conversion of tabular data into numerical values.
 
 positional arguments:
   src                   Path to input file.
   out                   Path to output file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i IGNORE [IGNORE ...], --ignore IGNORE [IGNORE ...]
                         Column names to ignore.
 ```
+
 # How to Contribute
 
 Basic workflow of contribution:
 
 - Fork the repository
 - Create a new branch
 - Make your changes
@@ -281,43 +298,43 @@
 - `ConversionProfile`: A collection of converters.
 - `Converter`: Transforms columns of data into columns of data.
 
 ## Converters
 
 Here's a quick overview of all converters:
 
-| Converters                  | Description                                                                       | Shorthand        | Example Usage                                                   |
-|-----------------------------|-----------------------------------------------------------------------------------|------------------|-----------------------------------------------------------------|
-| Basic:                      |                                                                                   |                  |                                                                 |
-| [`Float()`](#float)         | Converts numbers into floats.                                                     |                  |                                                                 |
-| [`Enumerate()`](#enumerate) |                                                                                   |                  |                                                                 |
-| [`OneHot()`](#onehot)       |                                                                                   |                  |                                                                 |
-| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |                  |                                                                 |
-| [`List()`](#list)           |                                                                                   |                  |                                                                 |
-| [`ListAndOr()`](#listandor) |                                                                                   |                  |                                                                 |
-| [`Map()`](#map)             |                                                                                   | dict             | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
-| [`Const()`](#const)         | Returns a constant value.                                                         | *any*            | 42<br>"foo"                                                     |
-| Text Processing:            |                                                                                   |                  |                                                                 |
-| [`Strip()`](#strip)         |                                                                                   |                  |                                                                 |
-| [`Split()`](#split)         |                                                                                   |                  |                                                                 |
-| Combining Converters:       |                                                                                   |                  |                                                                 |
-| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list             | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
-| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  |                  |                                                                 |
-| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |                  |                                                                 |
-| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               | tuple[Converter] | `(Strip(), Id(), lambda s: s[:3])`                              |
-| Special:                    |                                                                                   |                  |                                                                 |
-| [`Id()`](#id)               |                                                                                   |                  |                                                                 |
-| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None             | None                                                            |
-| [`Infer()`](#infer)         |                                                                                   |                  |                                                                 |
-| [`Label()`](#label)         |                                                                                   | tuple[str]       | ("A", "B", "C")<br>("A",)<br>Label("A")<br>Label("A", "B", "C") |
-| Dimensionality:             |                                                                                   |                  |                                                                 |
-| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |                  |                                                                 |
-| [`Transpose()`](#transpose) |                                                                                   |                  |                                                                 |
-| Arbitrary Functions:        |                                                                                   |                  |                                                                 |
-| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable*       | lambda x: x**2                                                  |
+| Converters                  | Description                                                                       | Shorthand  | Example Usage                                                   |
+|-----------------------------|-----------------------------------------------------------------------------------|------------|-----------------------------------------------------------------|
+| Basic:                      |                                                                                   |            |                                                                 |
+| [`Float()`](#float)         | Converts numbers into floats.                                                     |            |                                                                 |
+| [`Enumerate()`](#enumerate) |                                                                                   |            |                                                                 |
+| [`OneHot()`](#onehot)       |                                                                                   |            |                                                                 |
+| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |            |                                                                 |
+| [`List()`](#list)           |                                                                                   |            |                                                                 |
+| [`ListAndOr()`](#listandor) |                                                                                   |            |                                                                 |
+| [`Map()`](#map)             |                                                                                   | dict       | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
+| [`Const()`](#const)         | Returns a constant value.                                                         | *any*      | 42<br>"foo"                                                     |
+| Text Processing:            |                                                                                   |            |                                                                 |
+| [`Strip()`](#strip)         |                                                                                   |            |                                                                 |
+| [`Split()`](#split)         |                                                                                   |            |                                                                 |
+| Combining Converters:       |                                                                                   |            |                                                                 |
+| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list       | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
+| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  | tuple      | (Float(), Binary())                                             |
+| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |            |                                                                 |
+| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               |            |                                                                 |
+| Special:                    |                                                                                   |            |                                                                 |
+| [`Id()`](#id)               |                                                                                   |            |                                                                 |
+| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None       | None                                                            |
+| [`Infer()`](#infer)         |                                                                                   |            |                                                                 |
+| [`Label()`](#label)         |                                                                                   |            |                                                                 |
+| Dimensionality:             |                                                                                   |            |                                                                 |
+| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |            |                                                                 |
+| [`Transpose()`](#transpose) |                                                                                   |            |                                                                 |
+| Arbitrary Functions:        |                                                                                   |            |                                                                 |
+| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable* | lambda x: x**2                                                  |
 
 ---
 
 ### Float
 
 Converts a column of numbers into a column of numbers.
 If invalid values are encountered (`NaN`, `inf`, `None`, etc.),
@@ -538,15 +555,15 @@
 ```
 
 Returns value of the first converter that does not raise an exception,
 or the original value if all converters raise an exception.
 `Try()` always only applies one converter and returns its output (if it didn't fail).
 
 ```python
-"Product": Try(Float(), Infer()),  # will infer the converter for the samples that cannot be converted to floats
+"Product": Try(Float(), Infer())  # will infer the converter for the samples that cannot be converted to floats
 ```
 
 | Product | ⇒ | Product |
 |---------|---|---------|
 | Kiwi    |   | 48      |
 | Apple   |   | 0       |
 | 712356  |   | 712356  |
```

### Comparing `clevertable-2.1.0/README.md` & `clevertable-2.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,122 @@
+Metadata-Version: 2.1
+Name: clevertable
+Version: 2.1.1
+Summary: Low effort conversion of tabular data into numerical values.
+Author: Tom Mohr
+License: MIT License
+        
+        Copyright (c) 2023 Tom Mohr
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/tom-mohr/clevertable
+Keywords: parser,converter,numerical
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # CleverTable
 
-Consistent and intelligent conversion of tabular data into numerical values.<br>
+Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
 ```bash
 pip install clevertable
 ```
 
 Example:
 
 ```python
 from clevertable import *
 
 profile = ConversionProfile({
-    # optional: specify converters for specific columns
+    # optionally specify converters for specific columns:
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
-    "Hospitalized": Ignore(),
+    "Hospitalized": None,  # ignore column
 }, pre_processing=None)
 
 df = profile.fit_transform("datasets/survey.xlsx")  # transformed pandas.DataFrame
 ```
 
+# Why this Library?
+
+- CleverTable makes it really easy to convert text-based tabular data
+  (optionally mixed with numbers), e.g. a medical survey,
+  into numerical data, e.g. a Pandas DataFrame or a NumPy array.
+- If something is obvious, you should not need to specify it.
+  CleverTable will try to make choices for you if you don't make them.
+- You stay in control: All choices made by CleverTable can be modified and overridden.
+
+This is how CleverTable works:
+
+1. You create a new `profile = ConversionProfile()`.
+   Here, you can specify certain converters, but you don't have to.
+2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
+    - CleverTable chooses the best converter if you don't specify it.
+    - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
+3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
+   which converts the data according to the fixed profile.
+
+Here are some examples on what you can do with CleverTable:
+
+- Chain multiple converters to achieve complex conversions:
+  ```python
+  profile["Column 7"] = [
+      Split(),
+      ForEach(Strip()),
+      Flatten(),
+      Infer()  # Infer() -> CleverTable will choose what to put here
+  ]
+  ```
+- Use the `Infer()` converter where you want CleverTable to figure out the best solution (see above).
+- Concise shorthand writings with Python syntax:
+  ```python
+  profile["Column 1"] = [  # Python lists create pipelines
+    str.lower,             # functions /
+    lambda s: s.strip(),   # lambda expressions are allowed
+  ]
+  profile["Column 2"] = {"Hello": 1, "Bye": 2}
+  profile["Column 3"] = Float(), 1  # tries conversion to float, defaults to 1 on error
+  ```
+- Incremental configuration: If a column already has a correct converter, you can further process the column
+  by adding another converter.
+  This implicitly creates a pipeline.
+  ```python
+  profile["Column 5"] += OneHot()
+  ```
+- After `fit()`, you can access the inferred state of the converters.
+  ```python
+  my_weather_conv = profile["Weather"]            # e.g. OneHot()
+  my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
+  ```
+
 # Tutorial
 
 Suppose you want to convert the following table of survey results into a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
 | China   | 32  | benign    | no           | University      | cough, fever    |
@@ -196,28 +285,30 @@
 
 # CLI
 
 `pip install clevertable` also makes the command `clevertable` available
 in the command line.
 It can convert files with tabular data.
 Execute `clevertable --help` to see what arguments can be passed to the tool:
+
 ```text
 usage: clevertable [-h] [-i IGNORE [IGNORE ...]] src out
 
 Consistent and intelligent conversion of tabular data into numerical values.
 
 positional arguments:
   src                   Path to input file.
   out                   Path to output file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i IGNORE [IGNORE ...], --ignore IGNORE [IGNORE ...]
                         Column names to ignore.
 ```
+
 # How to Contribute
 
 Basic workflow of contribution:
 
 - Fork the repository
 - Create a new branch
 - Make your changes
@@ -244,43 +335,43 @@
 - `ConversionProfile`: A collection of converters.
 - `Converter`: Transforms columns of data into columns of data.
 
 ## Converters
 
 Here's a quick overview of all converters:
 
-| Converters                  | Description                                                                       | Shorthand        | Example Usage                                                   |
-|-----------------------------|-----------------------------------------------------------------------------------|------------------|-----------------------------------------------------------------|
-| Basic:                      |                                                                                   |                  |                                                                 |
-| [`Float()`](#float)         | Converts numbers into floats.                                                     |                  |                                                                 |
-| [`Enumerate()`](#enumerate) |                                                                                   |                  |                                                                 |
-| [`OneHot()`](#onehot)       |                                                                                   |                  |                                                                 |
-| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |                  |                                                                 |
-| [`List()`](#list)           |                                                                                   |                  |                                                                 |
-| [`ListAndOr()`](#listandor) |                                                                                   |                  |                                                                 |
-| [`Map()`](#map)             |                                                                                   | dict             | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
-| [`Const()`](#const)         | Returns a constant value.                                                         | *any*            | 42<br>"foo"                                                     |
-| Text Processing:            |                                                                                   |                  |                                                                 |
-| [`Strip()`](#strip)         |                                                                                   |                  |                                                                 |
-| [`Split()`](#split)         |                                                                                   |                  |                                                                 |
-| Combining Converters:       |                                                                                   |                  |                                                                 |
-| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list             | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
-| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  |                  |                                                                 |
-| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |                  |                                                                 |
-| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               | tuple[Converter] | `(Strip(), Id(), lambda s: s[:3])`                              |
-| Special:                    |                                                                                   |                  |                                                                 |
-| [`Id()`](#id)               |                                                                                   |                  |                                                                 |
-| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None             | None                                                            |
-| [`Infer()`](#infer)         |                                                                                   |                  |                                                                 |
-| [`Label()`](#label)         |                                                                                   | tuple[str]       | ("A", "B", "C")<br>("A",)<br>Label("A")<br>Label("A", "B", "C") |
-| Dimensionality:             |                                                                                   |                  |                                                                 |
-| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |                  |                                                                 |
-| [`Transpose()`](#transpose) |                                                                                   |                  |                                                                 |
-| Arbitrary Functions:        |                                                                                   |                  |                                                                 |
-| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable*       | lambda x: x**2                                                  |
+| Converters                  | Description                                                                       | Shorthand  | Example Usage                                                   |
+|-----------------------------|-----------------------------------------------------------------------------------|------------|-----------------------------------------------------------------|
+| Basic:                      |                                                                                   |            |                                                                 |
+| [`Float()`](#float)         | Converts numbers into floats.                                                     |            |                                                                 |
+| [`Enumerate()`](#enumerate) |                                                                                   |            |                                                                 |
+| [`OneHot()`](#onehot)       |                                                                                   |            |                                                                 |
+| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |            |                                                                 |
+| [`List()`](#list)           |                                                                                   |            |                                                                 |
+| [`ListAndOr()`](#listandor) |                                                                                   |            |                                                                 |
+| [`Map()`](#map)             |                                                                                   | dict       | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
+| [`Const()`](#const)         | Returns a constant value.                                                         | *any*      | 42<br>"foo"                                                     |
+| Text Processing:            |                                                                                   |            |                                                                 |
+| [`Strip()`](#strip)         |                                                                                   |            |                                                                 |
+| [`Split()`](#split)         |                                                                                   |            |                                                                 |
+| Combining Converters:       |                                                                                   |            |                                                                 |
+| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list       | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
+| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  | tuple      | (Float(), Binary())                                             |
+| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |            |                                                                 |
+| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               |            |                                                                 |
+| Special:                    |                                                                                   |            |                                                                 |
+| [`Id()`](#id)               |                                                                                   |            |                                                                 |
+| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None       | None                                                            |
+| [`Infer()`](#infer)         |                                                                                   |            |                                                                 |
+| [`Label()`](#label)         |                                                                                   |            |                                                                 |
+| Dimensionality:             |                                                                                   |            |                                                                 |
+| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |            |                                                                 |
+| [`Transpose()`](#transpose) |                                                                                   |            |                                                                 |
+| Arbitrary Functions:        |                                                                                   |            |                                                                 |
+| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable* | lambda x: x**2                                                  |
 
 ---
 
 ### Float
 
 Converts a column of numbers into a column of numbers.
 If invalid values are encountered (`NaN`, `inf`, `None`, etc.),
@@ -501,15 +592,15 @@
 ```
 
 Returns value of the first converter that does not raise an exception,
 or the original value if all converters raise an exception.
 `Try()` always only applies one converter and returns its output (if it didn't fail).
 
 ```python
-"Product": Try(Float(), Infer()),  # will infer the converter for the samples that cannot be converted to floats
+"Product": Try(Float(), Infer())  # will infer the converter for the samples that cannot be converted to floats
 ```
 
 | Product | ⇒ | Product |
 |---------|---|---------|
 | Kiwi    |   | 48      |
 | Apple   |   | 0       |
 | 712356  |   | 712356  |
```

### Comparing `clevertable-2.1.0/pyproject.toml` & `clevertable-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.1.0"
+version = "2.1.1"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "2.1.0"
+current_version = "2.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.1.0/src/clevertable/Binary.py` & `clevertable-2.1.1/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/ConversionProfile.py` & `clevertable-2.1.1/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Converter.py` & `clevertable-2.1.1/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/DataFrameProfile.py` & `clevertable-2.1.1/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Enumerate.py` & `clevertable-2.1.1/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Float.py` & `clevertable-2.1.1/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/ForEach.py` & `clevertable-2.1.1/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Function.py` & `clevertable-2.1.1/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Infer.py` & `clevertable-2.1.1/src/clevertable/Infer.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Label.py` & `clevertable-2.1.1/src/clevertable/Label.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/List.py` & `clevertable-2.1.1/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Map.py` & `clevertable-2.1.1/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/OneHot.py` & `clevertable-2.1.1/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Parallel.py` & `clevertable-2.1.1/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Pipeline.py` & `clevertable-2.1.1/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/RecordProfile.py` & `clevertable-2.1.1/src/clevertable/RecordProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Split.py` & `clevertable-2.1.1/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Strip.py` & `clevertable-2.1.1/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/Try.py` & `clevertable-2.1.1/src/clevertable/Try.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             if not convs:
                 return  # no need to transform with last converter
 
             next_rows = []  # values that raise an exception
             for row in rows:
                 try:
                     conv.transform(row)
-                    return
                 except Exception as e:
                     if not isinstance(e, self.exceptions):
                         raise e
                     next_rows.append(row)
             rows = next_rows
             if not rows:
                 warnings.warn(f"All rows raised exceptions for {conv.__class__.__name__} converter,"
@@ -61,7 +60,16 @@
         for conv in self.converters:
             try:
                 return conv.transform(row)
             except Exception as e:
                 if not isinstance(e, self.exceptions):
                     raise e
         return row
+
+    def __getitem__(self, item):
+        return self.converters[item]
+
+    def __setitem__(self, key, value):
+        self.converters[key] = _parse_converter(value)
+
+    def __repr__(self):
+        return repr(tuple(self.converters))
```

### Comparing `clevertable-2.1.0/src/clevertable/__init__.py` & `clevertable-2.1.1/src/clevertable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-2.1.0/src/clevertable/__main__.py` & `clevertable-2.1.1/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.1.0/src/clevertable/_utils.py` & `clevertable-2.1.1/src/clevertable/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 from .Converter import Converter
 
 
 def _parse_converter(value: any) -> Converter:
     # dynamic imports in order to break circular dependency
     from .Const import Const
     from .Ignore import Ignore
-    from .Label import Label
     from .Map import Map
     from .Function import Function
     from .Pipeline import Pipeline
+    from .Try import Try
 
     if isinstance(value, Converter):
         return value
     if value is None:
         return Ignore()
-    if isinstance(value, str):
-        return Label(value)
     if isinstance(value, dict):
         return Map(value)
     if isinstance(value, tuple):
-        return Label(*value)
+        return Try(*value)
     if isinstance(value, list):
         return Pipeline(*value)
     if callable(value):
         return Function(value)
     return Const(value)
```

### Comparing `clevertable-2.1.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-2.1.1/src/clevertable.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.1.0
+Version: 2.1.1
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,38 +33,90 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # CleverTable
 
-Consistent and intelligent conversion of tabular data into numerical values.<br>
+Consistent, intelligent transformation of text-based tabular data into numerical data.<br>
 Minimal configuration required.
 
 Installation:
 
 ```bash
 pip install clevertable
 ```
 
 Example:
 
 ```python
 from clevertable import *
 
 profile = ConversionProfile({
-    # optional: specify converters for specific columns
+    # optionally specify converters for specific columns:
     "Country": OneHot(),
     "Diagnosis": Binary(positive="cancer", negative="benign"),
-    "Hospitalized": Ignore(),
+    "Hospitalized": None,  # ignore column
 }, pre_processing=None)
 
 df = profile.fit_transform("datasets/survey.xlsx")  # transformed pandas.DataFrame
 ```
 
+# Why this Library?
+
+- CleverTable makes it really easy to convert text-based tabular data
+  (optionally mixed with numbers), e.g. a medical survey,
+  into numerical data, e.g. a Pandas DataFrame or a NumPy array.
+- If something is obvious, you should not need to specify it.
+  CleverTable will try to make choices for you if you don't make them.
+- You stay in control: All choices made by CleverTable can be modified and overridden.
+
+This is how CleverTable works:
+
+1. You create a new `profile = ConversionProfile()`.
+   Here, you can specify certain converters, but you don't have to.
+2. You call `profile.fit(data)` on a sample data set, which creates a fixed conversion profile.
+    - CleverTable chooses the best converter if you don't specify it.
+    - The converter (chosen by you or by CleverTable) adapts its internal state to fit the data.
+3. You call `profile.transform(data)` on the actual data set (which may be the same as for `fit()`),
+   which converts the data according to the fixed profile.
+
+Here are some examples on what you can do with CleverTable:
+
+- Chain multiple converters to achieve complex conversions:
+  ```python
+  profile["Column 7"] = [
+      Split(),
+      ForEach(Strip()),
+      Flatten(),
+      Infer()  # Infer() -> CleverTable will choose what to put here
+  ]
+  ```
+- Use the `Infer()` converter where you want CleverTable to figure out the best solution (see above).
+- Concise shorthand writings with Python syntax:
+  ```python
+  profile["Column 1"] = [  # Python lists create pipelines
+    str.lower,             # functions /
+    lambda s: s.strip(),   # lambda expressions are allowed
+  ]
+  profile["Column 2"] = {"Hello": 1, "Bye": 2}
+  profile["Column 3"] = Float(), 1  # tries conversion to float, defaults to 1 on error
+  ```
+- Incremental configuration: If a column already has a correct converter, you can further process the column
+  by adding another converter.
+  This implicitly creates a pipeline.
+  ```python
+  profile["Column 5"] += OneHot()
+  ```
+- After `fit()`, you can access the inferred state of the converters.
+  ```python
+  my_weather_conv = profile["Weather"]            # e.g. OneHot()
+  my_weather_categories = my_weather_conv.values  # e.g. ["sunny", "cloudy", "rainy"]
+  ```
+
 # Tutorial
 
 Suppose you want to convert the following table of survey results into a 2D numpy array of numbers:
 
 | Country | Age | Diagnosis | Hospitalized | Education level | Symptoms        |
 |---------|-----|-----------|--------------|-----------------|-----------------|
 | China   | 32  | benign    | no           | University      | cough, fever    |
@@ -233,28 +285,30 @@
 
 # CLI
 
 `pip install clevertable` also makes the command `clevertable` available
 in the command line.
 It can convert files with tabular data.
 Execute `clevertable --help` to see what arguments can be passed to the tool:
+
 ```text
 usage: clevertable [-h] [-i IGNORE [IGNORE ...]] src out
 
 Consistent and intelligent conversion of tabular data into numerical values.
 
 positional arguments:
   src                   Path to input file.
   out                   Path to output file.
 
 optional arguments:
   -h, --help            show this help message and exit
   -i IGNORE [IGNORE ...], --ignore IGNORE [IGNORE ...]
                         Column names to ignore.
 ```
+
 # How to Contribute
 
 Basic workflow of contribution:
 
 - Fork the repository
 - Create a new branch
 - Make your changes
@@ -281,43 +335,43 @@
 - `ConversionProfile`: A collection of converters.
 - `Converter`: Transforms columns of data into columns of data.
 
 ## Converters
 
 Here's a quick overview of all converters:
 
-| Converters                  | Description                                                                       | Shorthand        | Example Usage                                                   |
-|-----------------------------|-----------------------------------------------------------------------------------|------------------|-----------------------------------------------------------------|
-| Basic:                      |                                                                                   |                  |                                                                 |
-| [`Float()`](#float)         | Converts numbers into floats.                                                     |                  |                                                                 |
-| [`Enumerate()`](#enumerate) |                                                                                   |                  |                                                                 |
-| [`OneHot()`](#onehot)       |                                                                                   |                  |                                                                 |
-| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |                  |                                                                 |
-| [`List()`](#list)           |                                                                                   |                  |                                                                 |
-| [`ListAndOr()`](#listandor) |                                                                                   |                  |                                                                 |
-| [`Map()`](#map)             |                                                                                   | dict             | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
-| [`Const()`](#const)         | Returns a constant value.                                                         | *any*            | 42<br>"foo"                                                     |
-| Text Processing:            |                                                                                   |                  |                                                                 |
-| [`Strip()`](#strip)         |                                                                                   |                  |                                                                 |
-| [`Split()`](#split)         |                                                                                   |                  |                                                                 |
-| Combining Converters:       |                                                                                   |                  |                                                                 |
-| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list             | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
-| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  |                  |                                                                 |
-| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |                  |                                                                 |
-| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               | tuple[Converter] | `(Strip(), Id(), lambda s: s[:3])`                              |
-| Special:                    |                                                                                   |                  |                                                                 |
-| [`Id()`](#id)               |                                                                                   |                  |                                                                 |
-| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None             | None                                                            |
-| [`Infer()`](#infer)         |                                                                                   |                  |                                                                 |
-| [`Label()`](#label)         |                                                                                   | tuple[str]       | ("A", "B", "C")<br>("A",)<br>Label("A")<br>Label("A", "B", "C") |
-| Dimensionality:             |                                                                                   |                  |                                                                 |
-| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |                  |                                                                 |
-| [`Transpose()`](#transpose) |                                                                                   |                  |                                                                 |
-| Arbitrary Functions:        |                                                                                   |                  |                                                                 |
-| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable*       | lambda x: x**2                                                  |
+| Converters                  | Description                                                                       | Shorthand  | Example Usage                                                   |
+|-----------------------------|-----------------------------------------------------------------------------------|------------|-----------------------------------------------------------------|
+| Basic:                      |                                                                                   |            |                                                                 |
+| [`Float()`](#float)         | Converts numbers into floats.                                                     |            |                                                                 |
+| [`Enumerate()`](#enumerate) |                                                                                   |            |                                                                 |
+| [`OneHot()`](#onehot)       |                                                                                   |            |                                                                 |
+| [`Binary()`](#binary)       | Converts a column of text into a column of integers.                              |            |                                                                 |
+| [`List()`](#list)           |                                                                                   |            |                                                                 |
+| [`ListAndOr()`](#listandor) |                                                                                   |            |                                                                 |
+| [`Map()`](#map)             |                                                                                   | dict       | {<br>&nbsp;&nbsp;"foo": 1,<br>&nbsp;&nbsp;"bar": -2,<br>}       |
+| [`Const()`](#const)         | Returns a constant value.                                                         | *any*      | 42<br>"foo"                                                     |
+| Text Processing:            |                                                                                   |            |                                                                 |
+| [`Strip()`](#strip)         |                                                                                   |            |                                                                 |
+| [`Split()`](#split)         |                                                                                   |            |                                                                 |
+| Combining Converters:       |                                                                                   |            |                                                                 |
+| [`Pipeline()`](#pipeline)   | Applies multiple converters in sequence.                                          | list       | [<br>&nbsp;&nbsp;Split(),<br>&nbsp;&nbsp;ForEach(Strip()),<br>] |
+| [`Try()`](#try)             | Try multiple converters and returns the first one that succeeds.                  | tuple      | (Float(), Binary())                                             |
+| [`ForEach()`](#foreach)     | Apply the same converter to all items.                                            |            |                                                                 |
+| [`Parallel()`](#parallel)   | Apply different converters to the respective items.                               |            |                                                                 |
+| Special:                    |                                                                                   |            |                                                                 |
+| [`Id()`](#id)               |                                                                                   |            |                                                                 |
+| [`Ignore()`](#ignore)       | Drops the column.                                                                 | None       | None                                                            |
+| [`Infer()`](#infer)         |                                                                                   |            |                                                                 |
+| [`Label()`](#label)         |                                                                                   |            |                                                                 |
+| Dimensionality:             |                                                                                   |            |                                                                 |
+| [`Flatten()`](#flatten)     | Flattens a list of lists into a single list. This is often needed after ForEach() |            |                                                                 |
+| [`Transpose()`](#transpose) |                                                                                   |            |                                                                 |
+| Arbitrary Functions:        |                                                                                   |            |                                                                 |
+| [`Function()`](#function)   | Applies a user-defined function to the data.                                      | *callable* | lambda x: x**2                                                  |
 
 ---
 
 ### Float
 
 Converts a column of numbers into a column of numbers.
 If invalid values are encountered (`NaN`, `inf`, `None`, etc.),
@@ -538,15 +592,15 @@
 ```
 
 Returns value of the first converter that does not raise an exception,
 or the original value if all converters raise an exception.
 `Try()` always only applies one converter and returns its output (if it didn't fail).
 
 ```python
-"Product": Try(Float(), Infer()),  # will infer the converter for the samples that cannot be converted to floats
+"Product": Try(Float(), Infer())  # will infer the converter for the samples that cannot be converted to floats
 ```
 
 | Product | ⇒ | Product |
 |---------|---|---------|
 | Kiwi    |   | 48      |
 | Apple   |   | 0       |
 | 712356  |   | 712356  |
```

### Comparing `clevertable-2.1.0/src/clevertable.egg-info/SOURCES.txt` & `clevertable-2.1.1/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

