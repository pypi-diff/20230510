# Comparing `tmp/sunpy-sphinx-theme-1.2.8.tar.gz` & `tmp/sunpy-sphinx-theme-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunpy-sphinx-theme-1.2.8.tar", last modified: Wed May 29 12:18:08 2019, max compression
+gzip compressed data, was "dist/sunpy-sphinx-theme-1.2.9.tar", last modified: Tue Aug 20 21:15:54 2019, max compression
```

## Comparing `sunpy-sphinx-theme-1.2.8.tar` & `sunpy-sphinx-theme-1.2.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/.circleci/
--rw-r--r--   0 root         (0) root         (0)     1838 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/.github/
--rw-r--r--   0 root         (0) root         (0)      551 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/.github/main.workflow
--rw-r--r--   0 root         (0) root         (0)     1176 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)      177 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/.stylelintrc
--rw-r--r--   0 root         (0) root         (0)      181 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     1330 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      207 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      591 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      818 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/
--rw-r--r--   0 root         (0) root         (0)      276 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/
--rw-r--r--   0 root         (0) root         (0)      789 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/docsidebar.html
--rw-r--r--   0 root         (0) root         (0)     1734 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/footer.html
--rw-r--r--   0 root         (0) root         (0)     1373 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/layout.html
--rw-r--r--   0 root         (0) root         (0)     2150 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/navbar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/
--rw-r--r--   0 root         (0) root         (0)     2915 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/copybutton.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/
--rw-r--r--   0 root         (0) root         (0)     5430 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/favicon-32.ico
--rw-r--r--   0 root         (0) root         (0)    10706 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/numfocus-logo.svg
--rw-r--r--   0 root         (0) root         (0)   187674 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/sunpy-bg.jpg
--rw-r--r--   0 root         (0) root         (0)    15707 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/sunpy_icon.svg
--rw-r--r--   0 root         (0) root         (0)    11016 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/sunpy_style.css
--rw-r--r--   0 root         (0) root         (0)      165 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/version.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/
--rw-r--r--   0 root         (0) root         (0)      127 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/attribute.rst
--rw-r--r--   0 root         (0) root         (0)      862 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/class.rst
--rw-r--r--   0 root         (0) root         (0)      124 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/member.rst
--rw-r--r--   0 root         (0) root         (0)      124 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/method.rst
--rw-r--r--   0 root         (0) root         (0)      111 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/minimal_module.rst
--rw-r--r--   0 root         (0) root         (0)      554 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/theme.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      591 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1225 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2019-05-29 12:18:08.000000 sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      345 2019-05-29 12:17:43.000000 sunpy-sphinx-theme-1.2.8/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     1808 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      674 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 root         (0) root         (0)     1268 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      177 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/.stylelintrc
+-rw-r--r--   0 root         (0) root         (0)      181 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)     1330 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      279 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      591 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      455 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      818 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/
+-rw-r--r--   0 root         (0) root         (0)      276 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/
+-rw-r--r--   0 root         (0) root         (0)      789 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/docsidebar.html
+-rw-r--r--   0 root         (0) root         (0)     1734 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/footer.html
+-rw-r--r--   0 root         (0) root         (0)     1373 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/layout.html
+-rw-r--r--   0 root         (0) root         (0)     2150 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/navbar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/
+-rw-r--r--   0 root         (0) root         (0)     2915 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/copybutton.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/
+-rw-r--r--   0 root         (0) root         (0)     5430 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/favicon-32.ico
+-rw-r--r--   0 root         (0) root         (0)    10706 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/numfocus-logo.svg
+-rw-r--r--   0 root         (0) root         (0)   187674 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/sunpy-bg.jpg
+-rw-r--r--   0 root         (0) root         (0)    15707 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/sunpy_icon.svg
+-rw-r--r--   0 root         (0) root         (0)     5623 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/sunpy_icon_128x128.png
+-rw-r--r--   0 root         (0) root         (0)    11319 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/sunpy_style.css
+-rw-r--r--   0 root         (0) root         (0)      165 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/version.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/
+-rw-r--r--   0 root         (0) root         (0)      127 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/attribute.rst
+-rw-r--r--   0 root         (0) root         (0)      862 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/class.rst
+-rw-r--r--   0 root         (0) root         (0)      124 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/member.rst
+-rw-r--r--   0 root         (0) root         (0)      124 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/method.rst
+-rw-r--r--   0 root         (0) root         (0)      111 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/minimal_module.rst
+-rw-r--r--   0 root         (0) root         (0)      554 2019-08-20 21:15:49.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/theme.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      591 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2019-08-20 21:15:54.000000 sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/top_level.txt
```

### Comparing `sunpy-sphinx-theme-1.2.8/.circleci/config.yml` & `sunpy-sphinx-theme-1.2.9/.circleci/config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 apt-run: &apt-install
   name: Install apt packages
   command: |
     sudo apt update
