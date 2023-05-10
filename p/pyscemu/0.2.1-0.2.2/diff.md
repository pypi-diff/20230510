# Comparing `tmp/pyscemu-0.2.1.tar.gz` & `tmp/pyscemu-0.2.2.tar.gz`

## Comparing `pyscemu-0.2.1.tar` & `pyscemu-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.1/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.1/.gitignore
--rw-r--r--   0     1000     1000    11671 2023-05-01 10:48:40.000000 pyscemu-0.2.1/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10073 2023-05-01 10:57:14.000000 pyscemu-0.2.1/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.1/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.1/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.1/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.1/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.2.1/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.1/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-01 14:50:10.000000 pyscemu-0.2.1/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.1/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.1/pyproject.toml
--rw-r--r--   0     1000     1000    26702 2023-05-04 11:13:39.000000 pyscemu-0.2.1/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-05-04 11:32:11.000000 pyscemu-0.2.1/Cargo.lock
--rw-r--r--   0        0        0    10399 1970-01-01 00:00:00.000000 pyscemu-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.2/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.2/.gitignore
+-rw-r--r--   0     1000     1000    11685 2023-05-09 16:57:39.000000 pyscemu-0.2.2/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.2/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.2/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.2/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.2/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.2/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.2/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.2/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-01 14:50:10.000000 pyscemu-0.2.2/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.2/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.2/pyproject.toml
+-rw-r--r--   0     1000     1000    26736 2023-05-09 17:00:04.000000 pyscemu-0.2.2/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-05-09 17:10:49.000000 pyscemu-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.2/PKG-INFO
```

### Comparing `pyscemu-0.2.1/.github/workflows/CI.yml` & `pyscemu-0.2.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/.gitignore` & `pyscemu-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/DOCUMENTATION.md` & `pyscemu-0.2.2/DOCUMENTATION.md`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,15 @@
     # start emulating the binary after finding the first return.
 run_until_return()
 
     # emulate a single step, this is slower than run(address) or run(0)
 step() -> bool
 
     # start emulating the binary until reach the provided end_addr. 
-    # Use run(0) for emulating forever.
+    # Use run() with no params for emulating forever.
 run(end_addr:int)
 
     # read the number of instructions emulated since now.
 get_position() -> int
 
     # call a 32bits function, internally pushes params in reverse order.
 call32(addr:int, params:list) -> int
```

### Comparing `pyscemu-0.2.1/README.md` & `pyscemu-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 /!\ warning: raw sz:8704 off:8192 sz:512  off+sz:8704
 	created pe32 map for section `.reloc` at 0x776c5000 size: 88
 >>> 
 >>> emu.load_binary('/home/sha0/src/scemu/shellcodes32/shikata.bin')
 shellcode detected.
 >>> emu.set_verbose(0)   # by default already 0
 >>> emu.disable_console() # by default already disabled
->>> emu.run(0)   # 
+>>> emu.run()   # 
  ----- emulation -----
 ** 333368 kernel32!LoadLibraryA  'ws2_32' =0x77480000 
 ** 1618021 ws2_32!WsaStartup 
 ** 2902832 ws2_32!WsaSocketA 
 ** 4180546 ws2_32!connect  family: 2 192.168.1.38:1337 
 ** 5456468 ws2_32!recv   buff: 0x22de64 sz: 4 
 ** 5736281 kernel32!VirtualAlloc sz: 256 addr: 0x164 
@@ -70,15 +70,15 @@
 redirecting code flow to non maped address 0x264
 
 >>> help(emu.run)
 Help on built-in function run:
 
 run(end_addr) method of builtins.Emu instance
     start emulating the binary until reach the provided end_addr. 
-    Use run(0) for emulating forever.
+    Use run() with no param for emulating forever.
 ```
 
 
 ### Loading Danabot PE
 
 ```python
 >>> emu.load_binary('/home/sha0/samples/danabot/2023-04-03-MainModule/unpacked2/dbmm_unpacked.dll')
@@ -222,15 +222,15 @@
 >>> xloader_key1_keygen = 0x03DB687
 >>> old_eip = emu.set_reg('eip', xloader_key1_keygen)
 >>> ret_addr = old_eip
 >>> emu.stack_push32(struct_ptr)
 True
 >>> emu.stack_push32(ret_addr)
 True
->>> emu.run(ret_adr)  # point ret_addr to some mapped place and run until ret_address
+>>> emu.run(ret_addr)  # point ret_addr to some mapped place and run until ret_addr
 ```
 
 
 ### Spawn console by address or by position.
 
 ```python
 >>> emu.spawn_console_at_pos(6)
```

### Comparing `pyscemu-0.2.1/examples/danabot_rsa.ipynb` & `pyscemu-0.2.2/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/examples/raccoon_strings.ipynb` & `pyscemu-0.2.2/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/examples/scripts/raccoon_strings.py` & `pyscemu-0.2.2/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/examples/scripts/test.py` & `pyscemu-0.2.2/examples/scripts/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 emu.load_binary('/home/sha0/samples/danabot/2023-04-03-MainModule/unpacked2/dbmm_unpacked.dll')
 emu.set_verbose(3)
 emu.set_base_address(0x1E70000)
 emu.enable_banzai_mode()
 danabot_init = 0x022EBBC0 
 
 
