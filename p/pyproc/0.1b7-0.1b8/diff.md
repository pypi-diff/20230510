# Comparing `tmp/pyproc-0.1b7.tar.gz` & `tmp/pyproc-0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyproc-0.1b7.tar", last modified: Mon Apr 22 04:32:52 2019, max compression
+gzip compressed data, was "dist/pyproc-0.1b8.tar", last modified: Mon Apr 22 07:32:23 2019, max compression
```

## Comparing `pyproc-0.1b7.tar` & `pyproc-0.1b8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 04:32:52.000000 pyproc-0.1b7/
--rw-r--r--   0 root         (0) root         (0)     7533 2019-04-22 04:32:52.000000 pyproc-0.1b7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5303 2019-04-22 04:32:39.000000 pyproc-0.1b7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc/
--rw-rw-rw-   0 root         (0) root         (0)      254 2019-04-22 04:32:39.000000 pyproc-0.1b7/pyproc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2019-04-22 04:32:39.000000 pyproc-0.1b7/pyproc/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3155 2019-04-22 04:32:39.000000 pyproc-0.1b7/pyproc/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2019-04-22 04:32:39.000000 pyproc-0.1b7/pyproc/kategori.py
--rw-rw-rw-   0 root         (0) root         (0)    19258 2019-04-22 04:32:39.000000 pyproc-0.1b7/pyproc/lpse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7533 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      359 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-04-22 04:32:52.000000 pyproc-0.1b7/pyproc.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 04:32:52.000000 pyproc-0.1b7/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-04-22 04:32:39.000000 pyproc-0.1b7/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12996 2019-04-22 04:32:39.000000 pyproc-0.1b7/scripts/downloader.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-04-22 04:32:52.000000 pyproc-0.1b7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1569 2019-04-22 04:32:39.000000 pyproc-0.1b7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 07:32:23.000000 pyproc-0.1b8/
+-rw-r--r--   0 root         (0) root         (0)     7533 2019-04-22 07:32:23.000000 pyproc-0.1b8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5303 2019-04-22 07:32:11.000000 pyproc-0.1b8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2019-04-22 07:32:11.000000 pyproc-0.1b8/pyproc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2019-04-22 07:32:11.000000 pyproc-0.1b8/pyproc/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2019-04-22 07:32:11.000000 pyproc-0.1b8/pyproc/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2019-04-22 07:32:11.000000 pyproc-0.1b8/pyproc/kategori.py
+-rw-rw-rw-   0 root         (0) root         (0)    19258 2019-04-22 07:32:11.000000 pyproc-0.1b8/pyproc/lpse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7533 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      359 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-04-22 07:32:23.000000 pyproc-0.1b8/pyproc.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-04-22 07:32:23.000000 pyproc-0.1b8/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-04-22 07:32:11.000000 pyproc-0.1b8/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13597 2019-04-22 07:32:11.000000 pyproc-0.1b8/scripts/downloader.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-04-22 07:32:23.000000 pyproc-0.1b8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2019-04-22 07:32:11.000000 pyproc-0.1b8/setup.py
```

### Comparing `pyproc-0.1b7/PKG-INFO` & `pyproc-0.1b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproc
-Version: 0.1b7
+Version: 0.1b8
 Summary: Python SPSEv4 wrapper
 Home-page: https://gitlab.com/wakataw/pyproc
 Author: Agung Pratama
 Author-email: agungpratama1001@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://gitlab.com/wakataw/pyproc/issues
 Project-URL: Source, https://gitlab.com/wakataw/pyproc
```

### Comparing `pyproc-0.1b7/README.md` & `pyproc-0.1b8/README.md`

 * *Files identical despite different names*

### Comparing `pyproc-0.1b7/pyproc/helpers.py` & `pyproc-0.1b8/pyproc/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             detil = self.lpse.detil_paket_tender(id_paket)
         else:
             detil = self.lpse.detil_paket_non_tender(id_paket)
 
         try:
             detil.get_pengumuman()
             detil.get_pemenang()
+            detil.get_jadwal()
         except Exception as e:
 
             if retry < self.max_retry:
                 with self.lock:
                     self.lpse.session = requests.session()
                     self.lpse.session.verify = False
