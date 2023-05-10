# Comparing `tmp/benetech_annotation_parser-0.0.1.tar.gz` & `tmp/benetech_annotation_parser-0.0.3.tar.gz`

## Comparing `benetech_annotation_parser-0.0.1.tar` & `benetech_annotation_parser-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/Makefile
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/example/01_api_show_example.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/example/02_image_draw_example.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_image_generate.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_data/annotations/dummy_001.json
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_data/annotations/dummy_002.json
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_data/annotations/dummy_003.json
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_data/images/dummy_001.jpg
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_data/images/dummy_002.jpg
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/mock/dummy_data/images/dummy_003.jpg
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/src/convert_to_icdar2015.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/src/benetech_annotation_parser/_version.py
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/src/benetech_annotation_parser/annotation_api.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/LICENSE
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/README.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/Makefile
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/example/01_api_show_example.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/example/02_image_draw_example.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_image_generate.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_data/annotations/dummy_001.json
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_data/annotations/dummy_002.json
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_data/annotations/dummy_003.json
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_data/images/dummy_001.jpg
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_data/images/dummy_002.jpg
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/mock/dummy_data/images/dummy_003.jpg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/src/benetech_annotation_parser/_version.py
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/src/benetech_annotation_parser/annotation_api.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/README.md
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 benetech_annotation_parser-0.0.3/PKG-INFO
```

### Comparing `benetech_annotation_parser-0.0.1/.github/workflows/ci.yaml` & `benetech_annotation_parser-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/.github/workflows/publish.yaml` & `benetech_annotation_parser-0.0.3/.github/workflows/publish.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -15,17 +15,16 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.8"
       - name: Build-install
         run: |
           python -m pip install --upgrade pip
           pip install build hatch
+          python -m hatch version "${GITHUB_REF_NAME}"
           hatch build
       - name: build
         run: |
           python -m build
       - name: upload
         uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
-
-          
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `benetech_annotation_parser-0.0.1/example/01_api_show_example.py` & `benetech_annotation_parser-0.0.3/example/01_api_show_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.benetech_annotation_parser.annotation_api import AnnotationParser, Axis
+from benetech_annotation_parser.annotation_api import AnnotationParser, Axis
 
 annotation_parser = AnnotationParser("mock/dummy_data")
 
 # (0) "Extract one JSON data from a list of JSON file paths."
 p = annotation_parser.get_annotation(0)
 """
 print(p.name)
```

### Comparing `benetech_annotation_parser-0.0.1/example/02_image_draw_example.py` & `benetech_annotation_parser-0.0.3/example/02_image_draw_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Dict
 from PIL import Image, ImageDraw
 
-from src.benetech_annotation_parser.annotation_api import AnnotationParser, Axis
+from benetech_annotation_parser.annotation_api import AnnotationParser, Axis
 
 def draw_rect_angle(img:Image.Image, rectangle_coord:Dict[str, int]):
     x0 = rectangle_coord['x0']
     y0 = rectangle_coord['y0']
     h = rectangle_coord['height']
     w = rectangle_coord['width']
     draw = ImageDraw.Draw(img)
@@ -31,15 +31,15 @@
     
 def draw_point(img:Image.Image, coord:Dict[str, int]):
     draw = ImageDraw.Draw(img)
     draw.ellipse([(coord['x'] - 1 , coord['y']-1), (coord['x']+1, coord['y']+1)], fill="lime", outline="lime", width=10)
     
 if __name__ == "__main__":
     # bentech data path (i.e. /mnt/data/train/)
-    # The demo is available on a Kaggle notebook(link). 
+    # The demo is available on a Kaggle notebook(https://www.kaggle.com/koyyy0/benetech-annotation-parser/). 
     # Please refer to the Kaggle notebook for more details.
     data_path = 'mock/dummy_data'
     index = 0
 
     annotation_parser = AnnotationParser(data_path)
     ap= annotation_parser.get_annotation(index=0)
     img = Image.open(ap.image_path)
