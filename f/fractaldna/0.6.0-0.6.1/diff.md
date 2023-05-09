# Comparing `tmp/fractaldna-0.6.0.tar.gz` & `tmp/fractaldna-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractaldna-0.6.0.tar", max compression
+gzip compressed data, was "fractaldna-0.6.1.tar", max compression
```

## Comparing `fractaldna-0.6.0.tar` & `fractaldna-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2022-01-30 05:48:44.418142 fractaldna-0.6.0/LICENSE
--rw-r--r--   0        0        0     3858 2022-02-20 10:37:06.101028 fractaldna-0.6.0/README.md
--rw-r--r--   0        0        0      475 2022-01-26 04:49:20.891954 fractaldna-0.6.0/fractaldna/__init__.py
--rw-r--r--   0        0        0     1559 2022-01-26 04:49:20.892688 fractaldna-0.6.0/fractaldna/__main__.py
--rw-r--r--   0        0        0     8823 2022-01-25 04:36:02.962279 fractaldna-0.6.0/fractaldna/dna_models/basepair.py
--rw-r--r--   0        0        0    59977 2022-10-22 04:44:08.275849 fractaldna-0.6.0/fractaldna/dna_models/dnachain.py
--rw-r--r--   0        0        0    20498 2022-05-08 06:52:24.057297 fractaldna-0.6.0/fractaldna/dna_models/dnapositions.py
--rw-r--r--   0        0        0     9192 2022-01-25 04:36:02.964463 fractaldna-0.6.0/fractaldna/dna_models/molecules.py
--rw-r--r--   0        0        0      110 2022-01-25 04:36:02.964685 fractaldna-0.6.0/fractaldna/exceptions.py
--rw-r--r--   0        0        0        0 2022-01-25 04:36:02.964787 fractaldna-0.6.0/fractaldna/py.typed
--rw-r--r--   0        0        0     5334 2022-06-19 12:06:03.934172 fractaldna-0.6.0/fractaldna/structure_models/hilbert.py
--rw-r--r--   0        0        0    17929 2022-10-22 04:44:08.276732 fractaldna-0.6.0/fractaldna/structure_models/random_placements.py
--rw-r--r--   0        0        0    19928 2022-10-22 04:44:08.277579 fractaldna-0.6.0/fractaldna/structure_models/voxelisation.py
--rw-r--r--   0        0        0       37 2022-01-25 04:36:02.966719 fractaldna-0.6.0/fractaldna/utils/__init__.py
--rw-r--r--   0        0        0       99 2022-01-25 04:36:02.966892 fractaldna-0.6.0/fractaldna/utils/constants.py
--rw-r--r--   0        0        0      385 2022-01-25 04:36:02.967097 fractaldna-0.6.0/fractaldna/utils/logging.py
--rw-r--r--   0        0        0    14436 2022-05-08 06:52:24.060583 fractaldna-0.6.0/fractaldna/utils/rotations.py
--rw-r--r--   0        0        0      832 2022-01-25 04:36:02.967951 fractaldna-0.6.0/fractaldna/utils/sequence.py
--rw-r--r--   0        0        0     3963 2022-10-22 04:44:26.916880 fractaldna-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5061 2022-10-22 04:45:51.305392 fractaldna-0.6.0/setup.py
--rw-r--r--   0        0        0     5328 2022-10-22 04:45:51.305776 fractaldna-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-01-30 05:48:44.418142 fractaldna-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3858 2022-02-20 10:37:06.101028 fractaldna-0.6.1/README.md
+-rw-r--r--   0        0        0      475 2022-01-26 04:49:20.891954 fractaldna-0.6.1/fractaldna/__init__.py
+-rw-r--r--   0        0        0     1559 2022-01-26 04:49:20.892688 fractaldna-0.6.1/fractaldna/__main__.py
+-rw-r--r--   0        0        0     8823 2023-01-01 05:29:19.790141 fractaldna-0.6.1/fractaldna/dna_models/basepair.py
+-rw-r--r--   0        0        0    59977 2022-10-22 04:44:08.275849 fractaldna-0.6.1/fractaldna/dna_models/dnachain.py
+-rw-r--r--   0        0        0    20498 2022-05-08 06:52:24.057297 fractaldna-0.6.1/fractaldna/dna_models/dnapositions.py
+-rw-r--r--   0        0        0    10124 2023-05-09 23:45:11.416447 fractaldna-0.6.1/fractaldna/dna_models/molecules.py
+-rw-r--r--   0        0        0      110 2022-01-25 04:36:02.964685 fractaldna-0.6.1/fractaldna/exceptions.py
+-rw-r--r--   0        0        0        0 2022-01-25 04:36:02.964787 fractaldna-0.6.1/fractaldna/py.typed
+-rw-r--r--   0        0        0     5334 2022-06-19 12:06:03.934172 fractaldna-0.6.1/fractaldna/structure_models/hilbert.py
+-rw-r--r--   0        0        0    17929 2022-10-22 04:44:08.276732 fractaldna-0.6.1/fractaldna/structure_models/random_placements.py
+-rw-r--r--   0        0        0    19928 2022-10-22 04:44:08.277579 fractaldna-0.6.1/fractaldna/structure_models/voxelisation.py
+-rw-r--r--   0        0        0       37 2022-01-25 04:36:02.966719 fractaldna-0.6.1/fractaldna/utils/__init__.py
+-rw-r--r--   0        0        0       99 2022-01-25 04:36:02.966892 fractaldna-0.6.1/fractaldna/utils/constants.py
+-rw-r--r--   0        0        0      385 2022-01-25 04:36:02.967097 fractaldna-0.6.1/fractaldna/utils/logging.py
+-rw-r--r--   0        0        0    14436 2022-05-08 06:52:24.060583 fractaldna-0.6.1/fractaldna/utils/rotations.py
+-rw-r--r--   0        0        0      832 2022-01-25 04:36:02.967951 fractaldna-0.6.1/fractaldna/utils/sequence.py
+-rw-r--r--   0        0        0     4096 2023-05-09 23:45:27.704089 fractaldna-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5182 2023-05-09 23:46:40.844002 fractaldna-0.6.1/setup.py
+-rw-r--r--   0        0        0     5428 2023-05-09 23:46:40.844467 fractaldna-0.6.1/PKG-INFO
```

### Comparing `fractaldna-0.6.0/LICENSE` & `fractaldna-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/README.md` & `fractaldna-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/__main__.py` & `fractaldna-0.6.1/fractaldna/__main__.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/dna_models/basepair.py` & `fractaldna-0.6.1/fractaldna/dna_models/basepair.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/dna_models/dnachain.py` & `fractaldna-0.6.1/fractaldna/dna_models/dnachain.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/dna_models/dnapositions.py` & `fractaldna-0.6.1/fractaldna/dna_models/dnapositions.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/dna_models/molecules.py` & `fractaldna-0.6.1/fractaldna/dna_models/molecules.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,14 +147,38 @@
                 "pos_z": self.position[2],
                 "rot_x": self.rotation[0],
                 "rot_y": self.rotation[1],
                 "rot_z": self.rotation[2],
             }
         )
 
