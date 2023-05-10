# Comparing `tmp/getpack-0.2.5.tar.gz` & `tmp/getpack-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getpack-0.2.5.tar", last modified: Thu May  4 17:50:30 2023, max compression
+gzip compressed data, was "getpack-0.2.6.tar", last modified: Wed May 10 21:47:31 2023, max compression
```

## Comparing `getpack-0.2.5.tar` & `getpack-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.390493 getpack-0.2.5/
--rw-rw-rw-   0        0        0       37 2023-02-16 21:01:44.000000 getpack-0.2.5/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.317797 getpack-0.2.5/.vscode/
--rw-rw-rw-   0        0        0      186 2022-11-26 18:28:38.000000 getpack-0.2.5/.vscode/cspell.json
--rw-rw-rw-   0        0        0      534 2023-04-27 21:31:59.000000 getpack-0.2.5/.vscode/launch.json
--rw-rw-rw-   0        0        0      500 2022-11-26 18:28:38.000000 getpack-0.2.5/.vscode/settings.json
--rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     2504 2023-05-04 17:50:30.391494 getpack-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.5/README.md
--rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0      967 2023-05-04 17:50:30.402489 getpack-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.280795 getpack-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.339798 getpack-0.2.5/src/getpack/
--rw-rw-rw-   0        0        0      403 2023-05-04 08:53:10.000000 getpack-0.2.5/src/getpack/__init__.py
--rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.5/src/getpack/executable.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.379490 getpack-0.2.5/src/getpack/library/
--rw-rw-rw-   0        0        0     3024 2023-05-04 17:14:18.000000 getpack-0.2.5/src/getpack/library/__init__.py
--rw-rw-rw-   0        0        0    12129 2023-05-04 17:46:45.000000 getpack-0.2.5/src/getpack/resource.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.377487 getpack-0.2.5/src/getpack.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 17:50:30.000000 getpack-0.2.5/src/getpack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 17:50:30.389497 getpack-0.2.5/tests/
--rw-rw-rw-   0        0        0     1452 2023-05-04 17:20:38.000000 getpack-0.2.5/tests/test_common.py
--rw-rw-rw-   0        0        0     1071 2023-05-04 17:32:32.000000 getpack-0.2.5/tests/test_concurrency.py
--rw-rw-rw-   0        0        0      426 2023-03-31 19:43:17.000000 getpack-0.2.5/tests/test_executable.py
--rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.5/tests/test_unicode.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.777969 getpack-0.2.6/
+-rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     2222 2023-05-10 21:47:31.777969 getpack-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.6/README.md
+-rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1078 2023-05-10 21:47:31.790964 getpack-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.656966 getpack-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.694964 getpack-0.2.6/src/getpack/
+-rw-rw-rw-   0        0        0      403 2023-05-10 21:22:58.000000 getpack-0.2.6/src/getpack/__init__.py
+-rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.6/src/getpack/executable.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.763965 getpack-0.2.6/src/getpack/library/
+-rw-rw-rw-   0        0        0     3024 2023-05-04 17:14:18.000000 getpack-0.2.6/src/getpack/library/__init__.py
+-rw-rw-rw-   0        0        0    12295 2023-05-10 21:26:12.000000 getpack-0.2.6/src/getpack/resource.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.759968 getpack-0.2.6/src/getpack.egg-info/
+-rw-rw-rw-   0        0        0     2222 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.775966 getpack-0.2.6/tests/
+-rw-rw-rw-   0        0        0     1452 2023-05-10 20:32:48.000000 getpack-0.2.6/tests/test_common.py
+-rw-rw-rw-   0        0        0     1071 2023-05-10 21:29:25.000000 getpack-0.2.6/tests/test_concurrency.py
+-rw-rw-rw-   0        0        0      444 2023-05-10 21:41:05.000000 getpack-0.2.6/tests/test_executable.py
+-rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.6/tests/test_unicode.py
```

### Comparing `getpack-0.2.5/LICENSE` & `getpack-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getpack-0.2.5/PKG-INFO` & `getpack-0.2.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,37 @@
-Metadata-Version: 2.1
-Name: getpack
-Version: 0.2.5
-Summary: Declarative external resources with implicit deployment
-Home-page: https://github.com/kalemas/getpack
-Author: Konstantin Maslyuk
-Author-email: Kostya.Maslyuk@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
-Description: ### Declarative external resources any with implicit deployment
-        
-        This package provide classes that allow to setup external resources (utilities,
-        python packages etc.) that will be deployed as they are used. In most
-        cases data should be on the web and it will be deployed and cached locally on
-        only first usage.
-        
-        There are several examples in `test/` folder and `getpack.library` module
-        already defined and useable. But main intention is to provide framework for
-        declarative setup of any resource and work with it without care of deployment.
-        ```python
-        from getpack.resource import WebResource
-        class Example(WebResource):
-            version = '0.1'
-            archive_url = 'https://example.com/example-0.1.zip'
-        ```
-        then it would be used:
-        ```python
-        import subprocess
-        subprocess.call(Example()().path / 'example.exe')
-        ```
-        Second round braces required to actually make an effect from resource
-        and first round braces used to initialize resource class, that would produce
-        resource descriptions on the fly like follows:
-        ```python
-        Example(version='0.2', archive_url='https://Example.com/example-0.2.zip')
-        ```
-        You may experiment with following working snippet and try to change `PySide2`
-        version:
-        ```bash
-        python -c "import getpack.library;getpack.library.PySide2(version='5.14.1')(); import PySide2.QtWidgets; app=PySide2.QtWidgets.QApplication(); w=PySide2.QtWidgets.QPushButton(PySide2.__version__); w.clicked.connect(w.close); w.show(); app.exec_()"
-        ```
-        
-        ### TODO
-        
-        - Utilize `requirements.txt` to reproduce both development and production
-          environments.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+### Declarative external resources any with implicit deployment
+
+This package provide classes that allow to setup external resources (utilities,
+python packages etc.) that will be deployed as they are used. In most
+cases data should be on the web and it will be deployed and cached locally on
+only first usage.
+
+There are several examples in `test/` folder and `getpack.library` module
+already defined and useable. But main intention is to provide framework for
+declarative setup of any resource and work with it without care of deployment.
+```python
+from getpack.resource import WebResource
+class Example(WebResource):
+    version = '0.1'
+    archive_url = 'https://example.com/example-0.1.zip'
+```
+then it would be used:
+```python
+import subprocess
+subprocess.call(Example()().path / 'example.exe')
+```
+Second round braces required to actually make an effect from resource
+and first round braces used to initialize resource class, that would produce
+resource descriptions on the fly like follows:
+```python
+Example(version='0.2', archive_url='https://Example.com/example-0.2.zip')
+```
+You may experiment with following working snippet and try to change `PySide2`
+version:
+```bash
+python -c "import getpack.library;getpack.library.PySide2(version='5.14.1')(); import PySide2.QtWidgets; app=PySide2.QtWidgets.QApplication(); w=PySide2.QtWidgets.QPushButton(PySide2.__version__); w.clicked.connect(w.close); w.show(); app.exec_()"
+```
+
+### TODO
+
+- Utilize `requirements.txt` to reproduce both development and production
+  environments.
```

### Comparing `getpack-0.2.5/setup.cfg` & `getpack-0.2.6/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -37,25 +37,32 @@
 00000240: 646f 7773 203a 3a20 5769 6e64 6f77 7320  dows :: Windows 
 00000250: 3130 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  10....[options].
 00000260: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
 00000270: 0a09 3d73 7263 0d0a 7061 636b 6167 6573  ..=src..packages
 00000280: 203d 2066 696e 643a 0d0a 696e 7374 616c   = find:..instal
 00000290: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
 000002a0: 7061 7468 6c69 623b 2070 7974 686f 6e5f  pathlib; python_