-emu.disable_ctrlc()
+emu.enable_ctrlc()
 
 
 '''
 public_key_ptr = emu.alloc("pubkey", 1024)
 private_key_ptr = emu.alloc("privkey", 1024)
 pub_ptr = emu.alloc("pub_ptr", 4)
 priv_ptr = emu.alloc("priv_ptr", 4)
@@ -26,8 +26,10 @@
 emu.set_reg('eax', pub_ptr)
 emu.set_reg('edx', priv_ptr)
 '''
 
 emu.set_reg('eax', 1)
 emu.set_reg('esi', 1)
 ret_addr = emu.set_reg('eip', danabot_init)
-emu.run(ret_addr)
+
+#emu.run(ret_addr)
+emu.run()
```

### Comparing `pyscemu-0.2.1/examples/scripts/xloader_dexor.py` & `pyscemu-0.2.2/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/examples/xloader_keygen.ipynb` & `pyscemu-0.2.2/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.1/src/lib.rs` & `pyscemu-0.2.2/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -322,16 +322,16 @@
 
     /// emulate a single step, this is slower than run(address) or run(0)
     fn step(&mut self) -> PyResult<bool> {
         return Ok(self.emu.step());
     }
 
     /// Start emulating the binary until reach the provided end_addr. 
-    /// Use run(0) for emulating forever. or call32/call64 for calling a function.
-    fn run(&mut self, end_addr:u64) {
+    /// Use run() with no params for emulating forever. or call32/call64 for calling a function.
+    fn run(&mut self, end_addr:Option<u64>) {
         self.emu.run(end_addr);
     }
 
     /// read the number of instructions emulated since now.
     fn get_position(&mut self) -> PyResult<u64> {
         return Ok(self.emu.pos);
     }
@@ -341,27 +341,27 @@
         for i in (0..params.len()).rev() {
             self.emu.stack_push32(params[i]);
         }
         let ret_addr = self.emu.regs.get_eip();
         self.emu.stack_push32(ret_addr as u32);
         self.emu.regs.set_eip(address);
         //self.emu.set_eip(address, false);
-        self.emu.run(ret_addr);
+        self.emu.run(Some(ret_addr));
         return Ok(self.emu.regs.get_eax() as u32);
     }
 
     /// call a 64bits function, internally pushes params in reverse order.
     fn call64(&mut self, address:u64, params:Vec<u64>) -> PyResult<u64> {
         for i in (0..params.len()).rev() {
             self.emu.stack_push64(params[i]);
         }
         let ret_addr = self.emu.regs.rip;
         //self.emu.stack_push64(ret_addr);
         self.emu.set_eip(address, false);
-        self.emu.run(ret_addr);
+        self.emu.run(Some(ret_addr));
         return Ok(self.emu.regs.rax);
     }
 
     // registers
 
     /// read register value ie get_reg('rax')
     fn get_reg(&mut self, reg:&str) -> PyResult<u64> {
```

### Comparing `pyscemu-0.2.1/Cargo.lock` & `pyscemu-0.2.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1374234949ee4079edb4e61b312240ff61cee10919dfe9ffa611a8344797a98f"
+checksum = "f6467ad218e07547e5c3aa9464de0a0c0ef2c82dba6a1ce42b36c11978591f9b"
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
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.2.1/PKG-INFO` & `pyscemu-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
@@ -63,15 +63,15 @@
 /!\ warning: raw sz:8704 off:8192 sz:512  off+sz:8704
 	created pe32 map for section `.reloc` at 0x776c5000 size: 88
 >>> 
 >>> emu.load_binary('/home/sha0/src/scemu/shellcodes32/shikata.bin')
 shellcode detected.
 >>> emu.set_verbose(0)   # by default already 0
 >>> emu.disable_console() # by default already disabled
->>> emu.run(0)   # 
+>>> emu.run()   # 
  ----- emulation -----
 ** 333368 kernel32!LoadLibraryA  'ws2_32' =0x77480000 
 ** 1618021 ws2_32!WsaStartup 
 ** 2902832 ws2_32!WsaSocketA 
 ** 4180546 ws2_32!connect  family: 2 192.168.1.38:1337 
 ** 5456468 ws2_32!recv   buff: 0x22de64 sz: 4 
 ** 5736281 kernel32!VirtualAlloc sz: 256 addr: 0x164 
@@ -79,15 +79,15 @@
 redirecting code flow to non maped address 0x264
 
 >>> help(emu.run)
 Help on built-in function run:
 
 run(end_addr) method of builtins.Emu instance
     start emulating the binary until reach the provided end_addr. 
-    Use run(0) for emulating forever.
+    Use run() with no param for emulating forever.
 ```
 
 
 ### Loading Danabot PE
 
 ```python
 >>> emu.load_binary('/home/sha0/samples/danabot/2023-04-03-MainModule/unpacked2/dbmm_unpacked.dll')
@@ -231,15 +231,15 @@
 >>> xloader_key1_keygen = 0x03DB687
 >>> old_eip = emu.set_reg('eip', xloader_key1_keygen)
 >>> ret_addr = old_eip
 >>> emu.stack_push32(struct_ptr)
 True
 >>> emu.stack_push32(ret_addr)
 True
->>> emu.run(ret_adr)  # point ret_addr to some mapped place and run until ret_address
+>>> emu.run(ret_addr)  # point ret_addr to some mapped place and run until ret_addr
 ```
 
 
 ### Spawn console by address or by position.
 
 ```python
 >>> emu.spawn_console_at_pos(6)
```