```

### Comparing `pyproc-0.1b7/pyproc/lpse.py` & `pyproc-0.1b8/pyproc/lpse.py`

 * *Files identical despite different names*

### Comparing `pyproc-0.1b7/pyproc.egg-info/PKG-INFO` & `pyproc-0.1b8/pyproc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproc
-Version: 0.1b7
+Version: 0.1b8
 Summary: Python SPSEv4 wrapper
 Home-page: https://gitlab.com/wakataw/pyproc
 Author: Agung Pratama
 Author-email: agungpratama1001@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://gitlab.com/wakataw/pyproc/issues
 Project-URL: Source, https://gitlab.com/wakataw/pyproc
```

### Comparing `pyproc-0.1b7/scripts/downloader.py` & `pyproc-0.1b8/scripts/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,24 +145,31 @@
         'alamat': None,
         'harga_penawaran': None,
         'harga_terkoreksi': None,
         'hasil_negosiasi': None,
     }
 
     with open(detil_combined, 'w', encoding='utf8', errors="ignore") as csvf:
+        fieldnames = list(pengumuman_keys.keys() if jenis_paket == 'tender' else pengumuman_nontender_keys.keys())
+        fieldnames += ['penetapan_pemenang_mulai', 'penetapan_pemenang_sampai']
+
         writer = csv.DictWriter(
             csvf,
-            fieldnames=pengumuman_keys.keys() if jenis_paket == 'tender' else pengumuman_nontender_keys.keys()
+            fieldnames=fieldnames
         )
 
         writer.writeheader()
 
         for detil_file in detil_all:
             detil = pengumuman_keys.copy() if jenis_paket == 'tender' else pengumuman_nontender_keys.copy()
 
+            detil.update(
+                {'penetapan_pemenang_mulai': None, 'penetapan_pemenang_sampai': None}
+            )
+
             with open(detil_file, 'r', encoding='utf8', errors="ignore") as f:
                 data = json.loads(f.read())
 
             detil['id_paket'] = data['id_paket']
 
             if data['pengumuman']:
                 detil.update((k, data['pengumuman'][k]) for k in detil.keys() & data['pengumuman'].keys())
@@ -176,14 +183,21 @@
 
                 if detil[tahap]:
                     detil[tahap] = detil[tahap].strip(r' [...]')
 
             if data['pemenang']:
                 detil.update((k, data['pemenang'][k]) for k in detil.keys() & data['pemenang'].keys())
 
+            if data['jadwal']:
+                data_pemenang = list(filter(lambda x: x['tahap'] == 'Penetapan Pemenang', data['jadwal']))
+
+                if data_pemenang:
+                    detil['penetapan_pemenang_mulai'] = data_pemenang[0]['mulai']
+                    detil['penetapan_pemenang_sampai'] = data_pemenang[0]['sampai']
+
             writer.writerow(detil)
 
             del detil
 
     copy_result(folder_name, remove=remove)
 
 
@@ -377,15 +391,15 @@
             detil_downloader.set_host(lpse=_lpse)
 
             get_detil(downloader=detil_downloader, jenis_paket=jenis_paket, tahun_anggaran=tahun_anggaran,
                       index_path=index_path)
             print("\n- download selesai\n")
 
             print("Menggabungkan Data")
-            combine_data(_lpse.host, jenis_paket)
+            combine_data(_lpse.host, jenis_paket, not args.keep)
             print("- proses selesai")
 
     except KeyboardInterrupt:
         print("\n\nERROR: Proses dibatalkan oleh user, bye!")
         detil_downloader.stop_process()
     except Exception as e:
         print("\n\nERROR:", e)
```

### Comparing `pyproc-0.1b7/setup.py` & `pyproc-0.1b8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = path.abspath(path.dirname(__file__))
 
 with open(path.join(BASE_DIR, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyproc',
-    version='0.1b7',
+    version='0.1b8',
     description='Python SPSEv4 wrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/wakataw/pyproc',
     author='Agung Pratama',
     author_email='agungpratama1001@gmail.com',
     classifiers=[
```

