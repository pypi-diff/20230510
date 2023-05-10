# Comparing `tmp/bimcvcovid19i-0.0.5.tar.gz` & `tmp/bimcvcovid19i-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimcvcovid19i-0.0.5.tar", last modified: Mon Oct 24 13:46:36 2022, max compression
+gzip compressed data, was "bimcvcovid19i-0.0.6.tar", last modified: Wed May 10 21:10:21 2023, max compression
```

## Comparing `bimcvcovid19i-0.0.5.tar` & `bimcvcovid19i-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,26 @@
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2022-10-24 13:46:36.109768 bimcvcovid19i-0.0.5/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.0.5/LICENSE
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.0.5/MANIFEST.in
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1103 2022-10-24 13:46:36.109768 bimcvcovid19i-0.0.5/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      551 2022-10-20 16:04:50.000000 bimcvcovid19i-0.0.5/README.md
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2022-10-24 13:46:36.101768 bimcvcovid19i-0.0.5/bimcvcovid19i/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/__init__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/__init__.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2022-10-20 16:06:26.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/__version__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/__version__.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)    16418 2022-10-24 13:45:48.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/data.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1709 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/data.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-18 16:36:33.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/interface.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/interface.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/py.typed
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     5648 2022-10-21 12:40:09.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/tools.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      968 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/tools.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6675 2022-10-24 13:44:27.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/typing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2380 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/typing.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3608 2022-10-19 06:06:44.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/webdav.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      484 2022-10-24 13:46:35.000000 bimcvcovid19i-0.0.5/bimcvcovid19i/webdav.pyi
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2022-10-24 13:46:36.105768 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1103 2022-10-24 13:46:36.000000 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      655 2022-10-24 13:46:36.000000 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/SOURCES.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-24 13:46:36.000000 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/dependency_links.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/not-zip-safe
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       63 2022-10-24 13:46:36.000000 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/requires.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2022-10-24 13:46:36.000000 bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/top_level.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       63 2022-10-19 07:32:18.000000 bimcvcovid19i-0.0.5/requirements.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2022-10-24 13:46:36.109768 bimcvcovid19i-0.0.5/setup.cfg
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.0.5/setup.py
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.0.6/LICENSE
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.0.6/MANIFEST.in
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1108 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      576 2022-10-27 06:18:30.000000 bimcvcovid19i-0.0.6/README.md
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/bimcvcovid19i/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/__init__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2022-10-24 13:46:59.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/__version__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2022-12-02 18:20:47.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/assets.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)    16778 2023-05-08 09:30:42.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/data.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2022-10-18 16:36:33.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/interface.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2022-12-03 14:07:39.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/postprocessing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/py.typed
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     5648 2022-10-21 12:40:09.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/tools.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6988 2022-10-25 16:48:30.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/typing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.0.6/bimcvcovid19i/webdav.py
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1108 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      529 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/SOURCES.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/dependency_links.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/not-zip-safe
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/requires.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-05-10 21:10:21.000000 bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/top_level.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.0.6/requirements.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-05-10 21:10:21.748313 bimcvcovid19i-0.0.6/setup.cfg
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.0.6/setup.py
```

### Comparing `bimcvcovid19i-0.0.5/LICENSE` & `bimcvcovid19i-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.5/PKG-INFO` & `bimcvcovid19i-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BIMCV COVID 19 interface
+
 This repository provides a python interface for working with [BIMCV COVID 19 dataset](https://github.com/BIMCV-CSUSP/BIMCV-COVID-19)
 
 Before use, please read the [license agreement](https://github.com/BIMCV-CSUSP/BIMCV-COVID-19) for the use of the BIMCV-COVID19 Dataset.
 
 ## Installation
 
 ```bash
 pip install bimcvcovid19i
 ```
 
 ## System requirements
 
-|Dataset               |Original|Prepered|
-|----------------------|:------:|:------:|
-|BIMCV COVID19 negative|    469G|        |
-|BIMCV COVID19 positive|    390G|        |
-
-
+|Dataset               |Original|Prepered|Total|
+|----------------------|:------:|:------:|:---:|
+|BIMCV COVID19 positive|    390G|    408G| 797G|
+|BIMCV COVID19 negative|    469G|    480G| 948G|
```

### Comparing `bimcvcovid19i-0.0.5/README.md` & `bimcvcovid19i-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # BIMCV COVID 19 interface
+
 This repository provides a python interface for working with [BIMCV COVID 19 dataset](https://github.com/BIMCV-CSUSP/BIMCV-COVID-19)
 
 Before use, please read the [license agreement](https://github.com/BIMCV-CSUSP/BIMCV-COVID-19) for the use of the BIMCV-COVID19 Dataset.
 
 ## Installation
 
 ```bash
 pip install bimcvcovid19i
 ```
 
 ## System requirements
 
-|Dataset               |Original|Prepered|
-|----------------------|:------:|:------:|
-|BIMCV COVID19 negative|    469G|        |
-|BIMCV COVID19 positive|    390G|        |
+|Dataset               |Original|Prepered|Total|
+|----------------------|:------:|:------:|:---:|
+|BIMCV COVID19 positive|    390G|    408G| 797G|
+|BIMCV COVID19 negative|    469G|    480G| 948G|
```

### Comparing `bimcvcovid19i-0.0.5/bimcvcovid19i/data.py` & `bimcvcovid19i-0.0.6/bimcvcovid19i/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __all__ = [
-    "BIMCVCOVID19positiveData",
-    "BIMCVCOVID19negativeData",
+    "BIMCVCOVID19positiveData_12",
+    "BIMCVCOVID19positiveData_123",
+    "BIMCVCOVID19negativeData_12",
 ]
 
 import itertools as it
 import logging
 import operator as op
 import shutil
 import tarfile
@@ -20,14 +21,15 @@
     DatasetRoot,
     Labels,
     Series,
     SeriesRawPath,
     Session,
     Subject,
     Test,
+    EmptyFileError,
 )
 from .webdav import webdav_download_all
 
 
 class BIMCVCOVID19Root(DatasetRoot):
     @property
     def prepared_series(self) -> Path:
@@ -138,14 +140,16 @@
                         # NOTE: skip. This case is similar to a report containing personal data
                         if (
                             "Cannot cast array data from dtype([('R', 'u1'), ('G', 'u1'), ('B', 'u1')])"
                             in exc.args[0]
                         ):
                             continue
                     raise exc
+                except EmptyFileError:
+                    continue
 
     def subjects(self) -> tp.List[Subject]:
         path = self.original / self.subjects_tarfile_name
         subpath = self.subjects_tarfile_subpath
 
         with tools.open_from_tar(path, subpath) as file:
             dataframe = pd.read_csv(file, sep="\t")
@@ -368,15 +372,15 @@
             if not subject.series_ids:
                 continue
 
             subject.tests = tests.get(subject.uid)
             subject.save(self.prepared_subjects / subject.uid)
 
 
-class BIMCVCOVID19positiveData(BIMCVCOVID19Data):
+class BIMCVCOVID19positiveData_12(BIMCVCOVID19Data):
     webdav_hostname = "https://b2drop.bsc.es/public.php/webdav"
     webdav_login = "BIMCV-COVID19-cIter_1_2"
     webdav_password = "maybeempty"
 
     subjects_tarfile_name = "covid19_posi_subjects.tar.gz"
     subjects_tarfile_subpath = "covid19_posi/participants.tsv"
 
@@ -385,15 +389,22 @@
     tests_tarfile_name = "covid19_posi_head.tar.gz"
     tests_tarfile_subpath = "covid19_posi/derivatives/EHR/sil_reg_covid_posi.tsv"
 
     labels_tarfile_name = "covid19_posi_head.tar.gz"
     labels_tarfile_subpath = "covid19_posi/derivatives/labels/labels_covid_posi.tsv"
 
 
-class BIMCVCOVID19negativeData(BIMCVCOVID19Data):
+class BIMCVCOVID19positiveData_123(BIMCVCOVID19Data):
+    webdav_hostname = "https://b2drop.bsc.es/public.php/webdav"
+    webdav_login = "BIMCV-COVID19-cIter_1_2_3"
+    webdav_password = "maybeempty"
+    # TODO: maybe bug
+
+
+class BIMCVCOVID19negativeData_12(BIMCVCOVID19Data):
     webdav_hostname = "https://b2drop.bsc.es/public.php/webdav"
     webdav_login = "BIMCV-COVID19-cIter_1_2-Negative"
     webdav_password = "maybeempty"
 
     subjects_tarfile_name = "covid19_neg_metadata.tar.gz"
     subjects_tarfile_subpath = "covid19_neg/participants.tsv"
```

### Comparing `bimcvcovid19i-0.0.5/bimcvcovid19i/tools.py` & `bimcvcovid19i-0.0.6/bimcvcovid19i/tools.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.0.5/bimcvcovid19i/typing.py` & `bimcvcovid19i-0.0.6/bimcvcovid19i/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,31 +164,41 @@
         deli.save(self.modality, root / "modality.json")
 
     @classmethod
     def load(cls, root: LikePath) -> "Series":
         raise NotImplementedError
 
 
+class EmptyFileError(RuntimeError):
+    pass
+
+
 @dataclass
 class SeriesRawPath:
     uid: str
     image_path: tp.Optional[Path]
     tags_path: tp.Optional[Path]
 
     def read_item(self) -> Series:
         image = None
         spacing = None
         if self.image_path is not None:
-            if str(self.image_path).endswith(".png"):
-                image = tools.png2numpy(self.image_path)
-            elif str(self.image_path).endswith(".nii.gz"):
-                image = tools.nifty2numpy(self.image_path)
-                spacing = tools.spacing_from_nifty(self.image_path)
-            else:
-                raise NotImplementedError(self.image_path)
+            try:
+                if str(self.image_path).endswith(".png"):
+                    image = tools.png2numpy(self.image_path)
+                elif str(self.image_path).endswith(".nii.gz"):
+                    image = tools.nifty2numpy(self.image_path)
+                    spacing = tools.spacing_from_nifty(self.image_path)
+                else:
+                    raise NotImplementedError(self.image_path)
+            except RuntimeError as exc:
+                with open(self.image_path, "rb") as file:
+                    if file.read() == b"":
+                        raise EmptyFileError from exc
+                raise exc
             image = tools.down_type(image)
 
         tags = None
         if self.tags_path is not None:
             tags_data = deli.load(self.tags_path)
             assert isinstance(tags_data, dict)
             tags = tools.parse_dicom_tags(tags_data)
```

### Comparing `bimcvcovid19i-0.0.5/bimcvcovid19i/webdav.py` & `bimcvcovid19i-0.0.6/bimcvcovid19i/webdav.py`

 * *Files 20% similar despite different names*

```diff
@@ -90,24 +90,30 @@
         )
     )
 
     names = {Path(info["path"]).name for info in client.list(get_info=True)}
     if "webdav" in names:
         names.remove("webdav")
 
+    sha1sums_file_name = "sha1sums.txt"
+    if sha1sums_file_name not in names:
+        sha1sums_file_name = "sha1sum.txt"
+
     sha1sums = {}
-    if "sha1sums.txt" in names:
-        names.remove("sha1sums.txt")
+
+    if sha1sums_file_name in names:
+        names.remove(sha1sums_file_name)
         webdav_download_file(
             client=client,
-            remote_path="sha1sums.txt",
-            local_path=download_path / "sha1sums.txt",
+            remote_path=sha1sums_file_name,
+            local_path=download_path / sha1sums_file_name,
         )
-        sha1sums.update(read_checksums(download_path / "sha1sums.txt"))
+        sha1sums.update(read_checksums(download_path / sha1sums_file_name))
 
+    # TODO: use logging instead of tqdm?
     names_bar = tqdm(names)
     for name in names_bar:
         names_bar.set_description(f"donwloading {name:50}")
         webdav_download_file(
             client=client,
             remote_path=name,
             local_path=str(download_path / name),
@@ -120,9 +126,9 @@
             pass
             # if get_sha1(file_path) == value:
             #     pass
             # else:
             #     pass
         else:
             warnings.warn(
-                f"file '{name}' is listed in sha1sums.txt but has not been downloaded"
+                f"file '{name}' is listed in {sha1sums_file_name} but has not been downloaded"
             )
```

### Comparing `bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/PKG-INFO` & `bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BIMCV COVID 19 interface
+
 This repository provides a python interface for working with [BIMCV COVID 19 dataset](https://github.com/BIMCV-CSUSP/BIMCV-COVID-19)
 
 Before use, please read the [license agreement](https://github.com/BIMCV-CSUSP/BIMCV-COVID-19) for the use of the BIMCV-COVID19 Dataset.
 
 ## Installation
 
 ```bash
 pip install bimcvcovid19i
 ```
 
 ## System requirements
 
-|Dataset               |Original|Prepered|
-|----------------------|:------:|:------:|
-|BIMCV COVID19 negative|    469G|        |
-|BIMCV COVID19 positive|    390G|        |
-
-
+|Dataset               |Original|Prepered|Total|
+|----------------------|:------:|:------:|:---:|
+|BIMCV COVID19 positive|    390G|    408G| 797G|
+|BIMCV COVID19 negative|    469G|    480G| 948G|
```

### Comparing `bimcvcovid19i-0.0.5/bimcvcovid19i.egg-info/SOURCES.txt` & `bimcvcovid19i-0.0.6/bimcvcovid19i.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 bimcvcovid19i/__init__.py
-bimcvcovid19i/__init__.pyi
 bimcvcovid19i/__version__.py
-bimcvcovid19i/__version__.pyi
+bimcvcovid19i/assets.py
 bimcvcovid19i/data.py
-bimcvcovid19i/data.pyi
 bimcvcovid19i/interface.py
-bimcvcovid19i/interface.pyi
+bimcvcovid19i/postprocessing.py
 bimcvcovid19i/py.typed
 bimcvcovid19i/tools.py
-bimcvcovid19i/tools.pyi
 bimcvcovid19i/typing.py
-bimcvcovid19i/typing.pyi
 bimcvcovid19i/webdav.py
-bimcvcovid19i/webdav.pyi
 bimcvcovid19i.egg-info/PKG-INFO
 bimcvcovid19i.egg-info/SOURCES.txt
 bimcvcovid19i.egg-info/dependency_links.txt
 bimcvcovid19i.egg-info/not-zip-safe
 bimcvcovid19i.egg-info/requires.txt
 bimcvcovid19i.egg-info/top_level.txt
```

### Comparing `bimcvcovid19i-0.0.5/setup.py` & `bimcvcovid19i-0.0.6/setup.py`

 * *Files identical despite different names*

