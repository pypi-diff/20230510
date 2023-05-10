# Comparing `tmp/slurm-parallel-0.1.3.tar.gz` & `tmp/slurm-parallel-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-parallel-0.1.3.tar", last modified: Tue May  9 07:38:36 2023, max compression
+gzip compressed data, was "slurm-parallel-0.1.4.tar", last modified: Tue May  9 20:45:36 2023, max compression
```

## Comparing `slurm-parallel-0.1.3.tar` & `slurm-parallel-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.384932 slurm-parallel-0.1.3/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.3/LICENSE
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      150 2023-05-09 05:30:00.000000 slurm-parallel-0.1.3/MANIFEST.in
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-09 07:38:36.378884 slurm-parallel-0.1.3/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.3/README.md
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      714 2023-05-09 07:37:51.000000 slurm-parallel-0.1.3/pyproject.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-09 07:38:36.387165 slurm-parallel-0.1.3/setup.cfg
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:35.801493 slurm-parallel-0.1.3/src/
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.252032 slurm-parallel-0.1.3/src/slurm_parallel/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.3/src/slurm_parallel/__init__.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       37 2023-05-08 18:25:50.000000 slurm-parallel-0.1.3/src/slurm_parallel/cleanup.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.3/src/slurm_parallel/config.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      918 2023-05-09 07:36:00.000000 slurm-parallel-0.1.3/src/slurm_parallel/run.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       28 2023-05-09 04:55:29.000000 slurm-parallel-0.1.3/src/slurm_parallel/run.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)    11218 2023-05-09 07:37:31.000000 slurm-parallel-0.1.3/src/slurm_parallel/slurm.py
--rwxr-xr-x   0 hc3190   (413786699) domain users (413600513)     1050 2023-05-09 05:29:06.000000 slurm-parallel-0.1.3/src/slurm_parallel/summarize.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.3/src/slurm_parallel/utils.py
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.275006 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      498 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/SOURCES.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/dependency_links.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       20 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/requires.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-09 07:38:35.000000 slurm-parallel-0.1.3/src/slurm_parallel.egg-info/top_level.txt
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 07:38:36.281202 slurm-parallel-0.1.3/test/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1406 2023-05-09 07:35:16.000000 slurm-parallel-0.1.3/test/test.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 20:45:36.142360 slurm-parallel-0.1.4/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.4/LICENSE
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      112 2023-05-09 20:43:09.000000 slurm-parallel-0.1.4/MANIFEST.in
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-09 20:45:36.133731 slurm-parallel-0.1.4/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.4/README.md
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      714 2023-05-09 20:45:20.000000 slurm-parallel-0.1.4/pyproject.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-09 20:45:36.150401 slurm-parallel-0.1.4/setup.cfg
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 20:45:35.897507 slurm-parallel-0.1.4/src/
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 20:45:36.043577 slurm-parallel-0.1.4/src/slurm_parallel/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.4/src/slurm_parallel/__init__.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.4/src/slurm_parallel/config.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      918 2023-05-09 07:36:00.000000 slurm-parallel-0.1.4/src/slurm_parallel/run.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       28 2023-05-09 04:55:29.000000 slurm-parallel-0.1.4/src/slurm_parallel/run.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     9397 2023-05-09 20:44:05.000000 slurm-parallel-0.1.4/src/slurm_parallel/slurm.py
+-rwxr-xr-x   0 hc3190   (413786699) domain users (413600513)       46 2023-05-09 20:13:12.000000 slurm-parallel-0.1.4/src/slurm_parallel/summarize.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.4/src/slurm_parallel/utils.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 20:45:36.099386 slurm-parallel-0.1.4/src/slurm_parallel.egg-info/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-09 20:45:35.000000 slurm-parallel-0.1.4/src/slurm_parallel.egg-info/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      468 2023-05-09 20:45:35.000000 slurm-parallel-0.1.4/src/slurm_parallel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-09 20:45:35.000000 slurm-parallel-0.1.4/src/slurm_parallel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       20 2023-05-09 20:45:35.000000 slurm-parallel-0.1.4/src/slurm_parallel.egg-info/requires.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-09 20:45:35.000000 slurm-parallel-0.1.4/src/slurm_parallel.egg-info/top_level.txt
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-09 20:45:36.122239 slurm-parallel-0.1.4/test/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1406 2023-05-09 20:44:49.000000 slurm-parallel-0.1.4/test/test.py
```

### Comparing `slurm-parallel-0.1.3/LICENSE` & `slurm-parallel-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.3/PKG-INFO` & `slurm-parallel-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.3/pyproject.toml` & `slurm-parallel-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slurm-parallel"
-version = "0.1.3"
+version = "0.1.4"
 description = "Easy parallelization of python functions on SLURM using job arrays."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
