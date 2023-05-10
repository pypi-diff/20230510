# Comparing `tmp/types-docutils-0.19.1.9.tar.gz` & `tmp/types-docutils-0.20.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docutils-0.19.1.9.tar", last modified: Wed May  3 12:29:52 2023, max compression
+gzip compressed data, was "types-docutils-0.20.0.0.tar", last modified: Wed May 10 12:29:13 2023, max compression
```

## Comparing `types-docutils-0.19.1.9.tar` & `types-docutils-0.20.0.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/docutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/examples.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/frontend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/io.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/languages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/nodes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/recommonmark_wrapper.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.785030 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/admonitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/body.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/images.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/parts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/references.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/directives/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/roles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/parsers/rst/states.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/doctree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/pep.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/readers/standalone.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/statemachine.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/transforms/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/docutils-stubs/writers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/docutils_xml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/html4css1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/html5_polyglot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/latex2e.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/manpage.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/odf_odt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/pep_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/pseudoxml.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/s5_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 12:29:30.000000 types-docutils-0.19.1.9/docutils-stubs/writers/xetex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:52.789030 types-docutils-0.19.1.9/types_docutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 12:29:52.000000 types-docutils-0.19.1.9/types_docutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.724080 types-docutils-0.20.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-10 12:29:10.000000 types-docutils-0.20.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 12:29:10.000000 types-docutils-0.20.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-10 12:29:13.724080 types-docutils-0.20.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:29:10.000000 types-docutils-0.20.0.0/docutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/examples.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/frontend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/io.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/languages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/nodes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/recommonmark_wrapper.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/admonitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/body.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/parts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/references.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/directives/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/roles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/parsers/rst/states.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/readers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/readers/doctree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/readers/pep.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/readers/standalone.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/statemachine.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/transforms/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.720080 types-docutils-0.20.0.0/docutils-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.724080 types-docutils-0.20.0.0/docutils-stubs/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/docutils_xml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/html4css1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/html5_polyglot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/latex2e.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/manpage.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/odf_odt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/pep_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/pseudoxml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/s5_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:28:56.000000 types-docutils-0.20.0.0/docutils-stubs/writers/xetex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:29:13.724080 types-docutils-0.20.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-10 12:29:10.000000 types-docutils-0.20.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:29:13.724080 types-docutils-0.20.0.0/types_docutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-10 12:29:13.000000 types-docutils-0.20.0.0/types_docutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 12:29:13.000000 types-docutils-0.20.0.0/types_docutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:29:13.000000 types-docutils-0.20.0.0/types_docutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:29:13.000000 types-docutils-0.20.0.0/types_docutils.egg-info/top_level.txt
```

### Comparing `types-docutils-0.19.1.9/CHANGELOG.md` & `types-docutils-0.20.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.20.0.0 (2023-05-10)
+
+Bump docutils to 0.20.* (#10167)
+
 ## 0.19.1.9 (2023-05-03)
 
 [docutils] Add items to docutils.node (#10102)
 
 * Add class paragraph
 * Add class TextElement
 * Add Element.index(), .remove(), and .insert()
```

### Comparing `types-docutils-0.19.1.9/PKG-INFO` & `types-docutils-0.20.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.19.1.9
+Version: 0.20.0.0
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
+This package was generated from typeshed commit `adddc4f24aa4cc0e1b8981d9197f2999ab37bed3`.
```

### Comparing `types-docutils-0.19.1.9/docutils-stubs/__init__.pyi` & `types-docutils-0.20.0.0/docutils-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/frontend.pyi` & `types-docutils-0.20.0.0/docutils-stubs/frontend.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/io.pyi` & `types-docutils-0.20.0.0/docutils-stubs/io.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/nodes.pyi` & `types-docutils-0.20.0.0/docutils-stubs/nodes.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         self,
         condition: Callable[[Node], bool] | None = None,
         include_self: bool = False,
         descend: bool = True,
         siblings: bool = False,
         ascend: bool = False,
     ) -> Node: ...
-    def previous_sibling(self) -> Node | None: ...
 
 class Element(Node):
     children: list[Node]
     rawsource: str
     def __init__(self, rawsource: str = "", *children: Node, **attributes): ...
     def __len__(self) -> int: ...
     def __contains__(self, key: str | Node) -> bool: ...
@@ -106,14 +105,15 @@
     def copy(self) -> Self: ...
     def deepcopy(self) -> Self: ...
     def pformat(self, indent: str = "    ", level: int = 0) -> str: ...
     def astext(self) -> str: ...
     def index(self, item: Node, start: int = 0, stop: int = sys.maxsize) -> int: ...
     def remove(self, item: Node) -> None: ...
     def insert(self, index: SupportsIndex, item: Node | Iterable[Node] | None) -> None: ...
+    def previous_sibling(self) -> Node | None: ...
     def __getattr__(self, __name: str) -> Incomplete: ...
 
 class TextElement(Element):
     def __init__(self, rawsource: str = "", text: str = "", *children: Node, **attributes) -> None: ...
 
 class Text(Node, str):
     tagname: ClassVar[str]
```

### Comparing `types-docutils-0.19.1.9/docutils-stubs/parsers/__init__.pyi` & `types-docutils-0.20.0.0/docutils-stubs/parsers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/parsers/rst/__init__.pyi` & `types-docutils-0.20.0.0/docutils-stubs/parsers/rst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/parsers/rst/roles.pyi` & `types-docutils-0.20.0.0/docutils-stubs/parsers/rst/roles.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/transforms/__init__.pyi` & `types-docutils-0.20.0.0/docutils-stubs/transforms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.19.1.9/docutils-stubs/utils/__init__.pyi` & `types-docutils-0.20.0.0/docutils-stubs/utils/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from docutils import ApplicationError
 from docutils.io import FileOutput
 from docutils.nodes import document
 
 class DependencyList:
     list: _list[str]
     file: FileOutput | None
-    def __init__(self, output_file: str | None = None, dependencies: Iterable[str] = []) -> None: ...
+    def __init__(self, output_file: str | None = None, dependencies: Iterable[str] = ()) -> None: ...
     def set_output(self, output_file: str | None) -> None: ...
     def add(self, *filenames: str) -> None: ...
     def close(self) -> None: ...
 
 _SystemMessageLevel: TypeAlias = Literal[0, 1, 2, 3, 4]
 
 class Reporter:
```

### Comparing `types-docutils-0.19.1.9/setup.py` & `types-docutils-0.20.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
+This package was generated from typeshed commit `adddc4f24aa4cc0e1b8981d9197f2999ab37bed3`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.19.1.9",
+      version="0.20.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md",
```

### Comparing `types-docutils-0.19.1.9/types_docutils.egg-info/PKG-INFO` & `types-docutils-0.20.0.0/types_docutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.19.1.9
+Version: 0.20.0.0
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
+This package was generated from typeshed commit `adddc4f24aa4cc0e1b8981d9197f2999ab37bed3`.
```

### Comparing `types-docutils-0.19.1.9/types_docutils.egg-info/SOURCES.txt` & `types-docutils-0.20.0.0/types_docutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

