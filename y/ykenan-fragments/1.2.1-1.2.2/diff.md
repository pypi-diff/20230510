# Comparing `tmp/ykenan_fragments-1.2.1.tar.gz` & `tmp/ykenan_fragments-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.2.1.tar", last modified: Wed May 10 11:56:35 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.2.2.tar", last modified: Wed May 10 12:51:38 2023, max compression
```

## Comparing `ykenan_fragments-1.2.1.tar` & `ykenan_fragments-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:35.219272 ykenan_fragments-1.2.1/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      971 2023-05-10 11:56:35.219272 ykenan_fragments-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.1/README.md
--rw-rw-rw-   0        0        0      773 2023-05-10 11:54:42.000000 ykenan_fragments-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 11:56:35.219272 ykenan_fragments-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:35.197256 ykenan_fragments-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:35.205256 ykenan_fragments-1.2.1/src/ykenan_fragments/
--rw-rw-rw-   0        0        0     1788 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.1/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3327 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.1/src/ykenan_fragments/genome_transformation.py
--rw-rw-rw-   0        0        0    17087 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.1/src/ykenan_fragments/get_fragments.py
--rw-rw-rw-   0        0        0    15313 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.1/src/ykenan_fragments/get_sort_fragments.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:35.218255 ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      971 2023-05-10 11:56:35.000000 ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-10 11:56:35.000000 ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:56:35.000000 ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 11:56:35.000000 ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-10 11:56:35.000000 ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.375215 ykenan_fragments-1.2.2/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      971 2023-05-10 12:51:38.374216 ykenan_fragments-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.2/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-10 12:41:21.000000 ykenan_fragments-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:51:38.375215 ykenan_fragments-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.350270 ykenan_fragments-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.360216 ykenan_fragments-1.2.2/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0     1867 2023-05-10 12:44:39.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3327 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/genome_transformation.py
+-rw-rw-rw-   0        0        0    16945 2023-05-10 12:49:55.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/get_fragments.py
+-rw-rw-rw-   0        0        0    15330 2023-05-10 12:28:25.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/get_sort_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.373246 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      971 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.2.1/LICENSE` & `ykenan_fragments-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.1/PKG-INFO` & `ykenan_fragments-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.2.1
+Version: 1.2.2
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.2.1/pyproject.toml` & `ykenan_fragments-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.2.1/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.2.2/src/ykenan_fragments/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,43 +8,45 @@
 
 from ykenan_fragments.get_sort_fragments import GetSortFragments
 
 
 class Run:
 
     def __init__(self, path: str, lift_over_path: str = None, is_hg19_to_hg38: bool = True, callback=GetSortFragments):
-        self.base_path: str = os.path.join(path, "handler")
+        self.handler_path: str = os.path.join(path, "handler")
         self.source_path: str = os.path.join(path, "source")
         self.log = Logger("Run", "log/fragments.log")
         self.file = yf.StaticMethod(log_file="log")
         self.lift_over_path: str = lift_over_path
         self.is_hg19_to_hg38: bool = is_hg19_to_hg38
         self.callback = callback
         self.exec()
 
     def exec(self):
         # 尽量保证该路径下只有 GSE 号的文件
         dirs_dict: dict = self.file.entry_dirs_dict(self.source_path)
         dirs_name: list = dirs_dict["name"]
+        dirs_name.sort()
 
         if not os.path.exists(self.source_path):
             self.log.error(f"输入文件夹 {self.source_path} 不存在")
 
         # 执行
         for gsm in dirs_name:
 
-            archr_path = os.path.join(self.base_path, gsm, "ArchR")
+            archr_path = os.path.join(self.handler_path, gsm, "ArchR")
             if not os.path.exists(archr_path):
                 self.log.info(f"创建 {archr_path} 文件夹")
                 os.makedirs(archr_path)
 
             self.log.info(f"开始执行 {gsm} 内容信息")
             fragment = self.callback(
-                path=self.base_path,
+                source_path=self.source_path,
                 merge_path=archr_path,
                 gsm=gsm,
-                get_fragments_path=self.source_path,
+                handler_path=self.handler_path,
                 lift_over_path=self.lift_over_path,
                 is_hg19_to_hg38=self.is_hg19_to_hg38
             )
