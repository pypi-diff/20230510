# Comparing `tmp/FlyHash-0.2.0.tar.gz` & `tmp/FlyHash-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyHash-0.2.0.tar", last modified: Tue May  9 13:39:12 2023, max compression
+gzip compressed data, was "FlyHash-0.3.0.tar", last modified: Wed May 10 05:50:24 2023, max compression
```

## Comparing `FlyHash-0.2.0.tar` & `FlyHash-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.666074 FlyHash-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.666074 FlyHash-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 13:38:05.000000 FlyHash-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 13:38:05.000000 FlyHash-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-09 13:38:05.000000 FlyHash-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 13:38:05.000000 FlyHash-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 13:39:12.670074 FlyHash-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-09 13:38:05.000000 FlyHash-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 13:38:05.000000 FlyHash-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 13:39:12.670074 FlyHash-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-09 13:38:05.000000 FlyHash-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.666074 FlyHash-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/src/FlyHash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/src/flyhash/
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-09 13:38:05.000000 FlyHash-0.2.0/src/flyhash/FlyHash.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-09 13:38:05.000000 FlyHash-0.2.0/src/flyhash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 13:38:05.000000 FlyHash-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-09 13:38:05.000000 FlyHash-0.2.0/tests/test_FlyHash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-09 13:38:05.000000 FlyHash-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.cz.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.077652 FlyHash-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.077652 FlyHash-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 05:49:39.000000 FlyHash-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 05:49:39.000000 FlyHash-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-10 05:49:39.000000 FlyHash-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-10 05:49:39.000000 FlyHash-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 05:50:24.081652 FlyHash-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 05:49:39.000000 FlyHash-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-10 05:49:39.000000 FlyHash-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 05:49:39.000000 FlyHash-0.3.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 05:50:24.081652 FlyHash-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 05:49:39.000000 FlyHash-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.077652 FlyHash-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/src/FlyHash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:50:23.000000 FlyHash-0.3.0/src/FlyHash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/src/flyhash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-05-10 05:49:39.000000 FlyHash-0.3.0/src/flyhash/FlyHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 05:49:39.000000 FlyHash-0.3.0/src/flyhash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 05:49:39.000000 FlyHash-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-10 05:49:39.000000 FlyHash-0.3.0/tests/test_FlyHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-10 05:49:39.000000 FlyHash-0.3.0/tox.ini
```

### Comparing `FlyHash-0.2.0/.coveragerc` & `FlyHash-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/.github/workflows/ci.yml` & `FlyHash-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/.gitignore` & `FlyHash-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/.pre-commit-config.yaml` & `FlyHash-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/.readthedocs.yml` & `FlyHash-0.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/CONTRIBUTING.md` & `FlyHash-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/LICENSE.txt` & `FlyHash-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/PKG-INFO` & `FlyHash-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyHash
-Version: 0.2.0
+Version: 0.3.0
 Summary: A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
 Home-page: https://github.com/TeddyHuang-00/FlyHash
 Author: TeddyHuang-00
 Author-email: teddyhuangnan@gmail.com
 License: MIT
 Project-URL: Documentation, https://flyhash.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/TeddyHuang-00/FlyHash/
```

### Comparing `FlyHash-0.2.0/README.md` & `FlyHash-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/docs/Makefile` & `FlyHash-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/docs/conf.py` & `FlyHash-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/setup.cfg` & `FlyHash-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/setup.py` & `FlyHash-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/src/FlyHash.egg-info/PKG-INFO` & `FlyHash-0.3.0/src/FlyHash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyHash
-Version: 0.2.0
+Version: 0.3.0
 Summary: A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
 Home-page: https://github.com/TeddyHuang-00/FlyHash
 Author: TeddyHuang-00
 Author-email: teddyhuangnan@gmail.com
 License: MIT
 Project-URL: Documentation, https://flyhash.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/TeddyHuang-00/FlyHash/
```

### Comparing `FlyHash-0.2.0/src/FlyHash.egg-info/SOURCES.txt` & `FlyHash-0.3.0/src/FlyHash.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 .coveragerc
+.cz.json
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE.txt
 README.md
 pyproject.toml
+renovate.json
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
```

### Comparing `FlyHash-0.2.0/src/flyhash/FlyHash.py` & `FlyHash-0.3.0/src/flyhash/FlyHash.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,7 +205,26 @@
         else:
             # Quantize to steps as specified by quant_step.
             # Clipped by the range of dtype.
             result[indices] = np.ceil(input_vector[indices] / self.quant_step).clip(
                 0, np.iinfo(self.dtype).max
             )
         return result
+
+    def __repr__(self):
+        return (
+            f"HashEmbedding(input_dim={self.input_dim}, hash_dim={self.hash_dim}, "
+            f"density={self.density}, sparsity={self.sparsity}, "
+            f"quant_step={self.quant_step}, dtype={self.dtype}, seed={self.seed})"
+        )
+
+    def reset(self, seed: Optional[int] = None):
+        """Reset the random seed if provided and re-construct the projection matrix.
+
+        Parameters
+        ----------
+        seed : Optional[int], optional
+            The new seed to be used, omitted when set to `None`, by default `None`.
+        """
+        if seed is not None:
+            self.rng = np.random.default_rng(seed)
+        self._construct_projection_matrix()
```

### Comparing `FlyHash-0.2.0/src/flyhash/__init__.py` & `FlyHash-0.3.0/src/flyhash/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.2.0/tests/test_FlyHash.py` & `FlyHash-0.3.0/tests/test_FlyHash.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 __author__ = "TeddyHuang-00"
 __copyright__ = "TeddyHuang-00"
 __license__ = "MIT"
 
 
 def test_flyhash():
+    np.random.seed(1234)
+
     normal_input_dim = 10
     normal_hash_dim = 100
     normal_int_density = 6
     normal_float_density = 0.05
     normal_sparsity = 0.1
     normal_quant_step = 0.1
     normal_dtype = np.int16
@@ -131,14 +133,18 @@
     assert random_matrix.dtype == normal_dtype
 
     # Test random seed
     hasher_1 = FlyHash(normal_input_dim, normal_hash_dim, seed=normal_seed)
     hasher_2 = FlyHash(normal_input_dim, normal_hash_dim, seed=normal_seed)
     assert np.all(hasher_1(normal_matrix_data) == hasher_2(normal_matrix_data))
     assert np.all(hasher_1.projection_matrix == hasher_2.projection_matrix)
+    hasher_2.reset()
+    assert not np.all(hasher_1.projection_matrix == hasher_2.projection_matrix)
+    hasher_2.reset(normal_seed + 1)
+    assert not np.all(hasher_1.projection_matrix == hasher_2.projection_matrix)
 
     # Test clipping
     binary_clip_hasher = FlyHash(
         normal_input_dim,
         normal_hash_dim,
         sparsity=normal_sparsity,
         quant_step=None,
```

### Comparing `FlyHash-0.2.0/tox.ini` & `FlyHash-0.3.0/tox.ini`

 * *Files identical despite different names*

