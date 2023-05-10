# Comparing `tmp/docassemble.ALToolbox-0.8.0.tar.gz` & `tmp/docassemble.ALToolbox-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.ALToolbox-0.8.0.tar", last modified: Tue Apr 25 15:59:37 2023, max compression
+gzip compressed data, was "docassemble.ALToolbox-0.8.1.tar", last modified: Wed May 10 13:16:33 2023, max compression
```

## Comparing `docassemble.ALToolbox-0.8.0.tar` & `docassemble.ALToolbox-0.8.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2754 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.570706 docassemble.ALToolbox-0.8.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.570706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/Addup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/PhoneNumberDataType.py
--rw-r--r--   0 runner    (1001) docker     (122)    37755 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/ThreePartsDate.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/addenda.py
--rw-r--r--   0 runner    (1001) docker     (122)    50493 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/al_income.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/business_days.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/copy_button.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.566706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.574706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Addup.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Bells and whistles.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Profiling.yml
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Shorten a url.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/TextCounter.yml
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/ThreePartsDate.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml
--rw-r--r--   0 runner    (1001) docker     (122)    26884 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income.yml
--rw-r--r--   0 runner    (1001) docker     (122)    15092 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/altoolbox_overview.yml
--rw-r--r--   0 runner    (1001) docker     (122)     6056 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/business_days_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/collapse_template.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/collapse_template_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/copy_button.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/copy_button_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/display_template.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/display_template_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/escape_button.yml
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/escape_button_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect.yml
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone-number-validation.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/review_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/review_widget.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/save_input_data_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/three_parts_date_demo.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.574706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/TextCounter.js
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/al_three_parts_date.css
--rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.css
--rw-r--r--   0 runner    (1001) docker     (122)    81271 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.js
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/collapse_template.css
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.css
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.js
--rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/custom_504.html
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/display_template.css
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/escape_button.js
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/phone-number-validation.js
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/phone-number-validator.css
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/review_widget.css
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/review_widget.js
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)   184585 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/debts.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/output-checkbox.docx
--rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/table-addendum.docx
--rw-r--r--   0 runner    (1001) docker     (122)     5196 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx
--rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/display_template.py
--rw-r--r--   0 runner    (1001) docker     (122)    12200 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/save_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6812 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_al_income.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_altoolbox.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.570706 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.145041 docassemble.ALToolbox-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-05-10 13:16:33.145041 docassemble.ALToolbox-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2754 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.133040 docassemble.ALToolbox-0.8.1/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.137040 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/Addup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/PhoneNumberDataType.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37755 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/ThreePartsDate.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/addenda.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50493 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/al_income.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/business_days.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/copy_button.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.129040 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.141040 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Addup.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Bells and whistles.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Profiling.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Shorten a url.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/TextCounter.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/ThreePartsDate.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    26884 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/al_income.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    15092 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/al_income_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/altoolbox_overview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6056 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/business_days_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/collapse_template.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/collapse_template_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/copy_button.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/copy_button_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/display_template.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/display_template_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/escape_button.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/escape_button_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/multiselect.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/multiselect_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/phone-number-validation.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/review_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/review_widget.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/save_input_data_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/three_parts_date_demo.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.141040 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.145041 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/TextCounter.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/al_three_parts_date.css
+-rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.css
+-rw-r--r--   0 runner    (1001) docker     (122)    81271 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.js
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/collapse_template.css
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/copy_button.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/copy_button.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/custom_504.html
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/display_template.css
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/escape_button.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/phone-number-validation.js
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/phone-number-validator.css
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/review_widget.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/review_widget.js
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.145041 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)   184585 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/debts.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/output-checkbox.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/table-addendum.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     5196 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/display_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12200 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/save_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6812 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/test_al_income.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/test_altoolbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 13:16:33.133040 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-05-10 13:16:33.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-05-10 13:16:33.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 13:16:33.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-10 13:16:33.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 13:16:32.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-05-10 13:16:33.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-10 13:16:33.000000 docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-10 13:16:33.145041 docassemble.ALToolbox-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-05-10 13:16:20.000000 docassemble.ALToolbox-0.8.1/setup.py
```

### Comparing `docassemble.ALToolbox-0.8.0/LICENSE` & `docassemble.ALToolbox-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/PKG-INFO` & `docassemble.ALToolbox-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.ALToolbox
-Version: 0.8.0
+Version: 0.8.1
 Summary: Collection of small utility functions, classes, and web components for Docassemble interviews
 Home-page: https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox
 Author: AssemblyLine
 Author-email: 52798256+plocket@users.noreply.github.com
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.ALToolbox-0.8.0/README.md` & `docassemble.ALToolbox-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/Addup.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/Addup.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/PhoneNumberDataType.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/PhoneNumberDataType.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/ThreePartsDate.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/ThreePartsDate.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/addenda.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/addenda.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/al_income.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/al_income.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/business_days.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/business_days.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/copy_button.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/copy_button.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Addup.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Addup.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Bells and whistles.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Bells and whistles.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Profiling.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Profiling.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Shorten a url.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/Shorten a url.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/TextCounter.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/TextCounter.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/al_income.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/al_income_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/altoolbox_overview.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/altoolbox_overview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/business_days_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/business_days_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/collapse_template_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/collapse_template_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/copy_button_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/copy_button_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/display_template_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/display_template_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/escape_button_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/escape_button_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/multiselect.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/multiselect_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone-number-validation.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/phone-number-validation.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/review_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/review_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/save_input_data_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/save_input_data_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/three_parts_date_demo.yml` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/questions/three_parts_date_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/TextCounter.js` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/TextCounter.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/al_three_parts_date.css` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/al_three_parts_date.css`

 * *Files 22% similar despite different names*

