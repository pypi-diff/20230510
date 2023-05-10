# Comparing `tmp/pyscemu-0.2.3.tar.gz` & `tmp/pyscemu-0.2.4.tar.gz`

## Comparing `pyscemu-0.2.3.tar` & `pyscemu-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.3/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.3/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.3/.gitignore
--rw-r--r--   0     1000     1000    11685 2023-05-09 16:57:39.000000 pyscemu-0.2.3/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.3/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.3/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.3/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.3/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.3/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.3/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.3/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.3/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.3/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.3/pyproject.toml
--rw-r--r--   0     1000     1000    26649 2023-05-10 08:41:01.000000 pyscemu-0.2.3/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-05-10 08:39:59.000000 pyscemu-0.2.3/Cargo.lock
--rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.4/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.4/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.4/.gitignore
+-rw-r--r--   0     1000     1000    11699 2023-05-10 08:42:26.000000 pyscemu-0.2.4/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.4/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.4/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.4/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.4/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.4/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.4/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.4/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.4/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.4/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.4/pyproject.toml
+-rw-r--r--   0     1000     1000    26649 2023-05-10 08:41:01.000000 pyscemu-0.2.4/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-05-10 09:58:03.000000 pyscemu-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.4/PKG-INFO
```

### Comparing `pyscemu-0.2.3/.github/workflows/CI.yml` & `pyscemu-0.2.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/.gitignore` & `pyscemu-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/DOCUMENTATION.md` & `pyscemu-0.2.4/DOCUMENTATION.md`

 * *Files 0% similar despite different names*

```diff
@@ -392,22 +392,22 @@
     # spawn an interactive console.  
 spawn_console()
 
     # disassemble an address.  
 disassemble(addr:int, amount:int)
 
     # start emulating the binary after finding the first return.
-run_until_return()
+run_until_return() -> int
 
     # emulate a single step, this is slower than run(address) or run(0)
 step() -> bool
 
     # start emulating the binary until reach the provided end_addr. 
     # Use run() with no params for emulating forever.
-run(end_addr:int)
+run(end_addr:int) -> int
 
     # read the number of instructions emulated since now.
 get_position() -> int
 
     # call a 32bits function, internally pushes params in reverse order.
 call32(addr:int, params:list) -> int
```

### Comparing `pyscemu-0.2.3/README.md` & `pyscemu-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/examples/danabot_rsa.ipynb` & `pyscemu-0.2.4/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/examples/raccoon_strings.ipynb` & `pyscemu-0.2.4/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/examples/scripts/raccoon_strings.py` & `pyscemu-0.2.4/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/examples/scripts/test.py` & `pyscemu-0.2.4/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/examples/scripts/xloader_dexor.py` & `pyscemu-0.2.4/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/examples/xloader_keygen.ipynb` & `pyscemu-0.2.4/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/src/lib.rs` & `pyscemu-0.2.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.3/Cargo.lock` & `pyscemu-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "becae19b8be11f72b845545277b5c1be85fbb8516faab9da9edaa9642b7425e8"
+checksum = "2c42270cab539e9dea748d3258513c7813a2a1b00a1f0ef5701f7c9c9ab018f9"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.2.3/PKG-INFO` & `pyscemu-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