-    sudo apt install -y graphviz
-    sudo apt install -y pandoc
+    sudo apt install -y graphviz pandoc
 
 pip-run: &pip-install
   name: Install Python dependencies
   command: |
     python3 -m venv venv
     echo "source /home/circleci/project/venv/bin/activate" >> $BASH_ENV
 
 version: 2
 jobs:
+
   website:
     docker:
       - image: circleci/python:3.6
     steps:
       - checkout
       - run: *apt-install
       - run: *pip-install
-      - run: pip install -U setuptools
-      - run: pip install -e .
+      - run: pip install -U setuptools | cat
+      - run: pip install -e . | cat
       - run: git clone https://github.com/sunpy/sunpy.org.git
-      - run: pip install -r sunpy.org/requirements.txt
+      - run: pip install -r sunpy.org/requirements.txt | cat
       - run: make -C $HOME/project/sunpy.org html
 
       - store_artifacts:
           path: sunpy.org/_build/html
 
       - run:
           name: "Built documentation is available at:"
           command: DOCS_URL="${CIRCLE_BUILD_URL}/artifacts/${CIRCLE_NODE_INDEX}/${CIRCLE_WORKING_DIRECTORY/#\~/$HOME}/sunpy.org/_build/html/index.html"; echo $DOCS_URL
 
-  docs:
+  test_docs:
     docker:
       - image: circleci/python:3.6
     steps:
       - checkout
       - run: *apt-install
       - run: *pip-install
-      - run: pip install -U setuptools
-      - run: pip install -e .
-      - run: git clone --depth 1 https://github.com/sunpy/sunpy.git
-      - run: cd sunpy && pip install -e .[all,dev]
-      - run: cd sunpy && python setup.py build_docs -w
-
+      - run: pip install -U setuptools | cat
+      - run: pip install -e . | cat
+      - run: pip install sunpy[dev] | cat
+      - run: cd test_package && pip install -e . && cd docs && make html
       - store_artifacts:
-          path: sunpy/docs/_build/html
-
+          path: test_package/docs/_build/html
       - run:
           name: "Built documentation is available at:"
-          command: DOCS_URL="${CIRCLE_BUILD_URL}/artifacts/${CIRCLE_NODE_INDEX}/${CIRCLE_WORKING_DIRECTORY/#\~/$HOME}/sunpy/docs/_build/html/index.html"; echo $DOCS_URL
+          command: DOCS_URL="${CIRCLE_BUILD_URL}/artifacts/${CIRCLE_NODE_INDEX}/${CIRCLE_WORKING_DIRECTORY/#\~/$HOME}/test_package/docs/_build/html/index.html"; echo $DOCS_URL
 
 workflows:
   version: 2
 
   html-builds:
     jobs:
+      - test_docs
       - website
-      - docs
 
 notify:
   webhooks:
     - url: https://giles.cadair.com/circleci
```

### Comparing `sunpy-sphinx-theme-1.2.8/.gitignore` & `sunpy-sphinx-theme-1.2.9/.gitignore`

 * *Files 25% similar despite different names*

```diff
@@ -97,8 +97,13 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
 # vim tmp files
-*~
+*~
+
+# test_package
+test_package/docs/_build
+test_package/docs/generated
+test_package/docs/api
```

### Comparing `sunpy-sphinx-theme-1.2.8/LICENSE.md` & `sunpy-sphinx-theme-1.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/PKG-INFO` & `sunpy-sphinx-theme-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sunpy-sphinx-theme
-Version: 1.2.8
+Version: 1.2.9
 Summary: The sphinx theme for the SunPy website and documentation.
 Home-page: UNKNOWN
 Author: The SunPy Developers
 Author-email: UNKNOWN
 License: 2-clause BSD
 Description: The sphinx theme for the SunPy website and documentation.
 Platform: UNKNOWN