```

### Comparing `benetech_annotation_parser-0.0.1/mock/dummy_data/annotations/dummy_001.json` & `benetech_annotation_parser-0.0.3/mock/dummy_data/annotations/dummy_001.json`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/mock/dummy_data/annotations/dummy_002.json` & `benetech_annotation_parser-0.0.3/mock/dummy_data/annotations/dummy_002.json`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/mock/dummy_data/annotations/dummy_003.json` & `benetech_annotation_parser-0.0.3/mock/dummy_data/annotations/dummy_003.json`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/mock/dummy_data/images/dummy_001.jpg` & `benetech_annotation_parser-0.0.3/mock/dummy_data/images/dummy_001.jpg`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/mock/dummy_data/images/dummy_002.jpg` & `benetech_annotation_parser-0.0.3/mock/dummy_data/images/dummy_002.jpg`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/mock/dummy_data/images/dummy_003.jpg` & `benetech_annotation_parser-0.0.3/mock/dummy_data/images/dummy_003.jpg`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/src/benetech_annotation_parser/annotation_api.py` & `benetech_annotation_parser-0.0.3/src/benetech_annotation_parser/annotation_api.py`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/LICENSE` & `benetech_annotation_parser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `benetech_annotation_parser-0.0.1/README.md` & `benetech_annotation_parser-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # bentech annotation parser
-Simple Python API to read the annotation data of the Kaggle/Benetech-Making Graphs Accessible competition. For more details on the Kaggle/Benetech-Making Graphs Accessible competition, please refer to the following:[https://www.kaggle.com/competitions/benetech-making-graphs-accessible](https://www.kaggle.com/competitions/benetech-making-graphs-accessible).
+Simple Python API to read the annotation data of the Kaggle/Benetech-Making Graphs Accessible competition. For more details on the Kaggle/Benetech-Making Graphs Accessible competition, please refer to the following: [https://www.kaggle.com/competitions/benetech-making-graphs-accessible](https://www.kaggle.com/competitions/benetech-making-graphs-accessible).
 
 # Installing
 
 ```bash
 pip install benetech-annotation-parser
 ```
 
@@ -160,8 +160,8 @@
 """
 >>> p.data_series(filter='y')
 [15.66666, 5.555555]
 """
 ```
 
 # Demo
-The demo is available on a Kaggle notebook[(link)](url). Please refer to the Kaggle notebook for more details.
+The demo is available on a Kaggle notebook[[https://www.kaggle.com/koyyy0/benetech-annotation-parser/]](https://www.kaggle.com/koyyy0/benetech-annotation-parser/). Please refer to the Kaggle notebook for more details.
```

### Comparing `benetech_annotation_parser-0.0.1/pyproject.toml` & `benetech_annotation_parser-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,23 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = ["pillow"]
+dependencies = []
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/Kololu777/benetech-annotation-parser"
 
 [project.optional-dependencies]
 dev = [
+    "pillow",
     "build >=0.10.0",
     "pytest >=7.3.1",
     "black >=23.3.0",
     "flake8 >=6.0.0",
     "isort >=5.12.0",
     "twine >=4.0.2",
 ]
```

### Comparing `benetech_annotation_parser-0.0.1/PKG-INFO` & `benetech_annotation_parser-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: benetech-annotation-parser
-Version: 0.0.1
+Version: 0.0.3
 Summary: benetech annotation parser
 Project-URL: Homepage, https://github.com/Kololu777/benetech-annotation-parser
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: pillow
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: build>=0.10.0; extra == 'dev'
 Requires-Dist: flake8>=6.0.0; extra == 'dev'
 Requires-Dist: isort>=5.12.0; extra == 'dev'
+Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pytest>=7.3.1; extra == 'dev'
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # bentech annotation parser
-Simple Python API to read the annotation data of the Kaggle/Benetech-Making Graphs Accessible competition. For more details on the Kaggle/Benetech-Making Graphs Accessible competition, please refer to the following:[https://www.kaggle.com/competitions/benetech-making-graphs-accessible](https://www.kaggle.com/competitions/benetech-making-graphs-accessible).
+Simple Python API to read the annotation data of the Kaggle/Benetech-Making Graphs Accessible competition. For more details on the Kaggle/Benetech-Making Graphs Accessible competition, please refer to the following: [https://www.kaggle.com/competitions/benetech-making-graphs-accessible](https://www.kaggle.com/competitions/benetech-making-graphs-accessible).
 
 # Installing
 
 ```bash
 pip install benetech-annotation-parser
 ```
 
@@ -184,8 +184,8 @@
 """
 >>> p.data_series(filter='y')
 [15.66666, 5.555555]
 """
 ```
 
 # Demo
-The demo is available on a Kaggle notebook[(link)](url). Please refer to the Kaggle notebook for more details.
+The demo is available on a Kaggle notebook[[https://www.kaggle.com/koyyy0/benetech-annotation-parser/]](https://www.kaggle.com/koyyy0/benetech-annotation-parser/). Please refer to the Kaggle notebook for more details.
```

