# Comparing `tmp/RepRepBuild-0.7.2.tar.gz` & `tmp/RepRepBuild-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.7.2.tar", last modified: Thu Apr 27 13:55:20 2023, max compression
+gzip compressed data, was "RepRepBuild-0.7.3.tar", last modified: Wed May 10 14:56:01 2023, max compression
```

## Comparing `RepRepBuild-0.7.2.tar` & `RepRepBuild-0.7.3.tar`

### file list

```diff
@@ -1,26 +1,37 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.466222 RepRepBuild-0.7.2/
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.7.2/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-27 13:55:20.465222 RepRepBuild-0.7.2/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.7.2/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-27 13:54:45.000000 RepRepBuild-0.7.2/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-27 13:55:20.466222 RepRepBuild-0.7.2/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.448222 RepRepBuild-0.7.2/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.449222 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-27 13:55:20.000000 RepRepBuild-0.7.2/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-27 13:55:20.464222 RepRepBuild-0.7.2/src/reprepbuild/
--rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.7.2/src/reprepbuild/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)    11425 2023-04-27 13:39:02.000000 RepRepBuild-0.7.2/src/reprepbuild/__main__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.7.2/src/reprepbuild/articlezip.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.7.2/src/reprepbuild/bibtex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.7.2/src/reprepbuild/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4530 2023-04-19 14:02:59.000000 RepRepBuild-0.7.2/src/reprepbuild/latexdep.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.7.2/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4119 2023-04-19 09:59:27.000000 RepRepBuild-0.7.2/src/reprepbuild/pythonscript.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.7.2/src/reprepbuild/repeat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5130 2023-04-19 15:07:08.000000 RepRepBuild-0.7.2/src/reprepbuild/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.7.2/src/reprepbuild/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.937506 RepRepBuild-0.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.937506 RepRepBuild-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.933506 RepRepBuild-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.941506 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:56:01.945506 RepRepBuild-0.7.3/src/reprepbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 14:56:01.000000 RepRepBuild-0.7.3/src/reprepbuild/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/articlezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/latexdep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-10 14:55:49.000000 RepRepBuild-0.7.3/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.7.2/COPYING` & `RepRepBuild-0.7.3/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/PKG-INFO` & `RepRepBuild-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.2
+Version: 0.7.3
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,15 +690,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # RepRepBuild
 
 RepRepBuild is the build tool for [Reproducible Reporting](https://github.com/reproducible-reporting).
 Run `rr` in a source directory, and the publication will be rebuilt from its source.
```

### Comparing `RepRepBuild-0.7.2/README.md` & `RepRepBuild-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/pyproject.toml` & `RepRepBuild-0.7.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
-requires = ["setuptools>=65.0"]
+requires = ["setuptools>=65.0", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepRepBuild"
-version = "0.7.2"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Build tool for Reproducible Reporting"
 readme = "README.md"
 license = {file = "COPYING"}
-requires-python = ">=3.6"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "Framework :: Matplotlib",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -30,14 +29,15 @@
 dependencies = [
     "ninja",
     "pymupdf",
     "tqdm",
     "watchdog",
     "bibsane",
 ]
+dynamic = ["version"]
 
 [project.urls]
 Issues = "https://github.com/reproducible-reporting/reprepbuild/issues"
 Source = "https://github.com/reproducible-reporting/reprepbuild/"
 Changelog = "https://github.com/reproducible-reporting/reprepbuild/blob/main/CHANGELOG.md"
 
 [project.scripts]
@@ -46,7 +46,22 @@
 rr-zip = "reprepbuild.zip:main"
 rr-article-zip = "reprepbuild.articlezip:main"
 rr-latexdep = "reprepbuild.latexdep:main"
 rr-bibtex = "reprepbuild.bibtex:main"
 rr-latex = "reprepbuild.latex:main"
 rr-python-script = "reprepbuild.pythonscript:main"
 rr-normalize-pdf = "reprepbuild.normalizepdf:main"
+
+[tool.black]
+line-length = 100
+target-version = ['py310']
+
+[tool.ruff]
+select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF"]
+line-length = 100
+target-version = "py310"
+ignore = ["PLR2004", "PLR0913", "PLR0912", "PLW2901", "PLR0915"]
+
+[tool.setuptools_scm]
+write_to = "src/reprepbuild/_version.py"
+version_scheme = "post-release"
+local_scheme = "no-local-version"
```

### Comparing `RepRepBuild-0.7.2/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.7.3/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.2
+Version: 0.7.3
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,15 +690,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # RepRepBuild
 
 RepRepBuild is the build tool for [Reproducible Reporting](https://github.com/reproducible-reporting).
 Run `rr` in a source directory, and the publication will be rebuilt from its source.
```

### Comparing `RepRepBuild-0.7.2/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.7.3/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+.editorconfig
+.gitignore
+.pre-commit-config.yaml
+CHANGELOG.md
 COPYING
+DEVELOPMENT.md
+HEADER
 README.md
 pyproject.toml
+.github/dependabot.yaml
+.github/workflows/pypi.yaml
 src/RepRepBuild.egg-info/PKG-INFO
 src/RepRepBuild.egg-info/SOURCES.txt
 src/RepRepBuild.egg-info/dependency_links.txt
 src/RepRepBuild.egg-info/entry_points.txt
 src/RepRepBuild.egg-info/requires.txt
 src/RepRepBuild.egg-info/top_level.txt
 src/reprepbuild/__init__.py
 src/reprepbuild/__main__.py
+src/reprepbuild/_version.py
 src/reprepbuild/articlezip.py
 src/reprepbuild/bibtex.py
 src/reprepbuild/latex.py
 src/reprepbuild/latexdep.py
 src/reprepbuild/normalizepdf.py
 src/reprepbuild/pythonscript.py
 src/reprepbuild/repeat.py
```

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/__init__.py` & `RepRepBuild-0.7.3/HEADER`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/__main__.py` & `RepRepBuild-0.7.3/src/reprepbuild/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         "default": True,
     }
 
 
 def python_script_pattern(path):
     """Make ninja build commands for python scripts."""
     # for any valid python file
-    if not re.match(r"(?P<name>results-[a-z0-9-]*/[a-zA-Z0-9/_-]*).py$", path):
+    if not re.match(r"(?P<name>results(-[a-z0-9_-]*)?/[a-zA-Z0-9/_-]*).py$", path):
         return
 
     # Call reprepbuild_info as if the script is running in its own directory.
     orig_workdir = os.getcwd()
     workdir, fn_py = os.path.split(path)
     prefix = fn_py[:-3]
     try:
@@ -329,12 +329,12 @@
 
 
 def main():
     """Main program."""
     sanity_check()
     args = parse_args()
     write_ninja(DEFAULT_PATTERNS, DEFAULT_RULES)
-    subprocess.run(["ninja"] + args)
+    subprocess.run(["ninja", *args])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/articlezip.py` & `RepRepBuild-0.7.3/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/bibtex.py` & `RepRepBuild-0.7.3/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/latex.py` & `RepRepBuild-0.7.3/src/reprepbuild/latex.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 """
 
 import argparse
 import os
 import re
 import subprocess
 import sys
+from itertools import islice
 
 
 def main():
     """Main program."""
     args = parse_args()
     return compile_latex(args.path_tex)
 
@@ -67,15 +68,15 @@
     if os.environ.get("SOURCE_DATE_EPOCH") != "315532800":
         print("SOURCE_DATE_EPOCH is not set to 315532800.")
         return 3
 
     # Compile the LaTeX source with pdflatex, until converged, max three times
     args = ["pdflatex", "-interaction=nonstopmode", "-recorder", "-file-line-error", fn_tex]
     path_log = os.path.join(workdir, prefix + ".log")
-    for irep in range(4):
+    for _irep in range(4):
         found_error = False
         rerun = False
         try:
             subprocess.run(
                 args,
                 cwd=workdir,
                 check=True,
@@ -99,15 +100,15 @@
                     if b"Rerun to" in line:
                         rerun = True
                         break
                 if found_error:
                     # stdout tricks to dump the raw contents on the terminal.
                     sys.stdout.flush()
                     sys.stdout.buffer.write(b"        " + line)
-                    for line, _ in zip(f, range(4)):
+                    for line in islice(f, 4):
                         sys.stdout.buffer.write(b"        " + line)
                     print(f"    See {path_log} for more details.")
                     return 1
 
         if not rerun:
             break
```

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/latexdep.py` & `RepRepBuild-0.7.3/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.7.3/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.7.3/src/reprepbuild/pythonscript.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/repeat.py` & `RepRepBuild-0.7.3/src/reprepbuild/repeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     try:
         while True:
             if not event_handler.changed:
                 time.sleep(1)
                 continue
             event_handler.snooze()
             write_ninja(DEFAULT_PATTERNS, DEFAULT_RULES)
-            subprocess.run(["ninja"] + args)
+            subprocess.run(["ninja", *args])
             time.sleep(0.1)
             event_handler.reset()
             print("  Waiting for new changes.")
     except KeyboardInterrupt:
         print("  See you!")
     finally:
         observer.stop()
```

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/utils.py` & `RepRepBuild-0.7.3/src/reprepbuild/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,23 +120,23 @@
 
 def import_python_path(path):
     """Return a module by importing a Python file at a given path."""
     spec = importlib.util.spec_from_file_location("<pythonscript>", path)
     module = importlib.util.module_from_spec(spec)
     try:
         spec.loader.exec_module(module)
-    except Exception as e:
+    except Exception:
         # Ignore the script if it cannot be imported correctly.
         return None
     return module
 
 
 def check_script_args(script_args):
     for script_arg in script_args:
         if isinstance(script_arg, str):
             if not re.match(r"^[a-zA-Z0-9_-]*$", script_arg):
                 raise ValueError(
                     "Script argument must only contain letters, numbers, underscores, and hyphens."
                 )  # E:lin101
-        elif not isinstance(script_arg, (int, float)):
+        elif not isinstance(script_arg, int | float):
             raise TypeError("A script argument must be int, float or str.")
     return "".join(f"_{script_arg}" for script_arg in script_args)
```

### Comparing `RepRepBuild-0.7.2/src/reprepbuild/zip.py` & `RepRepBuild-0.7.3/src/reprepbuild/zip.py`

 * *Files identical despite different names*

