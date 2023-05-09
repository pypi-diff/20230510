# Comparing `tmp/YMS-0.71.tar.gz` & `tmp/YMS-0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.71.tar", last modified: Mon May  1 09:02:18 2023, max compression
+gzip compressed data, was "YMS-0.74.tar", last modified: Tue May  9 22:19:41 2023, max compression
```

## Comparing `YMS-0.71.tar` & `YMS-0.74.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-01 09:02:18.535226 YMS-0.71/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-01 09:02:18.535226 YMS-0.71/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.71/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-01 09:02:18.535226 YMS-0.71/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-01 09:02:18.000000 YMS-0.71/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-01 09:02:18.000000 YMS-0.71/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-01 09:02:18.000000 YMS-0.71/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-01 09:02:18.000000 YMS-0.71/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        5 2023-05-01 09:02:18.000000 YMS-0.71/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-01 09:02:18.000000 YMS-0.71/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-01 09:02:18.535226 YMS-0.71/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      455 2023-05-01 09:01:00.000000 YMS-0.71/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-01 09:02:18.535226 YMS-0.71/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1660 2023-05-01 08:33:20.000000 YMS-0.71/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.71/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     8020 2023-05-01 08:15:30.000000 YMS-0.71/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      995 2023-05-01 08:15:42.000000 YMS-0.71/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.71/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.71/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-09 22:19:41.555065 YMS-0.74/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-09 22:19:41.555065 YMS-0.74/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.74/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-09 22:19:41.555065 YMS-0.74/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-09 22:19:41.555065 YMS-0.74/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-09 22:04:47.000000 YMS-0.74/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-09 22:19:41.555065 YMS-0.74/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.74/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.74/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9581 2023-05-09 22:04:26.000000 YMS-0.74/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.74/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.74/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.74/yamas/utilities.py
```

### Comparing `YMS-0.71/README.md` & `YMS-0.74/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.71/yamas/__init__.py` & `YMS-0.74/yamas/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 def main():
     parser = argparse.ArgumentParser(description='YMS package')
     parser.add_argument('-v', '--version', action='version',
                         version='%(prog)s {version}'.format(version=pkg_resources.require("YMS")[0].version))
 
     parser.add_argument('--download', nargs='+', help='Add datasets to be downloaded')
-    parser.add_argument('--verbose', action='store_true', help='Enable verbose mode')
+    parser.add_argument('--type', nargs=1, choices=['16S', 'Shotgun'], help='Type of data to be downloaded')
     parser.add_argument('--export', nargs=7,
                         help="output_dir, trim, trunc, classifier_file, otu_output_file, taxonomy_output_file, threads")
     parser.add_argument('--config', help='Path to config file')
+    parser.add_argument('--verbose', action='store_true', help='Enable verbose mode')
     args = parser.parse_args()
 
     if args.config:
         with open(args.config) as f:
             config = json.load(f)
         specific_location = config.get('specific_location')
     else:
@@ -34,9 +35,13 @@
             trunc = int(args.export[2])
             classifier_file = args.export[3]
             export(output_dir, trim, trunc, classifier_file)
         except IndexError:
             print(f"missing {len(args.export)-1} arguments")
 
     if args.download:
-        for dataset_name in args.download:
-            download(dataset_name, args.verbose, specific_location)
+        if not(args.type):
+            raise ValueError("Missing dataset type. Use --type 16S/Shotgun")
+        else:
+            data_type = args.type[0]
+            for dataset_name in args.download:
+                download(dataset_name,data_type, args.verbose, specific_location)
```

### Comparing `YMS-0.71/yamas/create_visualization.py` & `YMS-0.74/yamas/create_visualization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import csv
 import os.path
 import pickle
 import datetime
 from tqdm import tqdm
-
+from metaphlan.utils.merge_metaphlan_tables import merge
 from .utilities import run_cmd, ReadsData, check_conda_qiime2
 
 CONDA_PREFIX = os.environ.get("CONDA_PREFIX", None)
 
 
 def check_input(acc_list: str):
     # flag = False
@@ -124,15 +124,32 @@
         "qiime", "demux", "summarize",
         "--i-data", qza_file_path,
         "--o-visualization", vis_file_path
     ]
     run_cmd(command)
     return vis_file_path
 
