# Comparing `tmp/simple-git-versioning-0.0.3.tar.gz` & `tmp/simple-git-versioning-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-git-versioning-0.0.3.tar", last modified: Sun Feb  5 23:21:01 2023, max compression
+gzip compressed data, was "simple-git-versioning-0.0.4.tar", last modified: Sun Feb  5 23:21:57 2023, max compression
```

## Comparing `simple-git-versioning-0.0.3.tar` & `simple-git-versioning-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:01.678623 simple-git-versioning-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4677 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-05 23:21:01.678623 simple-git-versioning-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/Pipfile.lock
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-05 23:21:01.679623 simple-git-versioning-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:01.676623 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-05 23:21:01.000000 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2023-02-05 23:21:01.000000 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-05 23:21:01.000000 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-02-05 23:21:01.000000 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-05 23:21:01.000000 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-05 23:21:01.000000 simple-git-versioning-0.0.3/simple_git_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:01.677623 simple-git-versioning-0.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:01.677623 simple-git-versioning-0.0.3/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6464 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/tests/unit/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:01.678623 simple-git-versioning-0.0.3/versioning/
--rw-rw-rw-   0 root         (0) root         (0)     3323 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/versioning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-05 23:20:45.000000 simple-git-versioning-0.0.3/versioning/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.839543 simple-git-versioning-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4677 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      887 2023-02-05 23:21:57.839543 simple-git-versioning-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-05 23:21:57.840460 simple-git-versioning-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.837710 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      455 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-02-05 23:21:57.000000 simple-git-versioning-0.0.4/simple_git_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.838626 simple-git-versioning-0.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.838626 simple-git-versioning-0.0.4/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6274 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/tests/unit/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-05 23:21:57.839543 simple-git-versioning-0.0.4/versioning/
+-rw-rw-rw-   0 root         (0) root         (0)     3323 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/versioning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-05 23:21:41.000000 simple-git-versioning-0.0.4/versioning/__main__.py
```

### Comparing `simple-git-versioning-0.0.3/.gitlab-ci.yml` & `simple-git-versioning-0.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.0.3/LICENSE` & `simple-git-versioning-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.0.3/PKG-INFO` & `simple-git-versioning-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.0.3
+Version: 0.0.4
 Summary: Thinly scoped and opinionated project that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `simple-git-versioning-0.0.3/Pipfile.lock` & `simple-git-versioning-0.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.0.3/pyproject.toml` & `simple-git-versioning-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.0.3/simple_git_versioning.egg-info/PKG-INFO` & `simple-git-versioning-0.0.4/simple_git_versioning.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.0.3
+Version: 0.0.4
 Summary: Thinly scoped and opinionated project that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `simple-git-versioning-0.0.3/tests/unit/test_version.py` & `simple-git-versioning-0.0.4/tests/unit/test_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 import pytest
 from packaging.version import Version
 from sh.contrib import git
 from versioning import version
 
-from . import tmpdir
+from . import gitdir, tmpdir
 
 
 def _format_commit_message(message: str) -> str:
     return "\n".join(map(str.strip, message.strip().split("\n")))
 
 
 def test_project_s_version_is_set():
@@ -22,31 +22,28 @@
 
 def test_version_not_in_git_repository(tmpdir):
     os.chdir(tmpdir)
     with pytest.raises(RuntimeError, match="not a git work tree"):
         version()
 
 
-def test_version_default(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_default(gitdir):
+    os.chdir(gitdir)
     assert version() == Version("0.0.0")
 
 
-def test_version_at_tag(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_at_tag(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     assert version() == Version("1.0.0")
 
 
-def test_version_patch(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_patch(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -55,17 +52,16 @@
             ci-version-bump: patch
             """
         ),
     )
     assert version() == Version("1.0.1")
 
 
-def test_version_minor(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_minor(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -74,17 +70,16 @@
             ci-version-bump: minor
             """
         ),
     )
     assert version() == Version("1.1.0")
 
 
-def test_version_major(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_major(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -93,17 +88,16 @@
             ci-version-bump: major
             """
         ),
     )
     assert version() == Version("2.0.0")
 
 
-def test_version_major_minor_patch(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_major_minor_patch(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -134,17 +128,16 @@
             ci-version-bump: patch
             """
         ),
     )
     assert version() == Version("2.1.1")
 
 
-def test_version_patch_minor_major(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_patch_minor_major(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -175,17 +168,16 @@
             ci-version-bump: major
             """
         ),
     )
     assert version() == Version("2.0.0")
 
 
-def test_version_patch_minor(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_patch_minor(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -205,28 +197,26 @@
             ci-version-bump: minor
             """
         ),
     )
     assert version() == Version("1.1.0")
 
 
-def test_version_default_bump_is_patch(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_default_bump_is_patch(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit("--allow-empty", "--message", "lorem ipsum dolor sit amet")
     git.commit("--allow-empty", "--message", "lorem ipsum dolor sit amet")
     git.commit("--allow-empty", "--message", "lorem ipsum dolor sit amet")
     assert version() == Version("1.0.3")
 
 
-def test_version_ignores_unrelated_trailers(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_ignores_unrelated_trailers(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
@@ -237,17 +227,16 @@
             Change-type: major
             """
         ),
     )
     assert version() == Version("1.0.1")
 
 
-def test_version_typos_in_trailer_values_get_caught(tmpdir):
-    os.chdir(tmpdir)
-    git.init(".")
+def test_version_typos_in_trailer_values_get_caught(gitdir):
+    os.chdir(gitdir)
     git.commit("--allow-empty", "--message", "initial empty commit")
     git.tag("--annotate", "--message", "version 1.0.0", "1.0.0")
     git.commit(
         "--allow-empty",
         "--message",
         _format_commit_message(
             """
```

### Comparing `simple-git-versioning-0.0.3/versioning/__init__.py` & `simple-git-versioning-0.0.4/versioning/__init__.py`

 * *Files identical despite different names*

