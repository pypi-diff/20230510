# Comparing `tmp/WinTraceroute-1.1.2.tar.gz` & `tmp/WinTraceroute-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.1.2.tar", last modified: Sat Apr 29 13:10:45 2023, max compression
+gzip compressed data, was "WinTraceroute-1.3.0.tar", last modified: Tue May  9 22:49:36 2023, max compression
```

## Comparing `WinTraceroute-1.1.2.tar` & `WinTraceroute-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:10:45.698981 WinTraceroute-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-29 13:09:56.000000 WinTraceroute-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-29 13:10:45.698981 WinTraceroute-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-29 13:09:56.000000 WinTraceroute-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:10:45.694980 WinTraceroute-1.1.2/WinTraceroute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-29 13:10:45.000000 WinTraceroute-1.1.2/WinTraceroute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-29 13:10:45.000000 WinTraceroute-1.1.2/WinTraceroute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:10:45.000000 WinTraceroute-1.1.2/WinTraceroute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 13:10:45.000000 WinTraceroute-1.1.2/WinTraceroute.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 13:10:45.000000 WinTraceroute-1.1.2/WinTraceroute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 13:10:45.000000 WinTraceroute-1.1.2/WinTraceroute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-29 13:09:56.000000 WinTraceroute-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:10:45.698981 WinTraceroute-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:10:45.694980 WinTraceroute-1.1.2/traceroute/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:09:56.000000 WinTraceroute-1.1.2/traceroute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-29 13:09:56.000000 WinTraceroute-1.1.2/traceroute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-29 13:09:56.000000 WinTraceroute-1.1.2/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 22:49:36.000000 WinTraceroute-1.3.0/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:49:36.619582 WinTraceroute-1.3.0/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-09 22:49:11.000000 WinTraceroute-1.3.0/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.1.2/LICENSE` & `WinTraceroute-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.1.2/PKG-INFO` & `WinTraceroute-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.1.2
+Version: 1.3.0
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -344,10 +344,10 @@
         Public License instead of this License.
         
 Project-URL: Homepage, https://github.com/NiRit100/WinTraceroute
 Keywords: traceroute,tracert,network,routing,scapy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `WinTraceroute-1.1.2/WinTraceroute.egg-info/PKG-INFO` & `WinTraceroute-1.3.0/WinTraceroute.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.1.2
+Version: 1.3.0
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -344,10 +344,10 @@
         Public License instead of this License.
         
 Project-URL: Homepage, https://github.com/NiRit100/WinTraceroute
 Keywords: traceroute,tracert,network,routing,scapy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `WinTraceroute-1.1.2/pyproject.toml` & `WinTraceroute-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.1.2"
+version = "1.3.0"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
 ]
 keywords = ["traceroute", "tracert", "network", "routing", "scapy"]
 dependencies = [
     "scapy==2.5.0"
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.1.2"
+current_version = "1.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
```

### Comparing `WinTraceroute-1.1.2/traceroute/traceroute.py` & `WinTraceroute-1.3.0/traceroute/traceroute.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                 else:
                     print(time_str_format.format(time) + '\t', end='', file=PRINT_FILE)
             else:
                 print(' '*time_str_width + '\t', end='', file=PRINT_FILE)
         print(host, file=PRINT_FILE)
         is_first_line = False
 
-def is_dest_reached(responses:list[tuple[SndRcvList,PacketList]], dest):
+def is_dest_reached(responses:list, dest):
     for rt in responses:
         if rt == None:
             continue
         else:
             rt_icmp = rt[ICMP]
             if rt_icmp.type == 3 or rt.src == dest:
                 return True  # Dest unreachable, port unavailable
```