+    def point_in_molecule(self, point: np.array) -> bool:
+        """
+        Assert whether a point (x, y, z) is inside the molecule.
+
+        :param: point (x, y, z)
+        :return: True/False point in molecule
+        """
+        point_ = np.asarray(point)
+        if point_.shape != (3,):
+            raise ValueError("Point should have shape (3, ). That is [1,2,3]")
+        # Step 1: assume molecule at (0, 0, 0)
+        point_ = point_ - self.position
+        # Step 2: We are going to treat the ellipse as un-rotated, so we apply
+        #         an inverse rotation to the point
+        rot_matrix = rot.eulerMatrix(*self.rotation)
+        point_ = np.matmul(np.linalg.inv(rot_matrix), point_.reshape(3, 1))
+
+        test = (
+            (point_[0] / self.dimensions[0]) ** 2.0
+            + (point_[1] / self.dimensions[1]) ** 2.0
+            + (point_[2] / self.dimensions[2]) ** 2.0
+        )
+        return test < 1
+
 
 # Define some standard molecules
 class Guanine(Molecule):
     """
     Guanine molecule
 
     :param strand: strand ID
```

### Comparing `fractaldna-0.6.0/fractaldna/structure_models/hilbert.py` & `fractaldna-0.6.1/fractaldna/structure_models/hilbert.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/structure_models/random_placements.py` & `fractaldna-0.6.1/fractaldna/structure_models/random_placements.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/structure_models/voxelisation.py` & `fractaldna-0.6.1/fractaldna/structure_models/voxelisation.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/utils/rotations.py` & `fractaldna-0.6.1/fractaldna/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/fractaldna/utils/sequence.py` & `fractaldna-0.6.1/fractaldna/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `fractaldna-0.6.0/pyproject.toml` & `fractaldna-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fractaldna"
-version = "v0.6.0"
+version = "v0.6.1"
 description = "FractalDNA is a Python package built to generate DNA geometries for simulations"
 readme = "README.md"
 authors = ["Nathanael Lampe"]
 license = "MIT"
 repository = "https://github.com/natl/fractaldna"
 homepage = "https://github.com/natl/fractaldna"
 documentation = "https://natl.github.io/fractaldna"
@@ -40,45 +40,48 @@
 python = ">=3.8,<3.11"
 typer = {extras = ["all"], version = ">=0.3.2,<0.5.0"}
 rich = ">=10.7,<13.0"
 numpy = "^1.22.0"
 pandas = "^1.3.3"
 matplotlib = "^3.4.3"
 scipy = "^1.8.0"
-pytest = ">=6.2.5,<8.0.0"
 importlib-metadata = "^4.8.2"
 tqdm = "^4.62.3"
-mistune = "0.8.4"
+mayavi = { version = "^4.8.1", optional = true }
+PyQt5 = { version = "^5.15.9", optional = true }
+vtk = { version = "^9.2.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.0"
 black = {version = "^22.1", allow-prereleases = true}
 darglint = "^1.8.0"
 isort = {extras = ["colors"], version = "^5.9.3"}
 mypy = "^0.961"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.14.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.14.3"
-pytest = "^6.2.5"
+pytest = "^7.2.0"
 pyupgrade = "^2.24.0"
-safety = "^1.10.3"
+safety = "^2.3.5"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autodoc-typehints = "^1.17.0"
 ipykernel = "^6.6.0"
+ipython = "<=8.12"
 ipyevents = "^2.0.1"
 nbsphinx = "^0.8.8"
+pandoc = "^2.3"
 
 [tool.poetry.extras]
 mayavi = ["mayavi", "PyQt5", "vtk"]
 
 [tool.black]
 # https://github.com/psf/black
-target-version = ["py38"]
+target-version = ["py39"]
 line-length = 88
 color = true
 
 exclude = '''
 /(
     \.git
     | \.hg
@@ -105,15 +108,15 @@
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.8
+python_version = 3.9
 pretty = true
 show_traceback = true
 color_output = true
 
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
@@ -142,8 +145,8 @@
 
 # Extra options:
 addopts = [
   "--strict-markers",
   "--tb=short",
   "--doctest-modules",
   "--doctest-continue-on-failure",
-]
+]
```

### Comparing `fractaldna-0.6.0/setup.py` & `fractaldna-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,38 +9,42 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['importlib-metadata>=4.8.2,<5.0.0',
  'matplotlib>=3.4.3,<4.0.0',
- 'mistune==0.8.4',
  'numpy>=1.22.0,<2.0.0',
  'pandas>=1.3.3,<2.0.0',
- 'pytest>=6.2.5,<8.0.0',
  'rich>=10.7,<13.0',
  'scipy>=1.8.0,<2.0.0',
  'tqdm>=4.62.3,<5.0.0',
  'typer[all]>=0.3.2,<0.5.0']
 
+extras_require = \
+{'mayavi': ['mayavi>=4.8.1,<5.0.0',
+            'PyQt5>=5.15.9,<6.0.0',
+            'vtk>=9.2.6,<10.0.0']}
+
 entry_points = \
 {'console_scripts': ['fractaldna = fractaldna.__main__:app']}
 
 setup_kwargs = {
     'name': 'fractaldna',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'FractalDNA is a Python package built to generate DNA geometries for simulations',
     'long_description': 'FractalDNA\n===\nPython routines for generating geometric models of DNA\n---\n\n*FractalDNA is being converted to a package, it is under active developmemt*\n\n<div align="center">\n\n[![Build status](https://github.com/natl/fractaldna/workflows/build/badge.svg?branch=master&event=push)](https://github.com/natl/fractaldna/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/fractaldna.svg)](https://pypi.org/project/fractaldna/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/natl/fractaldna/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/natl/fractaldna/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/natl/fractaldna/releases)\n[![License](https://img.shields.io/github/license/natl/fractaldna)](https://github.com/natl/fractaldna/blob/master/LICENSE)\n\n</div>\n\nFractalDNA is a Python package to make DNA geometries that can be joined together like\njigsaw puzzles. Both simple, sections of DNA and Solenoidal DNA can be built. This\nmodule was built to enable DNA-level simulations to be run in [Geant4-DNA](http://geant4-dna.in2p3.fr/), part of the\n[Geant4](geant4.cern.ch/) project.\n\nStructure models define the large scale structure of DNA,\nseeded from fractals. An example seeding fractal is below:\n\n<p align="center">\n  <img width="460" height="300" src="https://raw.githubusercontent.com/natl/fractaldna/master/docs/source/images/fractal-path.svg" alt="A 3-D iterated Hilbert Curve">\n</p>\n\nDNA Models provide straight and curved segments that can come together to\nmake DNA for use in simulations.\n\n<p align="center">\n  <img width="460" height="300" src="https://raw.githubusercontent.com/natl/fractaldna/master/docs/source/images/single_solenoid_line_plot.jpg" alt="A straight solenoidal DNA segment">\n</p>\n\nProject documentation is available [here](http://natl.github.io/fractaldna/) alongside [notebook examples](http://natl.github.io/fractaldna/examples.html)\n\n## ⚙️ Installation\n\nInstall FractalDNA with `pip`\n\n```bash\npip install fractaldna\n```\n\nor install with `Poetry`\n\n```bash\npoetry add fractaldna\n```\n\n## 🧬 Make some DNA\n\n```py\nfrom fractaldna.dna_models import dnachain as dna\n\n# Make a DNA Chain 40 base pairs long (repeating GATC).\nchain = dna.DNAChain("GTAC" * 10)\n\n# Export it to a DataFrame for use in another program\ndf = chain.to_frame()\n```\n\nFor more, check out the [notebook examples](http://natl.github.io/fractaldna/examples.html) in the project documentation.\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/natl/fractaldna)](https://github.com/natl/fractaldna/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/natl/fractaldna/blob/master/LICENSE) for more details.\n\n## 📃 Citation\n\n```bibtex\n@misc{fractaldna,\n  author = {Nathanael Lampe},\n  title = {FractalDNA},\n  year = {2021},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/natl/fractaldna}}\n}\n```\n\n## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)\n\nThis project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)',
     'author': 'Nathanael Lampe',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/natl/fractaldna',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fractaldna-0.6.0/PKG-INFO` & `fractaldna-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractaldna
-Version: 0.6.0
+Version: 0.6.1
 Summary: FractalDNA is a Python package built to generate DNA geometries for simulations
 Home-page: https://github.com/natl/fractaldna
 License: MIT
 Keywords: dna,geant4,simulation,modelling
 Author: Nathanael Lampe
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -15,24 +15,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: mayavi
+Requires-Dist: PyQt5 (>=5.15.9,<6.0.0); extra == "mayavi"
 Requires-Dist: importlib-metadata (>=4.8.2,<5.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
-Requires-Dist: mistune (==0.8.4)
+Requires-Dist: mayavi (>=4.8.1,<5.0.0); extra == "mayavi"
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
-Requires-Dist: pytest (>=6.2.5,<8.0.0)
 Requires-Dist: rich (>=10.7,<13.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: typer[all] (>=0.3.2,<0.5.0)
+Requires-Dist: vtk (>=9.2.6,<10.0.0); extra == "mayavi"
 Project-URL: Documentation, https://natl.github.io/fractaldna
 Project-URL: Repository, https://github.com/natl/fractaldna
 Description-Content-Type: text/markdown
 
 FractalDNA
 ===
 Python routines for generating geometric models of DNA
```