-000002b0: 7665 7273 696f 6e3c 2233 220d 0a09 7369  version<"3"...si
-000002c0: 780d 0a09 7479 7069 6e67 3b20 7079 7468  x...typing; pyth
-000002d0: 6f6e 5f76 6572 7369 6f6e 3c22 3322 0d0a  on_version<"3"..
-000002e0: 0970 6f72 7461 6c6f 636b 6572 3c32 0d0a  .portalocker<2..
-000002f0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000300: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000310: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000320: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-00000330: 655d 0d0a 6465 7620 3d20 0d0a 0966 6c61  e]..dev = ...fla
-00000340: 6b65 380d 0a09 666c 616b 6538 2d69 6d70  ke8...flake8-imp
-00000350: 6f72 742d 6f72 6465 720d 0a09 6d79 7079  ort-order...mypy
-00000360: 0d0a 0970 7974 6573 740d 0a09 7961 7066  ...pytest...yapf
-00000370: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 696d  ....[flake8]..im
-00000380: 706f 7274 2d6f 7264 6572 2d73 7479 6c65  port-order-style
-00000390: 203d 2067 6f6f 676c 650d 0a0d 0a5b 6567   = google....[eg
-000003a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000003b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000003c0: 3d20 300d 0a0d 0a                        = 0....
+000002b0: 7665 7273 696f 6e20 3c20 2233 220d 0a09  version < "3"...
+000002c0: 7369 780d 0a09 7479 7069 6e67 3b20 7079  six...typing; py
+000002d0: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
+000002e0: 3322 0d0a 0966 6173 7465 6e65 7273 3d3d  3"...fasteners==
+000002f0: 302e 3136 2e33 2020 2320 666f 7220 7079  0.16.3  # for py
+00000300: 3220 636f 6d70 6174 6962 696c 6974 790d  2 compatibility.
+00000310: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000320: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000330: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
+00000340: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000350: 7265 5d0d 0a64 6576 203d 200d 0a09 666c  re]..dev = ...fl
+00000360: 616b 6538 0d0a 0966 6c61 6b65 382d 696d  ake8...flake8-im
+00000370: 706f 7274 2d6f 7264 6572 0d0a 0966 7574  port-order...fut
+00000380: 7572 6573 3b20 7079 7468 6f6e 5f76 6572  ures; python_ver
+00000390: 7369 6f6e 203c 2022 3322 0d0a 096d 7970  sion < "3"...myp
+000003a0: 793b 2070 7974 686f 6e5f 7665 7273 696f  y; python_versio
+000003b0: 6e20 3e3d 2022 3322 0d0a 0970 7974 6573  n >= "3"...pytes
+000003c0: 740d 0a09 7961 7066 3b20 7079 7468 6f6e  t...yapf; python
+000003d0: 5f76 6572 7369 6f6e 203e 3d20 2233 220d  _version >= "3".
+000003e0: 0a0d 0a5b 666c 616b 6538 5d0d 0a69 6d70  ...[flake8]..imp
+000003f0: 6f72 742d 6f72 6465 722d 7374 796c 6520  ort-order-style 
+00000400: 3d20 676f 6f67 6c65 0d0a 0d0a 5b65 6767  = google....[egg
+00000410: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000420: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000430: 2030 0d0a 0d0a                            0....
```

### Comparing `getpack-0.2.5/src/getpack/executable.py` & `getpack-0.2.6/src/getpack/executable.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.5/src/getpack/library/__init__.py` & `getpack-0.2.6/src/getpack/library/__init__.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.5/src/getpack/resource.py` & `getpack-0.2.6/src/getpack/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,53 +20,57 @@
 import shutil
 import sys
 import tarfile
 import threading
 import typing
 import zipfile
 
-import portalocker
+import fasteners
 from six.moves import urllib
 
 
 __FILE_LOCK_TIMEOUT__ = 15 * 60
 
 
 class HybridLock:
     def __init__(self, key):
-        self.key = key.as_posix() + '.portalock'
+        self.key = key.as_posix() + '.lock'
         self.folder = os.path.dirname(self.key)
-        self.file_lock = portalocker.RLock(
-                self.key,
-                timeout=__FILE_LOCK_TIMEOUT__,
-                mode='w',
-            )
+        self.file_lock = fasteners.InterProcessLock(self.key)
         self.lock = threading.RLock()
+        self.counter = 0
 
     def __enter__(self):
         self.lock.acquire()
-        if not os.path.isdir(self.folder):
+
+        # no more single thread now can access here
+        self.counter += 1
+        if self.counter == 1:
+            if not os.path.isdir(self.folder):
+                try:
+                    os.makedirs(self.folder)
+                except OSError:
+                    pass  # may fail because of race
             try:
-                os.makedirs(self.folder)
-            except FileExistsError:
-                pass  # may fail because of race
-        try:
-            self.file_lock.acquire()
-        except Exception:
-            # attempt to fix rare PermissionError in multiprocess races, maybe
-            # timeout? Have no info on effectiveness of following code
-            self.file_lock.acquire()
+                self.file_lock.acquire()
+            except Exception:
+                # attempt to fix rare PermissionError in multi process races,
+                # maybe timeout? Have no info on effectiveness of following
+                # code
+                self.file_lock.acquire()
 
     def __exit__(self, *_):
-        self.file_lock.release()
+        self.counter -= 1
+        if not self.counter:
+            self.file_lock.release()
+            try:
+                os.unlink(self.key)
+            except Exception:
+                pass
         self.lock.release()
-        try:
-            os.unlink(self.key)
-        except Exception:
-            pass
 
 
 def lock(key, _locks={None: threading.Lock()}):
     with _locks[None]:
         if key not in _locks:
             _locks[key] = HybridLock(key)
     return _locks[key]
```

### Comparing `getpack-0.2.5/tests/test_common.py` & `getpack-0.2.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.5/tests/test_concurrency.py` & `getpack-0.2.6/tests/test_concurrency.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,21 +16,21 @@
         Python(local_base=temp_folder),
     ]
     list(pool.map(lambda r: r.cleanup(), resources))
     list(pool.map(lambda r: r.provide(), resources))
 
 
 def _cleanup_stub(id, folder):
-    resoruce = Python(local_base=folder)
-    resoruce.cleanup()
+    resource = Python(local_base=folder)
+    resource.cleanup()
 
 
 def _provide_stub(id, folder):
-    resoruce = Python(local_base=folder)
-    resoruce.provide()
+    resource = Python(local_base=folder)
+    resource.provide()
 
 
 def test_processes(temp_folder):
     num = 30
     pool = ProcessPoolExecutor(num)
     list(pool.map(_cleanup_stub, range(num), [temp_folder] * num))
     list(pool.map(_provide_stub, range(num), [temp_folder] * num))
```