```

### Comparing `sunpy-sphinx-theme-1.2.8/setup.py` & `sunpy-sphinx-theme-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/conf.py` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/conf.py`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/docsidebar.html` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/docsidebar.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/footer.html` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/footer.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/layout.html` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/layout.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/navbar.html` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/navbar.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/copybutton.js` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/copybutton.js`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/favicon-32.ico` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/favicon-32.ico`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/numfocus-logo.svg` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/numfocus-logo.svg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/sunpy-bg.jpg` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/sunpy-bg.jpg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/img/sunpy_icon.svg` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/img/sunpy_icon.svg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/static/sunpy_style.css` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/static/sunpy_style.css`

 * *Files 2% similar despite different names*

```diff
@@ -374,14 +374,15 @@
   background-color: #fff3e0;
   border: 1px solid #fe7900;
 }
 
 .alert-warning {
   background-color: #fff3e0;
   border: 1px solid #fe7900;
+  color: #333;
 }
 
 p.admonition-title {
   color: #333;
 }
 
 .alert>p+p {
@@ -797,7 +798,29 @@
 }
 
 .frametransformgraph {
   overflow-x: auto;
   width: 100%;
   border: 1px solid black;
 }
+
+
+.versionmodified {
+  font-style: italic;
+  font-weight: bold;
+}
+
+div.deprecated{
+  border: 1px solid #000000;
+  background-color: #b7c3cc;
+  color: #333;
+  border-radius: 4px;
+}
+
+card.img {
+  border-radius: 50%;
+}
+
+table tr div.deprecated {
+  border: none;
+  background-color: white;
+}
```

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/templates/autosummary/class.rst` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme/sunpy/theme.conf` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme/sunpy/theme.conf`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/PKG-INFO` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sunpy-sphinx-theme
-Version: 1.2.8
+Version: 1.2.9
 Summary: The sphinx theme for the SunPy website and documentation.
 Home-page: UNKNOWN
 Author: The SunPy Developers
 Author-email: UNKNOWN
 License: 2-clause BSD
 Description: The sphinx theme for the SunPy website and documentation.
 Platform: UNKNOWN
```

### Comparing `sunpy-sphinx-theme-1.2.8/sunpy_sphinx_theme.egg-info/SOURCES.txt` & `sunpy-sphinx-theme-1.2.9/sunpy_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 .gitignore
 .stylelintrc
 .travis.yml
 LICENSE.md
 MANIFEST.in
 README.md
 setup.py
-tool.py
 .circleci/config.yml
-.github/main.workflow
+.github/workflows/release_pypi.yml
 sunpy_sphinx_theme/__init__.py
 sunpy_sphinx_theme/conf.py
 sunpy_sphinx_theme.egg-info/PKG-INFO
 sunpy_sphinx_theme.egg-info/SOURCES.txt
 sunpy_sphinx_theme.egg-info/dependency_links.txt
 sunpy_sphinx_theme.egg-info/requires.txt
 sunpy_sphinx_theme.egg-info/top_level.txt
@@ -23,12 +22,13 @@
 sunpy_sphinx_theme/sunpy/static/copybutton.js
 sunpy_sphinx_theme/sunpy/static/sunpy_style.css
 sunpy_sphinx_theme/sunpy/static/version.js
 sunpy_sphinx_theme/sunpy/static/img/favicon-32.ico
 sunpy_sphinx_theme/sunpy/static/img/numfocus-logo.svg
 sunpy_sphinx_theme/sunpy/static/img/sunpy-bg.jpg
 sunpy_sphinx_theme/sunpy/static/img/sunpy_icon.svg
+sunpy_sphinx_theme/sunpy/static/img/sunpy_icon_128x128.png
 sunpy_sphinx_theme/sunpy/templates/autosummary/attribute.rst
 sunpy_sphinx_theme/sunpy/templates/autosummary/class.rst
 sunpy_sphinx_theme/sunpy/templates/autosummary/member.rst
 sunpy_sphinx_theme/sunpy/templates/autosummary/method.rst
 sunpy_sphinx_theme/sunpy/templates/autosummary/minimal_module.rst
```

