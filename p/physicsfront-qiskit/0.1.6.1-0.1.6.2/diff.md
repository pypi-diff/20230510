# Comparing `tmp/physicsfront-qiskit-0.1.6.1.tar.gz` & `tmp/physicsfront-qiskit-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsfront-qiskit-0.1.6.1.tar", last modified: Mon May  8 20:18:29 2023, max compression
+gzip compressed data, was "physicsfront-qiskit-0.1.6.2.tar", last modified: Wed May 10 02:18:35 2023, max compression
```

## Comparing `physicsfront-qiskit-0.1.6.1.tar` & `physicsfront-qiskit-0.1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 20:18:29.318709 physicsfront-qiskit-0.1.6.1/
--rw-rw-r--   0 gweon     (1000) gweon     (1000)    11357 2023-01-14 17:25:03.000000 physicsfront-qiskit-0.1.6.1/LICENSE
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     1259 2023-05-08 20:18:29.318709 physicsfront-qiskit-0.1.6.1/PKG-INFO
--rw-rw-r--   0 gweon     (1000) gweon     (1000)      452 2023-01-30 19:55:11.000000 physicsfront-qiskit-0.1.6.1/README.md
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 20:18:29.318709 physicsfront-qiskit-0.1.6.1/physicsfront/
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 20:18:29.318709 physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/
--rw-rw-r--   0 gweon     (1000) gweon     (1000)    36178 2023-05-08 18:47:42.000000 physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/__init__.py
--rw-rw-r--   0 gweon     (1000) gweon     (1000)      975 2023-05-06 19:09:30.000000 physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/_requires.py
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     8963 2023-05-08 20:08:39.000000 physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/colab.py
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     5774 2023-01-30 01:36:22.000000 physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/patch.py
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 20:18:29.318709 physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     1259 2023-05-08 20:18:29.000000 physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/PKG-INFO
--rw-rw-r--   0 gweon     (1000) gweon     (1000)      363 2023-05-08 20:18:29.000000 physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/SOURCES.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)        1 2023-05-08 20:18:29.000000 physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/dependency_links.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)       84 2023-05-08 20:18:29.000000 physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/requires.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)       13 2023-05-08 20:18:29.000000 physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/top_level.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)       38 2023-05-08 20:18:29.318709 physicsfront-qiskit-0.1.6.1/setup.cfg
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     4285 2023-05-08 20:18:07.000000 physicsfront-qiskit-0.1.6.1/setup.py
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-10 02:18:35.628829 physicsfront-qiskit-0.1.6.2/
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)    11357 2023-01-14 17:25:03.000000 physicsfront-qiskit-0.1.6.2/LICENSE
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     1259 2023-05-10 02:18:35.628829 physicsfront-qiskit-0.1.6.2/PKG-INFO
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)      452 2023-01-30 19:55:11.000000 physicsfront-qiskit-0.1.6.2/README.md
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-10 02:18:35.628829 physicsfront-qiskit-0.1.6.2/physicsfront/
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-10 02:18:35.628829 physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)    36908 2023-05-09 03:56:27.000000 physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/__init__.py
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)      975 2023-05-06 19:09:30.000000 physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/_requires.py
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     9731 2023-05-10 02:06:43.000000 physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/colab.py
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     5774 2023-01-30 01:36:22.000000 physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/patch.py
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-10 02:18:35.628829 physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     1259 2023-05-10 02:18:35.000000 physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/PKG-INFO
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)      363 2023-05-10 02:18:35.000000 physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)        1 2023-05-10 02:18:35.000000 physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)       84 2023-05-10 02:18:35.000000 physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/requires.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)       13 2023-05-10 02:18:35.000000 physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/top_level.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)       38 2023-05-10 02:18:35.628829 physicsfront-qiskit-0.1.6.2/setup.cfg
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     4285 2023-05-10 02:16:17.000000 physicsfront-qiskit-0.1.6.2/setup.py
```

### Comparing `physicsfront-qiskit-0.1.6.1/LICENSE` & `physicsfront-qiskit-0.1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsfront-qiskit-0.1.6.1/PKG-INFO` & `physicsfront-qiskit-0.1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsfront-qiskit
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: Utility package for qiskit
 Home-page: https://github.com/sam-pf/pf-qiskit
 Author: Physics Front LLC
 Author-email: info@physicsfront.com
 License: Apache 2.0
 Project-URL: GitHub, https://github.com/sam-pf/pf-qiskit
 Platform: Posix; MacOS X; Windows