+            print(fragment.endswith_list)
             fragment.exec_fragments()
             fragment.exec_sort_fragments()
```

### Comparing `ykenan_fragments-1.2.1/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.2.2/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.1/src/ykenan_fragments/get_fragments.py` & `ykenan_fragments-1.2.2/src/ykenan_fragments/get_fragments.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         self.log.info(f"Filter file information under {self.base_path} path")
         for file in files:
             file: str
             for endswith in self.endswith_list:
                 if file.endswith(endswith):
                     gz_files.append(file)
                     before = file.split(endswith)[0]
-                    if gz_files_before.count(before) == 0:
+                    if before not in gz_files_before:
                         gz_files_before.append(before)
-                        gz_files_and_before.update({file: before})
+                    gz_files_and_before.update({file: before})
                     break
         # Void judgment
         if len(gz_files) == 0:
             self.log.info(f"Gz compressed file is 0")
         else:
             # 简单验证
             if len(gz_files) % 3 == 0:
@@ -241,20 +241,16 @@
         peaks_len: int = len(peaks)
 
         if barcodes_len < 2 or peaks_len < 2:
             self.log.error(f"Insufficient file read length {self.barcodes_key}: {barcodes_len}, {self.peaks_key}: {peaks_len}")
             raise ValueError("Insufficient file read length")
 
         # 转成字典
-        barcodes_dict: dict = {}
-        for barcodes_i in range(barcodes_len):
-            barcodes_dict.update({barcodes_i, barcodes[barcodes_i]})
-        peaks_dict: dict = {}
-        for peak_i in range(peaks_len):
-            peaks_dict.update({peak_i, peaks[peak_i]})
+        barcodes_dict: dict = dict(zip(list(range(barcodes_len)), barcodes))
+        peaks_dict: dict = dict(zip(list(range(peaks_len)), peaks))
 
         self.log.info(f"Quantity or Path {self.barcodes_key}: {barcodes_len}, {self.mtx_key}: {mtx_path}, {self.peaks_key}: {peaks_len}")
         # Read quantity
         mtx_count: int = 0
         error_count: int = 0
         mtx_all_number: int = 0
         # create a file
```

### Comparing `ykenan_fragments-1.2.1/src/ykenan_fragments/get_sort_fragments.py` & `ykenan_fragments-1.2.2/src/ykenan_fragments/get_sort_fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 from ykenan_fragments.genome_transformation import Hg19AndHg38
 from ykenan_fragments.get_fragments import GetFragments
 
 
 class GetSortFragments(GetFragments):
 
-    def __init__(self, path: str, merge_path: str, gsm: str, get_fragments_path: str, lift_over_path: str, is_hg19_to_hg38: bool = True):
+    def __init__(self, source_path: str, merge_path: str, gsm: str, handler_path: str, lift_over_path: str, is_hg19_to_hg38: bool = True):
         """
         Form a fragments
-        :param path: Path to store unordered fragments files
+        :param source_path: Path to store unordered fragments files
         :param merge_path: Path to generate fragments files
         :param gsm: GSE number (here is a folder name)
-        :param get_fragments_path: base_path parameter in GetFragments class
+        :param handler_path: base_path parameter in GetFragments class
         :param is_hg19_to_hg38: 是否为 hg19 文件
         """
-        super().__init__(get_fragments_path, path, gsm)
-        self.base_path: str = os.path.join(path, gsm)
-        self.fragments_path: str = os.path.join(self.base_path, "fragments")
+        super().__init__(source_path, handler_path, gsm)
+        self.handler_path: str = os.path.join(handler_path, gsm)
+        self.fragments_path: str = os.path.join(self.handler_path, "fragments")
         self.merge_input_path: str = merge_path
         self.lift_over_path: str = lift_over_path
         self.is_hg19_to_hg38: bool = is_hg19_to_hg38
         self.genome_source: str = "hg19" if self.is_hg19_to_hg38 else "hg38"
         self.genome_generate: str = "hg38" if self.is_hg19_to_hg38 else "hg19"
         self.genomes: list = [self.genome_source, self.genome_generate]
         self.chr_list: dict = {
```

### Comparing `ykenan_fragments-1.2.1/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.2.1
+Version: 1.2.2
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