```

### Comparing `slurm-parallel-0.1.3/src/slurm_parallel/run.py` & `slurm-parallel-0.1.4/src/slurm_parallel/run.py`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.3/src/slurm_parallel/slurm.py` & `slurm-parallel-0.1.4/src/slurm_parallel/slurm.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,18 +20,36 @@
 
 from . import config, utils
 
 logger = logging.getLogger(__name__)
 run_script = resources.files('slurm_parallel').joinpath('run.sh')
 run_py_script = resources.files('slurm_parallel').joinpath('run.py')
 summarize_script = resources.files('slurm_parallel').joinpath('summarize.sh')
-# cleanup_script = resources.files('slurm_parallel').joinpath('cleanup.sh')
 
 allowed_args = {'A', 'account', 'acctg_freq', 'batch', 'bb', 'bbf', 'b', 'begin', 'D', 'chdir', 'cluster_constraint', 'M', 'clusters', 'comment', 'C', 'constraint', 'container', 'container_id', 'contiguous', 'S', 'core-spec', 'cores_per_socket', 'cpu_freq', 'cpus_per_gpu', 'c', 'cpus_per_task', 'deadline', 'delay_boot', 'd', 'dependency', 'm', 'distribution', 'e', 'error', 'x', 'exclude', 'exclusive', 'export', 'export_file', 'extra', 'B', 'extra_node_info', 'get_user_env', 'gid', 'gpu_bind', 'gpu_freq', 'G', 'gpus', 'gpus_per_node', 'gpus_per_socket', 'gpus_per_task', 'gres', 'gres_flags', 'h', 'help', 'hint', 'H', 'hold', 'ignore_pbs', 'i', 'input', 'J', 'job_name', 'kill_on_invalid_dep', 'L', 'licenses', 'mail_type', 'mail_user', 'mcs_label', 'mem', 'mem_bind', 'mem_per_cpu', 'mem_per_gpu', 'mincpus', 'network', 'nice', 'k', 'no_kill', 'no_requeue', 'F', 'nodefile', 'w', 'nodelist', 'N', 'nodes', 'n', 'ntasks', 'ntasks_per_core', 'ntasks_per_gpu', 'ntasks_per_node', 'ntasks_per_socket', 'open_mode', 'O', 'overcommit', 's', 'oversubscribe', 'p', 'partition', 'power', 'prefer', 'priority', 'profile', 'propagate', 'q', 'qos', 'Q', 'quiet', 'reboot', 'requeue', 'reservation', 'signal', 'sockets_per_node', 'spread_job', 'switches', 'test_only', 'thread_spec', 'threads_per_core', 't', 'time', 'time_min', 'tmp', 'tres_per_task', 'uid', 'usage', 'use_min_nodes', 'v', 'verbose', 'V', 'version', 'wait_all_nodes', 'wckey', 'wrap'}
 
+# See https://slurm.schedmd.com/sacct.html#SECTION_JOB-STATE-CODES
+STATE_CODES = [
+    'BOOT_FAIL',
+    'CANCELLED',
+    'COMPLETED',
+    'DEADLINE',
+    'FAILED',
+    'NODE_FAIL',
+    'OUT_OF_MEMORY',
+    'PENDING',
+    'PREEMPTED',
+    'RUNNING',
+    'REQUEUED',
+    'RESIZING',
+    'REVOKED',
+    'SUSPENDED',
+    'TIMEOUT',
+]
+
 __all__ = ['parallelize']
 
 class StringTemplate(Template):
     delimiter = '%'
     idpattern = "(?a-i:[sF])" # ASCII-only, don't ignore case
 
 @lib.functools.parametrized
@@ -159,91 +177,42 @@
                         match = re.search('Submitted batch job ([0-9]{6})', line)
                         if match is not None:
                             run_PID = match.group(1)
                             break
 
                     logger.info(f'Submitted batch job {run_PID} for {pathlib.Path(filename).stem}.{funcname}')
 
-                    n = 0
+                    t0, n_completed = 0, 0
                     with tqdm(total=n_tasks) as t:
                         while True:
-                            summary = subprocess.run([summarize_script, run_PID], capture_output=True, check=True, text=True)
-                            n_completed = summary.stdout.count('COMPLETED')
-                            n_failed = summary.stdout.count('FAILED')
-                            n_running = summary.stdout.count('RUNNING')
-
-                            t.update(n=(n_completed + n_failed - n))
-                            t.set_postfix(n_completed=n_completed, n_failed=n_failed, n_running=n_running)
-
-                            n = n_completed + n_failed
-
-                            if n >= n_tasks:
-                                break
+                            if (p.poll() is not None) or (time.time() - t0 > progress_dt):
+                                summary = subprocess.run([summarize_script, run_PID], capture_output=True, check=True, text=True)
+                                state_info = {k.lower(): summary.stdout.count(k) for k in STATE_CODES}
+
+                                t.update(n=(state_info['completed'] - n_completed))
+                                n_completed = state_info.pop('completed')
+                                t.set_postfix({k: v for k, v in state_info.items() if v > 0})
+                                
+                                if p.poll() is not None:
+                                    break
+                                    
+                                t0 = time.time()
 
-                            time.sleep(progress_dt)
+                    if p.returncode != 0:
+                        raise subprocess.CalledProcessError(p.returncode, p.args)
                             
-                if p.returncode != 0:
-                    raise subprocess.CalledProcessError(p.returncode, p.args)
-                    
             except Exception as err:
                 raise err
                 
             else:
                 success = True
                 
             finally:
                 if not success:
                     subprocess.run(['scancel', run_PID], check=True)
                     logger.info(f"Ensured batch job {run_PID} for {pathlib.Path(filename).stem}.{funcname} is cancelled.")
-            
-        
-#         try:
-#             with tempfile.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False) as f:
-#                 json.dump(configs, f)
-                
-#             tmp_filename = f.name
-#             logger.info(f"Saved configs to tmp file {tmp_filename}.")
-            
-#             args = ["sbatch", *run_options, run_script, run_py_script, filename, funcname, tmp_filename, *logging_options]
-#             logger.debug(f"Invoking subprocess with arguments {args}")
-            
-#             completed_process = subprocess.run(args, capture_output=not wait, check=True)
-            
-#             if wait:
-#                 pathlib.Path(tmp_filename).unlink(missing_ok=True)
-#                 logger.info(f"{tmp_filename} removed")
-                
-#             else:
-#                 run_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
-#                 print(f"Submitted batch job {run_PID}")
-            
-#                 cleanup_kwargs = {
-#                     'c': 1,
-#                     'mem_per_cpu': '1mb',
-#                     'time': 1, # 1 minute
-#                     'dependency': f'afterany:{run_PID}',
-#                     'output': out_dir / "cleanup.out",
-#                     'parsable': True,
-#                     'job_name': f'{pathlib.Path(filename).stem}_{funcname}_cleanup',
-#                 }
-#                 cleanup_options = utils.to_cmd_options(**cleanup_kwargs)
-
-#                 args = ["sbatch", *cleanup_options, cleanup_script, tmp_filename]
-#                 logger.debug(f"Invoking subprocess with arguments {args}")
-                
-#                 completed_process = subprocess.run(args, capture_output=True, check=True)
-                
-#                 cleanup_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
-#                 logger.debug(f"Submitted cleanup batch job with job ID {cleanup_PID}")
-                
-#                 return run_PID
-            
-#         except Exception as err:
-#             pathlib.Path(tmp_filename).unlink(missing_ok=True)
-#             logger.info(f"{tmp_filename} removed")
-#             raise err
     
     func.run_task = run_task
     func.remote = remote
     
     return func
```

### Comparing `slurm-parallel-0.1.3/src/slurm_parallel/utils.py` & `slurm-parallel-0.1.4/src/slurm_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.3/src/slurm_parallel.egg-info/PKG-INFO` & `slurm-parallel-0.1.4/src/slurm_parallel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.3/test/test.py` & `slurm-parallel-0.1.4/test/test.py`

 * *Files identical despite different names*