```

### Comparing `physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/__init__.py` & `physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,15 +740,15 @@
 def jobs_monitor (jobs, interval = None, # <<< # pylint: disable=W0621
                   quiet = False, job_id_minlen = 6,
                   line_discipline = "\r", output = None):
     """
     A bit like of qiskit.tools.monitor.job_monitor, but for an iterable of
     jobs, instead of a single job.
     """
-    import sys, time
+    import datetime, sys, time
     if interval is None:
         interval = 5
     assert type (interval) is int and interval >= 1
     assert type (job_id_minlen) is int and job_id_minlen >= 4
     assert type (line_discipline) is str
     if output is None:
         output = sys.stderr
@@ -761,25 +761,41 @@
     while True:
         job_ids_short = list (j [:job_id_minlen] for j in job_ids)
         if len (set (job_ids_short)) == n_jobs:
             break
         job_id_minlen += 2
     all_ended = False
     msg_len = 0
+    loop_count = 0
     while True:
+        loop_count += 1
         all_ended = True
         for i, job in enumerate (jobs):
             if states [i] in ended:
                 continue
             status = job.status ()
             state = status.name
             if state == 'QUEUED':
-                queue_position = job.queue_position ()
+                queue_position = job.queue_position (refresh = loop_count %
+                                                     10 == 0)
                 if queue_position is not None:
-                    state += f'({queue_position})'
+                    state += f'({queue_position}' # )
+                    ect = job.queue_info ()
+                    if ect is not None:
+                        ect = ect.estimated_complete_time
+                    if ect:
+                        # add estimated time information
+                        tz = ect.tzinfo
+                        dt = ect - datetime.datetime.now (tz)
+                        dt_s = str (dt)
+                        dotpos = dt_s.rfind ('.')
+                        if dotpos > 0:
+                            dt_s = dt_s [: dotpos]
+                        state += f'; {dt_s}' # (
+                    state += ')'
             states [i] = state
             all_ended = False
         msg = (f'Status for {n_jobs} job{"s" if n_jobs > 1 else ""}: ' +
             ', '.join (':'.join ([job_id_short, state])
                 for job_id_short, state in zip (job_ids_short, states)))
         lendiff = msg_len - len (msg)
         if lendiff > 0:
```

### Comparing `physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/_requires.py` & `physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/_requires.py`

 * *Files identical despite different names*

### Comparing `physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/colab.py` & `physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/colab.py`

 * *Files 15% similar despite different names*

```diff
@@ -157,48 +157,66 @@
     # deprecated.  As of 2023-05-07, it has been noted that the jobs executed
     # in the last couple of days do not show up, if the job query is made
     # from the deprecated provider.  They do show up if the job query is made
     # from a provider of new type, which is recommended for use.  So, it is
     # time to move on to the new style.
     ##
     if not quiet:
-        print ("== Account setup (you might be prompted for an API TOKEN) ...",
-               end = ' ', flush = True)
+        print ("== Account setup (you may be prompted for an API TOKEN) ...")
     from . import get_provider
     provider = get_provider (provider = 'cached', instance = instance)
     if provider and not reload:
         if not quiet:
-            print ("OK! (account already active; reload not requested)\n"
-                "   Restart runtime if you wish to restart everything anew.")
+            print (
+'''   Account is active already and reload was not requested.
+   Restart runtime if you wish to restart everything anew.''')
         return
     _, rv = _check_setup_file ('json', fallback_filename = filename)
-    if rv:
+    if rv and False: # temporary
         provider = get_provider (provider = 'renew' if reload else None,
                                  instance = instance)
     else:
