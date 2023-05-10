# Comparing `tmp/coco_types-0.0.8.tar.gz` & `tmp/coco_types-0.0.9.tar.gz`

## Comparing `coco_types-0.0.8.tar` & `coco_types-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 coco_types-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 coco_types-0.0.8/pytest.ini
--rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 coco_types-0.0.8/setup.cfg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 coco_types-0.0.8/requirements/README.md
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 coco_types-0.0.8/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 coco_types-0.0.8/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 coco_types-0.0.8/requirements/requirements-test.txt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 coco_types-0.0.8/requirements/requirements.txt
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/__init__.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/coco_keypoints.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/coco_object_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/py.typed
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/dicts/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/dicts/coco_keypoints.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 coco_types-0.0.8/src/coco_types/dicts/coco_object_detection.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 coco_types-0.0.8/tests/test_load_pydantic.py
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 coco_types-0.0.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 coco_types-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 coco_types-0.0.8/README.md
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 coco_types-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 coco_types-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 coco_types-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 coco_types-0.0.9/pytest.ini
+-rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 coco_types-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 coco_types-0.0.9/requirements/README.md
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 coco_types-0.0.9/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 coco_types-0.0.9/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 coco_types-0.0.9/requirements/requirements-flake8.txt
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 coco_types-0.0.9/requirements/requirements-test.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 coco_types-0.0.9/requirements/requirements.txt
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/__init__.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/coco_keypoints.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/coco_object_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/py.typed
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/dicts/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/dicts/coco_keypoints.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 coco_types-0.0.9/src/coco_types/dicts/coco_object_detection.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 coco_types-0.0.9/tests/test_load_pydantic.py
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 coco_types-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 coco_types-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 coco_types-0.0.9/README.md
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 coco_types-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 coco_types-0.0.9/PKG-INFO
```

### Comparing `coco_types-0.0.8/.pre-commit-config.yaml` & `coco_types-0.0.9/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -11,22 +11,37 @@
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
-        exclude: typings
       - id: trailing-whitespace
-        exclude: typings
       - id: mixed-line-ending
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.253"
     hooks:
       - id: ruff
 
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.300
     hooks:
     - id: pyright
-      additional_dependencies: ["pydantic", "coco_types"]
+      additional_dependencies: ["pydantic", "numpy", "coco_types"]
+
+  - repo: https://github.com/PyCQA/flake8
+    rev: 5.0.4
+    hooks:
+      - id: flake8
+        additional_dependencies:
+          - flake8-bugbear
+          - flake8-comprehensions
+          - flake8-docstrings
+          - flake8-builtins
+          - flake8-quotes
+          - pep8-naming
+          - flake8-import-order
+          - flake8-noqa
+          - flake8-broken-line
+          - flake8-commas
+          - Flake8-pyproject
```

### Comparing `coco_types-0.0.8/setup.cfg` & `coco_types-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.8/requirements/README.md` & `coco_types-0.0.9/requirements/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,8 +2,9 @@
 
 The requirements can be re-generated with the following commands
 ```
 pip-compile --output-file=requirements/requirements.txt --resolver=backtracking pyproject.toml
 pip-compile --extra=test --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml
 pip-compile --extra=dev --output-file=requirements/requirements-dev.txt --resolver=backtracking pyproject.toml
 pip-compile --extra=build --output-file=requirements/requirements-build.txt --resolver=backtracking pyproject.toml
+pip-compile --extra=flake8 --output-file=requirements/requirements-flake8.txt --resolver=backtracking pyproject.toml
 ```
```

### Comparing `coco_types-0.0.8/requirements/requirements-build.txt` & `coco_types-0.0.9/requirements/requirements-build.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,34 +18,34 @@
     #   userpath
 cryptography==40.0.2
     # via secretstorage
 distlib==0.3.6
     # via virtualenv
 editables==0.3
     # via hatchling
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
 h11==0.14.0
     # via httpcore
 hatch==1.7.0
-    # via coco_types (pyproject.toml)
-hatchling==1.14.0
+    # via coco-types (pyproject.toml)
+hatchling==1.14.1
     # via hatch
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
     # via hatch
 hyperlink==21.0.0
     # via hatch
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   hyperlink
-importlib-metadata==6.4.1
+importlib-metadata==6.6.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
@@ -53,58 +53,60 @@
     # via hatch
 markdown-it-py==2.2.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
