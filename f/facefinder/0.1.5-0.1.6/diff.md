# Comparing `tmp/facefinder-0.1.5.tar.gz` & `tmp/facefinder-0.1.6.tar.gz`

## Comparing `facefinder-0.1.5.tar` & `facefinder-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.5/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.5/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.5/.gitignore
--rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.5/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-02 06:23:15.000000 facefinder-0.1.5/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.5/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    22918 2023-05-08 10:50:24.000000 facefinder-0.1.5/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.5/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.5/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-05-08 10:52:24.000000 facefinder-0.1.5/Cargo.lock
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.6/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.6/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.6/.gitignore
+-rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.6/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-02 06:23:15.000000 facefinder-0.1.6/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.6/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    23934 2023-05-10 01:58:46.000000 facefinder-0.1.6/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.6/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.6/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-05-10 02:00:03.000000 facefinder-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.6/PKG-INFO
```

### Comparing `facefinder-0.1.5/.github/workflows/CI.yml` & `facefinder-0.1.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.5/.gitignore` & `facefinder-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.5/pyproject.toml` & `facefinder-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.5/src/python/facefinder/interact.py` & `facefinder-0.1.6/src/python/facefinder/interact.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.5/src/python/facefinder/metadata.py` & `facefinder-0.1.6/src/python/facefinder/metadata.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.5/src/python/facefinder/metrics.py` & `facefinder-0.1.6/src/python/facefinder/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,14 +138,29 @@
 
     a = np.matmul(target_reprs, source_reprs.T)
     b = np.sqrt(np.sum(target_reprs**2, axis=1))
     c = np.sqrt(np.sum(source_reprs**2, axis=1))
     return np.ones(a.shape) - (a / np.matmul(b[:, None], c[None, :]))
 
 
+def euclid_dist(
+    source_reprs: np.ndarray,
+    target_reprs: np.ndarray,
+) -> np.ndarray:
+    # Dims 1 must match (length of representation vector)
+    target_reprs = np.array(target_reprs)[:, None, :]
+    source_reprs = np.array(source_reprs)[None, :, :]
+    assert source_reprs.shape[2] == target_reprs.shape[2]
+
+    target_reprs = target_reprs.repeat(source_reprs.shape[1], axis=1)
+    source_reprs = source_reprs.repeat(target_reprs.shape[0], axis=0)
+
+    return ((source_reprs - target_reprs) ** 2).sum(axis=2) ** 0.5
+
+
 def filter_duplicates(paths: list[Path], distances: list[float]) -> list[int]:
     """Returns a numpy index that will filter out the duplicates with non-max scores"""
     visited = defaultdict(list)
     for i, path in enumerate(paths):
         visited[path].append(i)
     duplicates = {k: v for k, v in visited.items() if len(v) > 1}
     visited = {k: v[0] for k, v in visited.items()}
@@ -158,15 +173,15 @@
 
 def get_filtered(
     target_repr: list[float],
     candidate_reprs: list[list[float]],
     candidate_paths: list[Path],
 ) -> tuple[list[Path], list[list[float]], list[float]]:
     # Finding metrics for distance from target image (BASE_FACE)
-    target_distances = cosine_dist(target_repr, candidate_reprs)
+    target_distances = euclid_dist(target_repr, candidate_reprs)
 
     # Filtering embedding duplicates by distance to target
     non_duplicate_idx = filter_duplicates(candidate_paths, target_distances)
     candidate_paths = np.array(candidate_paths)[non_duplicate_idx]
     candidate_reprs = np.array(candidate_reprs)[non_duplicate_idx]
     target_distances = np.array(target_distances)[non_duplicate_idx]
 
@@ -226,15 +241,15 @@
         target_representation, representations, paths
     )
 
     mean_target_distance = float(np.mean(embedding_target_distances))
 
     # Finding overall similarity between faces in the embedding train set
     embedding_embedding_distances = np.mean(
-        cosine_dist(representations, representations), axis=1
+        euclid_dist(representations, representations), axis=1
     )
     mean_embedding_distance = float(np.mean(embedding_embedding_distances))
 
     return {
         "target_path": target_path,
         "target_representation": target_representation,
         "representations": representations,
@@ -262,28 +277,28 @@
 
     # Filtering processed images by distance to target
     paths, representations, candidate_target_distances = get_filtered(
         target_repr, representations, paths
     )
 
     # Distances between candidates and embeddings
-    candidate_embedding_pair_distances = cosine_dist(embedding_reprs, representations)
+    candidate_embedding_pair_distances = euclid_dist(embedding_reprs, representations)
     candidate_embedding_distances = candidate_embedding_pair_distances.mean(axis=1)
 
     # Weighting the candidate distances by the embedding image scores (relative to the target)
     candidate_weighted_distances = calculate_weighted_distances(
         embedding_target_distances,
         candidate_embedding_pair_distances,
         target_distance_bias,
     )
 
     # Doing the same for embedding images
     embedding_weighted_distances = calculate_weighted_distances(
         embedding_target_distances,
-        cosine_dist(embedding_reprs, embedding_reprs),
+        euclid_dist(embedding_reprs, embedding_reprs),
         target_distance_bias,
     )
 
     return {
         "paths": paths,
         "representations": representations,
         "candidate_target_distances": candidate_target_distances,
@@ -456,14 +471,27 @@
     for distance in distances.values():
         total_distance += np.sum(distance)
         total_size += distance.size
 
     return total_distance / total_size
 
 
+def normalize(distances: np.ndarray) -> np.ndarray:
+    """Returns a set of z scores that have been right-shifted to min=0, mean=1"""
+    mean = distances.mean()
+    std = np.std(distances)
+    zscores = (distances - mean) / std
+
+    # Normalizing to min=0, mean (originally 0 by definition) = 1
+    zmin = -zscores.min()
+    zscores = (zscores + zmin) / zmin
+
+    return zscores
+
+
 def merge_metrics(metrics: list[dict[str, Any]]) -> dict[str, Any]:
     if not metrics:
         raise ValueError(f"list of metrics must not be empty, {len(metrics)=}")
 
     paths = metrics[0]["paths"]
     representations = {m["metadata"]["model"]: m["representations"] for m in metrics}
     metadata = {
@@ -502,17 +530,20 @@
         "candidate_embedding": [],
         "pairs": [],
     }
 
     for k in distances:
         for m in metrics:
             distance = m["distances"][k]
+            distance = normalize(distance)
             if len(distance.shape) == 1:
                 distance = distance[:, None]
-            distances[k].append(distance[..., None])
+            distance = distance[:, None]
+
+            distances[k].append(distance)
         distances[k] = np.mean(np.concatenate(distances[k], axis=2), axis=2)
 
     candidate_weighted_distances = calculate_weighted_distances(
         distances["embedding_target"],
         distances["candidate_embedding"],
         np.mean(metadata["target_distance_bias"]),
     )
```

### Comparing `facefinder-0.1.5/src/python/facefinder/prompting.py` & `facefinder-0.1.6/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.5/Cargo.lock` & `facefinder-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