-def visualization(acc_list, dataset_id, verbose_print, specific_location):
+def metaphlan_extraction(reads_data, dataset_id):
+    fastq_path = os.path.join(reads_data.dir_path, "fastq")
+    export_path = os.path.join(reads_data.dir_path, "export")
+    run_cmd([f"mkdir {export_path}"])
+    final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
+    run_cmd([f"touch {final_output_path}"])
+    args = []
+    for fastq_file in tqdm(os.listdir(fastq_path)):
+        fastq, extension = os.path.splitext(fastq_file)
+        input = os.path.join(fastq_path,fastq)
+        output = os.path.join(os.path.join(reads_data.dir_path, 'qza'), f'{fastq}_profile.txt')
+        command = [f"metaphlan {input} --input_type fastq --nproc 16 > {output} "]
+        run_cmd(command)
+        args.append(output)
+    merge(args, open(final_output_path, 'w'), gtdb=False)
+
+
+def visualization(acc_list, dataset_id, data_type, verbose_print, specific_location):
     verbose_print("\n")
     verbose_print(datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S'))
     dir_name = f"{dataset_id}-{datetime.datetime.now().strftime('%d-%m-%Y_%H-%M-%S')}"
     verbose_print("Starting conversion to VIS file")
 
     verbose_print("\n")
     verbose_print('Checking environment...', end=" ")
@@ -141,49 +158,59 @@
     verbose_print("Checking inputs:")
     check_input(acc_list)
 
     verbose_print("\n")
     verbose_print("Creating a new directory for this dataset import:'", dir_name, "'")
     dir_path = create_dir(dir_name,specific_location)
     verbose_print("Find ALL NEW data in:", dir_path)
+    stages_length = 5 if data_type=='16S' else 3
 
     verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start prefetch (1/5)")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start prefetch (1/{stages_length})")
     download_data_from_sra(dir_path, acc_list)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish prefetch (1/5)")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish prefetch (1/{stages_length})")
 
     verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start conversion (2/5)")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start conversion (2/{stages_length})")
     reads_data = sra_to_fastq(dir_path)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish conversion (2/5)")
+    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish conversion (2/{stages_length})")
 
-    verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start creating manifest (3/5)")
-    create_manifest(reads_data)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish creating manifest (3/5)")
+    if data_type == '16S':
+        verbose_print("\n")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start creating manifest (3/5)")
+        create_manifest(reads_data)
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish creating manifest (3/5)")
+
+        verbose_print("\n")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start 'qiime import' (4/5)")
+        qza_file_path = qiime_import(reads_data)
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish 'qiime import' (4/5)")
+
+        verbose_print("\n")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start 'qiime demux' (5/5)")
+        vis_file_path = qiime_demux(reads_data, qza_file_path, dataset_id)
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish 'qiime demux' (5/5)")
+
+        pickle.dump(reads_data, open(os.path.join(reads_data.dir_path, "reads_data.pkl"), "wb"))
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish creating visualization\n")
+
+        print(f"Visualization file is located in {vis_file_path}\n"
+              f"Please drag this file to https://view.qiime2.org/ and continue.\n")
+        if reads_data.fwd and reads_data.rev:
+            print(f"Note: The data has both forward and reverse reads.\n"
+                  f"Therefore, you must give the parameters 'trim' and 'trunc' of export() "
+                  f"as a tuple of two integers."
+                  f"The first place related to the forward read and the second to the reverse.")
+        else:
+            print(f"Note: The data has only a forward read.\n"
+                  f"Therefore, you must give the parameters 'trim' and 'trunc' of export() "
+                  f"exactly one integers value which is related to the forward read.")
 
-    verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start 'qiime import' (4/5)")
-    qza_file_path = qiime_import(reads_data)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish 'qiime import' (4/5)")
-
-    verbose_print("\n")
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start 'qiime demux' (5/5)")
-    vis_file_path = qiime_demux(reads_data, qza_file_path, dataset_id)
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish 'qiime demux' (5/5)")
-
-    pickle.dump(reads_data, open(os.path.join(reads_data.dir_path, "reads_data.pkl"), "wb"))
-    verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish creating visualization\n")
-
-    print(f"Visualization file is located in {vis_file_path}\n"
-          f"Please drag this file to https://view.qiime2.org/ and continue.\n")
-    if reads_data.fwd and reads_data.rev:
-        print(f"Note: The data has both forward and reverse reads.\n"
-              f"Therefore, you must give the parameters 'trim' and 'trunc' of export() "
-              f"as a tuple of two integers."
-              f"The first place related to the forward read and the second to the reverse.")
+        return reads_data.dir_path
     else:
-        print(f"Note: The data has only a forward read.\n"
-              f"Therefore, you must give the parameters 'trim' and 'trunc' of export() "
-              f"exactly one integers value which is related to the forward read.")
+        verbose_print("\n")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (3/3)")
+        metaphlan_extraction(reads_data, dataset_id)
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (3/3)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finished downloading.\n")
+
 
-    return reads_data.dir_path
```

### Comparing `YMS-0.71/yamas/dataset_downloading.py` & `YMS-0.74/yamas/dataset_downloading.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     get_acc_info_command = f"cat {bio_project_name}_run_info.csv | cut -f 1 -d ',' | grep -e ERR -e SRR > {bio_project_name}_acc_info.txt"
     os.system(get_acc_info_command)
     verbose_print(f"downloaded the accession list at {bio_project_name}_acc_info.txt")
 
     return f"{bio_project_name}_acc_info.txt"
 
 
-def download(dataset_name, verbose,specific_location):
+def download(dataset_name,data_type, verbose,specific_location):
     verbose_print = print if verbose else lambda *a, **k: None
 
     verbose_print("\n")
     verbose_print("download starts.")
 
     acc_list_path = get_acc_list(dataset_name, verbose_print)
-    visualization(acc_list_path, dataset_name, verbose_print,specific_location)
+    visualization(acc_list_path, dataset_name,data_type, verbose_print,specific_location)
```

### Comparing `YMS-0.71/yamas/export_data.py` & `YMS-0.74/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.71/yamas/utilities.py` & `YMS-0.74/yamas/utilities.py`

 * *Files identical despite different names*