+numpy==1.24.3
+    # via coco-types (pyproject.toml)
 packaging==23.1
     # via
     #   hatch
     #   hatchling
 pathspec==0.11.1
     # via hatchling
 pexpect==4.8.0
     # via hatch
-platformdirs==3.2.0
+platformdirs==3.5.0
     # via
     #   hatch
     #   virtualenv
 pluggy==1.0.0
     # via hatchling
 ptyprocess==0.7.0
     # via pexpect
 pycparser==2.21
     # via cffi
 pydantic==1.10.7
-    # via coco_types (pyproject.toml)
-pygments==2.15.0
+    # via coco-types (pyproject.toml)
+pygments==2.15.1
     # via rich
 pyperclip==1.8.2
     # via hatch
-rich==13.3.4
+rich==13.3.5
     # via hatch
 secretstorage==3.3.3
     # via keyring
 shellingham==1.5.0.post1
     # via hatch
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
 tomli==2.0.1
     # via hatchling
 tomli-w==1.0.0
     # via hatch
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via hatch
-trove-classifiers==2023.3.9
+trove-classifiers==2023.4.29
     # via hatchling
 typing-extensions==4.5.0
     # via pydantic
 userpath==1.8.0
     # via hatch
-virtualenv==20.21.0
+virtualenv==20.23.0
     # via hatch
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `coco_types-0.0.8/requirements/requirements-dev.txt` & `coco_types-0.0.9/requirements/requirements-dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,47 +8,49 @@
     # via pip-tools
 cfgv==3.3.1
     # via pre-commit
 click==8.1.3
     # via pip-tools
 distlib==0.3.6
     # via virtualenv
-filelock==3.11.0
+filelock==3.12.0
     # via virtualenv
-identify==2.5.22
+identify==2.5.23
     # via pre-commit
 nodeenv==1.7.0
     # via
     #   pre-commit
     #   pyright
+numpy==1.24.3
+    # via coco-types (pyproject.toml)
 packaging==23.1
     # via build
 pip-tools==6.13.0
-    # via coco_types (pyproject.toml)
-platformdirs==3.2.0
+    # via coco-types (pyproject.toml)
+platformdirs==3.5.0
     # via virtualenv
 pre-commit==3.2.2
-    # via coco_types (pyproject.toml)
+    # via coco-types (pyproject.toml)
 pydantic==1.10.7
-    # via coco_types (pyproject.toml)
+    # via coco-types (pyproject.toml)
 pyproject-hooks==1.0.0
     # via build
-pyright==1.1.303
-    # via coco_types (pyproject.toml)
+pyright==1.1.305
+    # via coco-types (pyproject.toml)
 pyyaml==6.0
     # via pre-commit
-ruff==0.0.261
-    # via coco_types (pyproject.toml)
+ruff==0.0.263
+    # via coco-types (pyproject.toml)
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
 typing-extensions==4.5.0
     # via pydantic
-virtualenv==20.21.0
+virtualenv==20.23.0
     # via pre-commit
 wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `coco_types-0.0.8/requirements/requirements-test.txt` & `coco_types-0.0.9/requirements/requirements-test.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 #
 #    pip-compile --extra=test --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml
 #
 exceptiongroup==1.1.1
     # via pytest
 iniconfig==2.0.0
     # via pytest
+numpy==1.24.3
+    # via coco-types (pyproject.toml)
 packaging==23.1
     # via pytest
 pluggy==1.0.0
     # via pytest
 pydantic==1.10.7
-    # via coco_types (pyproject.toml)
+    # via coco-types (pyproject.toml)
 pytest==7.3.1
-    # via coco_types (pyproject.toml)
+    # via coco-types (pyproject.toml)
 tomli==2.0.1
     # via pytest
 typing-extensions==4.5.0
     # via pydantic
```

### Comparing `coco_types-0.0.8/src/coco_types/__init__.py` & `coco_types-0.0.9/src/coco_types/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from . import dicts  # pyright: ignore[reportUnusedImport]
 from .coco_keypoints import AnnotationKP, AnnotationKPAny, CategoryKP, DatasetKP
 from .coco_object_detection import (
     Annotation,
     AnnotationAny,
     Category,
     COCO_RLE,
     Dataset,
+    EvaluationResult,
     Image,
     Info,
     Licence,
     RLE,
     TPolygonSegmentation,
 )
 
 __all__ = [
-    "Annotation", "AnnotationAny", "Category", "COCO_RLE", "Dataset", "Image", "Info", "RLE", "Licence",
-    "TPolygonSegmentation",
+    "Annotation", "AnnotationAny", "Category", "COCO_RLE", "Dataset", "EvaluationResult", "Image", "Info", "RLE",
+    "Licence", "TPolygonSegmentation",
     "AnnotationKPAny", "AnnotationKP", "CategoryKP", "DatasetKP",
 ]