-        old_token = '' # d ['token'] if d else ''
-        import IPython # pylint: disable=E0401
-        display = IPython.display.display
-        from google.colab import output # pylint: disable=E0401,E0611
-        display (IPython.display.Javascript (f'window._key = "{old_token}"'))
-        display (IPython.display.Javascript ('''
-window._key = prompt ("Please enter your IBM Quantum API TOKEN:", window._key)
-        '''))
-        token = output.eval_js ('_key')
+        ##
+        # This code based on 'prompt' deos not work for chrome (works for
+        # firefox though).  In chrome, the 'prompt' part does nothing, while
+        # there is no message of any kind.
+        #
+        #old_token = '' # d ['token'] if d else ''
+        #import IPython # pylint: disable=E0401
+        #display = IPython.display.display
+        #from google.colab import output # pylint: disable=E0401,E0611
+        #display (IPython.display.Javascript (f'window._key = "{old_token}"'))
+        #display (IPython.display.Javascript ('''
+#window._key = prompt ("Please enter your IBM Quantum API TOKEN:", window._key)
+        #'''))
+        #token = output.eval_js ('_key')
         # for safety; even if javascript is sandboxed per cell
-        output.eval_js ('delete window._key')
+        #output.eval_js ('delete window._key')
+        ##
+        import getpass
+        print ("   Paste your IBM Quantum API token and then hit Enter.")
+        token = getpass.getpass ("   Your IBM Quantum API token: ")
+        # Be tolerant about copy-paste mistake up to partial quotation marks.
+        if token.startswith ("'"):
+            token = token [1:]
+            if token.endswith ("'"):
+                token = token [:-1]
+        elif token.startswith ('"'):
+            token = token [1:]
+            if token.endswith ('"'):
+                token = token [:-1]
         provider = get_provider (token = token, instance = instance)
     if not provider:
         raise Exception ("Failed to set up an IBM Quantum provider.") # pylint: disable=W0719
     if not rv:
         dargs = provider.active_account ()
         dargs.pop ('channel', None)
         provider.save_account (** dargs)
     if not quiet:
-        print ("OK!")
+        print ("   Your account is successfully set up!")
 # >>>
 def _setup_settings (reload = False, quiet = False, filename = None): # <<<
     if not quiet:
         print ("== Qiskit settings file check ...", end = ' ', flush = True)
     setupfname, rv = _check_setup_file ('conf', fallback_filename = filename)
     msg = ''
     if rv:
```

### Comparing `physicsfront-qiskit-0.1.6.1/physicsfront/qiskit/patch.py` & `physicsfront-qiskit-0.1.6.2/physicsfront/qiskit/patch.py`

 * *Files identical despite different names*

### Comparing `physicsfront-qiskit-0.1.6.1/physicsfront_qiskit.egg-info/PKG-INFO` & `physicsfront-qiskit-0.1.6.2/physicsfront_qiskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsfront-qiskit
-Version: 0.1.6.1
+Version: 0.1.6.2
 Summary: Utility package for qiskit
 Home-page: https://github.com/sam-pf/pf-qiskit
 Author: Physics Front LLC
 Author-email: info@physicsfront.com
 License: Apache 2.0
 Project-URL: GitHub, https://github.com/sam-pf/pf-qiskit
 Platform: Posix; MacOS X; Windows
```

### Comparing `physicsfront-qiskit-0.1.6.1/setup.py` & `physicsfront-qiskit-0.1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 author = "Physics Front LLC"
 author_email = "info@physicsfront.com"
 url = "https://github.com/sam-pf/pf-qiskit"
 project_urls = {
     'GitHub': url,
     # potential useful keys: 'Documentation', 'ChangeLog', 'Issues', ...
 }
-version = "0.1.6.1"
+version = "0.1.6.2"
 license_ = "Apache 2.0"
 description = "Utility package for qiskit"
 long_description = "This package provides modules such as physicsfront.qiskit and physicsfront.qiskit.colab.  These modules can be used to aid the usage of qiskit in various environments, e.g., in the Google Colab environment."
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
```