```diff
@@ -22,7 +22,12 @@
   background-position: right calc(0.375em + 0.1875rem) center;
   background-size: calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
 
 .al_three_parts_date.al_invalid .col-year {
   padding-right: 0;
 }
+
+/* Avoid AL styles elongating date and year fields and codify widths. */
+.al_three_parts_date .col > * {
+  width: 100%;
+}
```

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.css` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.css`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.js` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.css` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/copy_button.css`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.js` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/copy_button.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/custom_504.html` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/custom_504.html`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/phone-number-validation.js` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/phone-number-validation.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/review_widget.js` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/static/review_widget.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/debts.pdf` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/debts.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/output-checkbox.docx` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/output-checkbox.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/table-addendum.docx` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/table-addendum.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/display_template.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/display_template.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/misc.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/misc.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/save_input_data.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/save_input_data.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_al_income.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/test_al_income.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_altoolbox.py` & `docassemble.ALToolbox-0.8.1/docassemble/ALToolbox/test_altoolbox.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/PKG-INFO` & `docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.ALToolbox
-Version: 0.8.0
+Version: 0.8.1
 Summary: Collection of small utility functions, classes, and web components for Docassemble interviews
 Home-page: https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox
 Author: AssemblyLine
 Author-email: 52798256+plocket@users.noreply.github.com
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/SOURCES.txt` & `docassemble.ALToolbox-0.8.1/docassemble.ALToolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.8.0/setup.py` & `docassemble.ALToolbox-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.ALToolbox',
-      version='0.8.0',
+      version='0.8.1',
       description=('Collection of small utility functions, classes, and web components for Docassemble interviews'),
       long_description='# ALToolbox\r\n\r\n[![PyPI version](https://badge.fury.io/py/docassemble-ALToolbox.svg)](https://badge.fury.io/py/docassemble-ALToolbox)\r\n\r\nThis repository is used to host small Python modules, widgets, and JavaScript web components js files that enhance Docassemble interviews. These modules were\r\nbuilt as part of the Suffolk University Law School LIT Lab\'s [Document Assembly Line project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\nThey are placed here\r\nrather than in https://github.com/SuffolkLitLab/docassemble-AssemblyLine because we believe these small components can easily be used\r\nby anyone, regardless of whether they use any other code from the Document Assembly Line project.\r\n\r\nIf you want to add a small fuction to this project, consider adding it to the existing misc.py to avoid creating too many module files.\r\n\r\n## Documentation\r\n\r\nRead the [documentation for the functions and components](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox) to learn\r\nhow to use these components in your own [Docassemble](https://github.com/jhpyle/docassemble) projects.\r\n\r\n## Suffolk LIT Lab Document Assembly Line\r\n\r\n<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>\r\n\r\nThe Assembly Line Project is a collection of volunteers, students, and institutions who joined together\r\nduring the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,\r\neasy to use **guided** online forms that help empower litigants to access the court remotely.\r\n\r\nOur signature project is [CourtFormsOnline.org](https://courtformsonline.org).\r\n\r\nWe designed a step-by-step, assembly line style process for automating court forms on top of Docassemble\r\nand built several tools along the way that **you** can use in your home jurisdiction.\r\n\r\nThis package contains **runtime code** and **pre-written questions** to support authoring robust, \r\nconsistent, and attractive Docassemble interviews that help complete court forms.\r\n\r\nRead more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\n\r\n\r\n# Related repositories\r\n\r\n* https://github.com/SuffolkLitLab/docassemble-AssemblyLine\r\n* https://github.com/SuffolkLitLab/docassemble-ALWeaver\r\n* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts\r\n* https://github.com/SuffolkLitLab/docassemble-MassAccess\r\n* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate\r\n* https://github.com/SuffolkLitLab/EfileProxyServer\r\n\r\n## Contributors:\r\n* @plocket  \r\n* @nonprofittechy\r\n* @purplesky2016\r\n* @brycestevenwilley\r\n',
       long_description_content_type='text/markdown',
       author='AssemblyLine',
       author_email='52798256+plocket@users.noreply.github.com',
       license='The MIT License (MIT)',
       url='https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox',
```