```

### Comparing `coco_types-0.0.8/src/coco_types/coco_keypoints.py` & `coco_types-0.0.9/src/coco_types/coco_keypoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pydantic import validator  # pyright: ignore[reportUnknownVariableType]
 
 from .coco_object_detection import Annotation, Category, COCO_RLE, Dataset, RLE, TPolygonSegmentation
 
 TSegmentation = TypeVar("TSegmentation", TPolygonSegmentation, RLE, COCO_RLE)
 
+
 class AnnotationKP(Annotation[TSegmentation], Generic[TSegmentation]):
     keypoints: list[int]
     num_keypoints: int
 
     @validator("keypoints")
     def keypoints_length(cls, keypoints: list[int]) -> list[int]:
         assert len(keypoints) % 3 == 0, (
@@ -27,16 +28,18 @@
     @validator("num_keypoints")
     def num_keypoints_matches_keypoints_length(cls, num_keypoints: int, values: dict[str, list[int]]) -> int:
         if len(values["keypoints"]) // 3 != num_keypoints:
             raise ValueError(f"Length of the keypoints list ({len(values['keypoints'])}) does not match "
                              f"the number of keypoints ({num_keypoints}).")
         return num_keypoints
 
+
 AnnotationKPAny: TypeAlias = AnnotationKP[TPolygonSegmentation] | AnnotationKP[RLE] | AnnotationKP[COCO_RLE]
 
+
 class CategoryKP(Category):
     keypoints: list[str]
     skeleton: list[tuple[int, int]]
 
 
 class DatasetKP(Dataset):
     annotations: list[AnnotationKPAny]
```

### Comparing `coco_types-0.0.8/src/coco_types/coco_object_detection.py` & `coco_types-0.0.9/src/coco_types/coco_object_detection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Generic, Literal, TypeAlias, TypeVar
 
+import numpy as np
+import numpy.typing as npt
 from pydantic import BaseModel
 from pydantic.generics import GenericModel
 
 
 class Info(BaseModel):
     year: int
     version: str
@@ -53,21 +55,40 @@
     segmentation: _TSegmentation
     area: float
     # The COCO bounding box format is [top left x position, top left y position, width, height].
     # bbox exemple:  "bbox": [473.07,395.93,38.65,28.67]
     bbox: list[float]
     iscrowd: Literal[0] | Literal[1]
 
+
 AnnotationAny: TypeAlias = Annotation[TPolygonSegmentation] | Annotation[RLE] | Annotation[COCO_RLE]
 
+
 class Category(BaseModel):
     id: int
     name: str
     supercategory: str
 
 
 class Dataset(BaseModel):
     info: Info | None = None
     licences: list[Licence] | None = None
     images: list[Image]
     annotations: list[AnnotationAny]
     categories: list[Category]
+
+
+class EvaluationResult(BaseModel):
+    image_id: int
+    category_id: int
+    aRng: list[int]
+    maxDet: int
+    dtIds: list[int]
+    gtIds: list[int]
+    dtMatches: npt.NDArray[np.float64]
+    gtMatches: npt.NDArray[np.float64]
+    dtScores: list[float]
+    gtIgnore: npt.NDArray[np.float64]
+    dtIgnore: npt.NDArray[np.float64]
+
+    class Config:
+        arbitrary_types_allowed = True
```

### Comparing `coco_types-0.0.8/src/coco_types/dicts/coco_object_detection.py` & `coco_types-0.0.9/src/coco_types/dicts/coco_object_detection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from typing import Literal, TypeAlias, TypedDict
 
+import numpy as np
+import numpy.typing as npt
+
 
 class Info(TypedDict):
     year: int
     version: str
     description: str
     contributor: str
     url: str
@@ -59,7 +62,21 @@
 
 class Dataset(TypedDict):
     info: Info
     licences: list[Licence]
     images: list[Image]
     annotations: list[Annotation]
     categories: list[Category]
+
+
+class EvaluationResult(TypedDict):
+    image_id: int
+    category_id: int
+    aRng: list[int]
+    maxDet: int
+    dtIds: list[int]
+    gtIds: list[int]
+    dtMatches: npt.NDArray[np.float64]
+    gtMatches: npt.NDArray[np.float64]
+    dtScores: list[float]
+    gtIgnore: npt.NDArray[np.float64]
+    dtIgnore: npt.NDArray[np.float64]
```

### Comparing `coco_types-0.0.8/LICENSE.md` & `coco_types-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.8/README.md` & `coco_types-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coco_types-0.0.8/pyproject.toml` & `coco_types-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -14,25 +14,26 @@
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Operating System :: OS Independent",
             "Intended Audience :: Developers",
 ]
 license = {text = "MIT"}
 dynamic = ["version"]
