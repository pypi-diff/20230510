# Comparing `tmp/parquet2lance-0.0.6.tar.gz` & `tmp/parquet2lance-0.1.0.tar.gz`

## Comparing `parquet2lance-0.0.6.tar` & `parquet2lance-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/Cargo.toml
--rw-r--r--   0      503       20    90730 2023-05-07 09:03:26.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/Cargo.lock
--rw-r--r--   0      503       20     1064 2023-05-06 09:51:06.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/LICENSE
--rw-r--r--   0      503       20      856 2023-05-06 10:53:28.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/README.md
--rw-r--r--   0      503       20     1513 2023-05-05 09:28:08.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/fs.rs
--rw-r--r--   0      503       20     3391 2023-05-05 09:33:32.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/gcs.rs
--rw-r--r--   0      503       20     1060 2023-05-05 10:03:50.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/reader.rs
--rw-r--r--   0      503       20     3908 2023-05-06 06:36:50.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/util.rs
--rw-r--r--   0      503       20     1081 2023-05-07 08:53:08.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io.rs
--rw-r--r--   0      503       20       44 2023-05-06 08:43:19.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/lib.rs
--rw-r--r--   0      503       20      698 2023-05-07 08:51:22.000000 parquet2lance-0.0.6/local_dependencies/parquet2lance/src/main.rs
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 parquet2lance-0.0.6/Cargo.toml
--rw-r--r--   0      503       20     1064 2023-05-06 09:51:20.000000 parquet2lance-0.0.6/LICENSE
--rw-r--r--   0      503       20       69 2023-05-06 10:22:32.000000 parquet2lance-0.0.6/README.md
--rw-r--r--   0      503       20      617 2023-05-07 15:05:09.000000 parquet2lance-0.0.6/pyproject.toml
--rw-r--r--   0      503       20      562 2023-05-06 10:15:09.000000 parquet2lance-0.0.6/src/lib.rs
--rw-r--r--   0      503       20    97302 2023-05-08 06:47:57.000000 parquet2lance-0.0.6/Cargo.lock
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 parquet2lance-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/Cargo.toml
+-rw-r--r--   0      503       20    90730 2023-05-10 07:42:14.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/Cargo.lock
+-rw-r--r--   0      503       20     1064 2023-05-06 09:51:06.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/LICENSE
+-rw-r--r--   0      503       20      856 2023-05-06 10:53:28.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/README.md
+-rw-r--r--   0      503       20     1513 2023-05-05 09:28:08.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/fs.rs
+-rw-r--r--   0      503       20     3391 2023-05-05 09:33:32.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/gcs.rs
+-rw-r--r--   0      503       20     1060 2023-05-05 10:03:50.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/reader.rs
+-rw-r--r--   0      503       20     3908 2023-05-06 06:36:50.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/util.rs
+-rw-r--r--   0      503       20     1081 2023-05-07 08:53:08.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io.rs
+-rw-r--r--   0      503       20       44 2023-05-06 08:43:19.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/lib.rs
+-rw-r--r--   0      503       20      698 2023-05-07 08:51:22.000000 parquet2lance-0.1.0/local_dependencies/parquet2lance/src/main.rs
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 parquet2lance-0.1.0/Cargo.toml
+-rw-r--r--   0      503       20     1064 2023-05-06 09:51:20.000000 parquet2lance-0.1.0/LICENSE
+-rw-r--r--   0      503       20       69 2023-05-06 10:22:32.000000 parquet2lance-0.1.0/README.md
+-rw-r--r--   0      503       20      617 2023-05-07 15:05:09.000000 parquet2lance-0.1.0/pyproject.toml
+-rw-r--r--   0      503       20      562 2023-05-06 10:15:09.000000 parquet2lance-0.1.0/src/lib.rs
+-rw-r--r--   0      503       20    97302 2023-05-10 07:50:35.000000 parquet2lance-0.1.0/Cargo.lock
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 parquet2lance-0.1.0/PKG-INFO
```

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/Cargo.toml` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "parquet2lance"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 description = "Convert parquet files to lance"
 repository = "https://github.com/haoxins/parquet2lance"
 license-file = "LICENSE"
 keywords = ["parquet", "lance", "object_store", "gcs"]
 
 [dependencies]
 arrow = { version = "37.0", features = ["prettyprint"] }
 arrow-array = "37.0"
 clap = { version = "4", features = ["derive"] }
 futures = "0.3"
-lance = "0.4.6"
+lance = "0.4.8"
 object_store = { version = "0.5", features = ["aws", "gcp"] }
 parquet = "37"
 rayon = "1"
 tokio = { version = "1", features = ["full"] }
```

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/Cargo.lock` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1737,17 +1737,17 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lance"
-version = "0.4.6"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0be48532dda07b0cd5a5b087710bbbba6972a882f7c771a316940a4868d66a6"
+checksum = "817ed800f59541840d871ebc6674c93d43b35b4623f9bc9a7891dc6ba41c598b"
 dependencies = [
  "accelerate-src",
  "arrow",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
@@ -2288,15 +2288,15 @@
  "tokio",
  "twox-hash",
  "zstd",
 ]
 
 [[package]]
 name = "parquet2lance"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "arrow",
  "arrow-array",
  "clap",
  "futures",
  "lance",
  "object_store",
```

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/LICENSE` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/LICENSE`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/README.md` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/README.md`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/fs.rs` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/fs.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/gcs.rs` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/gcs.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/reader.rs` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/reader.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io/util.rs` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io/util.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/src/io.rs` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/src/io.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/local_dependencies/parquet2lance/src/main.rs` & `parquet2lance-0.1.0/local_dependencies/parquet2lance/src/main.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/LICENSE` & `parquet2lance-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/pyproject.toml` & `parquet2lance-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/src/lib.rs` & `parquet2lance-0.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.6/Cargo.lock` & `parquet2lance-0.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1799,17 +1799,17 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lance"
-version = "0.4.6"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0be48532dda07b0cd5a5b087710bbbba6972a882f7c771a316940a4868d66a6"
+checksum = "817ed800f59541840d871ebc6674c93d43b35b4623f9bc9a7891dc6ba41c598b"
 dependencies = [
  "accelerate-src",
  "arrow",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
@@ -2299,15 +2299,15 @@
 name = "outref"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4030760ffd992bef45b0ae3f10ce1aba99e33464c90d14dd7c039884963ddc7a"
 
 [[package]]
 name = "p2l"
-version = "0.0.6"
+version = "0.1.0"
 dependencies = [
  "parquet2lance",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
@@ -2364,15 +2364,15 @@
  "tokio",
  "twox-hash",
  "zstd",
 ]
 
 [[package]]
 name = "parquet2lance"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "arrow",
  "arrow-array",
  "clap",
  "futures",
  "lance",
  "object_store",
```

### Comparing `parquet2lance-0.0.6/PKG-INFO` & `parquet2lance-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parquet2lance
-Version: 0.0.6
+Version: 0.1.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Summary: The Python wrapper for the Rust parquet2lance
 Keywords: arrow,lance,parquet
 Author-email: Hao Xin <haoxinst@gmail.com>
```

