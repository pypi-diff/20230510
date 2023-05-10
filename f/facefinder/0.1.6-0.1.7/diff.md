# Comparing `tmp/facefinder-0.1.6.tar.gz` & `tmp/facefinder-0.1.7.tar.gz`

## Comparing `facefinder-0.1.6.tar` & `facefinder-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.6/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.6/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.6/.gitignore
--rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.6/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-02 06:23:15.000000 facefinder-0.1.6/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.6/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    23934 2023-05-10 01:58:46.000000 facefinder-0.1.6/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.6/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.6/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-05-10 02:00:03.000000 facefinder-0.1.6/Cargo.lock
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.7/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.7/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.7/.gitignore
+-rw-r--r--   0        0        0      547 2023-05-10 14:39:00.000000 facefinder-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.7/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-10 14:38:00.000000 facefinder-0.1.7/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     4565 2023-05-10 04:29:33.000000 facefinder-0.1.7/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    28631 2023-05-10 10:42:06.000000 facefinder-0.1.7/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.7/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.7/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-05-10 14:40:07.000000 facefinder-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 facefinder-0.1.7/PKG-INFO
```

### Comparing `facefinder-0.1.6/.github/workflows/CI.yml` & `facefinder-0.1.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.6/.gitignore` & `facefinder-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.6/pyproject.toml` & `facefinder-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "facefinder"
-requires-python = ">=3.7"
+requires-python = ">=3.7,<3.11"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
```

### Comparing `facefinder-0.1.6/src/python/facefinder/interact.py` & `facefinder-0.1.7/src/python/facefinder/interact.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.6/src/python/facefinder/metadata.py` & `facefinder-0.1.7/src/python/facefinder/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,26 @@
     "DeepFace": (152, 152),
     "ArcFace": (112, 112),
     "SFace": (112, 112),
 }
 
 DEFAULT_EMBEDDING_COHERENCE_WEIGHT = 1
 
+THRESHOLDS = {
+    "VGG-Face": {"cosine": 0.40, "euclidean": 0.60, "euclidean_l2": 0.86},
+    "Facenet": {"cosine": 0.40, "euclidean": 10, "euclidean_l2": 0.80},
+    "Facenet512": {"cosine": 0.30, "euclidean": 23.56, "euclidean_l2": 1.04},
+    "ArcFace": {"cosine": 0.68, "euclidean": 4.15, "euclidean_l2": 1.13},
+    "Dlib": {"cosine": 0.07, "euclidean": 0.6, "euclidean_l2": 0.4},
+    "SFace": {"cosine": 0.593, "euclidean": 10.734, "euclidean_l2": 1.055},
+    "OpenFace": {"cosine": 0.10, "euclidean": 0.55, "euclidean_l2": 0.55},
+    "DeepFace": {"cosine": 0.23, "euclidean": 64, "euclidean_l2": 0.64},
+    "DeepID": {"cosine": 0.015, "euclidean": 45, "euclidean_l2": 0.17},
+}
+
 
 class _Singleton(type):
     __instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls.__instances:
             cls.__instances[cls] = super(_Singleton, cls).__call__(*args, **kwargs)
```

### Comparing `facefinder-0.1.6/src/python/facefinder/prompting.py` & `facefinder-0.1.7/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.6/Cargo.lock` & `facefinder-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