-dependencies = ["pydantic"]
+dependencies = ["pydantic", "numpy"]
 requires-python = ">=3.9"
 
 [project.urls]
-"Homepage" = "https://github.com/hoel-bagard/coco_types"
-"Bug Tracker" = "https://github.com/hoel-bagard/coco_types/issues"
+"Homepage" = "https://github.com/hoel-bagard/coco-types"
+"Bug Tracker" = "https://github.com/hoel-bagard/coco-types/issues"
 
 [project.optional-dependencies]
 test = ["pytest"]
 dev = ["pre-commit", "pip-tools", "ruff", "pyright"]
 build = ["hatch"]
+flake8 = ["flake8", "flake8-bugbear", "flake8-comprehensions", "flake8-docstrings", "flake8-builtins", "flake8-quotes", "pep8-naming", "flake8-import-order", "flake8-noqa", "flake8-broken-line", "flake8-commas", "Flake8-pyproject"]
 
 [tool.hatch.version]
 path = "src/coco_types/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
@@ -101,7 +102,32 @@
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
 
 pythonVersion = "3.10"
 pythonPlatform = "Linux"
+
+[tool.flake8]
+max-line-length = 120
+docstring-convention = "google"
+import-order-style = "smarkets"
+application_import_names = "src"
+
+# F401  # Imported but unused
+# N801  # class name 'COCO_RLE' should use CapWords convention
+per-file-ignores = [
+    "__init__.py:F401,F403",
+    "*detection.py:N801"
+]
+exclude = ["env", "venv"]
+
+# D1    # Do not require docstrings
+# W503  # Line break occurred before a binary operator  (Should already be gone so...)
+# E226  # Missing whitespace around arithmetic operator  --> 0.1*b + 0.2*c is considered "wrong"
+# N805  # first argument of a method should be named 'self'
+# A003  # class attribute "id" is shadowing a python builtin
+# N815  # variable 'X' in class scope should not be mixedCase
+ignore = ["A003", "D1", "W503", "E226", "N805", "N815"]
+inline-quotes = "double"
+# Cyclomatic complexity for functions
+max-complexity = 20
```

### Comparing `coco_types-0.0.8/PKG-INFO` & `coco_types-0.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 Metadata-Version: 2.1
 Name: coco-types
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for handling COCO datasets types.
-Project-URL: Homepage, https://github.com/hoel-bagard/coco_types
-Project-URL: Bug Tracker, https://github.com/hoel-bagard/coco_types/issues
+Project-URL: Homepage, https://github.com/hoel-bagard/coco-types
+Project-URL: Bug Tracker, https://github.com/hoel-bagard/coco-types/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE.md
 Keywords: COCO,COCO dataset
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
+Requires-Dist: numpy
 Requires-Dist: pydantic
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: flake8
+Requires-Dist: flake8; extra == 'flake8'
+Requires-Dist: flake8-broken-line; extra == 'flake8'
+Requires-Dist: flake8-bugbear; extra == 'flake8'
+Requires-Dist: flake8-builtins; extra == 'flake8'
+Requires-Dist: flake8-commas; extra == 'flake8'
+Requires-Dist: flake8-comprehensions; extra == 'flake8'
+Requires-Dist: flake8-docstrings; extra == 'flake8'
+Requires-Dist: flake8-import-order; extra == 'flake8'
+Requires-Dist: flake8-noqa; extra == 'flake8'
+Requires-Dist: flake8-pyproject; extra == 'flake8'
+Requires-Dist: flake8-quotes; extra == 'flake8'
+Requires-Dist: pep8-naming; extra == 'flake8'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # COCO Types
 
 Note: This package loads the data as is and does not create dictionaries mapping ids to lists of images/annotations/categories.
```

