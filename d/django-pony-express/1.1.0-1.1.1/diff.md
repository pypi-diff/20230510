# Comparing `tmp/django-pony-express-1.1.0.tar.gz` & `tmp/django-pony-express-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pony-express-1.1.0.tar", last modified: Thu May  4 13:58:29 2023, max compression
+gzip compressed data, was "django-pony-express-1.1.1.tar", last modified: Wed May 10 08:33:55 2023, max compression
```

## Comparing `django-pony-express-1.1.0.tar` & `django-pony-express-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
--rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.1.0/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-05-04 13:52:30.444591 django-pony-express-1.1.0/.coveragerc
--rw-r--r--   0        0        0      288 2023-05-04 13:52:30.444591 django-pony-express-1.1.0/.editorconfig
--rw-r--r--   0        0        0     1700 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/.gitignore
--rw-r--r--   0        0        0      904 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/.readthedocs.yml
--rw-r--r--   0        0        0      370 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/CHANGES.md
--rw-r--r--   0        0        0     1107 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/LICENSE.md
--rw-r--r--   0        0        0      138 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/MANIFEST.in
--rw-r--r--   0        0        0     5227 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/README.md
--rw-r--r--   0        0        0       85 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/django_pony_express/__init__.py
--rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/errors.py
--rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/services/base.py
--rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      654 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/docs/Makefile
--rw-r--r--   0        0        0     2819 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/docs/conf.py
--rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.1.0/docs/features/changelog.rst
--rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/docs/features/mail.md
--rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/docs/features/tests.md
--rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/manage.py
--rw-r--r--   0        0        0     3720 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/pytest.init
--rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.1.0/settings.py
--rw-r--r--   0        0        0       69 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/__init__.py
--rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/files/testfile.txt
--rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/test_email_test_service.py
--rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/test_mail_services.py
--rw-r--r--   0        0        0     7210 1970-01-01 00:00:00.000000 django-pony-express-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.1.1/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-10 08:29:28.854483 django-pony-express-1.1.1/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-10 08:29:28.854483 django-pony-express-1.1.1/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-10 08:29:28.893613 django-pony-express-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-10 08:29:28.870155 django-pony-express-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-10 08:29:28.870155 django-pony-express-1.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0      498 2023-05-10 08:33:32.740440 django-pony-express-1.1.1/CHANGES.md
+-rw-r--r--   0        0        0     1107 2023-05-10 08:29:28.870155 django-pony-express-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-05-10 08:29:28.870155 django-pony-express-1.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     5733 2023-05-10 08:29:28.890356 django-pony-express-1.1.1/README.md
+-rw-r--r--   0        0        0       82 2023-05-10 08:31:44.027402 django-pony-express-1.1.1/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/django_pony_express/errors.py
+-rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.1.1/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/django_pony_express/services/base.py
+-rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      654 2023-05-10 08:29:28.897825 django-pony-express-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0     2819 2023-05-10 08:29:28.895692 django-pony-express-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.1.1/docs/features/changelog.rst
+-rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/docs/features/mail.md
+-rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/docs/features/tests.md
+-rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-10 08:29:28.897304 django-pony-express-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.1.1/manage.py
+-rw-r--r--   0        0        0     3721 2023-05-10 08:29:28.870155 django-pony-express-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-10 08:29:28.870155 django-pony-express-1.1.1/pytest.init
+-rw-r--r--   0        0        0       50 2023-05-10 08:29:28.897825 django-pony-express-1.1.1/scripts/publish_to_pypi.ps1
+-rw-r--r--   0        0        0       50 2023-05-10 08:29:28.901831 django-pony-express-1.1.1/scripts/publish_to_pypi.sh
+-rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.1.1/settings.py
+-rw-r--r--   0        0        0       69 2023-05-10 08:29:28.892001 django-pony-express-1.1.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/testapp/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/tests/files/testfile.txt
+-rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/tests/test_email_test_service.py
+-rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.1.1/tests/test_mail_services.py
+-rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 django-pony-express-1.1.1/PKG-INFO
```

### Comparing `django-pony-express-1.1.0/.ambient-package-update/metadata.py` & `django-pony-express-1.1.1/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/.github/workflows/ci.yml` & `django-pony-express-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/.gitignore` & `django-pony-express-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/.pre-commit-config.yaml` & `django-pony-express-1.1.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
       - id: black
         args: [ --check, --diff, --config, ./pyproject.toml ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.264'
+    rev: 'v0.0.265'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: [ --py38-plus ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/adamchainz/django-upgrade
```

### Comparing `django-pony-express-1.1.0/.readthedocs.yml` & `django-pony-express-1.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/LICENSE.md` & `django-pony-express-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/README.md` & `django-pony-express-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -146,7 +146,16 @@
 
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
   ```
+
+### Maintenance
+
+Please note that this package supports the [ambient-package-update](https://pypi.org/project/ambient-package-update/).
+So you don't have to worry about the maintenance of this package. All important configuration and setup files are
+being rendered by this updater. It works similar to well-known updaters like `pyupgrade` or `django-upgrade`.
+
+To run an update, refer to the [documentation page](https://pypi.org/project/ambient-package-update/)
+of the "ambient-package-update".
```

### Comparing `django-pony-express-1.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po` & `django-pony-express-1.1.1/django_pony_express/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/django_pony_express/services/base.py` & `django-pony-express-1.1.1/django_pony_express/services/base.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/django_pony_express/services/tests.py` & `django-pony-express-1.1.1/django_pony_express/services/tests.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/docs/Makefile` & `django-pony-express-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/docs/conf.py` & `django-pony-express-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/docs/features/mail.md` & `django-pony-express-1.1.1/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/docs/features/tests.md` & `django-pony-express-1.1.1/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/docs/make.bat` & `django-pony-express-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/manage.py` & `django-pony-express-1.1.1/manage.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/pyproject.toml` & `django-pony-express-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
    'pre-commit~=3.2',
    'black~=23.3',
    'Django~=3.2',
    'sphinx==4.2.0',
    'sphinx-rtd-theme==1.0.0',
    'm2r2==0.3.1',
    'mistune<2.0.0',
-   'ambient-package-update~=23.5.4',
+   'ambient-package-update~=23.5.10',
 ]
 
 [tool.flit.module]
 name = "django_pony_express"
 
 [project.urls]
 'Homepage' = 'https://github.com/ambient-innovation/django-pony-express/'
```

### Comparing `django-pony-express-1.1.0/settings.py` & `django-pony-express-1.1.1/settings.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/tests/test_email_test_service.py` & `django-pony-express-1.1.1/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/tests/test_mail_services.py` & `django-pony-express-1.1.1/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.1.0/PKG-INFO` & `django-pony-express-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 1.1.0
+Version: 1.1.1
 Summary: Class-based emails including a test suite for Django
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -32,15 +32,15 @@
 Requires-Dist: pre-commit~=3.2 ; extra == "dev"
 Requires-Dist: black~=23.3 ; extra == "dev"
 Requires-Dist: Django~=3.2 ; extra == "dev"
 Requires-Dist: sphinx==4.2.0 ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
 Requires-Dist: m2r2==0.3.1 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.5.4 ; extra == "dev"
+Requires-Dist: ambient-package-update~=23.5.10 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/django-pony-express/issues
 Project-URL: Changelog, https://django-pony-express.readthedocs.io/en/latest/features/changelog.html
 Project-URL: Documentation, https://django-pony-express.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/ambient-innovation/django-pony-express/
 Project-URL: Maintained by, https://ambient.digital/
 Provides-Extra: dev
 
@@ -193,7 +193,16 @@
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
   ```
 
+### Maintenance
+
+Please note that this package supports the [ambient-package-update](https://pypi.org/project/ambient-package-update/).
+So you don't have to worry about the maintenance of this package. All important configuration and setup files are
+being rendered by this updater. It works similar to well-known updaters like `pyupgrade` or `django-upgrade`.
+
+To run an update, refer to the [documentation page](https://pypi.org/project/ambient-package-update/)
+of the "ambient-package-update".
+
```

