# Comparing `tmp/sympy-1.9.tar.gz` & `tmp/sympy-1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympy-1.9.tar", last modified: Thu Sep 30 22:28:05 2021, max compression
+gzip compressed data, was "sympy-1.9rc1.tar", last modified: Sun Sep 19 19:52:01 2021, max compression
```

## Comparing `sympy-1.9.tar` & `sympy-1.9rc1.tar`

### file list

```diff
@@ -1,2039 +1,2039 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.999352 sympy-1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    44032 2021-09-30 22:23:57.024181 sympy-1.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     7885 2021-09-30 22:23:57.024181 sympy-1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12034 2021-09-30 22:28:04.999352 sympy-1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10987 2021-09-30 22:23:57.024181 sympy-1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      509 2021-09-30 22:23:57.024181 sympy-1.9/bin/isympy
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.931351 sympy-1.9/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/data/TeXmacs/
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-09-30 22:23:57.028182 sympy-1.9/data/TeXmacs/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/data/TeXmacs/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2349 2021-09-30 22:23:57.028182 sympy-1.9/data/TeXmacs/bin/tm_sympy
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/data/TeXmacs/progs/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-09-30 22:23:57.028182 sympy-1.9/data/TeXmacs/progs/init-sympy.scm
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2021-09-30 22:23:57.028182 sympy-1.9/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-09-30 22:23:57.028182 sympy-1.9/doc/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/api/
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-09-30 22:23:57.028182 sympy-1.9/doc/api/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-30 22:23:57.028182 sympy-1.9/doc/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-30 22:23:57.028182 sympy-1.9/doc/apidoc.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/cheatsheet/
--rw-r--r--   0 runner    (1001) docker     (121)     8792 2021-09-30 22:23:57.028182 sympy-1.9/doc/cheatsheet/cheatsheet.tex
--rw-r--r--   0 runner    (1001) docker     (121)    23570 2021-09-30 22:23:57.028182 sympy-1.9/doc/cheatsheet/combinatoric_cheatsheet.tex
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-09-30 22:28:02.271317 sympy-1.9/doc/commit_hash.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/ext/
--rw-r--r--   0 runner    (1001) docker     (121)    16898 2021-09-30 22:23:57.028182 sympy-1.9/doc/ext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (121)     9421 2021-09-30 22:23:57.028182 sympy-1.9/doc/ext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (121)     6272 2021-09-30 22:23:57.028182 sympy-1.9/doc/ext/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2021-09-30 22:23:57.028182 sympy-1.9/doc/ext/sympylive.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9472 2021-09-30 22:23:57.028182 sympy-1.9/doc/generate_logos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/man/
--rw-r--r--   0 runner    (1001) docker     (121)     6659 2021-09-30 22:23:57.028182 sympy-1.9/doc/man/isympy.1
--rw-r--r--   0 runner    (1001) docker     (121)    17844 2021-09-30 22:23:57.028182 sympy-1.9/doc/man/isympy.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     6785 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/_static/default.css_t
--rw-r--r--   0 runner    (1001) docker     (121)    19711 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/_static/sympylogo.png
--rw-r--r--   0 runner    (1001) docker     (121)   167361 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/_static/sympylogo_big.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/aboutus.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/citing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9489 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    50723 2021-09-30 22:23:57.028182 sympy-1.9/doc/src/documentation-style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)    27968 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/gotchas.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/guides/
--rw-r--r--   0 runner    (1001) docker     (121)    55371 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/guides/assumptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15907 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/guides/booleans.rst
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      855 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/logo/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/logo/info.txt
--rw-r--r--   0 runner    (1001) docker     (121)    34099 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/logo/sympy-use-text.svg
--rw-r--r--   0 runner    (1001) docker     (121)    40583 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/logo/sympy.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/abc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/algebras.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/assumptions/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/assumptions/ask.rst
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/assumptions/assume.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/assumptions/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/assumptions/predicates.rst
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/assumptions/refine.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/calculus/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/calculus/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/categories.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23741 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/codegen.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/combinatorics/
--rw-r--r--   0 runner    (1001) docker     (121)    11344 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/fp_groups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/graycode.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/group_constructs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/named_groups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/partitions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/pc_groups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/perm_groups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/permutations.rst
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/polyhedron.rst
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/prufer.rst
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/subsets.rst
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/tensor_can.rst
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/testutil.rst
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/combinatorics/util.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/concrete.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/core.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/crypto.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/diffgeom.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/discrete.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13689 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/evalf.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/functions/
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/functions/combinatorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5783 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/functions/elementary.rst
--rw-r--r--   0 runner    (1001) docker     (121)      385 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/functions/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7089 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/functions/special.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/curves.rst
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/ellipses.rst
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/entities.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6665 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/lines.rst
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/plane.rst
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/points.rst
--rw-r--r--   0 runner    (1001) docker     (121)      173 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/polygons.rst
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/geometry/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/holonomic/
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/about.rst
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/convert.rst
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/internal.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/operations.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/represent.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/holonomic/uses.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/integrals/
--rw-r--r--   0 runner    (1001) docker     (121)    31196 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/integrals/g-functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12920 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/integrals/integrals.rst
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/interactive.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.943351 sympy-1.9/doc/src/modules/liealgebras/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2021-09-30 22:23:57.032182 sympy-1.9/doc/src/modules/liealgebras/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/logic.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/matrices/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/common.rst
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/dense.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/expressions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/immutablematrices.rst
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14159 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/matrices.rst
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/sparse.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/matrices/sparsetools.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/ntheory.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/numeric-computation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/parsing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/continuum_mechanics/
--rw-r--r--   0 runner    (1001) docker     (121)     9011 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/continuum_mechanics/allowed-sign-conventions.png
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/continuum_mechanics/beam.rst
--rw-r--r--   0 runner    (1001) docker     (121)    48599 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/continuum_mechanics/beam_problems.rst
--rw-r--r--   0 runner    (1001) docker     (121)    31500 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/continuum_mechanics/ildreaction.png
--rw-r--r--   0 runner    (1001) docker     (121)    46549 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/continuum_mechanics/ildshear.png
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/continuum_mechanics/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/control/
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/control/control.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/control/control_plots.rst
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/control/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/control/lti.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/hep/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/hep/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/hydrogen.rst
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/matrices.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/mechanics/
--rw-r--r--   0 runner    (1001) docker     (121)     6131 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/advanced.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/mechanics/api/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/body.rst
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/expr_manip.rst
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/joint.rst
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/kane_lagrange.rst
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/part_bod.rst
--rw-r--r--   0 runner    (1001) docker     (121)      465 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/printing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/api/system.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21620 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/autolev_parser.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/mechanics/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    18210 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/bicycle_example.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10648 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/lin_pend_nonmin_example.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7277 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/multi_degree_freedom_holonomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (121)    68787 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/multidof-holonomic.png
--rw-r--r--   0 runner    (1001) docker     (121)    22831 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/pendulum_nonmin.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9492 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc.svg
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3348 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane_constraints.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example_lagrange.rst
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6321 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/kane.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/lagrange.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13663 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13824 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/masses.rst
--rw-r--r--   0 runner    (1001) docker     (121)      917 2021-09-30 22:23:57.036182 sympy-1.9/doc/src/modules/physics/mechanics/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)    47681 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/mechanics/sympy_mechanics_for_autolev_users.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7588 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/mechanics/symsystem.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/optics/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/optics/gaussopt.rst
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/optics/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/optics/medium.rst
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/optics/polarization.rst
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/optics/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/optics/waves.rst
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/paulialgebra.rst
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/qho_1d.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/quantum/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/anticommutator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/cartesian.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/cg.rst
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/circuitplot.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/commutator.rst
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/constants.rst
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/dagger.rst
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/gate.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/grover.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/hilbert.rst
--rw-r--r--   0 runner    (1001) docker     (121)      774 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/innerproduct.rst
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/operator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/operatorset.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/piab.rst
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/qapply.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/qft.rst
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/qubit.rst
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/represent.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/shor.rst
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/spin.rst
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/state.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/quantum/tensorproduct.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/secondquant.rst
--rw-r--r--   0 runner    (1001) docker     (121)      153 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/sho.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/units/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/dimensions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9966 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/philosophy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/prefixes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      309 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/quantities.rst
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/units/unitsystem.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/vector/
--rw-r--r--   0 runner    (1001) docker     (121)     6011 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/advanced.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.947351 sympy-1.9/doc/src/modules/physics/vector/api/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/api/fieldfunctions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/api/functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/api/kinematics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/api/printing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13626 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/fields.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8723 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_1.svg
--rw-r--r--   0 runner    (1001) docker     (121)    25763 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_1pt.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13720 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    16112 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_2pt.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12267 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_3.svg
--rw-r--r--   0 runner    (1001) docker     (121)    18006 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_4.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12819 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_angvel1.svg
--rw-r--r--   0 runner    (1001) docker     (121)    23357 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_angvel2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14105 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_angvel3.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10993 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kin_rolling.svg
--rw-r--r--   0 runner    (1001) docker     (121)    21732 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/kinematics.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/simp_rot.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7722 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_add.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10009 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_cross.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10637 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_dot.svg
--rw-r--r--   0 runner    (1001) docker     (121)    15641 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_fix_notfix.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_mul.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5311 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_rep.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14527 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vec_simp_der.svg
--rw-r--r--   0 runner    (1001) docker     (121)    30182 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/vector/vectors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/physics/wigner.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9028 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/plotting.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/polys/
--rw-r--r--   0 runner    (1001) docker     (121)    14916 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/polys/agca.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21504 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/polys/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2021-09-30 22:23:57.040182 sympy-1.9/doc/src/modules/polys/domainmatrix.rst
--rw-r--r--   0 runner    (1001) docker     (121)    56088 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/domainsintro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8428 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/domainsref.rst
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    24930 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/internals.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6527 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/literature.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4683 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8816 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/ringseries.rst
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/solvers.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15616 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/polys/wester.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17534 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/printing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4459 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/rewriting.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/series/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/series/formal.rst
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/series/fourier.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/series/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/series/limitseq.rst
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/series/sequences.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5326 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/series/series.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/sets.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/simplify/
--rw-r--r--   0 runner    (1001) docker     (121)     8382 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/simplify/fu.rst
--rw-r--r--   0 runner    (1001) docker     (121)    27713 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/simplify/hyperexpand.rst
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/simplify/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/simplify/simplify.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)    20258 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/solvers/diophantine.rst
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/solvers/inequalities.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10710 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/solvers/ode.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/solvers/pde.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/solvers/solvers.rst
--rw-r--r--   0 runner    (1001) docker     (121)    22507 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/solvers/solveset.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7771 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/stats.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/tensor/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/tensor/array.rst
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/tensor/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/tensor/index_methods.rst
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/tensor/indexed.rst
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/tensor/tensor.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/tensor/toperators.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/testing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/testing/pytest.rst
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/testing/randtest.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/testing/runtests.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/autowrap.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/decorator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/enumerative.rst
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/iterables.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/lambdify.rst
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/memoization.rst
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/pkgdata.rst
--rw-r--r--   0 runner    (1001) docker     (121)      122 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/source.rst
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/utilities/timeutils.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/vector/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/modules/vector/api/
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      830 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/api/orienterclasses.rst
--rw-r--r--   0 runner    (1001) docker     (121)      921 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/api/vectorfunctions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7773 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9615 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/coordsys.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/coordsys_rot.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12820 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/fields.rst
--rw-r--r--   0 runner    (1001) docker     (121)      779 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5450 2021-09-30 22:23:57.044182 sympy-1.9/doc/src/modules/vector/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6134 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/modules/vector/vector_integration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      978 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/outreach.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/pics/
--rw-r--r--   0 runner    (1001) docker     (121)   141216 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/pics/consoleascii.png
--rw-r--r--   0 runner    (1001) docker     (121)   120924 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/pics/consoleunicode.png
--rw-r--r--   0 runner    (1001) docker     (121)    37262 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/pics/ipythonnotebook.png
--rw-r--r--   0 runner    (1001) docker     (121)   244487 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/pics/ipythonqtconsole.png
--rw-r--r--   0 runner    (1001) docker     (121)     3251 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/pics/pngview1.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/special_topics/
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/special_topics/classification.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11892 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/special_topics/finite_diff_derivatives.rst
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/special_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/special_topics/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/doc/src/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)     7059 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/tutorial/basic_operations.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12199 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/tutorial/calculus.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11114 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/tutorial/gotchas.rst
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8428 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/tutorial/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21465 2021-09-30 22:23:57.048183 sympy-1.9/doc/src/tutorial/manipulation.rst
--rw-r--r--   0 runner    (1001) docker     (121)    18034 2021-09-30 22:23:57.052183 sympy-1.9/doc/src/tutorial/matrices.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2021-09-30 22:23:57.052183 sympy-1.9/doc/src/tutorial/preliminaries.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2021-09-30 22:23:57.052183 sympy-1.9/doc/src/tutorial/printing.rst
--rw-r--r--   0 runner    (1001) docker     (121)    29238 2021-09-30 22:23:57.052183 sympy-1.9/doc/src/tutorial/simplification.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7303 2021-09-30 22:23:57.052183 sympy-1.9/doc/src/tutorial/solvers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-09-30 22:23:57.052183 sympy-1.9/doc/src/wiki.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2021-09-30 22:23:57.052183 sympy-1.9/examples/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/examples/advanced/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8893 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/autowrap_integrators.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2388 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/autowrap_ufuncify.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3694 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/curvilinear_coordinates.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1501 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/dense_coding_example.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5567 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/fem.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3544 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/gibbs_phenomenon.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2081 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/grover_example.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      702 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/hydrogen.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2716 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/pidigits.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7178 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/pyglet_plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3401 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/qft.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4312 2021-09-30 22:23:57.052183 sympy-1.9/examples/advanced/relativity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6732 2021-09-30 22:23:57.052183 sympy-1.9/examples/all.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/examples/beginner/
--rwxr-xr-x   0 runner    (1001) docker     (121)      336 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      679 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/differentiation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      361 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/expansion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      394 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      813 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/limits_examples.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1913 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/plot_examples.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      407 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/plotting_nice_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      443 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/precision.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      879 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/print_pretty.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      417 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/series.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      704 2021-09-30 22:23:57.052183 sympy-1.9/examples/beginner/substitution.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/examples/intermediate/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3689 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/coupled_cluster.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      583 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/differential_equations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2914 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/infinite_1d_box.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      965 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/mplot2d.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1248 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/mplot3d.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1981 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/partial_differential_eqs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      384 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/print_gtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/sample.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      717 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/trees.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4638 2021-09-30 22:23:57.052183 sympy-1.9/examples/intermediate/vandermonde.py
--rw-r--r--   0 runner    (1001) docker     (121)    11199 2021-09-30 22:23:57.056183 sympy-1.9/isympy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-09-30 22:23:57.060183 sympy-1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)    14748 2021-09-30 22:23:57.060183 sympy-1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/sympy/
--rw-r--r--   0 runner    (1001) docker     (121)    28517 2021-09-30 22:23:57.060183 sympy-1.9/sympy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2021-09-30 22:23:57.060183 sympy-1.9/sympy/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/sympy/algebras/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-09-30 22:23:57.060183 sympy-1.9/sympy/algebras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21719 2021-09-30 22:23:57.060183 sympy-1.9/sympy/algebras/quaternion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.951351 sympy-1.9/sympy/algebras/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.060183 sympy-1.9/sympy/algebras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8979 2021-09-30 22:23:57.060183 sympy-1.9/sympy/algebras/tests/test_quaternion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/assumptions/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18421 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/ask.py
--rw-r--r--   0 runner    (1001) docker     (121)    17083 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/ask_generated.py
--rw-r--r--   0 runner    (1001) docker     (121)    14321 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/assume.py
--rw-r--r--   0 runner    (1001) docker     (121)    12645 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/cnf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/facts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/assumptions/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7198 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/calculus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    22339 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     7213 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/ntheory.py
--rw-r--r--   0 runner    (1001) docker     (121)    12283 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/order.py
--rw-r--r--   0 runner    (1001) docker     (121)    23164 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/handlers/sets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/assumptions/predicates/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1889 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/calculus.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    12151 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/ntheory.py
--rw-r--r--   0 runner    (1001) docker     (121)     9508 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     8928 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/predicates/sets.py
--rw-r--r--   0 runner    (1001) docker     (121)    12007 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/refine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/assumptions/relation/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/relation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6222 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/relation/binrel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7160 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/relation/equality.py
--rw-r--r--   0 runner    (1001) docker     (121)    11235 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/satask.py
--rw-r--r--   0 runner    (1001) docker     (121)     9466 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/sathandlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/assumptions/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/tests/test_assumptions_2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)    12162 2021-09-30 22:23:57.060183 sympy-1.9/sympy/assumptions/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)    97928 2021-09-30 22:23:57.064183 sympy-1.9/sympy/assumptions/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     8195 2021-09-30 22:23:57.064183 sympy-1.9/sympy/assumptions/tests/test_refine.py
--rw-r--r--   0 runner    (1001) docker     (121)    15442 2021-09-30 22:23:57.064183 sympy-1.9/sympy/assumptions/tests/test_satask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-09-30 22:23:57.064183 sympy-1.9/sympy/assumptions/tests/test_sathandlers.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-09-30 22:23:57.064183 sympy-1.9/sympy/assumptions/tests/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2021-09-30 22:23:57.064183 sympy-1.9/sympy/assumptions/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.064183 sympy-1.9/sympy/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-09-30 22:23:57.064183 sympy-1.9/sympy/benchmarks/bench_discrete_log.py
--rw-r--r--   0 runner    (1001) docker     (121)    11334 2021-09-30 22:23:57.064183 sympy-1.9/sympy/benchmarks/bench_meijerint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2021-09-30 22:23:57.064183 sympy-1.9/sympy/benchmarks/bench_symbench.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/calculus/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3264 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/euler.py
--rw-r--r--   0 runner    (1001) docker     (121)    17466 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)    11369 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/singularities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/calculus/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/tests/test_euler.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/tests/test_finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/tests/test_singularities.py
--rw-r--r--   0 runner    (1001) docker     (121)    24884 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    53951 2021-09-30 22:23:57.064183 sympy-1.9/sympy/calculus/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/categories/
--rw-r--r--   0 runner    (1001) docker     (121)      984 2021-09-30 22:23:57.064183 sympy-1.9/sympy/categories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31444 2021-09-30 22:23:57.064183 sympy-1.9/sympy/categories/baseclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)    95531 2021-09-30 22:23:57.064183 sympy-1.9/sympy/categories/diagram_drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/categories/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.064183 sympy-1.9/sympy/categories/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2021-09-30 22:23:57.064183 sympy-1.9/sympy/categories/tests/test_baseclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)    27838 2021-09-30 22:23:57.064183 sympy-1.9/sympy/categories/tests/test_drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/codegen/
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4865 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/approximations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/array_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    55021 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)    11818 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/cfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/cnodes.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/cutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/cxxnodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    18892 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/fnodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/futils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/matrix_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/numpy_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-09-30 22:23:57.064183 sympy-1.9/sympy/codegen/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11250 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/scipy_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/codegen/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4702 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_applications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_approximations.py
--rw-r--r--   0 runner    (1001) docker     (121)    21355 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4535 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_cfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_cnodes.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_cxxnodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6629 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_fnodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_numpy_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_pyutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13081 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2021-09-30 22:23:57.068184 sympy-1.9/sympy/codegen/tests/test_scipy_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/combinatorics/
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42956 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/coset_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    47977 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/fp_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    40003 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/free_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     7492 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    11237 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/graycode.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/group_constructs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19341 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/homomorphisms.py
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/named_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    20907 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/partitions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21303 2021-09-30 22:23:57.068184 sympy-1.9/sympy/combinatorics/pc_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)   183825 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/perm_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    87583 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/permutations.py
--rw-r--r--   0 runner    (1001) docker     (121)    36023 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/polyhedron.py
--rw-r--r--   0 runner    (1001) docker     (121)    11859 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/prufer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17175 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/rewritingsystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/rewritingsystem_fsm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/schur_number.py
--rw-r--r--   0 runner    (1001) docker     (121)    15858 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/subsets.py
--rw-r--r--   0 runner    (1001) docker     (121)    40758 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tensor_can.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/combinatorics/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28460 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_coset_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    10011 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_fp_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_free_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_graycode.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_group_constructs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_homomorphisms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_named_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     4103 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_partitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_pc_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    39338 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_perm_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    20199 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_permutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_polyhedron.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_prufer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_schur_number.py
--rw-r--r--   0 runner    (1001) docker     (121)     2503 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (121)    24676 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_tensor_can.py
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_testutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    11165 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/testutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    16423 2021-09-30 22:23:57.072184 sympy-1.9/sympy/combinatorics/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.955351 sympy-1.9/sympy/concrete/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10103 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/delta.py
--rw-r--r--   0 runner    (1001) docker     (121)    11332 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/expr_with_intlimits.py
--rw-r--r--   0 runner    (1001) docker     (121)    19401 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/expr_with_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     5559 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/gosper.py
--rw-r--r--   0 runner    (1001) docker     (121)    17373 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/guess.py
--rw-r--r--   0 runner    (1001) docker     (121)    18712 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/products.py
--rw-r--r--   0 runner    (1001) docker     (121)    53769 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/summations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/concrete/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23694 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/tests/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (121)     7640 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/tests/test_gosper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/tests/test_guess.py
--rw-r--r--   0 runner    (1001) docker     (121)    13671 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/tests/test_products.py
--rw-r--r--   0 runner    (1001) docker     (121)    58467 2021-09-30 22:23:57.076184 sympy-1.9/sympy/concrete/tests/test_sums_products.py
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-09-30 22:23:57.076184 sympy-1.9/sympy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/_print_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    41654 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/add.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/alphabets.py
--rw-r--r--   0 runner    (1001) docker     (121)    17828 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    69145 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/core/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/bench_arit.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/bench_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/bench_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/bench_expand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/bench_numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/benchmarks/bench_sympify.py
--rw-r--r--   0 runner    (1001) docker     (121)     4320 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    19705 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     9937 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2870 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/coreerrors.py
--rw-r--r--   0 runner    (1001) docker     (121)     9428 2021-09-30 22:23:57.076184 sympy-1.9/sympy/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    54285 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/evalf.py
--rw-r--r--   0 runner    (1001) docker     (121)   140435 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)    51257 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/exprtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    15735 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/facts.py
--rw-r--r--   0 runner    (1001) docker     (121)   114608 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/function.py
--rw-r--r--   0 runner    (1001) docker     (121)    11587 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/kind.py
--rw-r--r--   0 runner    (1001) docker     (121)    10879 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/logic.py
--rw-r--r--   0 runner    (1001) docker     (121)     7565 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    75406 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/mul.py
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-09-30 22:23:57.080184 sympy-1.9/sympy/core/multidimensional.py
--rw-r--r--   0 runner    (1001) docker     (121)   121934 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)    24320 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3749 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    71834 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/power.py
--rw-r--r--   0 runner    (1001) docker     (121)    46397 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/relational.py
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     6983 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/singleton.py
--rw-r--r--   0 runner    (1001) docker     (121)    26767 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)    19419 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/sympify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/core/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   176679 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (121)    74105 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_arit.py
--rw-r--r--   0 runner    (1001) docker     (121)    39848 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9692 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    21517 2021-09-30 22:23:57.084184 sympy-1.9/sympy/core/tests/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_constructor_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6867 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5017 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_count_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5421 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_equal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (121)    22809 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_evalf.py
--rw-r--r--   0 runner    (1001) docker     (121)    11857 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_expand.py
--rw-r--r--   0 runner    (1001) docker     (121)    71905 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (121)    18053 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_exprtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    11579 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_facts.py
--rw-r--r--   0 runner    (1001) docker     (121)    50134 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)    21787 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_multidimensional.py
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_noncommutative.py
--rw-r--r--   0 runner    (1001) docker     (121)    73112 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2756 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    23116 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (121)    41870 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_relational.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (121)    28941 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_subs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12044 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)    25319 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_sympify.py
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_truediv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/tests/test_var.py
--rw-r--r--   0 runner    (1001) docker     (121)     6183 2021-09-30 22:23:57.088184 sympy-1.9/sympy/core/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2021-09-30 22:23:57.088184 sympy-1.9/sympy/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    89384 2021-09-30 22:23:57.092184 sympy-1.9/sympy/crypto/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/crypto/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.092184 sympy-1.9/sympy/crypto/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19752 2021-09-30 22:23:57.092184 sympy-1.9/sympy/crypto/tests/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/diffgeom/
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    71461 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/diffgeom.py
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/rn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/diffgeom/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/tests/test_class_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)    13542 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/tests/test_diffgeom.py
--rw-r--r--   0 runner    (1001) docker     (121)     5258 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/tests/test_function_diffgeom_book.py
--rw-r--r--   0 runner    (1001) docker     (121)     2583 2021-09-30 22:23:57.092184 sympy-1.9/sympy/diffgeom/tests/test_hyperbolic_space.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/discrete/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14472 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/recurrences.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/discrete/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16950 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/tests/test_recurrences.py
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    11683 2021-09-30 22:23:57.092184 sympy-1.9/sympy/discrete/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/external/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/gmpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7844 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/importtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    11870 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/pythonmpq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/external/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9619 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/test_autowrap.py
--rw-r--r--   0 runner    (1001) docker     (121)    12082 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/test_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/test_importtools.py
--rw-r--r--   0 runner    (1001) docker     (121)     9553 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5605 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/test_pythonmpq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-09-30 22:23:57.092184 sympy-1.9/sympy/external/tests/test_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/functions/
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/functions/combinatorial/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/combinatorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36913 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/combinatorial/factorials.py
--rw-r--r--   0 runner    (1001) docker     (121)    68094 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/combinatorial/numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/functions/combinatorial/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/combinatorial/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25685 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/combinatorial/tests/test_comb_factorials.py
--rw-r--r--   0 runner    (1001) docker     (121)    26322 2021-09-30 22:23:57.092184 sympy-1.9/sympy/functions/combinatorial/tests/test_comb_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.959351 sympy-1.9/sympy/functions/elementary/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/functions/elementary/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/benchmarks/bench_exp.py
--rw-r--r--   0 runner    (1001) docker     (121)    42081 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/complexes.py
--rw-r--r--   0 runner    (1001) docker     (121)    39917 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/exponential.py
--rw-r--r--   0 runner    (1001) docker     (121)    51578 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/hyperbolic.py
--rw-r--r--   0 runner    (1001) docker     (121)    17385 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/integers.py
--rw-r--r--   0 runner    (1001) docker     (121)    26672 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (121)    50105 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/piecewise.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/functions/elementary/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32084 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_complexes.py
--rw-r--r--   0 runner    (1001) docker     (121)    24838 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_exponential.py
--rw-r--r--   0 runner    (1001) docker     (121)    35865 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_hyperbolic.py
--rw-r--r--   0 runner    (1001) docker     (121)    17778 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_integers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    16011 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (121)    50554 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (121)    82448 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/tests/test_trigonometric.py
--rw-r--r--   0 runner    (1001) docker     (121)   108787 2021-09-30 22:23:57.096185 sympy-1.9/sympy/functions/elementary/trigonometric.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/functions/special/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/functions/special/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/benchmarks/bench_special.py
--rw-r--r--   0 runner    (1001) docker     (121)    56887 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/bessel.py
--rw-r--r--   0 runner    (1001) docker     (121)    11724 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/beta_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10225 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/bsplines.py
--rw-r--r--   0 runner    (1001) docker     (121)    20215 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/delta_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14600 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/elliptic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    76545 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    41901 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/gamma_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    37344 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/hyper.py
--rw-r--r--   0 runner    (1001) docker     (121)     6578 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/mathieu_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    40530 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/polynomials.py
--rw-r--r--   0 runner    (1001) docker     (121)     8283 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/singularity_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11112 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/spherical_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (121)    12750 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tensor_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/functions/special/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30238 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_bessel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_beta_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6967 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_bsplines.py
--rw-r--r--   0 runner    (1001) docker     (121)     6838 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_delta_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6532 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_elliptic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    30164 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_error_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    28489 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_gamma_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15314 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_hyper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_mathieu.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_singularity_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15644 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_spec_polynomials.py
--rw-r--r--   0 runner    (1001) docker     (121)     3571 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_spherical_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5354 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_tensor_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9218 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/tests/test_zeta_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21398 2021-09-30 22:23:57.100185 sympy-1.9/sympy/functions/special/zeta_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-30 22:23:57.100185 sympy-1.9/sympy/galgebra.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2021-09-30 22:23:57.100185 sympy-1.9/sympy/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10060 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    50789 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)    20586 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    77083 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/line.py
--rw-r--r--   0 runner    (1001) docker     (121)    10255 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/parabola.py
--rw-r--r--   0 runner    (1001) docker     (121)    27265 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/plane.py
--rw-r--r--   0 runner    (1001) docker     (121)    36678 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (121)    81770 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/geometry/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4267 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    25154 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_geometrysets.py
--rw-r--r--   0 runner    (1001) docker     (121)    35532 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     5170 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_parabola.py
--rw-r--r--   0 runner    (1001) docker     (121)    12341 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)    15918 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (121)    26869 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    19471 2021-09-30 22:23:57.104185 sympy-1.9/sympy/geometry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/holonomic/
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-09-30 22:23:57.104185 sympy-1.9/sympy/holonomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    94482 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/holonomic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/holonomicerrors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/numerical.py
--rw-r--r--   0 runner    (1001) docker     (121)    10983 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/recurrence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/holonomic/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34042 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/tests/test_holonomic.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2021-09-30 22:23:57.108185 sympy-1.9/sympy/holonomic/tests/test_recurrence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/benchmarks/bench_integrate.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/benchmarks/bench_trigintegrate.py
--rw-r--r--   0 runner    (1001) docker     (121)     7426 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/deltafunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)    25487 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/heurisch.py
--rw-r--r--   0 runner    (1001) docker     (121)    63943 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    43221 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/intpoly.py
--rw-r--r--   0 runner    (1001) docker     (121)    63318 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/manualintegrate.py
--rw-r--r--   0 runner    (1001) docker     (121)    78435 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/meijerint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/meijerint_doc.py
--rw-r--r--   0 runner    (1001) docker     (121)    51995 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/prde.py
--rw-r--r--   0 runner    (1001) docker     (121)    17012 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (121)    10585 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/rationaltools.py
--rw-r--r--   0 runner    (1001) docker     (121)    27182 2021-09-30 22:23:57.108185 sympy-1.9/sympy/integrals/rde.py
--rw-r--r--   0 runner    (1001) docker     (121)    67527 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/risch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/rubi/
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   295122 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/rubi/parsetools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/generate_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/generate_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     9374 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/header.py.txt
--rw-r--r--   0 runner    (1001) docker     (121)    27553 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/rubi/parsetools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8211 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/parsetools/tests/test_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/rubi/rubi_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/rubi_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.963351 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30426 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_1_2.py
--rw-r--r--   0 runner    (1001) docker     (121)    61185 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)    10426 2021-09-30 22:23:57.112185 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_1_4.py
--rw-r--r--   0 runner    (1001) docker     (121)   250958 2021-09-30 22:23:57.116186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_exponential.py
--rw-r--r--   0 runner    (1001) docker     (121)    79552 2021-09-30 22:23:57.116186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_hyperbolic_sine.py
--rw-r--r--   0 runner    (1001) docker     (121)    65172 2021-09-30 22:23:57.116186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_inverse_hyperbolic_sine.py
--rw-r--r--   0 runner    (1001) docker     (121)    84206 2021-09-30 22:23:57.116186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_inverse_sine.py
--rw-r--r--   0 runner    (1001) docker     (121)   442127 2021-09-30 22:23:57.116186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_logarithms.py
--rw-r--r--   0 runner    (1001) docker     (121)   526173 2021-09-30 22:23:57.120186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_miscellaneous_algebra.py
--rw-r--r--   0 runner    (1001) docker     (121)    93397 2021-09-30 22:23:57.120186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_secant.py
--rw-r--r--   0 runner    (1001) docker     (121)   164373 2021-09-30 22:23:57.120186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_sine.py
--rw-r--r--   0 runner    (1001) docker     (121)    48347 2021-09-30 22:23:57.120186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_special_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)   132374 2021-09-30 22:23:57.120186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_tangent.py
--rw-r--r--   0 runner    (1001) docker     (121)  1508403 2021-09-30 22:23:57.124186 sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_trinomials.py
--rw-r--r--   0 runner    (1001) docker     (121)     8104 2021-09-30 22:23:57.124186 sympy-1.9/sympy/integrals/rubi/rubimain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/integrals/rubi/rules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.124186 sympy-1.9/sympy/integrals/rubi/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   199170 2021-09-30 22:23:57.128186 sympy-1.9/sympy/integrals/rubi/rules/binomial_products.py
--rw-r--r--   0 runner    (1001) docker     (121)    62876 2021-09-30 22:23:57.128186 sympy-1.9/sympy/integrals/rubi/rules/exponential.py
--rw-r--r--   0 runner    (1001) docker     (121)   218004 2021-09-30 22:23:57.132186 sympy-1.9/sympy/integrals/rubi/rules/hyperbolic.py
--rw-r--r--   0 runner    (1001) docker     (121)    23181 2021-09-30 22:23:57.132186 sympy-1.9/sympy/integrals/rubi/rules/integrand_simplification.py
--rw-r--r--   0 runner    (1001) docker     (121)   350893 2021-09-30 22:23:57.132186 sympy-1.9/sympy/integrals/rubi/rules/inverse_hyperbolic.py
--rw-r--r--   0 runner    (1001) docker     (121)   317185 2021-09-30 22:23:57.132186 sympy-1.9/sympy/integrals/rubi/rules/inverse_trig.py
--rw-r--r--   0 runner    (1001) docker     (121)    91552 2021-09-30 22:23:57.132186 sympy-1.9/sympy/integrals/rubi/rules/linear_products.py
--rw-r--r--   0 runner    (1001) docker     (121)    97838 2021-09-30 22:23:57.136186 sympy-1.9/sympy/integrals/rubi/rules/logarithms.py
--rw-r--r--   0 runner    (1001) docker     (121)   232625 2021-09-30 22:23:57.136186 sympy-1.9/sympy/integrals/rubi/rules/miscellaneous_algebraic.py
--rw-r--r--   0 runner    (1001) docker     (121)    50567 2021-09-30 22:23:57.136186 sympy-1.9/sympy/integrals/rubi/rules/miscellaneous_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)   189265 2021-09-30 22:23:57.136186 sympy-1.9/sympy/integrals/rubi/rules/miscellaneous_trig.py
--rw-r--r--   0 runner    (1001) docker     (121)    19898 2021-09-30 22:23:57.136186 sympy-1.9/sympy/integrals/rubi/rules/piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (121)   317214 2021-09-30 22:23:57.140187 sympy-1.9/sympy/integrals/rubi/rules/quadratic_products.py
--rw-r--r--   0 runner    (1001) docker     (121)   450602 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/rules/secant.py
--rw-r--r--   0 runner    (1001) docker     (121)   733180 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/rules/sine.py
--rw-r--r--   0 runner    (1001) docker     (121)    89418 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/rules/special_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)   314352 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/rules/tangent.py
--rw-r--r--   0 runner    (1001) docker     (121)   242580 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/rules/trinomial_products.py
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/integrals/rubi/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/tests/test_rubi_integrate.py
--rw-r--r--   0 runner    (1001) docker     (121)    81616 2021-09-30 22:23:57.144187 sympy-1.9/sympy/integrals/rubi/tests/test_utility_function.py
--rw-r--r--   0 runner    (1001) docker     (121)   269192 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/rubi/utility_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/singularityfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/integrals/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3495 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_deltafunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7027 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_failing_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_heurisch.py
--rw-r--r--   0 runner    (1001) docker     (121)    66544 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    36169 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_intpoly.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_lineintegrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    25950 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_manual.py
--rw-r--r--   0 runner    (1001) docker     (121)    30204 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_meijerint.py
--rw-r--r--   0 runner    (1001) docker     (121)    16117 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_prde.py
--rw-r--r--   0 runner    (1001) docker     (121)    19919 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (121)     4979 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_rationaltools.py
--rw-r--r--   0 runner    (1001) docker     (121)     9494 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_rde.py
--rw-r--r--   0 runner    (1001) docker     (121)    37245 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_risch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_singularityfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)    38189 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3869 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/tests/test_trigonometry.py
--rw-r--r--   0 runner    (1001) docker     (121)    69129 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    11080 2021-09-30 22:23:57.148187 sympy-1.9/sympy/integrals/trigonometry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/interactive/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-09-30 22:23:57.148187 sympy-1.9/sympy/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-09-30 22:23:57.148187 sympy-1.9/sympy/interactive/ipythonprinting.py
--rw-r--r--   0 runner    (1001) docker     (121)    22933 2021-09-30 22:23:57.152187 sympy-1.9/sympy/interactive/printing.py
--rw-r--r--   0 runner    (1001) docker     (121)    15401 2021-09-30 22:23:57.152187 sympy-1.9/sympy/interactive/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/interactive/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.152187 sympy-1.9/sympy/interactive/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2021-09-30 22:23:57.152187 sympy-1.9/sympy/interactive/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2021-09-30 22:23:57.152187 sympy-1.9/sympy/interactive/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)     9501 2021-09-30 22:23:57.152187 sympy-1.9/sympy/interactive/tests/test_ipythonprinting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/liealgebras/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/cartan_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/cartan_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/dynkin_diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/root_system.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/liealgebras/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_cartan_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_cartan_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_dynkin_diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_root_system.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_A.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_B.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_C.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_D.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_E.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_F.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_type_G.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/tests/test_weyl_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_a.py
--rw-r--r--   0 runner    (1001) docker     (121)     4564 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_b.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_c.py
--rw-r--r--   0 runner    (1001) docker     (121)     4694 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_d.py
--rw-r--r--   0 runner    (1001) docker     (121)     9781 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_e.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_f.py
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/type_g.py
--rw-r--r--   0 runner    (1001) docker     (121)    14725 2021-09-30 22:23:57.152187 sympy-1.9/sympy/liealgebras/weyl_group.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/logic/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/logic/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9175 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/algorithms/dpll.py
--rw-r--r--   0 runner    (1001) docker     (121)    20379 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/algorithms/dpll2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/algorithms/minisat22_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/algorithms/pycosat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    98003 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/boolalg.py
--rw-r--r--   0 runner    (1001) docker     (121)     8582 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/logic/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    45827 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/tests/test_boolalg.py
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/tests/test_dimacs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13169 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/tests/test_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/logic/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-09-30 22:23:57.152187 sympy-1.9/sympy/logic/utilities/dimacs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/matrices/
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-09-30 22:23:57.152187 sympy-1.9/sympy/matrices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/matrices/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.152187 sympy-1.9/sympy/matrices/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-09-30 22:23:57.152187 sympy-1.9/sympy/matrices/benchmarks/bench_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    96132 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    48092 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/decompositions.py
--rw-r--r--   0 runner    (1001) docker     (121)    20272 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/dense.py
--rw-r--r--   0 runner    (1001) docker     (121)     5485 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/densearith.py
--rw-r--r--   0 runner    (1001) docker     (121)    11704 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/densesolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     5473 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/densetools.py
--rw-r--r--   0 runner    (1001) docker     (121)    30219 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/determinant.py
--rw-r--r--   0 runner    (1001) docker     (121)    40170 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/eigen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.967351 sympy-1.9/sympy/matrices/expressions/
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     6604 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/applyfunc.py
--rw-r--r--   0 runner    (1001) docker     (121)    31501 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/blockmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/companion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/determinant.py
--rw-r--r--   0 runner    (1001) docker     (121)     6143 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/diagonal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/dotproduct.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/factorizations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/funcmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    13782 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/hadamard.py
--rw-r--r--   0 runner    (1001) docker     (121)     2699 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/inverse.py
--rw-r--r--   0 runner    (1001) docker     (121)    13438 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/kronecker.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/matadd.py
--rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/matexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)    13924 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/matmul.py
--rw-r--r--   0 runner    (1001) docker     (121)     5074 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/matpow.py
--rw-r--r--   0 runner    (1001) docker     (121)     8028 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/permutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     6942 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/special.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/matrices/expressions/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_applyfunc.py
--rw-r--r--   0 runner    (1001) docker     (121)    14559 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_blockmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_companion.py
--rw-r--r--   0 runner    (1001) docker     (121)    14717 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_determinant.py
--rw-r--r--   0 runner    (1001) docker     (121)     4294 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_dotproduct.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_factorizations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_funcmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2021-09-30 22:23:57.156187 sympy-1.9/sympy/matrices/expressions/tests/test_hadamard.py
--rw-r--r--   0 runner    (1001) docker     (121)    10373 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_kronecker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_matadd.py
--rw-r--r--   0 runner    (1001) docker     (121)    15718 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_matexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5212 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (121)     6241 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_matpow.py
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     6622 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_special.py
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (121)     4963 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/trace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/expressions/transpose.py
--rw-r--r--   0 runner    (1001) docker     (121)     9076 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/immutable.py
--rw-r--r--   0 runner    (1001) docker     (121)    11376 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/inverse.py
--rw-r--r--   0 runner    (1001) docker     (121)    77907 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/normalforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    10179 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/reductions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21431 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/repmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    22801 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14567 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     9182 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/sparsetools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/subspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/matrices/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38812 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_commonmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    13853 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_decompositions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_densearith.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_densesolve.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_densetools.py
--rw-r--r--   0 runner    (1001) docker     (121)    12876 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_determinant.py
--rw-r--r--   0 runner    (1001) docker     (121)    21681 2021-09-30 22:23:57.160187 sympy-1.9/sympy/matrices/tests/test_eigen.py
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_interactions.py
--rw-r--r--   0 runner    (1001) docker     (121)   142839 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_normalforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    13909 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_reductions.py
--rw-r--r--   0 runner    (1001) docker     (121)    20225 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)    22482 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     4834 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_sparsetools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3839 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/tests/test_subspaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-09-30 22:23:57.164188 sympy-1.9/sympy/matrices/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/multipledispatch/
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/conflict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    12233 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/multipledispatch/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/tests/test_conflict.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     6205 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-09-30 22:23:57.164188 sympy-1.9/sympy/multipledispatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/ntheory/
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5213 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/bbp_pi.py
--rw-r--r--   0 runner    (1001) docker     (121)    10075 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/continued_fraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3692 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/digits.py
--rw-r--r--   0 runner    (1001) docker     (121)    10141 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/ecm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6810 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/egyptian_fraction.py
--rw-r--r--   0 runner    (1001) docker     (121)    11473 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/elliptic_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    75312 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/factor_.py
--rw-r--r--   0 runner    (1001) docker     (121)    30338 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/modular.py
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/multinomial.py
--rw-r--r--   0 runner    (1001) docker     (121)     5970 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/partitions_.py
--rw-r--r--   0 runner    (1001) docker     (121)    19378 2021-09-30 22:23:57.164188 sympy-1.9/sympy/ntheory/primetest.py
--rw-r--r--   0 runner    (1001) docker     (121)    18418 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/qs.py
--rw-r--r--   0 runner    (1001) docker     (121)    39856 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/residue_ntheory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/ntheory/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9422 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_bbp_pi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_continued_fraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_digits.py
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_ecm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_egyptian_fraction.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_elliptic_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    24601 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_factor_.py
--rw-r--r--   0 runner    (1001) docker     (121)     7927 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_modular.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_multinomial.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_partitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7049 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_primetest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_qs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12856 2021-09-30 22:23:57.168188 sympy-1.9/sympy/ntheory/tests/test_residue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/parsing/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/ast_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/parsing/autolev/
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/Autolev.g4
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/parsing/autolev/_antlr/
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/_antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16845 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/_antlr/autolevlexer.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/_antlr/autolevlistener.py
--rw-r--r--   0 runner    (1001) docker     (121)   111528 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/_antlr/autolevparser.py
--rw-r--r--   0 runner    (1001) docker     (121)   104758 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/_listener_autolev_antlr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/_parse_autolev_antlr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/parsing/autolev/test-examples/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.al
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/double_pendulum.al
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/mass_spring_damper.al
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/mass_spring_damper.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/non_min_pendulum.al
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/non_min_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest1.al
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest1.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest10.al
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest10.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest11.al
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest11.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest12.al
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest12.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest2.al
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest2.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest3.al
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest3.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest4.al
--rw-r--r--   0 runner    (1001) docker     (121)      682 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest4.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest5.al
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest5.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest6.al
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest6.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest7.al
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest7.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2021-09-30 22:23:57.168188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest8.al
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest8.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest9.al
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/autolev/test-examples/ruletest9.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.971351 sympy-1.9/sympy/parsing/c/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39276 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/c/c_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/parsing/fortran/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11598 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/fortran/fortran_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/parsing/latex/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5614 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/LaTeX.g4
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/parsing/latex/_antlr/
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/_antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37558 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/_antlr/latexlexer.py
--rw-r--r--   0 runner    (1001) docker     (121)   124634 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/_antlr/latexparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/_build_latex_antlr.py
--rw-r--r--   0 runner    (1001) docker     (121)    19866 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/_parse_latex_antlr.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/latex/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    12987 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/mathematica.py
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/maxima.py
--rw-r--r--   0 runner    (1001) docker     (121)     8894 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/sym_expr.py
--rw-r--r--   0 runner    (1001) docker     (121)    38725 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/sympy_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/parsing/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_ast_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     6610 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_autolev.py
--rw-r--r--   0 runner    (1001) docker     (121)   154616 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_c_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    11816 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_fortran_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7449 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_implicit_multiplication_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     9968 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_latex.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_mathematica.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_maxima.py
--rw-r--r--   0 runner    (1001) docker     (121)     5657 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_sym_expr.py
--rw-r--r--   0 runner    (1001) docker     (121)     9375 2021-09-30 22:23:57.172188 sympy-1.9/sympy/parsing/tests/test_sympy_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-09-30 22:23:57.172188 sympy-1.9/sympy/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/continuum_mechanics/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-09-30 22:23:57.172188 sympy-1.9/sympy/physics/continuum_mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   145108 2021-09-30 22:23:57.172188 sympy-1.9/sympy/physics/continuum_mechanics/beam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/continuum_mechanics/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/continuum_mechanics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26123 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/continuum_mechanics/tests/test_beam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/control/
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30102 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/control/control_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)   111602 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/control/lti.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/control/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/control/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15573 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/control/tests/test_control_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    58453 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/control/tests/test_lti.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/gaussopt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/hep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/hep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24184 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/hep/gamma_matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/hep/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/hep/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13812 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/hep/tests/test_gamma_matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/hydrogen.py
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/mechanics/
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17568 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/body.py
--rw-r--r--   0 runner    (1001) docker     (121)    23459 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    24437 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/joint.py
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/jointsmethod.py
--rw-r--r--   0 runner    (1001) docker     (121)    27263 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/kane.py
--rw-r--r--   0 runner    (1001) docker     (121)    18316 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/lagrange.py
--rw-r--r--   0 runner    (1001) docker     (121)    15349 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/linearize.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/method.py
--rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7577 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/particle.py
--rw-r--r--   0 runner    (1001) docker     (121)    10807 2021-09-30 22:23:57.176188 sympy-1.9/sympy/physics/mechanics/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (121)    18655 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/system.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/mechanics/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9288 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (121)     9101 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    20576 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_joint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_jointsmethod.py
--rw-r--r--   0 runner    (1001) docker     (121)    13422 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_kane.py
--rw-r--r--   0 runner    (1001) docker     (121)    19025 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_kane2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14271 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_kane3.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_kane4.py
--rw-r--r--   0 runner    (1001) docker     (121)     9407 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_lagrange2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11745 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_particle.py
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (121)     8695 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/mechanics/tests/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/optics/
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20313 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/gaussopt.py
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/medium.py
--rw-r--r--   0 runner    (1001) docker     (121)    21201 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/polarization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/optics/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/tests/test_gaussopt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/tests/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/tests/test_polarization.py
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/tests/test_waves.py
--rw-r--r--   0 runner    (1001) docker     (121)    21468 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9575 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/optics/waves.py
--rw-r--r--   0 runner    (1001) docker     (121)     5890 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/paulialgebra.py
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/pring.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/qho_1d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.975351 sympy-1.9/sympy/physics/quantum/
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/anticommutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6095 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/boson.py
--rw-r--r--   0 runner    (1001) docker     (121)     8810 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (121)    23033 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/cg.py
--rw-r--r--   0 runner    (1001) docker     (121)    11945 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/circuitplot.py
--rw-r--r--   0 runner    (1001) docker     (121)    13807 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/circuitutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/commutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/dagger.py
--rw-r--r--   0 runner    (1001) docker     (121)     9497 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/density.py
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2021-09-30 22:23:57.180188 sympy-1.9/sympy/physics/quantum/fermion.py
--rw-r--r--   0 runner    (1001) docker     (121)    41687 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/gate.py
--rw-r--r--   0 runner    (1001) docker     (121)     9804 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/grover.py
--rw-r--r--   0 runner    (1001) docker     (121)    19449 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/hilbert.py
--rw-r--r--   0 runner    (1001) docker     (121)    27466 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/identitysearch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/innerproduct.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/matrixcache.py
--rw-r--r--   0 runner    (1001) docker     (121)     8412 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/matrixutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19023 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11504 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/operatorordering.py
--rw-r--r--   0 runner    (1001) docker     (121)     9598 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/operatorset.py
--rw-r--r--   0 runner    (1001) docker     (121)    17262 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/pauli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/piab.py
--rw-r--r--   0 runner    (1001) docker     (121)     7021 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/qapply.py
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/qasm.py
--rw-r--r--   0 runner    (1001) docker     (121)    14144 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/qexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/qft.py
--rw-r--r--   0 runner    (1001) docker     (121)    25628 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/qubit.py
--rw-r--r--   0 runner    (1001) docker     (121)    18277 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/represent.py
--rw-r--r--   0 runner    (1001) docker     (121)    20844 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/sho1d.py
--rw-r--r--   0 runner    (1001) docker     (121)     5371 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/shor.py
--rw-r--r--   0 runner    (1001) docker     (121)    72785 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/spin.py
--rw-r--r--   0 runner    (1001) docker     (121)    30432 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/state.py
--rw-r--r--   0 runner    (1001) docker     (121)    14482 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tensorproduct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/quantum/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_anticommutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_boson.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (121)     8715 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_cg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_circuitplot.py
--rw-r--r--   0 runner    (1001) docker     (121)    13119 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_circuitutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_commutator.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_dagger.py
--rw-r--r--   0 runner    (1001) docker     (121)     9598 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_fermion.py
--rw-r--r--   0 runner    (1001) docker     (121)    12322 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_gate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_hilbert.py
--rw-r--r--   0 runner    (1001) docker     (121)    17706 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_identitysearch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_innerproduct.py
--rw-r--r--   0 runner    (1001) docker     (121)     4063 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_matrixutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6946 2021-09-30 22:23:57.184188 sympy-1.9/sympy/physics/quantum/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_operatorordering.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_operatorset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_pauli.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_piab.py
--rw-r--r--   0 runner    (1001) docker     (121)    30068 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4438 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_qapply.py
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_qasm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_qexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_qft.py
--rw-r--r--   0 runner    (1001) docker     (121)     8782 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_qubit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5119 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_represent.py
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_sho1d.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_shor.py
--rw-r--r--   0 runner    (1001) docker     (121)   344475 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_spin.py
--rw-r--r--   0 runner    (1001) docker     (121)     6391 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/quantum/tests/test_tensorproduct.py
--rw-r--r--   0 runner    (1001) docker     (121)    89896 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/secondquant.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/sho.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9241 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_clebsch_gordan.py
--rw-r--r--   0 runner    (1001) docker     (121)     4689 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_hydrogen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_paulialgebra.py
--rw-r--r--   0 runner    (1001) docker     (121)     2815 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_physics_matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_pring.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_qho_1d.py
--rw-r--r--   0 runner    (1001) docker     (121)    48231 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_secondquant.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/tests/test_sho.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/units/
--rw-r--r--   0 runner    (1001) docker     (121)    12011 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/units/definitions/
--rw-r--r--   0 runner    (1001) docker     (121)     7194 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/units/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/units/definitions/dimension_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13695 2021-09-30 22:23:57.188189 sympy-1.9/sympy/physics/units/definitions/unit_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)    23549 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5938 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7381 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/units/systems/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/cgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/length_weight_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/mks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/mksa.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/natural.py
--rw-r--r--   0 runner    (1001) docker     (121)    13649 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/systems/si.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/units/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5894 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_dimensionsystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_prefixes.py
--rw-r--r--   0 runner    (1001) docker     (121)    16089 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_quantities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_unit_system_cgs_gauss.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_unitsystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     6314 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     7453 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/unitsystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     7741 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/units/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/vector/
--rw-r--r--   0 runner    (1001) docker     (121)      985 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19382 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/dyadic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8513 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/fieldfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)    52776 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/frame.py
--rw-r--r--   0 runner    (1001) docker     (121)    24510 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    20602 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/point.py
--rw-r--r--   0 runner    (1001) docker     (121)    11776 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/printing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/physics/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4153 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_dyadic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5727 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_fieldfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21731 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (121)    20546 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (121)    10131 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (121)    10284 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (121)     7762 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)    26436 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/vector/vector.py
--rw-r--r--   0 runner    (1001) docker     (121)    31382 2021-09-30 22:23:57.192189 sympy-1.9/sympy/physics/wigner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-09-30 22:23:57.192189 sympy-1.9/sympy/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22892 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/experimental_lambdify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/plotting/intervalmath/
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15530 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/interval_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/interval_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)    14809 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/lib_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/plotting/intervalmath/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9862 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/tests/test_interval_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4216 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/tests/test_interval_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)     9034 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/intervalmath/tests/test_intervalmath.py
--rw-r--r--   0 runner    (1001) docker     (121)    90816 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    15550 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/plot_implicit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/plotting/pygletplot/
--rw-r--r--   0 runner    (1001) docker     (121)     3732 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12456 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/color_scheme.py
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/managed_window.py
--rw-r--r--   0 runner    (1001) docker     (121)    13324 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8655 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_axes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4001 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     6941 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)     5362 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_interval.py
--rw-r--r--   0 runner    (1001) docker     (121)    14113 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)    11496 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_mode_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5333 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_modes.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_rotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3811 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4838 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/plot_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/plotting/pygletplot/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/pygletplot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.979351 sympy-1.9/sympy/plotting/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_experimental_lambdify.py
--rw-r--r--   0 runner    (1001) docker     (121)    23787 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_plot_implicit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_region_and.png
--rw-r--r--   0 runner    (1001) docker     (121)     7939 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_region_not.png
--rw-r--r--   0 runner    (1001) docker     (121)     8809 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_region_or.png
--rw-r--r--   0 runner    (1001) docker     (121)    10002 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_region_xor.png
--rw-r--r--   0 runner    (1001) docker     (121)    12191 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/tests/test_textplot.py
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2021-09-30 22:23:57.196189 sympy-1.9/sympy/plotting/textplot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2021-09-30 22:23:57.196189 sympy-1.9/sympy/polys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/agca/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-09-30 22:23:57.196189 sympy-1.9/sympy/polys/agca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-09-30 22:23:57.196189 sympy-1.9/sympy/polys/agca/extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21937 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/homomorphisms.py
--rw-r--r--   0 runner    (1001) docker     (121)    10788 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/ideals.py
--rw-r--r--   0 runner    (1001) docker     (121)    46881 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/agca/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/tests/test_homomorphisms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/tests/test_ideals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13539 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/agca/tests/test_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/benchmarks/bench_galoispolys.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/benchmarks/bench_groebnertools.py
--rw-r--r--   0 runner    (1001) docker     (121)   446790 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/benchmarks/bench_solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)    57410 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)    11480 2021-09-30 22:23:57.200189 sympy-1.9/sympy/polys/constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)    33396 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/densearith.py
--rw-r--r--   0 runner    (1001) docker     (121)    35901 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/densebasic.py
--rw-r--r--   0 runner    (1001) docker     (121)    25891 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/densetools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (121)    21781 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/distributedmodules.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domainmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/domains/
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14715 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/algebraicfield.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/characteristiczero.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/complexfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/compositedomain.py
--rw-r--r--   0 runner    (1001) docker     (121)    35140 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/domain.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/domainelement.py
--rw-r--r--   0 runner    (1001) docker     (121)     6907 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/expressiondomain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/expressionrawdomain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2591 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/field.py
--rw-r--r--   0 runner    (1001) docker     (121)     6022 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/finitefield.py
--rw-r--r--   0 runner    (1001) docker     (121)     5945 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/fractionfield.py
--rw-r--r--   0 runner    (1001) docker     (121)    18005 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/gaussiandomains.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/gmpyfinitefield.py
--rw-r--r--   0 runner    (1001) docker     (121)     3017 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/gmpyintegerring.py
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/gmpyrationalfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/groundtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5823 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/integerring.py
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/modularinteger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4616 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/mpelements.py
--rw-r--r--   0 runner    (1001) docker     (121)     6178 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/old_fractionfield.py
--rw-r--r--   0 runner    (1001) docker     (121)    14912 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/old_polynomialring.py
--rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/polynomialring.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/pythonfinitefield.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/pythonintegerring.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/pythonrational.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/pythonrationalfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/quotientring.py
--rw-r--r--   0 runner    (1001) docker     (121)     4608 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/rationalfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/realfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/ring.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/simpledomain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/domains/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41388 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/tests/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/tests/test_polynomialring.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/domains/tests/test_quotientring.py
--rw-r--r--   0 runner    (1001) docker     (121)    41215 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/euclidtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    38036 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/factortools.py
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2021-09-30 22:23:57.204189 sympy-1.9/sympy/polys/fglmtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    21205 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    51834 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/galoistools.py
--rw-r--r--   0 runner    (1001) docker     (121)    23339 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/groebnertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3732 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/heuristicgcd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/matrices/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12319 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/ddm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8255 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/dense.py
--rw-r--r--   0 runner    (1001) docker     (121)    40398 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/domainmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3643 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/domainscalar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/eigen.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6749 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/linsolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/normalforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    34639 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/sdm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.983351 sympy-1.9/sympy/polys/matrices/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14440 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_ddm.py
--rw-r--r--   0 runner    (1001) docker     (121)     9479 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (121)    29619 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_domainmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_domainscalar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_eigen.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_linsolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_normalforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    12794 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/matrices/tests/test_sdm.py
--rw-r--r--   0 runner    (1001) docker     (121)    58652 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/modulargcd.py
--rw-r--r--   0 runner    (1001) docker     (121)    18968 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/monomials.py
--rw-r--r--   0 runner    (1001) docker     (121)    14915 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/multivariate_resultants.py
--rw-r--r--   0 runner    (1001) docker     (121)    34132 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/numberfields.py
--rw-r--r--   0 runner    (1001) docker     (121)     8515 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/orderings.py
--rw-r--r--   0 runner    (1001) docker     (121)    10096 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/orthopolys.py
--rw-r--r--   0 runner    (1001) docker     (121)    14661 2021-09-30 22:23:57.208190 sympy-1.9/sympy/polys/partfrac.py
--rw-r--r--   0 runner    (1001) docker     (121)    53300 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     4519 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyerrors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10258 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9749 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polymatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    21995 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyoptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    96034 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyquinticconst.py
--rw-r--r--   0 runner    (1001) docker     (121)    33603 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyroots.py
--rw-r--r--   0 runner    (1001) docker     (121)   186927 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polytools.py
--rw-r--r--   0 runner    (1001) docker     (121)    14113 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/polyutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/rationaltools.py
--rw-r--r--   0 runner    (1001) docker     (121)    57846 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/ring_series.py
--rw-r--r--   0 runner    (1001) docker     (121)    69021 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/rings.py
--rw-r--r--   0 runner    (1001) docker     (121)    60650 2021-09-30 22:23:57.212190 sympy-1.9/sympy/polys/rootisolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    39800 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/rootoftools.py
--rw-r--r--   0 runner    (1001) docker     (121)    13346 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11087 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/specialpolys.py
--rw-r--r--   0 runner    (1001) docker     (121)    11464 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/sqfreetools.py
--rw-r--r--   0 runner    (1001) docker     (121)    87900 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/subresultants_qq_zz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/polys/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6160 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)    40017 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_densearith.py
--rw-r--r--   0 runner    (1001) docker     (121)    21464 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_densebasic.py
--rw-r--r--   0 runner    (1001) docker     (121)    24475 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_densetools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (121)     7639 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_distributedmodules.py
--rw-r--r--   0 runner    (1001) docker     (121)    19482 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_euclidtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    24409 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_factortools.py
--rw-r--r--   0 runner    (1001) docker     (121)    10128 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    27866 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_galoistools.py
--rw-r--r--   0 runner    (1001) docker     (121)    18584 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_groebnertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_heuristicgcd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_injections.py
--rw-r--r--   0 runner    (1001) docker     (121)     9007 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_modulargcd.py
--rw-r--r--   0 runner    (1001) docker     (121)    10988 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_monomials.py
--rw-r--r--   0 runner    (1001) docker     (121)     9453 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_multivariate_resultants.py
--rw-r--r--   0 runner    (1001) docker     (121)    35418 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_numberfields.py
--rw-r--r--   0 runner    (1001) docker     (121)     4254 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_orderings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5322 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_orthopolys.py
--rw-r--r--   0 runner    (1001) docker     (121)     6880 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_partfrac.py
--rw-r--r--   0 runner    (1001) docker     (121)    13070 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_polyclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_polyfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7218 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_polymatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    12320 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_polyoptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    25246 2021-09-30 22:23:57.216190 sympy-1.9/sympy/polys/tests/test_polyroots.py
--rw-r--r--   0 runner    (1001) docker     (121)   120860 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_polytools.py
--rw-r--r--   0 runner    (1001) docker     (121)    11223 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_polyutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4143 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_pythonrational.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_rationaltools.py
--rw-r--r--   0 runner    (1001) docker     (121)    24233 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_ring_series.py
--rw-r--r--   0 runner    (1001) docker     (121)    43182 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_rings.py
--rw-r--r--   0 runner    (1001) docker     (121)    31460 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_rootisolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    19906 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_rootoftools.py
--rw-r--r--   0 runner    (1001) docker     (121)    13655 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4795 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_specialpolys.py
--rw-r--r--   0 runner    (1001) docker     (121)     4387 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_sqfreetools.py
--rw-r--r--   0 runner    (1001) docker     (121)    13091 2021-09-30 22:23:57.220190 sympy-1.9/sympy/polys/tests/test_subresultants_qq_zz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/printing/
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17803 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/aesaracode.py
--rw-r--r--   0 runner    (1001) docker     (121)    26762 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/c.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/ccode.py
--rw-r--r--   0 runner    (1001) docker     (121)    32612 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/codeprinter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5665 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/cxx.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/cxxcode.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     8285 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/dot.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/fcode.py
--rw-r--r--   0 runner    (1001) docker     (121)    28305 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/fortran.py
--rw-r--r--   0 runner    (1001) docker     (121)    20494 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/glsl.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/gtk.py
--rw-r--r--   0 runner    (1001) docker     (121)    11494 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/jscode.py
--rw-r--r--   0 runner    (1001) docker     (121)    22646 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/julia.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-09-30 22:23:57.220190 sympy-1.9/sympy/printing/lambdarepr.py
--rw-r--r--   0 runner    (1001) docker     (121)   113920 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/latex.py
--rw-r--r--   0 runner    (1001) docker     (121)    16709 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/llvmjitcode.py
--rw-r--r--   0 runner    (1001) docker     (121)    10347 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/maple.py
--rw-r--r--   0 runner    (1001) docker     (121)    12417 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/mathematica.py
--rw-r--r--   0 runner    (1001) docker     (121)    75196 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/mathml.py
--rw-r--r--   0 runner    (1001) docker     (121)    19395 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)    25522 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/octave.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/precedence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/printing/pretty/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pretty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   103452 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pretty/pretty.py
--rw-r--r--   0 runner    (1001) docker     (121)    20063 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pretty/pretty_symbology.py
--rw-r--r--   0 runner    (1001) docker     (121)    18737 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pretty/stringpict.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/printing/pretty/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pretty/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   176127 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pretty/tests/test_pretty.py
--rw-r--r--   0 runner    (1001) docker     (121)    11806 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/preview.py
--rw-r--r--   0 runner    (1001) docker     (121)    14472 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/printer.py
--rw-r--r--   0 runner    (1001) docker     (121)    19966 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/pycode.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/python.py
--rw-r--r--   0 runner    (1001) docker     (121)    14603 2021-09-30 22:23:57.224190 sympy-1.9/sympy/printing/rcode.py
--rw-r--r--   0 runner    (1001) docker     (121)    11607 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/repr.py
--rw-r--r--   0 runner    (1001) docker     (121)    20957 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/rust.py
--rw-r--r--   0 runner    (1001) docker     (121)    32901 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/str.py
--rw-r--r--   0 runner    (1001) docker     (121)    11694 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tableform.py
--rw-r--r--   0 runner    (1001) docker     (121)    10750 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/printing/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20827 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_aesaracode.py
--rw-r--r--   0 runner    (1001) docker     (121)    28967 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_c.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_codeprinter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_cupy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2453 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_cxx.py
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_dot.py
--rw-r--r--   0 runner    (1001) docker     (121)    33854 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_fortran.py
--rw-r--r--   0 runner    (1001) docker     (121)    28787 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_glsl.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_gtk.py
--rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_jscode.py
--rw-r--r--   0 runner    (1001) docker     (121)    13517 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_julia.py
--rw-r--r--   0 runner    (1001) docker     (121)     6544 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_lambdarepr.py
--rw-r--r--   0 runner    (1001) docker     (121)   116747 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_latex.py
--rw-r--r--   0 runner    (1001) docker     (121)     5560 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_llvmjit.py
--rw-r--r--   0 runner    (1001) docker     (121)    12928 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_maple.py
--rw-r--r--   0 runner    (1001) docker     (121)    10933 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_mathematica.py
--rw-r--r--   0 runner    (1001) docker     (121)    94860 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_mathml.py
--rw-r--r--   0 runner    (1001) docker     (121)     9473 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)    18365 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_octave.py
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_precedence.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (121)    13125 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_pycode.py
--rw-r--r--   0 runner    (1001) docker     (121)     7480 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (121)    14101 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_rcode.py
--rw-r--r--   0 runner    (1001) docker     (121)    11422 2021-09-30 22:23:57.228190 sympy-1.9/sympy/printing/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)    11644 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tests/test_rust.py
--rw-r--r--   0 runner    (1001) docker     (121)    40014 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tests/test_str.py
--rw-r--r--   0 runner    (1001) docker     (121)     5641 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tests/test_tableform.py
--rw-r--r--   0 runner    (1001) docker     (121)    15607 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tests/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    20837 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tests/test_theanocode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6080 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    18196 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/theanocode.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-09-30 22:23:57.232190 sympy-1.9/sympy/printing/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-09-30 22:23:57.232190 sympy-1.9/sympy/release.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/sandbox/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-09-30 22:23:57.232190 sympy-1.9/sympy/sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-09-30 22:23:57.232190 sympy-1.9/sympy/sandbox/indexed_integrals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/sandbox/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.232190 sympy-1.9/sympy/sandbox/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-09-30 22:23:57.232190 sympy-1.9/sympy/sandbox/tests/test_indexed_integrals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/series/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3115 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/approximants.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/aseries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/series/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/benchmarks/bench_limit.py
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/benchmarks/bench_order.py
--rw-r--r--   0 runner    (1001) docker     (121)    51747 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/formal.py
--rw-r--r--   0 runner    (1001) docker     (121)    22798 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)    23291 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/gruntz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/kauers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11465 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     7686 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/limitseq.py
--rw-r--r--   0 runner    (1001) docker     (121)    18726 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/residues.py
--rw-r--r--   0 runner    (1001) docker     (121)    35570 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/series.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/series_class.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.987351 sympy-1.9/sympy/series/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_approximants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_aseries.py
--rw-r--r--   0 runner    (1001) docker     (121)     4649 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_demidovich.py
--rw-r--r--   0 runner    (1001) docker     (121)    21897 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_formal.py
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)    15591 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_gruntz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_kauers.py
--rw-r--r--   0 runner    (1001) docker     (121)    32678 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_limits.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_limitseq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_lseries.py
--rw-r--r--   0 runner    (1001) docker     (121)    16723 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_nseries.py
--rw-r--r--   0 runner    (1001) docker     (121)    15257 2021-09-30 22:23:57.232190 sympy-1.9/sympy/series/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2021-09-30 22:23:57.236191 sympy-1.9/sympy/series/tests/test_residues.py
--rw-r--r--   0 runner    (1001) docker     (121)    10604 2021-09-30 22:23:57.236191 sympy-1.9/sympy/series/tests/test_sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)    13698 2021-09-30 22:23:57.236191 sympy-1.9/sympy/series/tests/test_series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/sets/
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7782 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/conditionset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/contains.py
--rw-r--r--   0 runner    (1001) docker     (121)    47552 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/fancysets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/sets/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     8756 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    16967 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/intersection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5252 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/issubset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/mul.py
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/power.py
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/handlers/union.py
--rw-r--r--   0 runner    (1001) docker     (121)     7583 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/powerset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/setexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)    72439 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/sets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/sets/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10685 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_conditionset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_contains.py
--rw-r--r--   0 runner    (1001) docker     (121)    48157 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_fancysets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_ordinals.py
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_powerset.py
--rw-r--r--   0 runner    (1001) docker     (121)    14487 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_setexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)    63220 2021-09-30 22:23:57.236191 sympy-1.9/sympy/sets/tests/test_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/simplify/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-09-30 22:23:57.236191 sympy-1.9/sympy/simplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-09-30 22:23:57.236191 sympy-1.9/sympy/simplify/combsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    30330 2021-09-30 22:23:57.236191 sympy-1.9/sympy/simplify/cse_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2021-09-30 22:23:57.236191 sympy-1.9/sympy/simplify/cse_opts.py
--rw-r--r--   0 runner    (1001) docker     (121)    10177 2021-09-30 22:23:57.236191 sympy-1.9/sympy/simplify/epathtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    61845 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/fu.py
--rw-r--r--   0 runner    (1001) docker     (121)    18842 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/gammasimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    84686 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/hyperexpand.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/hyperexpand_doc.py
--rw-r--r--   0 runner    (1001) docker     (121)    26364 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/powsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    40310 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/radsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7604 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/ratsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    73380 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/simplify.py
--rw-r--r--   0 runner    (1001) docker     (121)    21596 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/sqrtdenest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/simplify/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_combsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    18887 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_cse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_epathtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    18248 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_fu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_gammasimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    39828 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_hyperexpand.py
--rw-r--r--   0 runner    (1001) docker     (121)    13406 2021-09-30 22:23:57.240191 sympy-1.9/sympy/simplify/tests/test_powsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)    17977 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_radsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_ratsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_rewrite.py
--rw-r--r--   0 runner    (1001) docker     (121)    38859 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (121)     7379 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_sqrtdenest.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_traversaltools.py
--rw-r--r--   0 runner    (1001) docker     (121)    18548 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/tests/test_trigsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/traversaltools.py
--rw-r--r--   0 runner    (1001) docker     (121)    44915 2021-09-30 22:23:57.244191 sympy-1.9/sympy/simplify/trigsimp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/benchmarks/bench_solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)    17882 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/bivariate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/decompogen.py
--rw-r--r--   0 runner    (1001) docker     (121)    10338 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/deutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/diophantine/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/diophantine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   119692 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/diophantine/diophantine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/diophantine/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/diophantine/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41561 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/diophantine/tests/test_diophantine.py
--rw-r--r--   0 runner    (1001) docker     (121)    33678 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/inequalities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/ode/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9677 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/ode/hypergeometric.py
--rw-r--r--   0 runner    (1001) docker     (121)    39242 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/ode/lie_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    18175 2021-09-30 22:23:57.244191 sympy-1.9/sympy/solvers/ode/nonhomogeneous.py
--rw-r--r--   0 runner    (1001) docker     (121)   145216 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (121)    30662 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/riccati.py
--rw-r--r--   0 runner    (1001) docker     (121)   110201 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/single.py
--rw-r--r--   0 runner    (1001) docker     (121)    16171 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/subscheck.py
--rw-r--r--   0 runner    (1001) docker     (121)    71802 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/systems.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/ode/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2021-09-30 22:23:57.248191 sympy-1.9/sympy/solvers/ode/tests/test_lie_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    44416 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/ode/tests/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (121)    28866 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/ode/tests/test_riccati.py
--rw-r--r--   0 runner    (1001) docker     (121)    99025 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/ode/tests/test_single.py
--rw-r--r--   0 runner    (1001) docker     (121)    12118 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/ode/tests/test_subscheck.py
--rw-r--r--   0 runner    (1001) docker     (121)   130037 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/ode/tests/test_systems.py
--rw-r--r--   0 runner    (1001) docker     (121)    35885 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/pde.py
--rw-r--r--   0 runner    (1001) docker     (121)    11281 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/polysys.py
--rw-r--r--   0 runner    (1001) docker     (121)    24884 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/recurr.py
--rw-r--r--   0 runner    (1001) docker     (121)   130460 2021-09-30 22:23:57.252191 sympy-1.9/sympy/solvers/solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)   132158 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/solveset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_constantsimp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_decompogen.py
--rw-r--r--   0 runner    (1001) docker     (121)    20173 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_inequalities.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     9057 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (121)     4855 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_polysys.py
--rw-r--r--   0 runner    (1001) docker     (121)     9149 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_recurr.py
--rw-r--r--   0 runner    (1001) docker     (121)    94260 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)   117579 2021-09-30 22:23:57.256192 sympy-1.9/sympy/solvers/tests/test_solveset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/stats/
--rw-r--r--   0 runner    (1001) docker     (121)     8454 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7818 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/compound_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    20513 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/crv.py
--rw-r--r--   0 runner    (1001) docker     (121)   119086 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/crv_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    11476 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/drv.py
--rw-r--r--   0 runner    (1001) docker     (121)    18648 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/drv_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/error_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)    16467 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/frv.py
--rw-r--r--   0 runner    (1001) docker     (121)    22777 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/frv_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    15693 2021-09-30 22:23:57.256192 sympy-1.9/sympy/stats/joint_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    29713 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/joint_rv_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    21570 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/matrix_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/random_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    14830 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/random_matrix_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    53686 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    13692 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/rv_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/stats/sampling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/sample_numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/sample_pymc3.py
--rw-r--r--   0 runner    (1001) docker     (121)     6269 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/sample_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.991351 sympy-1.9/sympy/stats/sampling/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/tests/test_sample_continuous_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3286 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/tests/test_sample_discrete_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/sampling/tests/test_sample_finite_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/stochastic_process.py
--rw-r--r--   0 runner    (1001) docker     (121)    87390 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/stochastic_process_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    10179 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/symbolic_multivariate_probability.py
--rw-r--r--   0 runner    (1001) docker     (121)    22786 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/symbolic_probability.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_compound_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    54762 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_continuous_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    11192 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_discrete_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_error_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)    19728 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_finite_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    16818 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_joint_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)     8578 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_matrix_distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_mix.py
--rw-r--r--   0 runner    (1001) docker     (121)     5373 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_random_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    12257 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)    38196 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_stochastic_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     5433 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_symbolic_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (121)     9087 2021-09-30 22:23:57.260192 sympy-1.9/sympy/stats/tests/test_symbolic_probability.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/strategies/
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-09-30 22:23:57.260192 sympy-1.9/sympy/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/strategies/branch/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/strategies/branch/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/tests/test_traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/branch/traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2941 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/rl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/strategies/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/test_rl.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/test_strat.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/test_traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-09-30 22:23:57.264192 sympy-1.9/sympy/strategies/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/tensor/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/tensor/array/
--rw-r--r--   0 runner    (1001) docker     (121)     7299 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11869 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/array_comprehension.py
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/array_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)    16294 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/arrayop.py
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/dense_ndim_array.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/tensor/array/expressions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    59914 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/array_expressions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/arrayexpr_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)    28886 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/conv_array_to_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     7185 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/conv_indexed_to_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/conv_matrix_to_array.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/tensor/array/expressions/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20979 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/test_array_expressions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/test_arrayexpr_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/test_as_explicit.py
--rw-r--r--   0 runner    (1001) docker     (121)    21096 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/test_convert_array_to_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     6059 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/test_convert_index_to_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3595 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/tests/test_convert_matrix_to_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/expressions/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/mutable_ndim_array.py
--rw-r--r--   0 runner    (1001) docker     (121)    18749 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/ndim_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     6362 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/sparse_ndim_array.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/tensor/array/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_array_comprehension.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_array_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)    24261 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_arrayop.py
--rw-r--r--   0 runner    (1001) docker     (121)    15602 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_immutable_ndim_array.py
--rw-r--r--   0 runner    (1001) docker     (121)    12888 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_mutable_ndim_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_ndim_array.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/array/tests/test_ndim_array_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-09-30 22:23:57.264192 sympy-1.9/sympy/tensor/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15435 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/index_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)    24566 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/indexed.py
--rw-r--r--   0 runner    (1001) docker     (121)   144970 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/tensor/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7089 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/test_index_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)    15823 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/test_indexed.py
--rw-r--r--   0 runner    (1001) docker     (121)    70994 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/test_tensor_element.py
--rw-r--r--   0 runner    (1001) docker     (121)    17126 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/tests/test_tensor_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6617 2021-09-30 22:23:57.268192 sympy-1.9/sympy/tensor/toperators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     9715 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/quality_unicode.py
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/randtest.py
--rw-r--r--   0 runner    (1001) docker     (121)    88459 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/runtests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9691 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/tests/diagnose_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    18591 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/tests/test_code_quality.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/tests/test_module_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     7753 2021-09-30 22:23:57.268192 sympy-1.9/sympy/testing/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-09-30 22:23:57.272192 sympy-1.9/sympy/testing/tmpfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-30 22:23:57.272192 sympy-1.9/sympy/this.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/unify/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7037 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/rewrite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/unify/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/tests/test_rewrite.py
--rw-r--r--   0 runner    (1001) docker     (121)     5561 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/tests/test_sympy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/tests/test_unify.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2021-09-30 22:23:57.272192 sympy-1.9/sympy/unify/usympy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/utilities/_compilation/
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/availability.py
--rw-r--r--   0 runner    (1001) docker     (121)    20491 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/compilation.py
--rw-r--r--   0 runner    (1001) docker     (121)     9053 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/utilities/_compilation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/tests/test_compilation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7807 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/_compilation/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    41293 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/autowrap.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (121)    81465 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)     7199 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)    43513 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/enumerative.py
--rw-r--r--   0 runner    (1001) docker     (121)     7163 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    76983 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/iterables.py
--rw-r--r--   0 runner    (1001) docker     (121)    49485 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/lambdify.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/magic.py
--rw-r--r--   0 runner    (1001) docker     (121)     9382 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/matchpy_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/utilities/mathml/
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/mathml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.995351 sympy-1.9/sympy/utilities/mathml/data/
--rw-r--r--   0 runner    (1001) docker     (121)   114443 2021-09-30 22:23:57.272192 sympy-1.9/sympy/utilities/mathml/data/mmlctop.xsl
--rw-r--r--   0 runner    (1001) docker     (121)   137304 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/mathml/data/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (121)   114432 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/mathml/data/simple_mmlctop.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/memoization.py
--rw-r--r--   0 runner    (1001) docker     (121)    13510 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/pkgdata.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/quality_unicode.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/randtest.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/runtests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.999352 sympy-1.9/sympy/utilities/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14687 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_autowrap.py
--rw-r--r--   0 runner    (1001) docker     (121)    54928 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)    18268 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_codegen_julia.py
--rw-r--r--   0 runner    (1001) docker     (121)    17688 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_codegen_octave.py
--rw-r--r--   0 runner    (1001) docker     (121)    12202 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_codegen_rust.py
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_enumerative.py
--rw-r--r--   0 runner    (1001) docker     (121)    31561 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_iterables.py
--rw-r--r--   0 runner    (1001) docker     (121)    47719 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_lambdify.py
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_matchpy_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3399 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    22931 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (121)      797 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_timeutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    92412 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tests/test_wester.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/timeutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-30 22:23:57.276192 sympy-1.9/sympy/utilities/tmpfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.999352 sympy-1.9/sympy/vector/
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-09-30 22:23:57.276192 sympy-1.9/sympy/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11391 2021-09-30 22:23:57.276192 sympy-1.9/sympy/vector/basisdependent.py
--rw-r--r--   0 runner    (1001) docker     (121)    37194 2021-09-30 22:23:57.276192 sympy-1.9/sympy/vector/coordsysrect.py
--rw-r--r--   0 runner    (1001) docker     (121)     3555 2021-09-30 22:23:57.276192 sympy-1.9/sympy/vector/deloperator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-09-30 22:23:57.276192 sympy-1.9/sympy/vector/dyadic.py
--rw-r--r--   0 runner    (1001) docker     (121)    15579 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15972 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/implicitregion.py
--rw-r--r--   0 runner    (1001) docker     (121)     6833 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10609 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/operators.py
--rw-r--r--   0 runner    (1001) docker     (121)    11677 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/orienters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5913 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/parametricregion.py
--rw-r--r--   0 runner    (1001) docker     (121)     4516 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/point.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 22:28:04.999352 sympy-1.9/sympy/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19426 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_coordsysrect.py
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_dyadic.py
--rw-r--r--   0 runner    (1001) docker     (121)    14058 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_field_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7829 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_implicitregion.py
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3942 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_parametricregion.py
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)    17801 2021-09-30 22:23:57.280192 sympy-1.9/sympy/vector/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)    44032 2021-09-19 19:47:03.941182 sympy-1.9rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     7885 2021-09-19 19:47:03.941182 sympy-1.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12037 2021-09-19 19:52:01.401290 sympy-1.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10987 2021-09-19 19:47:03.945182 sympy-1.9rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      509 2021-09-19 19:47:03.945182 sympy-1.9rc1/bin/isympy
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.317290 sympy-1.9rc1/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/data/TeXmacs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-09-19 19:47:03.945182 sympy-1.9rc1/data/TeXmacs/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/data/TeXmacs/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2349 2021-09-19 19:47:03.945182 sympy-1.9rc1/data/TeXmacs/bin/tm_sympy
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/data/TeXmacs/progs/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-09-19 19:47:03.945182 sympy-1.9rc1/data/TeXmacs/progs/init-sympy.scm
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)     5036 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/api/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/apidoc.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/doc/cheatsheet/
+-rw-r--r--   0 runner    (1001) docker     (121)     8792 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/cheatsheet/cheatsheet.tex
+-rw-r--r--   0 runner    (1001) docker     (121)    23570 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/cheatsheet/combinatoric_cheatsheet.tex
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-09-19 19:51:58.469288 sympy-1.9rc1/doc/commit_hash.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/doc/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)    16898 2021-09-19 19:47:03.945182 sympy-1.9rc1/doc/ext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9421 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/ext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6272 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/ext/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1245 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/ext/sympylive.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9472 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/generate_logos.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.329290 sympy-1.9rc1/doc/man/
+-rw-r--r--   0 runner    (1001) docker     (121)     6659 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/man/isympy.1
+-rw-r--r--   0 runner    (1001) docker     (121)    17844 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/man/isympy.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.333290 sympy-1.9rc1/doc/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.333290 sympy-1.9rc1/doc/src/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     6785 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/_static/default.css_t
+-rw-r--r--   0 runner    (1001) docker     (121)    19711 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/_static/sympylogo.png
+-rw-r--r--   0 runner    (1001) docker     (121)   167361 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/_static/sympylogo_big.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.333290 sympy-1.9rc1/doc/src/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/aboutus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9489 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50723 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/documentation-style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    27968 2021-09-19 19:47:03.949182 sympy-1.9rc1/doc/src/gotchas.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.333290 sympy-1.9rc1/doc/src/guides/
+-rw-r--r--   0 runner    (1001) docker     (121)    55371 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/guides/assumptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15907 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/guides/booleans.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.333290 sympy-1.9rc1/doc/src/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/logo/info.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    34099 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/logo/sympy-use-text.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    40583 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/logo/sympy.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.333290 sympy-1.9rc1/doc/src/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/abc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/algebras.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/assumptions/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/assumptions/ask.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/assumptions/assume.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/assumptions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4676 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/assumptions/predicates.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/assumptions/refine.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/calculus/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/calculus/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/categories.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    23741 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/codegen.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/combinatorics/
+-rw-r--r--   0 runner    (1001) docker     (121)    11344 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/fp_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/graycode.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/group_constructs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/named_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/partitions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9634 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/pc_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/perm_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/permutations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/polyhedron.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/prufer.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/subsets.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/tensor_can.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/testutil.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/combinatorics/util.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3034 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/concrete.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/core.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/crypto.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/diffgeom.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/discrete.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13689 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/evalf.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/functions/
+-rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/functions/combinatorial.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5783 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/functions/elementary.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/functions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7089 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/functions/special.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/curves.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/ellipses.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/entities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6665 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/lines.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/plane.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/points.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/polygons.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/geometry/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/holonomic/
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/about.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/convert.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/operations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2314 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/represent.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/holonomic/uses.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2021-09-19 19:47:03.953182 sympy-1.9rc1/doc/src/modules/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/integrals/
+-rw-r--r--   0 runner    (1001) docker     (121)    31196 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/integrals/g-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12920 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/integrals/integrals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/interactive.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/liealgebras/
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/liealgebras/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3310 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/logic.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/matrices/
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/common.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/dense.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1699 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/expressions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/immutablematrices.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14159 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/matrices.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/sparse.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/matrices/sparsetools.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4988 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/ntheory.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6460 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/numeric-computation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3920 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/parsing.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/
+-rw-r--r--   0 runner    (1001) docker     (121)     9011 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/allowed-sign-conventions.png
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/beam.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    48599 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/beam_problems.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    31500 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/ildreaction.png
+-rw-r--r--   0 runner    (1001) docker     (121)    46549 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/ildshear.png
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/control/
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/control/control.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/control/control_plots.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/control/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/control/lti.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/hep/
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/hep/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/hydrogen.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/matrices.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (121)     6131 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/advanced.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/body.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/expr_manip.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/joint.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/kane_lagrange.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/part_bod.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/printing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/api/system.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21620 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/autolev_parser.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)    18210 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/bicycle_example.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10648 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/lin_pend_nonmin_example.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7277 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/multi_degree_freedom_holonomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    68787 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/multidof-holonomic.png
+-rw-r--r--   0 runner    (1001) docker     (121)    22831 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/pendulum_nonmin.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     9492 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3613 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3348 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane_constraints.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example_lagrange.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2021-09-19 19:47:03.957182 sympy-1.9rc1/doc/src/modules/physics/mechanics/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4043 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6321 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/kane.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4704 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/lagrange.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13663 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13824 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/masses.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    47681 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/sympy_mechanics_for_autolev_users.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7588 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/mechanics/symsystem.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.337290 sympy-1.9rc1/doc/src/modules/physics/optics/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/optics/gaussopt.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/optics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/optics/medium.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/optics/polarization.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/optics/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/optics/waves.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/paulialgebra.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/qho_1d.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/physics/quantum/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/anticommutator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/cartesian.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/cg.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/circuitplot.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/commutator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/dagger.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/gate.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/grover.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/hilbert.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/innerproduct.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/operator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/operatorset.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/piab.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/qapply.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/qft.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/qubit.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/represent.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/shor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/spin.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/state.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/quantum/tensorproduct.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/secondquant.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/sho.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/physics/units/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/dimensions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9966 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/philosophy.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/prefixes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/quantities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/units/unitsystem.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/physics/vector/
+-rw-r--r--   0 runner    (1001) docker     (121)     6011 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/advanced.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/physics/vector/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/api/fieldfunctions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/api/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/api/kinematics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/api/printing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13626 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/fields.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8723 2021-09-19 19:47:03.961182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_1.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    25763 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_1pt.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    13720 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_2.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    16112 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_2pt.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    12267 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_3.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    18006 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_4.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    12819 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_angvel1.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    23357 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_angvel2.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    14105 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_angvel3.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    10993 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kin_rolling.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    21732 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/kinematics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10488 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/simp_rot.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7722 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_add.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    10009 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_cross.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    10637 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_dot.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    15641 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_fix_notfix.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     4845 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_mul.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5311 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_rep.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    14527 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vec_simp_der.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    30182 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/vector/vectors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/physics/wigner.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9028 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/plotting.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/polys/
+-rw-r--r--   0 runner    (1001) docker     (121)    14916 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/agca.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21504 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/domainmatrix.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    56088 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/domainsintro.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8428 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/domainsref.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    24930 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6527 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/literature.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4683 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8816 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/ringseries.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/solvers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15616 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/polys/wester.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    17534 2021-09-19 19:47:03.965182 sympy-1.9rc1/doc/src/modules/printing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4459 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/rewriting.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/series/
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/series/formal.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/series/fourier.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/series/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/series/limitseq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/series/sequences.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5326 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/series/series.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2994 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/sets.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/simplify/
+-rw-r--r--   0 runner    (1001) docker     (121)     8382 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/simplify/fu.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    27713 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/simplify/hyperexpand.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/simplify/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/simplify/simplify.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/solvers/
+-rw-r--r--   0 runner    (1001) docker     (121)    20258 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/solvers/diophantine.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/solvers/inequalities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10710 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/solvers/ode.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/solvers/pde.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/solvers/solvers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    22507 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/solvers/solveset.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7771 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/stats.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/tensor/
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/tensor/array.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/tensor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/tensor/index_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/tensor/indexed.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/tensor/tensor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/tensor/toperators.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/testing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/testing/pytest.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/testing/randtest.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/testing/runtests.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/autowrap.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/decorator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/enumerative.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/iterables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/lambdify.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/memoization.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/pkgdata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/source.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/utilities/timeutils.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/vector/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.341290 sympy-1.9rc1/doc/src/modules/vector/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/api/orienterclasses.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/api/vectorfunctions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7773 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9615 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/coordsys.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10488 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/coordsys_rot.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3455 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12820 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/fields.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5450 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6134 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/modules/vector/vector_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2021-09-19 19:47:03.969182 sympy-1.9rc1/doc/src/outreach.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/doc/src/pics/
+-rw-r--r--   0 runner    (1001) docker     (121)   141216 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/pics/consoleascii.png
+-rw-r--r--   0 runner    (1001) docker     (121)   120924 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/pics/consoleunicode.png
+-rw-r--r--   0 runner    (1001) docker     (121)    37262 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/pics/ipythonnotebook.png
+-rw-r--r--   0 runner    (1001) docker     (121)   244487 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/pics/ipythonqtconsole.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3251 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/pics/pngview1.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/doc/src/special_topics/
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/special_topics/classification.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11892 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/special_topics/finite_diff_derivatives.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/special_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/special_topics/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/doc/src/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)     7059 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/basic_operations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12199 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/calculus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11114 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/gotchas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8428 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21465 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/manipulation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    18034 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/matrices.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/preliminaries.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7633 2021-09-19 19:47:03.973183 sympy-1.9rc1/doc/src/tutorial/printing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    29238 2021-09-19 19:47:03.977182 sympy-1.9rc1/doc/src/tutorial/simplification.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7303 2021-09-19 19:47:03.977182 sympy-1.9rc1/doc/src/tutorial/solvers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-09-19 19:47:03.977182 sympy-1.9rc1/doc/src/wiki.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/README
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/examples/advanced/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8893 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/autowrap_integrators.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2388 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/autowrap_ufuncify.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3694 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/curvilinear_coordinates.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1501 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/dense_coding_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5567 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/fem.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3544 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/gibbs_phenomenon.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2081 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/grover_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      702 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/hydrogen.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2716 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/pidigits.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7178 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/pyglet_plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3401 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/qft.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4312 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/advanced/relativity.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6732 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/all.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/examples/beginner/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      336 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      679 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/differentiation.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      361 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/expansion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      394 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      813 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/limits_examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1913 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/plot_examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      407 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/plotting_nice_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      443 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/precision.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      879 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/print_pretty.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      417 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/series.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      704 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/beginner/substitution.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/examples/intermediate/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3689 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/coupled_cluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      583 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/differential_equations.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2914 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/infinite_1d_box.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      965 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/mplot2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1248 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/mplot3d.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1981 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/partial_differential_eqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      384 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/print_gtk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/sample.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      717 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/trees.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4638 2021-09-19 19:47:03.977182 sympy-1.9rc1/examples/intermediate/vandermonde.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11199 2021-09-19 19:47:03.985182 sympy-1.9rc1/isympy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-09-19 19:47:03.985182 sympy-1.9rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14748 2021-09-19 19:47:03.985182 sympy-1.9rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/
+-rw-r--r--   0 runner    (1001) docker     (121)    28517 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3662 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/algebras/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/algebras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21719 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/algebras/quaternion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/algebras/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/algebras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8979 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/algebras/tests/test_quaternion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/assumptions/
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/assumptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18421 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/assumptions/ask.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17083 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/assumptions/ask_generated.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14321 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/assumptions/assume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12645 2021-09-19 19:47:03.985182 sympy-1.9rc1/sympy/assumptions/cnf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7644 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/facts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/assumptions/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7198 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3939 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22339 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7213 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/ntheory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12283 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/order.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23164 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/handlers/sets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/assumptions/predicates/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1889 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2283 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12151 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2546 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/ntheory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9508 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8928 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/predicates/sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12007 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/refine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/assumptions/relation/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/relation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6222 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/relation/binrel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7160 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/relation/equality.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11235 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/satask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9466 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/sathandlers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/assumptions/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_assumptions_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12162 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97928 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8195 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15442 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_satask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_sathandlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/tests/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4196 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/assumptions/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/benchmarks/bench_discrete_log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11334 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/benchmarks/bench_meijerint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2740 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/benchmarks/bench_symbench.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/calculus/
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3264 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/euler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17466 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11369 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/singularities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.345290 sympy-1.9rc1/sympy/calculus/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/tests/test_euler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7752 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/tests/test_finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3661 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/tests/test_singularities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24884 2021-09-19 19:47:03.989183 sympy-1.9rc1/sympy/calculus/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53951 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/calculus/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/categories/
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/categories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31444 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/categories/baseclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    95531 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/categories/diagram_drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/categories/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/categories/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5700 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/categories/tests/test_baseclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27838 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/categories/tests/test_drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/codegen/
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4865 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6437 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55021 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/ast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11818 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/cfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/cnodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/cutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/cxxnodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18892 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/fnodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/futils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/matrix_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/numpy_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11250 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/scipy_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/codegen/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4702 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_applications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_approximations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21355 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4535 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_cfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3039 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_cnodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_cxxnodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6629 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_fnodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_numpy_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13081 2021-09-19 19:47:03.993183 sympy-1.9rc1/sympy/codegen/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/codegen/tests/test_scipy_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/combinatorics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42956 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/coset_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47977 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/fp_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40003 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/free_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7492 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11237 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/graycode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/group_constructs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19341 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/homomorphisms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7900 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/named_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20907 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21303 2021-09-19 19:47:03.997182 sympy-1.9rc1/sympy/combinatorics/pc_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)   183825 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/perm_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87583 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36023 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/polyhedron.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11859 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/prufer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17175 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/rewritingsystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/rewritingsystem_fsm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4128 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/schur_number.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15858 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40758 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tensor_can.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/combinatorics/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28460 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_coset_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10011 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_fp_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_free_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3567 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2800 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_graycode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_group_constructs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_homomorphisms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_named_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4103 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_partitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2739 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_pc_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39338 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_perm_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20199 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_permutations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4217 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_polyhedron.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2649 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_prufer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1787 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1723 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_schur_number.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2503 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24676 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_tensor_can.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1718 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_testutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-09-19 19:47:04.001183 sympy-1.9rc1/sympy/combinatorics/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11165 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/combinatorics/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16423 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/combinatorics/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/concrete/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10103 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/delta.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11332 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/expr_with_intlimits.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19401 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/expr_with_limits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5559 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/gosper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17373 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/guess.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18712 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/products.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53769 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/summations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.349290 sympy-1.9rc1/sympy/concrete/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23694 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/tests/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7640 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/tests/test_gosper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/tests/test_guess.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13671 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/tests/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58467 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/concrete/tests/test_sums_products.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     2860 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2388 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/core/_print_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41654 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/core/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/core/alphabets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17828 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/core/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3215 2021-09-19 19:47:04.005183 sympy-1.9rc1/sympy/core/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69145 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/core/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/bench_arit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/bench_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/bench_basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/bench_expand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/bench_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/benchmarks/bench_sympify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4320 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19705 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9937 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/coreerrors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9428 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54285 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/evalf.py
+-rw-r--r--   0 runner    (1001) docker     (121)   140435 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/expr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51257 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/exprtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15735 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/facts.py
+-rw-r--r--   0 runner    (1001) docker     (121)   114608 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11587 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/kind.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10879 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7565 2021-09-19 19:47:04.009183 sympy-1.9rc1/sympy/core/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75406 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/mul.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/multidimensional.py
+-rw-r--r--   0 runner    (1001) docker     (121)   121934 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24320 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3749 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71834 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/power.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46397 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/relational.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6983 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26767 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19419 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/sympify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.013182 sympy-1.9rc1/sympy/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   176679 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74105 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_arit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39848 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9692 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2458 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21517 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_constructor_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6867 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5017 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_count_ops.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5421 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_equal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22809 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_evalf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11857 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_expand.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71905 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18053 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_exprtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11579 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_facts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50134 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21787 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_multidimensional.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4092 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_noncommutative.py
+-rw-r--r--   0 runner    (1001) docker     (121)    73112 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2021-09-19 19:47:04.017183 sympy-1.9rc1/sympy/core/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23116 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41870 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_relational.py
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28941 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_subs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12044 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25319 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_sympify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2823 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_truediv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/tests/test_var.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6183 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/core/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/crypto/
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    89384 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/crypto/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/crypto/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/crypto/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19752 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/crypto/tests/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/diffgeom/
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71461 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/diffgeom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/rn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/diffgeom/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/tests/test_class_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13542 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/tests/test_diffgeom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5258 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/tests/test_function_diffgeom_book.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2583 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/diffgeom/tests/test_hyperbolic_space.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/discrete/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14472 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5090 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/recurrences.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/discrete/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16950 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2957 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/tests/test_recurrences.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5533 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11683 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/discrete/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.353290 sympy-1.9rc1/sympy/external/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2910 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/external/gmpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7844 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/external/importtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11870 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/external/pythonmpq.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/external/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/external/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9619 2021-09-19 19:47:04.021183 sympy-1.9rc1/sympy/external/tests/test_autowrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12082 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/external/tests/test_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/external/tests/test_importtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9553 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/external/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5605 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/external/tests/test_pythonmpq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/external/tests/test_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/
+-rw-r--r--   0 runner    (1001) docker     (121)     5075 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/combinatorial/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/combinatorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36913 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/combinatorial/factorials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68094 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/combinatorial/numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/combinatorial/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/combinatorial/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25685 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/combinatorial/tests/test_comb_factorials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26322 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/combinatorial/tests/test_comb_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/elementary/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/elementary/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/benchmarks/bench_exp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42081 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/complexes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39917 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51578 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/hyperbolic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17385 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/integers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26672 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50105 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/piecewise.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/elementary/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32084 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/tests/test_complexes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24838 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/tests/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35865 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/tests/test_hyperbolic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17778 2021-09-19 19:47:04.025183 sympy-1.9rc1/sympy/functions/elementary/tests/test_integers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1876 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/elementary/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16011 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/elementary/tests/test_miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50554 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/elementary/tests/test_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82448 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/elementary/tests/test_trigonometric.py
+-rw-r--r--   0 runner    (1001) docker     (121)   108787 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/elementary/trigonometric.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/special/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/special/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/benchmarks/bench_special.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56887 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/bessel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11724 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/beta_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10225 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/bsplines.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20215 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/delta_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14600 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/elliptic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    76545 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41901 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/gamma_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37344 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6578 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/mathieu_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40530 2021-09-19 19:47:04.029183 sympy-1.9rc1/sympy/functions/special/polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8283 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/singularity_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11112 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12750 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tensor_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/functions/special/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30238 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_bessel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_beta_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6967 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_bsplines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6838 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_delta_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6532 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_elliptic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30164 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28489 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_gamma_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15314 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_hyper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_mathieu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5182 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_singularity_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15644 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_spec_polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3571 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5354 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_tensor_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9218 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/tests/test_zeta_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21398 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/functions/special/zeta_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/galgebra.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10060 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/geometry/curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50789 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/geometry/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20586 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/geometry/entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-09-19 19:47:04.033183 sympy-1.9rc1/sympy/geometry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    77083 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/line.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10255 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/parabola.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27265 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36678 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81770 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/geometry/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4267 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25154 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_geometrysets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35532 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5170 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_parabola.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12341 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15918 2021-09-19 19:47:04.037183 sympy-1.9rc1/sympy/geometry/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26869 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/geometry/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5771 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/geometry/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19471 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/geometry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/holonomic/
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    94482 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/holonomic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/holonomicerrors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2730 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10983 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/recurrence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/holonomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34042 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/tests/test_holonomic.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/holonomic/tests/test_recurrence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/integrals/
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.357290 sympy-1.9rc1/sympy/integrals/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/benchmarks/bench_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/benchmarks/bench_trigintegrate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7426 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/deltafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25487 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/heurisch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63943 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43221 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/intpoly.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63318 2021-09-19 19:47:04.041183 sympy-1.9rc1/sympy/integrals/manualintegrate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78435 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/meijerint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/meijerint_doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51995 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/prde.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17012 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10585 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rationaltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27182 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rde.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67527 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/risch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/
+-rw-r--r--   0 runner    (1001) docker     (121)     3464 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   295122 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/parsetools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2841 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/generate_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2707 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/generate_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9374 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/header.py.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    27553 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/parsetools/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8211 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/parsetools/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30426 2021-09-19 19:47:04.045183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61185 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10426 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_1_4.py
+-rw-r--r--   0 runner    (1001) docker     (121)   250958 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79552 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_hyperbolic_sine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65172 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_inverse_hyperbolic_sine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84206 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_inverse_sine.py
+-rw-r--r--   0 runner    (1001) docker     (121)   442127 2021-09-19 19:47:04.049183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_logarithms.py
+-rw-r--r--   0 runner    (1001) docker     (121)   526173 2021-09-19 19:47:04.053183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_miscellaneous_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (121)    93397 2021-09-19 19:47:04.053183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_secant.py
+-rw-r--r--   0 runner    (1001) docker     (121)   164373 2021-09-19 19:47:04.053183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_sine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48347 2021-09-19 19:47:04.053183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_special_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)   132374 2021-09-19 19:47:04.053183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_tangent.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1508403 2021-09-19 19:47:04.061183 sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_trinomials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8104 2021-09-19 19:47:04.061183 sympy-1.9rc1/sympy/integrals/rubi/rubimain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/rules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.061183 sympy-1.9rc1/sympy/integrals/rubi/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   199170 2021-09-19 19:47:04.061183 sympy-1.9rc1/sympy/integrals/rubi/rules/binomial_products.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62876 2021-09-19 19:47:04.061183 sympy-1.9rc1/sympy/integrals/rubi/rules/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (121)   218004 2021-09-19 19:47:04.065183 sympy-1.9rc1/sympy/integrals/rubi/rules/hyperbolic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23181 2021-09-19 19:47:04.065183 sympy-1.9rc1/sympy/integrals/rubi/rules/integrand_simplification.py
+-rw-r--r--   0 runner    (1001) docker     (121)   350893 2021-09-19 19:47:04.069183 sympy-1.9rc1/sympy/integrals/rubi/rules/inverse_hyperbolic.py
+-rw-r--r--   0 runner    (1001) docker     (121)   317185 2021-09-19 19:47:04.069183 sympy-1.9rc1/sympy/integrals/rubi/rules/inverse_trig.py
+-rw-r--r--   0 runner    (1001) docker     (121)    91552 2021-09-19 19:47:04.069183 sympy-1.9rc1/sympy/integrals/rubi/rules/linear_products.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97838 2021-09-19 19:47:04.069183 sympy-1.9rc1/sympy/integrals/rubi/rules/logarithms.py
+-rw-r--r--   0 runner    (1001) docker     (121)   232625 2021-09-19 19:47:04.069183 sympy-1.9rc1/sympy/integrals/rubi/rules/miscellaneous_algebraic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50567 2021-09-19 19:47:04.069183 sympy-1.9rc1/sympy/integrals/rubi/rules/miscellaneous_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)   189265 2021-09-19 19:47:04.073183 sympy-1.9rc1/sympy/integrals/rubi/rules/miscellaneous_trig.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19898 2021-09-19 19:47:04.073183 sympy-1.9rc1/sympy/integrals/rubi/rules/piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)   317214 2021-09-19 19:47:04.073183 sympy-1.9rc1/sympy/integrals/rubi/rules/quadratic_products.py
+-rw-r--r--   0 runner    (1001) docker     (121)   450602 2021-09-19 19:47:04.077183 sympy-1.9rc1/sympy/integrals/rubi/rules/secant.py
+-rw-r--r--   0 runner    (1001) docker     (121)   733180 2021-09-19 19:47:04.077183 sympy-1.9rc1/sympy/integrals/rubi/rules/sine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    89418 2021-09-19 19:47:04.077183 sympy-1.9rc1/sympy/integrals/rubi/rules/special_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)   314352 2021-09-19 19:47:04.077183 sympy-1.9rc1/sympy/integrals/rubi/rules/tangent.py
+-rw-r--r--   0 runner    (1001) docker     (121)   242580 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/rubi/rules/trinomial_products.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/rubi/symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/rubi/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/rubi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/rubi/tests/test_rubi_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81616 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/rubi/tests/test_utility_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)   269192 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/rubi/utility_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/singularityfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/integrals/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3495 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_deltafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7027 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_failing_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_heurisch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66544 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36169 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_intpoly.py
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_lineintegrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25950 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_manual.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30204 2021-09-19 19:47:04.081183 sympy-1.9rc1/sympy/integrals/tests/test_meijerint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16117 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_prde.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19919 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4979 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_rationaltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9494 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_rde.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37245 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_risch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_singularityfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38189 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3869 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/tests/test_trigonometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69129 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11080 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/integrals/trigonometry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/interactive/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/ipythonprinting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22933 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/printing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15401 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/interactive/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9501 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/interactive/tests/test_ipythonprinting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/liealgebras/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/cartan_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/cartan_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/dynkin_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/root_system.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/liealgebras/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_cartan_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_cartan_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_dynkin_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_root_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_A.py
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_B.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_C.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_D.py
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_E.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_F.py
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_type_G.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/tests/test_weyl_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4315 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_a.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4564 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_b.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4440 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_c.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4694 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9781 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_e.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4417 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_f.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2965 2021-09-19 19:47:04.085183 sympy-1.9rc1/sympy/liealgebras/type_g.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14725 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/liealgebras/weyl_group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/logic/
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/logic/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9175 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/algorithms/dpll.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20379 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/algorithms/dpll2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1317 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/algorithms/minisat22_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1207 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/algorithms/pycosat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    98003 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/boolalg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8582 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/logic/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45827 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/tests/test_boolalg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3886 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/tests/test_dimacs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13169 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/tests/test_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.361290 sympy-1.9rc1/sympy/logic/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/logic/utilities/dimacs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/matrices/
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/matrices/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/benchmarks/bench_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96132 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48092 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/decompositions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20272 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/dense.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5485 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/densearith.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11704 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/densesolve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5473 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/densetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30219 2021-09-19 19:47:04.089183 sympy-1.9rc1/sympy/matrices/determinant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40170 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/eigen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/matrices/expressions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6604 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/applyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31501 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/blockmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/companion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3050 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/determinant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6143 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/dotproduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/factorizations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3518 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/funcmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13782 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/hadamard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2699 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13438 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/kronecker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4330 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/matadd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/matexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13924 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5074 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/matpow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8028 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3312 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/slice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6942 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/special.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/matrices/expressions/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3472 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_applyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14559 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_blockmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_companion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14717 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_determinant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4294 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_dotproduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_factorizations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2247 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_funcmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4029 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_hadamard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10373 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5217 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_kronecker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_matadd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15718 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_matexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5212 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6241 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_matpow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6622 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_special.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3062 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4963 2021-09-19 19:47:04.093183 sympy-1.9rc1/sympy/matrices/expressions/trace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/expressions/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9076 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11376 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    77907 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/normalforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10179 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/reductions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21431 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/repmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22801 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14567 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9182 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/sparsetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/subspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/matrices/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38812 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_commonmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13853 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_decompositions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2336 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_densearith.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_densesolve.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_densetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12876 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_determinant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21681 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)   142839 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-09-19 19:47:04.097183 sympy-1.9rc1/sympy/matrices/tests/test_normalforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13909 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/matrices/tests/test_reductions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20225 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/matrices/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22482 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/matrices/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4834 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/matrices/tests/test_sparsetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3839 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/matrices/tests/test_subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/matrices/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/multipledispatch/
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/conflict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12233 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/multipledispatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/tests/test_conflict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6205 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/multipledispatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.365290 sympy-1.9rc1/sympy/ntheory/
+-rw-r--r--   0 runner    (1001) docker     (121)     2746 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5213 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/bbp_pi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10075 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/continued_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3692 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/digits.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10141 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/ecm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6810 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/egyptian_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11473 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/elliptic_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75312 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/factor_.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30338 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7659 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/modular.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5970 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/partitions_.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19378 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/primetest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18418 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/qs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39856 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/residue_ntheory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/ntheory/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9422 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_bbp_pi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_continued_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1182 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_digits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_ecm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_egyptian_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_elliptic_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24601 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_factor_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7927 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2021-09-19 19:47:04.101183 sympy-1.9rc1/sympy/ntheory/tests/test_modular.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/ntheory/tests/test_multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/ntheory/tests/test_partitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7049 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/ntheory/tests/test_primetest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4116 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/ntheory/tests/test_qs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12856 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/ntheory/tests/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/ast_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/autolev/
+-rw-r--r--   0 runner    (1001) docker     (121)     4154 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/Autolev.g4
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/autolev/_antlr/
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/_antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16845 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/_antlr/autolevlexer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10049 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/_antlr/autolevlistener.py
+-rw-r--r--   0 runner    (1001) docker     (121)   111528 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/_antlr/autolevparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)   104758 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/_listener_autolev_antlr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/_parse_autolev_antlr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/autolev/test-examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.al
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/double_pendulum.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/double_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/mass_spring_damper.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/mass_spring_damper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/non_min_pendulum.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/non_min_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest1.al
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest10.al
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest10.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest11.al
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest11.py
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest12.al
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest12.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest2.al
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest3.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest4.al
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest5.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest6.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest6.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest7.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest7.py
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest8.al
+-rw-r--r--   0 runner    (1001) docker     (121)     2690 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest8.py
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest9.al
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-09-19 19:47:04.105183 sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest9.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/c/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39276 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/c/c_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/fortran/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11598 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/fortran/fortran_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/latex/
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5614 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/LaTeX.g4
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/latex/_antlr/
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/_antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37558 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/_antlr/latexlexer.py
+-rw-r--r--   0 runner    (1001) docker     (121)   124634 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/_antlr/latexparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/_build_latex_antlr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19866 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/_parse_latex_antlr.py
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/latex/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12987 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/mathematica.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/maxima.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8894 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/sym_expr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38725 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/sympy_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/parsing/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_ast_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6610 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_autolev.py
+-rw-r--r--   0 runner    (1001) docker     (121)   154616 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_c_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11816 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_fortran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7449 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_implicit_multiplication_application.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9968 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_latex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_mathematica.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_maxima.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5657 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_sym_expr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9375 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/parsing/tests/test_sympy_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/continuum_mechanics/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-09-19 19:47:04.109183 sympy-1.9rc1/sympy/physics/continuum_mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   145108 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/continuum_mechanics/beam.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/continuum_mechanics/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/continuum_mechanics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26123 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/continuum_mechanics/tests/test_beam.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/control/
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30102 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/control/control_plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)   111602 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/control/lti.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/control/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/control/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15573 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/control/tests/test_control_plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58453 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/control/tests/test_lti.py
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/gaussopt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/hep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/hep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24184 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/hep/gamma_matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.369290 sympy-1.9rc1/sympy/physics/hep/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/hep/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13812 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/hep/tests/test_gamma_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7357 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/hydrogen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3904 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17568 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/mechanics/body.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23459 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/mechanics/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24437 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/mechanics/joint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8440 2021-09-19 19:47:04.113183 sympy-1.9rc1/sympy/physics/mechanics/jointsmethod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27263 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/kane.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18316 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15349 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/linearize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7577 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/particle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10807 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18655 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/system.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/mechanics/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9288 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9101 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20576 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_joint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5710 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_jointsmethod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13422 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19025 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14271 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9407 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_lagrange2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11745 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5073 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_particle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8695 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/mechanics/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/optics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20313 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/gaussopt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5541 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/medium.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21201 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/polarization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/optics/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/tests/test_gaussopt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/tests/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/tests/test_polarization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7790 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3183 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/tests/test_waves.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21468 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9575 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/optics/waves.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5890 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/paulialgebra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2091 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/pring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/qho_1d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/quantum/
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4348 2021-09-19 19:47:04.117183 sympy-1.9rc1/sympy/physics/quantum/anticommutator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6095 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/boson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8810 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23033 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/cg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11945 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/circuitplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13807 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/circuitutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7399 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/commutator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/dagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9497 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/density.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4479 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/fermion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41687 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/gate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9804 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/grover.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19449 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/hilbert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27466 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/identitysearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4221 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/innerproduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3462 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/matrixcache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8412 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/matrixutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19023 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11504 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/operatorordering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9598 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/operatorset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17262 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/pauli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/piab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7021 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/qapply.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6291 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14144 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/qexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/qft.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25628 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/qubit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18277 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/represent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20844 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/sho1d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5371 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/shor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    72785 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/spin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30432 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/state.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14482 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/tensorproduct.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/quantum/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-09-19 19:47:04.121183 sympy-1.9rc1/sympy/physics/quantum/tests/test_anticommutator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_boson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8715 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_cg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_circuitplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13119 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_circuitutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2685 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_commutator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1833 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_dagger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9598 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_fermion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12322 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_gate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_hilbert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17706 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_identitysearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_innerproduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4063 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_matrixutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6946 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_operatorordering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_operatorset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_pauli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_piab.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30068 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4438 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_qapply.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_qexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_qft.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8782 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_qubit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5119 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_represent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4556 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_sho1d.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_shor.py
+-rw-r--r--   0 runner    (1001) docker     (121)   344475 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_spin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6391 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-09-19 19:47:04.125183 sympy-1.9rc1/sympy/physics/quantum/tests/test_tensorproduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)    89896 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/secondquant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/sho.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.373290 sympy-1.9rc1/sympy/physics/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9241 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_clebsch_gordan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4689 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_hydrogen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_paulialgebra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2815 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_physics_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_pring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_qho_1d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48231 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_secondquant.py
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/tests/test_sho.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/physics/units/
+-rw-r--r--   0 runner    (1001) docker     (121)    12011 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/physics/units/definitions/
+-rw-r--r--   0 runner    (1001) docker     (121)     7194 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/definitions/dimension_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13695 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/definitions/unit_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23549 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5938 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7381 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/physics/units/systems/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/cgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6726 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/length_weight_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/mks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1599 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/mksa.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/natural.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13649 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/systems/si.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/physics/units/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5894 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3110 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_dimensionsystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16089 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_unit_system_cgs_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_unitsystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6314 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7453 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/unitsystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7741 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/units/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/physics/vector/
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19382 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/vector/dyadic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8513 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/vector/fieldfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52776 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/vector/frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24510 2021-09-19 19:47:04.129183 sympy-1.9rc1/sympy/physics/vector/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20602 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/point.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11776 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/printing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/physics/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4153 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_dyadic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5727 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_fieldfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21731 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20546 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10131 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10284 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7762 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26436 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/vector/vector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31382 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/physics/wigner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/plotting/
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22892 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/experimental_lambdify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/plotting/intervalmath/
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15530 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/interval_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2385 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/interval_membership.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14809 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/lib_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/plotting/intervalmath/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9862 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/tests/test_interval_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4216 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/tests/test_interval_membership.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9034 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/intervalmath/tests/test_intervalmath.py
+-rw-r--r--   0 runner    (1001) docker     (121)    90816 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15550 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/plot_implicit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/plotting/pygletplot/
+-rw-r--r--   0 runner    (1001) docker     (121)     3732 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/pygletplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12456 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/pygletplot/color_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3064 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/pygletplot/managed_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13324 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/pygletplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8655 2021-09-19 19:47:04.133183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_axes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4001 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6941 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5362 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_interval.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14113 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11496 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_mode_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5333 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_modes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3811 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4838 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/plot_window.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/plotting/pygletplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/pygletplot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.377290 sympy-1.9rc1/sympy/plotting/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_experimental_lambdify.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23787 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4848 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_plot_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6864 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_region_and.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7939 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_region_not.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8809 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_region_or.png
+-rw-r--r--   0 runner    (1001) docker     (121)    10002 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_region_xor.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12191 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/tests/test_textplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5061 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/plotting/textplot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/
+-rw-r--r--   0 runner    (1001) docker     (121)     5174 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/agca/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21937 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/homomorphisms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10788 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/ideals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46881 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/agca/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4164 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/tests/test_homomorphisms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/tests/test_ideals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13539 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/agca/tests/test_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/benchmarks/bench_galoispolys.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2021-09-19 19:47:04.137183 sympy-1.9rc1/sympy/polys/benchmarks/bench_groebnertools.py
+-rw-r--r--   0 runner    (1001) docker     (121)   446790 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/benchmarks/bench_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57410 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11480 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33396 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/densearith.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35901 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/densebasic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25891 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/densetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5740 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21781 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/distributedmodules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domainmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/domains/
+-rw-r--r--   0 runner    (1001) docker     (121)     1873 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14715 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/algebraicfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/characteristiczero.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4620 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/complexfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/compositedomain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35140 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/domainelement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6907 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/expressiondomain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/expressionrawdomain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2591 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6022 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/finitefield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5945 2021-09-19 19:47:04.141183 sympy-1.9rc1/sympy/polys/domains/fractionfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18005 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/gaussiandomains.py
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/gmpyfinitefield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3017 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/gmpyintegerring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3178 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/gmpyrationalfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/groundtypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5823 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/integerring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5087 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/modularinteger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4616 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/mpelements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6178 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/old_fractionfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14912 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/old_polynomialring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/polynomialring.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/pythonfinitefield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/pythonintegerring.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/pythonrational.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/pythonrationalfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5853 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/quotientring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4608 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/rationalfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/realfield.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/ring.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/simpledomain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/domains/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41388 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/tests/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3312 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/tests/test_polynomialring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/domains/tests/test_quotientring.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41215 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/euclidtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38036 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/factortools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4328 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/fglmtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21205 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51834 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/galoistools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23339 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/groebnertools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3732 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/heuristicgcd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/matrices/
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12319 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8255 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/dense.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40398 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/domainmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3643 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/domainscalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/eigen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6749 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/linsolve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-09-19 19:47:04.145183 sympy-1.9rc1/sympy/polys/matrices/normalforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34639 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/sdm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.381290 sympy-1.9rc1/sympy/polys/matrices/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14440 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_ddm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9479 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29619 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_domainmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3624 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_domainscalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3101 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_linsolve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_normalforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12794 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/matrices/tests/test_sdm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58652 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/modulargcd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18968 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/monomials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14915 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/multivariate_resultants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34132 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/numberfields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8515 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/orderings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10096 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/orthopolys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14661 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/partfrac.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53300 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyerrors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10258 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9749 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21995 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyoptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96034 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyquinticconst.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33603 2021-09-19 19:47:04.149183 sympy-1.9rc1/sympy/polys/polyroots.py
+-rw-r--r--   0 runner    (1001) docker     (121)   186927 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/polytools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14113 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/polyutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/rationaltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    57846 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/ring_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69021 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/rings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60650 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/rootisolation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39800 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/rootoftools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13346 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11087 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/specialpolys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11464 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/sqfreetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87900 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/subresultants_qq_zz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/polys/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6160 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/tests/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40017 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/tests/test_densearith.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21464 2021-09-19 19:47:04.153183 sympy-1.9rc1/sympy/polys/tests/test_densebasic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24475 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_densetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3183 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7639 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_distributedmodules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19482 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_euclidtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24409 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_factortools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10128 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27866 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_galoistools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18584 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_groebnertools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_heuristicgcd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_injections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9007 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_modulargcd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10988 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_monomials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9453 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_multivariate_resultants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35418 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_numberfields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4254 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_orderings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5322 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_orthopolys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6880 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_partfrac.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13070 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polyclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polyfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7218 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12320 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polyoptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25246 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polyroots.py
+-rw-r--r--   0 runner    (1001) docker     (121)   120860 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polytools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11223 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_polyutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4143 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_pythonrational.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2125 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_rationaltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24233 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_ring_series.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43182 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_rings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31460 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_rootisolation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19906 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_rootoftools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13655 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4795 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_specialpolys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4387 2021-09-19 19:47:04.157183 sympy-1.9rc1/sympy/polys/tests/test_sqfreetools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13091 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/polys/tests/test_subresultants_qq_zz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/printing/
+-rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17803 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/aesaracode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26762 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/c.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/ccode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32612 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/codeprinter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2565 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5665 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/cxx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/cxxcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8285 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/dot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/fcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28305 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20494 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/glsl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/gtk.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11494 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/jscode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22646 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/julia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/lambdarepr.py
+-rw-r--r--   0 runner    (1001) docker     (121)   113920 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/latex.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16709 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/llvmjitcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10347 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/maple.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12417 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/mathematica.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75196 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/mathml.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19395 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25522 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/octave.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5264 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/precedence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/printing/pretty/
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2021-09-19 19:47:04.161183 sympy-1.9rc1/sympy/printing/pretty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   103452 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/pretty/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20063 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/pretty/pretty_symbology.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18737 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/pretty/stringpict.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/printing/pretty/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/pretty/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   176127 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/pretty/tests/test_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11806 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/preview.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14472 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19966 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/pycode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/python.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14603 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/rcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11607 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/repr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20957 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/rust.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32901 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/str.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11694 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tableform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10750 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/printing/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20827 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_aesaracode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28967 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_c.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_codeprinter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2453 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_cxx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4369 2021-09-19 19:47:04.165183 sympy-1.9rc1/sympy/printing/tests/test_dot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33854 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_fortran.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28787 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_glsl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_gtk.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_jscode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13517 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_julia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6544 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_lambdarepr.py
+-rw-r--r--   0 runner    (1001) docker     (121)   116747 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_latex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5560 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_llvmjit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12928 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_maple.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10933 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_mathematica.py
+-rw-r--r--   0 runner    (1001) docker     (121)    94860 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_mathml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9473 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18365 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_octave.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_precedence.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13125 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_pycode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7480 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14101 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_rcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11422 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11644 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40014 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5641 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_tableform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15607 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20837 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_theanocode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6080 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18196 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/theanocode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/printing/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/release.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/sandbox/indexed_integrals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/sandbox/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/sandbox/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/sandbox/tests/test_indexed_integrals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/series/
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3115 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/approximants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/aseries.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.385290 sympy-1.9rc1/sympy/series/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/benchmarks/bench_limit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-09-19 19:47:04.169183 sympy-1.9rc1/sympy/series/benchmarks/bench_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51747 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/formal.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22798 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23291 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/gruntz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/kauers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11465 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/limits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7686 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/limitseq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18726 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/residues.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35570 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/series_class.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/series/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_approximants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1796 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_aseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4649 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_demidovich.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21897 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_formal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15591 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_gruntz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_kauers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32678 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_limits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5049 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_limitseq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_lseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16723 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_nseries.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15257 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2663 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_residues.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10604 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13698 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/series/tests/test_series.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/sets/
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7782 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/conditionset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/contains.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47552 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/fancysets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/sets/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8756 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16967 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5252 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/issubset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/mul.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3252 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/power.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/handlers/union.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7583 2021-09-19 19:47:04.173183 sympy-1.9rc1/sympy/sets/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2895 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/powerset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/setexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    72439 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/sets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/sets/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10685 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_conditionset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_contains.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48157 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_fancysets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_powerset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14487 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_setexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63220 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/sets/tests/test_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/simplify/
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/combsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30330 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/cse_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/cse_opts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10177 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/epathtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61845 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/fu.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18842 2021-09-19 19:47:04.177183 sympy-1.9rc1/sympy/simplify/gammasimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84686 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/hyperexpand.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/hyperexpand_doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26364 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/powsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40310 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/radsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7604 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/ratsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    73380 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21596 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/sqrtdenest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/simplify/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_combsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18887 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_cse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_epathtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18248 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_fu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_gammasimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39828 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_hyperexpand.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13406 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_powsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17977 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_radsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_ratsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38859 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7379 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_sqrtdenest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_traversaltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18548 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/tests/test_trigsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2021-09-19 19:47:04.181183 sympy-1.9rc1/sympy/simplify/traversaltools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44915 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/simplify/trigsimp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/benchmarks/bench_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17882 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/bivariate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/decompogen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10338 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/deutils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/diophantine/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/diophantine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   119692 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/diophantine/diophantine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/diophantine/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/diophantine/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41561 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/diophantine/tests/test_diophantine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33678 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/inequalities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/ode/
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9677 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/ode/hypergeometric.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39242 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/ode/lie_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18175 2021-09-19 19:47:04.185183 sympy-1.9rc1/sympy/solvers/ode/nonhomogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (121)   145216 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30662 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/riccati.py
+-rw-r--r--   0 runner    (1001) docker     (121)   110201 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/single.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16171 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/subscheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71802 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/systems.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/ode/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5059 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/tests/test_lie_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44416 2021-09-19 19:47:04.189183 sympy-1.9rc1/sympy/solvers/ode/tests/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28866 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/ode/tests/test_riccati.py
+-rw-r--r--   0 runner    (1001) docker     (121)    99025 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/ode/tests/test_single.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12118 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/ode/tests/test_subscheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)   130037 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/ode/tests/test_systems.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35885 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/pde.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11281 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/polysys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24884 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/recurr.py
+-rw-r--r--   0 runner    (1001) docker     (121)   130460 2021-09-19 19:47:04.193183 sympy-1.9rc1/sympy/solvers/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)   132158 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/solveset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.389290 sympy-1.9rc1/sympy/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8316 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_constantsimp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_decompogen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20173 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_inequalities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9057 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4855 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_polysys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9149 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_recurr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    94260 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)   117579 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/solvers/tests/test_solveset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/stats/
+-rw-r--r--   0 runner    (1001) docker     (121)     8454 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7818 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/compound_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20513 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/crv.py
+-rw-r--r--   0 runner    (1001) docker     (121)   119086 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/crv_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11476 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/drv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18648 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/drv_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/error_prop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16467 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/frv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22777 2021-09-19 19:47:04.197183 sympy-1.9rc1/sympy/stats/frv_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15693 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/joint_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29713 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/joint_rv_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21570 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/matrix_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/random_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14830 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/random_matrix_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53686 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13692 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/rv_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/stats/sampling/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2649 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/sample_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/sample_pymc3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6269 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/sample_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/stats/sampling/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/tests/test_sample_continuous_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3286 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/tests/test_sample_discrete_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2990 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/sampling/tests/test_sample_finite_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2301 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/stochastic_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87390 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/stochastic_process_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10179 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/symbolic_multivariate_probability.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22786 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/symbolic_probability.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5511 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_compound_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54762 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_continuous_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11192 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_discrete_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_error_prop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19728 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_finite_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16818 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_joint_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8578 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_matrix_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3417 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_mix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5373 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_random_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12257 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_rv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38196 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_stochastic_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5433 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_symbolic_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9087 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/stats/tests/test_symbolic_probability.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/strategies/
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-09-19 19:47:04.201183 sympy-1.9rc1/sympy/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/strategies/branch/
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2748 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/strategies/branch/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/tests/test_traverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/branch/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2941 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4359 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/rl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/strategies/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/test_rl.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/test_strat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1752 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/test_traverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2559 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3747 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/strategies/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/tensor/
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/tensor/array/
+-rw-r--r--   0 runner    (1001) docker     (121)     7299 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11869 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/array_comprehension.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4748 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/array_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16294 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/arrayop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6187 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/dense_ndim_array.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/tensor/array/expressions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59914 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/array_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5470 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/arrayexpr_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28886 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/conv_array_to_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7185 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/conv_indexed_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3068 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/conv_matrix_to_array.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/tensor/array/expressions/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20979 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_array_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_arrayexpr_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2251 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_as_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21096 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_convert_array_to_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6059 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_convert_index_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3595 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_convert_matrix_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3568 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/expressions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/mutable_ndim_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18749 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/ndim_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6362 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/sparse_ndim_array.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.393290 sympy-1.9rc1/sympy/tensor/array/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4596 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/tests/test_array_comprehension.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-09-19 19:47:04.205183 sympy-1.9rc1/sympy/tensor/array/tests/test_array_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24261 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/array/tests/test_arrayop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15602 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/array/tests/test_immutable_ndim_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12888 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/array/tests/test_mutable_ndim_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/array/tests/test_ndim_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/array/tests/test_ndim_array_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15435 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/index_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24566 2021-09-19 19:47:04.209183 sympy-1.9rc1/sympy/tensor/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (121)   144970 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/tensor/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7089 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/test_index_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15823 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/test_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    70994 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/test_tensor_element.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17126 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/tests/test_tensor_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6617 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/tensor/toperators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9715 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/quality_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5319 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/randtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    88459 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/runtests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9691 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/tests/diagnose_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18591 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/tests/test_code_quality.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/tests/test_module_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7753 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/testing/tmpfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/this.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/unify/
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7037 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1798 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/rewrite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/unify/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/tests/test_rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5561 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/tests/test_sympy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3021 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/tests/test_unify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3952 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/unify/usympy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/utilities/_compilation/
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/utilities/_compilation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2884 2021-09-19 19:47:04.213183 sympy-1.9rc1/sympy/utilities/_compilation/availability.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20491 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/_compilation/compilation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9053 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/_compilation/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/utilities/_compilation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/_compilation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1733 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/_compilation/tests/test_compilation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7807 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/_compilation/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41293 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/autowrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81465 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7199 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43513 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/enumerative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7163 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    76983 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49485 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/lambdify.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/magic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9382 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/matchpy_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/utilities/mathml/
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/mathml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/utilities/mathml/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   114443 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/mathml/data/mmlctop.xsl
+-rw-r--r--   0 runner    (1001) docker     (121)   137304 2021-09-19 19:47:04.217183 sympy-1.9rc1/sympy/utilities/mathml/data/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (121)   114432 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/mathml/data/simple_mmlctop.xsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13510 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/pkgdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/quality_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/randtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/utilities/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14687 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_autowrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54928 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18268 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_codegen_julia.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17688 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_codegen_octave.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12202 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_codegen_rust.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6089 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_enumerative.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31561 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_iterables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47719 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_lambdify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3913 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_matchpy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3399 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22931 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    92412 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tests/test_wester.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/utilities/tmpfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/vector/
+-rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11391 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/basisdependent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37194 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/coordsysrect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3555 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/deloperator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/dyadic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15579 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15972 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/implicitregion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6833 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10609 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11677 2021-09-19 19:47:04.221183 sympy-1.9rc1/sympy/vector/orienters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5913 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/parametricregion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4516 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/point.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:52:01.397290 sympy-1.9rc1/sympy/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19426 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_coordsysrect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4194 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_dyadic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14058 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_field_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7829 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4121 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_implicitregion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4935 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3942 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_parametricregion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5804 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6993 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17801 2021-09-19 19:47:04.225183 sympy-1.9rc1/sympy/vector/vector.py
```

### Comparing `sympy-1.9/AUTHORS` & `sympy-1.9rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `sympy-1.9/LICENSE` & `sympy-1.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sympy-1.9/PKG-INFO` & `sympy-1.9rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy
-Version: 1.9
+Version: 1.9rc1
 Summary: Computer algebra system (CAS) in Python
 Home-page: https://sympy.org
 Author: SymPy development team
 Author-email: sympy@googlegroups.com
 License: BSD
 Keywords: Math CAS
 Platform: UNKNOWN
```

### Comparing `sympy-1.9/README.md` & `sympy-1.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `sympy-1.9/data/TeXmacs/LICENSE` & `sympy-1.9rc1/data/TeXmacs/LICENSE`

 * *Files identical despite different names*

### Comparing `sympy-1.9/data/TeXmacs/bin/tm_sympy` & `sympy-1.9rc1/data/TeXmacs/bin/tm_sympy`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/Makefile` & `sympy-1.9rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/api/conf.py` & `sympy-1.9rc1/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/cheatsheet/cheatsheet.tex` & `sympy-1.9rc1/doc/cheatsheet/cheatsheet.tex`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/cheatsheet/combinatoric_cheatsheet.tex` & `sympy-1.9rc1/doc/cheatsheet/combinatoric_cheatsheet.tex`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/ext/docscrape.py` & `sympy-1.9rc1/doc/ext/docscrape.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/ext/docscrape_sphinx.py` & `sympy-1.9rc1/doc/ext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/ext/numpydoc.py` & `sympy-1.9rc1/doc/ext/numpydoc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/ext/sympylive.py` & `sympy-1.9rc1/doc/ext/sympylive.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/generate_logos.py` & `sympy-1.9rc1/doc/generate_logos.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/man/isympy.1` & `sympy-1.9rc1/doc/man/isympy.1`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/man/isympy.xml` & `sympy-1.9rc1/doc/man/isympy.xml`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/_static/default.css_t` & `sympy-1.9rc1/doc/src/_static/default.css_t`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/_static/sympylogo.png` & `sympy-1.9rc1/doc/src/_static/sympylogo.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/_static/sympylogo_big.png` & `sympy-1.9rc1/doc/src/_static/sympylogo_big.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/aboutus.rst` & `sympy-1.9rc1/doc/src/aboutus.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/citing.rst` & `sympy-1.9rc1/doc/src/citing.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/conf.py` & `sympy-1.9rc1/doc/src/conf.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/documentation-style-guide.rst` & `sympy-1.9rc1/doc/src/documentation-style-guide.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/gotchas.rst` & `sympy-1.9rc1/doc/src/gotchas.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/guides/assumptions.rst` & `sympy-1.9rc1/doc/src/guides/assumptions.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/guides/booleans.rst` & `sympy-1.9rc1/doc/src/guides/booleans.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/index.rst` & `sympy-1.9rc1/doc/src/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/install.rst` & `sympy-1.9rc1/doc/src/install.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/logo/sympy-use-text.svg` & `sympy-1.9rc1/doc/src/logo/sympy-use-text.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/logo/sympy.svg` & `sympy-1.9rc1/doc/src/logo/sympy.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/assumptions/index.rst` & `sympy-1.9rc1/doc/src/modules/assumptions/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/assumptions/predicates.rst` & `sympy-1.9rc1/doc/src/modules/assumptions/predicates.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/categories.rst` & `sympy-1.9rc1/doc/src/modules/categories.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/codegen.rst` & `sympy-1.9rc1/doc/src/modules/codegen.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/combinatorics/fp_groups.rst` & `sympy-1.9rc1/doc/src/modules/combinatorics/fp_groups.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/combinatorics/pc_groups.rst` & `sympy-1.9rc1/doc/src/modules/combinatorics/pc_groups.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/combinatorics/permutations.rst` & `sympy-1.9rc1/doc/src/modules/combinatorics/permutations.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/concrete.rst` & `sympy-1.9rc1/doc/src/modules/concrete.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/core.rst` & `sympy-1.9rc1/doc/src/modules/core.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/crypto.rst` & `sympy-1.9rc1/doc/src/modules/crypto.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/diffgeom.rst` & `sympy-1.9rc1/doc/src/modules/diffgeom.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/discrete.rst` & `sympy-1.9rc1/doc/src/modules/discrete.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/evalf.rst` & `sympy-1.9rc1/doc/src/modules/evalf.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/functions/combinatorial.rst` & `sympy-1.9rc1/doc/src/modules/functions/combinatorial.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/functions/elementary.rst` & `sympy-1.9rc1/doc/src/modules/functions/elementary.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/functions/special.rst` & `sympy-1.9rc1/doc/src/modules/functions/special.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/geometry/index.rst` & `sympy-1.9rc1/doc/src/modules/geometry/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/holonomic/about.rst` & `sympy-1.9rc1/doc/src/modules/holonomic/about.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/holonomic/operations.rst` & `sympy-1.9rc1/doc/src/modules/holonomic/operations.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/holonomic/represent.rst` & `sympy-1.9rc1/doc/src/modules/holonomic/represent.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/holonomic/uses.rst` & `sympy-1.9rc1/doc/src/modules/holonomic/uses.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/index.rst` & `sympy-1.9rc1/doc/src/modules/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/integrals/g-functions.rst` & `sympy-1.9rc1/doc/src/modules/integrals/g-functions.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/integrals/integrals.rst` & `sympy-1.9rc1/doc/src/modules/integrals/integrals.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/liealgebras/index.rst` & `sympy-1.9rc1/doc/src/modules/liealgebras/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/logic.rst` & `sympy-1.9rc1/doc/src/modules/logic.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/matrices/expressions.rst` & `sympy-1.9rc1/doc/src/modules/matrices/expressions.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/matrices/immutablematrices.rst` & `sympy-1.9rc1/doc/src/modules/matrices/immutablematrices.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/matrices/matrices.rst` & `sympy-1.9rc1/doc/src/modules/matrices/matrices.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/ntheory.rst` & `sympy-1.9rc1/doc/src/modules/ntheory.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/numeric-computation.rst` & `sympy-1.9rc1/doc/src/modules/numeric-computation.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/parsing.rst` & `sympy-1.9rc1/doc/src/modules/parsing.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/continuum_mechanics/allowed-sign-conventions.png` & `sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/allowed-sign-conventions.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/continuum_mechanics/beam_problems.rst` & `sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/beam_problems.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/continuum_mechanics/ildreaction.png` & `sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/ildreaction.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/continuum_mechanics/ildshear.png` & `sympy-1.9rc1/doc/src/modules/physics/continuum_mechanics/ildshear.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/control/control.rst` & `sympy-1.9rc1/doc/src/modules/physics/control/control.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/control/control_plots.rst` & `sympy-1.9rc1/doc/src/modules/physics/control/control_plots.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/advanced.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/advanced.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/api/part_bod.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/api/part_bod.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/autolev_parser.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/autolev_parser.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/bicycle_example.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/bicycle_example.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/lin_pend_nonmin_example.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/lin_pend_nonmin_example.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/multi_degree_freedom_holonomic_system.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/multi_degree_freedom_holonomic_system.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/multidof-holonomic.png` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/multidof-holonomic.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/pendulum_nonmin.svg` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/pendulum_nonmin.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc.svg` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane_constraints.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example_kane_constraints.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples/rollingdisc_example_lagrange.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples/rollingdisc_example_lagrange.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/examples.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/examples.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/index.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/kane.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/kane.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/lagrange.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/lagrange.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/linearize.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/linearize.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/masses.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/masses.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/reference.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/reference.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/sympy_mechanics_for_autolev_users.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/sympy_mechanics_for_autolev_users.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/mechanics/symsystem.rst` & `sympy-1.9rc1/doc/src/modules/physics/mechanics/symsystem.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/quantum/index.rst` & `sympy-1.9rc1/doc/src/modules/physics/quantum/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/units/examples.rst` & `sympy-1.9rc1/doc/src/modules/physics/units/examples.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/units/index.rst` & `sympy-1.9rc1/doc/src/modules/physics/units/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/units/philosophy.rst` & `sympy-1.9rc1/doc/src/modules/physics/units/philosophy.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/advanced.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/advanced.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/api/fieldfunctions.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/api/fieldfunctions.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/api/functions.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/api/functions.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/fields.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/fields.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/index.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_1.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_1.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_1pt.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_1pt.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_2.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_2.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_2pt.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_2pt.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_3.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_3.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_4.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_4.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_angvel1.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_angvel1.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_angvel2.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_angvel2.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_angvel3.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_angvel3.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kin_rolling.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/kin_rolling.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/kinematics.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/kinematics.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/simp_rot.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/simp_rot.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_add.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_add.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_cross.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_cross.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_dot.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_dot.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_fix_notfix.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_fix_notfix.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_mul.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_mul.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_rep.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_rep.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vec_simp_der.svg` & `sympy-1.9rc1/doc/src/modules/physics/vector/vec_simp_der.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/physics/vector/vectors.rst` & `sympy-1.9rc1/doc/src/modules/physics/vector/vectors.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/plotting.rst` & `sympy-1.9rc1/doc/src/modules/plotting.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/agca.rst` & `sympy-1.9rc1/doc/src/modules/polys/agca.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/basics.rst` & `sympy-1.9rc1/doc/src/modules/polys/basics.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/domainmatrix.rst` & `sympy-1.9rc1/doc/src/modules/polys/domainmatrix.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/domainsintro.rst` & `sympy-1.9rc1/doc/src/modules/polys/domainsintro.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/domainsref.rst` & `sympy-1.9rc1/doc/src/modules/polys/domainsref.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/index.rst` & `sympy-1.9rc1/doc/src/modules/polys/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/internals.rst` & `sympy-1.9rc1/doc/src/modules/polys/internals.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/literature.rst` & `sympy-1.9rc1/doc/src/modules/polys/literature.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/reference.rst` & `sympy-1.9rc1/doc/src/modules/polys/reference.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/ringseries.rst` & `sympy-1.9rc1/doc/src/modules/polys/ringseries.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/solvers.rst` & `sympy-1.9rc1/doc/src/modules/polys/solvers.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/polys/wester.rst` & `sympy-1.9rc1/doc/src/modules/polys/wester.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/printing.rst` & `sympy-1.9rc1/doc/src/modules/printing.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/rewriting.rst` & `sympy-1.9rc1/doc/src/modules/rewriting.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/series/formal.rst` & `sympy-1.9rc1/doc/src/modules/series/formal.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/series/sequences.rst` & `sympy-1.9rc1/doc/src/modules/series/sequences.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/series/series.rst` & `sympy-1.9rc1/doc/src/modules/series/series.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/sets.rst` & `sympy-1.9rc1/doc/src/modules/sets.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/simplify/fu.rst` & `sympy-1.9rc1/doc/src/modules/simplify/fu.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/simplify/hyperexpand.rst` & `sympy-1.9rc1/doc/src/modules/simplify/hyperexpand.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/simplify/simplify.rst` & `sympy-1.9rc1/doc/src/modules/simplify/simplify.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/solvers/diophantine.rst` & `sympy-1.9rc1/doc/src/modules/solvers/diophantine.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/solvers/ode.rst` & `sympy-1.9rc1/doc/src/modules/solvers/ode.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/solvers/pde.rst` & `sympy-1.9rc1/doc/src/modules/solvers/pde.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/solvers/solvers.rst` & `sympy-1.9rc1/doc/src/modules/solvers/solvers.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/solvers/solveset.rst` & `sympy-1.9rc1/doc/src/modules/solvers/solveset.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/stats.rst` & `sympy-1.9rc1/doc/src/modules/stats.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/tensor/tensor.rst` & `sympy-1.9rc1/doc/src/modules/tensor/tensor.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/utilities/autowrap.rst` & `sympy-1.9rc1/doc/src/modules/utilities/autowrap.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/utilities/codegen.rst` & `sympy-1.9rc1/doc/src/modules/utilities/codegen.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/utilities/enumerative.rst` & `sympy-1.9rc1/doc/src/modules/utilities/enumerative.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/utilities/iterables.rst` & `sympy-1.9rc1/doc/src/modules/utilities/iterables.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/api/classes.rst` & `sympy-1.9rc1/doc/src/modules/vector/api/classes.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/api/orienterclasses.rst` & `sympy-1.9rc1/doc/src/modules/vector/api/orienterclasses.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/api/vectorfunctions.rst` & `sympy-1.9rc1/doc/src/modules/vector/api/vectorfunctions.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/basics.rst` & `sympy-1.9rc1/doc/src/modules/vector/basics.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/coordsys.rst` & `sympy-1.9rc1/doc/src/modules/vector/coordsys.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/coordsys_rot.svg` & `sympy-1.9rc1/doc/src/modules/vector/coordsys_rot.svg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/examples.rst` & `sympy-1.9rc1/doc/src/modules/vector/examples.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/fields.rst` & `sympy-1.9rc1/doc/src/modules/vector/fields.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/index.rst` & `sympy-1.9rc1/doc/src/modules/vector/index.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/intro.rst` & `sympy-1.9rc1/doc/src/modules/vector/intro.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/modules/vector/vector_integration.rst` & `sympy-1.9rc1/doc/src/modules/vector/vector_integration.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/outreach.rst` & `sympy-1.9rc1/doc/src/outreach.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/pics/consoleascii.png` & `sympy-1.9rc1/doc/src/pics/consoleascii.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/pics/consoleunicode.png` & `sympy-1.9rc1/doc/src/pics/consoleunicode.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/pics/ipythonnotebook.png` & `sympy-1.9rc1/doc/src/pics/ipythonnotebook.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/pics/ipythonqtconsole.png` & `sympy-1.9rc1/doc/src/pics/ipythonqtconsole.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/pics/pngview1.png` & `sympy-1.9rc1/doc/src/pics/pngview1.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/special_topics/classification.rst` & `sympy-1.9rc1/doc/src/special_topics/classification.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/special_topics/finite_diff_derivatives.rst` & `sympy-1.9rc1/doc/src/special_topics/finite_diff_derivatives.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/basic_operations.rst` & `sympy-1.9rc1/doc/src/tutorial/basic_operations.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/calculus.rst` & `sympy-1.9rc1/doc/src/tutorial/calculus.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/gotchas.rst` & `sympy-1.9rc1/doc/src/tutorial/gotchas.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/intro.rst` & `sympy-1.9rc1/doc/src/tutorial/intro.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/manipulation.rst` & `sympy-1.9rc1/doc/src/tutorial/manipulation.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/matrices.rst` & `sympy-1.9rc1/doc/src/tutorial/matrices.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/preliminaries.rst` & `sympy-1.9rc1/doc/src/tutorial/preliminaries.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/printing.rst` & `sympy-1.9rc1/doc/src/tutorial/printing.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/simplification.rst` & `sympy-1.9rc1/doc/src/tutorial/simplification.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/doc/src/tutorial/solvers.rst` & `sympy-1.9rc1/doc/src/tutorial/solvers.rst`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/README` & `sympy-1.9rc1/examples/README`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/autowrap_integrators.py` & `sympy-1.9rc1/examples/advanced/autowrap_integrators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/autowrap_ufuncify.py` & `sympy-1.9rc1/examples/advanced/autowrap_ufuncify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/curvilinear_coordinates.py` & `sympy-1.9rc1/examples/advanced/curvilinear_coordinates.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/dense_coding_example.py` & `sympy-1.9rc1/examples/advanced/dense_coding_example.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/fem.py` & `sympy-1.9rc1/examples/advanced/fem.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/gibbs_phenomenon.py` & `sympy-1.9rc1/examples/advanced/gibbs_phenomenon.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/grover_example.py` & `sympy-1.9rc1/examples/advanced/grover_example.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/hydrogen.py` & `sympy-1.9rc1/examples/advanced/hydrogen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/pidigits.py` & `sympy-1.9rc1/examples/advanced/pidigits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/pyglet_plotting.py` & `sympy-1.9rc1/examples/advanced/pyglet_plotting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/qft.py` & `sympy-1.9rc1/examples/advanced/qft.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/advanced/relativity.py` & `sympy-1.9rc1/examples/advanced/relativity.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/all.py` & `sympy-1.9rc1/examples/all.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/beginner/differentiation.py` & `sympy-1.9rc1/examples/beginner/differentiation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/beginner/limits_examples.py` & `sympy-1.9rc1/examples/beginner/limits_examples.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/beginner/plot_examples.py` & `sympy-1.9rc1/examples/beginner/plot_examples.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/beginner/print_pretty.py` & `sympy-1.9rc1/examples/beginner/print_pretty.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/beginner/substitution.py` & `sympy-1.9rc1/examples/beginner/substitution.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/coupled_cluster.py` & `sympy-1.9rc1/examples/intermediate/coupled_cluster.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/differential_equations.py` & `sympy-1.9rc1/examples/intermediate/differential_equations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/infinite_1d_box.py` & `sympy-1.9rc1/examples/intermediate/infinite_1d_box.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/mplot2d.py` & `sympy-1.9rc1/examples/intermediate/mplot2d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/mplot3d.py` & `sympy-1.9rc1/examples/intermediate/mplot3d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/partial_differential_eqs.py` & `sympy-1.9rc1/examples/intermediate/partial_differential_eqs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/sample.py` & `sympy-1.9rc1/examples/intermediate/sample.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/trees.py` & `sympy-1.9rc1/examples/intermediate/trees.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/examples/intermediate/vandermonde.py` & `sympy-1.9rc1/examples/intermediate/vandermonde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/isympy.py` & `sympy-1.9rc1/isympy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/setup.cfg` & `sympy-1.9rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sympy-1.9/setup.py` & `sympy-1.9rc1/setup.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/__init__.py` & `sympy-1.9rc1/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/abc.py` & `sympy-1.9rc1/sympy/abc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/algebras/quaternion.py` & `sympy-1.9rc1/sympy/algebras/quaternion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/algebras/tests/test_quaternion.py` & `sympy-1.9rc1/sympy/algebras/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/__init__.py` & `sympy-1.9rc1/sympy/assumptions/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/ask.py` & `sympy-1.9rc1/sympy/assumptions/ask.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/ask_generated.py` & `sympy-1.9rc1/sympy/assumptions/ask_generated.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/assume.py` & `sympy-1.9rc1/sympy/assumptions/assume.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/cnf.py` & `sympy-1.9rc1/sympy/assumptions/cnf.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/facts.py` & `sympy-1.9rc1/sympy/assumptions/facts.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/handlers/calculus.py` & `sympy-1.9rc1/sympy/assumptions/handlers/calculus.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/handlers/common.py` & `sympy-1.9rc1/sympy/assumptions/handlers/common.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/handlers/matrices.py` & `sympy-1.9rc1/sympy/assumptions/handlers/matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/handlers/ntheory.py` & `sympy-1.9rc1/sympy/assumptions/handlers/ntheory.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/handlers/order.py` & `sympy-1.9rc1/sympy/assumptions/handlers/order.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/handlers/sets.py` & `sympy-1.9rc1/sympy/assumptions/handlers/sets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/predicates/calculus.py` & `sympy-1.9rc1/sympy/assumptions/predicates/calculus.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/predicates/common.py` & `sympy-1.9rc1/sympy/assumptions/predicates/common.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/predicates/matrices.py` & `sympy-1.9rc1/sympy/assumptions/predicates/matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/predicates/ntheory.py` & `sympy-1.9rc1/sympy/assumptions/predicates/ntheory.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/predicates/order.py` & `sympy-1.9rc1/sympy/assumptions/predicates/order.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/predicates/sets.py` & `sympy-1.9rc1/sympy/assumptions/predicates/sets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/refine.py` & `sympy-1.9rc1/sympy/assumptions/refine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/relation/binrel.py` & `sympy-1.9rc1/sympy/assumptions/relation/binrel.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/relation/equality.py` & `sympy-1.9rc1/sympy/assumptions/relation/equality.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/satask.py` & `sympy-1.9rc1/sympy/assumptions/satask.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/sathandlers.py` & `sympy-1.9rc1/sympy/assumptions/sathandlers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_assumptions_2.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_assumptions_2.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_context.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_matrices.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_query.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_refine.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_refine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_satask.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_satask.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_sathandlers.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_sathandlers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/tests/test_wrapper.py` & `sympy-1.9rc1/sympy/assumptions/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/assumptions/wrapper.py` & `sympy-1.9rc1/sympy/assumptions/wrapper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/benchmarks/bench_discrete_log.py` & `sympy-1.9rc1/sympy/benchmarks/bench_discrete_log.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/benchmarks/bench_meijerint.py` & `sympy-1.9rc1/sympy/benchmarks/bench_meijerint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/benchmarks/bench_symbench.py` & `sympy-1.9rc1/sympy/benchmarks/bench_symbench.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/__init__.py` & `sympy-1.9rc1/sympy/calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/euler.py` & `sympy-1.9rc1/sympy/calculus/euler.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/finite_diff.py` & `sympy-1.9rc1/sympy/calculus/finite_diff.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/singularities.py` & `sympy-1.9rc1/sympy/calculus/singularities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/tests/test_euler.py` & `sympy-1.9rc1/sympy/calculus/tests/test_euler.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/tests/test_finite_diff.py` & `sympy-1.9rc1/sympy/calculus/tests/test_finite_diff.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/tests/test_singularities.py` & `sympy-1.9rc1/sympy/calculus/tests/test_singularities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/tests/test_util.py` & `sympy-1.9rc1/sympy/calculus/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/calculus/util.py` & `sympy-1.9rc1/sympy/calculus/util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/categories/__init__.py` & `sympy-1.9rc1/sympy/categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/categories/baseclasses.py` & `sympy-1.9rc1/sympy/categories/baseclasses.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/categories/diagram_drawing.py` & `sympy-1.9rc1/sympy/categories/diagram_drawing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/categories/tests/test_baseclasses.py` & `sympy-1.9rc1/sympy/categories/tests/test_baseclasses.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/categories/tests/test_drawing.py` & `sympy-1.9rc1/sympy/categories/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/__init__.py` & `sympy-1.9rc1/sympy/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/algorithms.py` & `sympy-1.9rc1/sympy/codegen/algorithms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/approximations.py` & `sympy-1.9rc1/sympy/codegen/approximations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/array_utils.py` & `sympy-1.9rc1/sympy/codegen/array_utils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/ast.py` & `sympy-1.9rc1/sympy/codegen/ast.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/cfunctions.py` & `sympy-1.9rc1/sympy/codegen/cfunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/cnodes.py` & `sympy-1.9rc1/sympy/codegen/cnodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/fnodes.py` & `sympy-1.9rc1/sympy/codegen/fnodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/futils.py` & `sympy-1.9rc1/sympy/codegen/futils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/matrix_nodes.py` & `sympy-1.9rc1/sympy/codegen/matrix_nodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/numpy_nodes.py` & `sympy-1.9rc1/sympy/codegen/numpy_nodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/pyutils.py` & `sympy-1.9rc1/sympy/codegen/pyutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/rewriting.py` & `sympy-1.9rc1/sympy/codegen/rewriting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/scipy_nodes.py` & `sympy-1.9rc1/sympy/codegen/scipy_nodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_algorithms.py` & `sympy-1.9rc1/sympy/codegen/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_applications.py` & `sympy-1.9rc1/sympy/codegen/tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_approximations.py` & `sympy-1.9rc1/sympy/codegen/tests/test_approximations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_ast.py` & `sympy-1.9rc1/sympy/codegen/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_cfunctions.py` & `sympy-1.9rc1/sympy/codegen/tests/test_cfunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_cnodes.py` & `sympy-1.9rc1/sympy/codegen/tests/test_cnodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_fnodes.py` & `sympy-1.9rc1/sympy/codegen/tests/test_fnodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_numpy_nodes.py` & `sympy-1.9rc1/sympy/codegen/tests/test_numpy_nodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_rewriting.py` & `sympy-1.9rc1/sympy/codegen/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/codegen/tests/test_scipy_nodes.py` & `sympy-1.9rc1/sympy/codegen/tests/test_scipy_nodes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/__init__.py` & `sympy-1.9rc1/sympy/combinatorics/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/coset_table.py` & `sympy-1.9rc1/sympy/combinatorics/coset_table.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/fp_groups.py` & `sympy-1.9rc1/sympy/combinatorics/fp_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/free_groups.py` & `sympy-1.9rc1/sympy/combinatorics/free_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/generators.py` & `sympy-1.9rc1/sympy/combinatorics/generators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/graycode.py` & `sympy-1.9rc1/sympy/combinatorics/graycode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/group_constructs.py` & `sympy-1.9rc1/sympy/combinatorics/group_constructs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/homomorphisms.py` & `sympy-1.9rc1/sympy/combinatorics/homomorphisms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/named_groups.py` & `sympy-1.9rc1/sympy/combinatorics/named_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/partitions.py` & `sympy-1.9rc1/sympy/combinatorics/partitions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/pc_groups.py` & `sympy-1.9rc1/sympy/combinatorics/pc_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/perm_groups.py` & `sympy-1.9rc1/sympy/combinatorics/perm_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/permutations.py` & `sympy-1.9rc1/sympy/combinatorics/permutations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/polyhedron.py` & `sympy-1.9rc1/sympy/combinatorics/polyhedron.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/prufer.py` & `sympy-1.9rc1/sympy/combinatorics/prufer.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/rewritingsystem.py` & `sympy-1.9rc1/sympy/combinatorics/rewritingsystem.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/rewritingsystem_fsm.py` & `sympy-1.9rc1/sympy/combinatorics/rewritingsystem_fsm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/schur_number.py` & `sympy-1.9rc1/sympy/combinatorics/schur_number.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/subsets.py` & `sympy-1.9rc1/sympy/combinatorics/subsets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tensor_can.py` & `sympy-1.9rc1/sympy/combinatorics/tensor_can.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_coset_table.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_coset_table.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_fp_groups.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_fp_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_free_groups.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_free_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_generators.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_graycode.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_graycode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_homomorphisms.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_homomorphisms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_named_groups.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_named_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_partitions.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_partitions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_pc_groups.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_pc_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_perm_groups.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_perm_groups.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_permutations.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_permutations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_polyhedron.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_polyhedron.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_prufer.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_prufer.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_rewriting.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_schur_number.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_schur_number.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_subsets.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_tensor_can.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_tensor_can.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_testutil.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_testutil.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/tests/test_util.py` & `sympy-1.9rc1/sympy/combinatorics/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/testutil.py` & `sympy-1.9rc1/sympy/combinatorics/testutil.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/combinatorics/util.py` & `sympy-1.9rc1/sympy/combinatorics/util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/delta.py` & `sympy-1.9rc1/sympy/concrete/delta.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/expr_with_intlimits.py` & `sympy-1.9rc1/sympy/concrete/expr_with_intlimits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/expr_with_limits.py` & `sympy-1.9rc1/sympy/concrete/expr_with_limits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/gosper.py` & `sympy-1.9rc1/sympy/concrete/gosper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/guess.py` & `sympy-1.9rc1/sympy/concrete/guess.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/products.py` & `sympy-1.9rc1/sympy/concrete/products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/summations.py` & `sympy-1.9rc1/sympy/concrete/summations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/tests/test_delta.py` & `sympy-1.9rc1/sympy/concrete/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/tests/test_gosper.py` & `sympy-1.9rc1/sympy/concrete/tests/test_gosper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/tests/test_guess.py` & `sympy-1.9rc1/sympy/concrete/tests/test_guess.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/tests/test_products.py` & `sympy-1.9rc1/sympy/concrete/tests/test_products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/concrete/tests/test_sums_products.py` & `sympy-1.9rc1/sympy/concrete/tests/test_sums_products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/conftest.py` & `sympy-1.9rc1/sympy/conftest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/__init__.py` & `sympy-1.9rc1/sympy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/_print_helpers.py` & `sympy-1.9rc1/sympy/core/_print_helpers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/add.py` & `sympy-1.9rc1/sympy/core/add.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/assumptions.py` & `sympy-1.9rc1/sympy/core/assumptions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/backend.py` & `sympy-1.9rc1/sympy/core/backend.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/basic.py` & `sympy-1.9rc1/sympy/core/basic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/benchmarks/bench_numbers.py` & `sympy-1.9rc1/sympy/core/benchmarks/bench_numbers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/cache.py` & `sympy-1.9rc1/sympy/core/cache.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/compatibility.py` & `sympy-1.9rc1/sympy/core/compatibility.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/containers.py` & `sympy-1.9rc1/sympy/core/containers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/core.py` & `sympy-1.9rc1/sympy/core/core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/decorators.py` & `sympy-1.9rc1/sympy/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/evalf.py` & `sympy-1.9rc1/sympy/core/evalf.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/expr.py` & `sympy-1.9rc1/sympy/core/expr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/exprtools.py` & `sympy-1.9rc1/sympy/core/exprtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/facts.py` & `sympy-1.9rc1/sympy/core/facts.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/function.py` & `sympy-1.9rc1/sympy/core/function.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/kind.py` & `sympy-1.9rc1/sympy/core/kind.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/logic.py` & `sympy-1.9rc1/sympy/core/logic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/mod.py` & `sympy-1.9rc1/sympy/core/mod.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/mul.py` & `sympy-1.9rc1/sympy/core/mul.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/multidimensional.py` & `sympy-1.9rc1/sympy/core/multidimensional.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/numbers.py` & `sympy-1.9rc1/sympy/core/numbers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/operations.py` & `sympy-1.9rc1/sympy/core/operations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/parameters.py` & `sympy-1.9rc1/sympy/core/parameters.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/power.py` & `sympy-1.9rc1/sympy/core/power.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/relational.py` & `sympy-1.9rc1/sympy/core/relational.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/rules.py` & `sympy-1.9rc1/sympy/core/rules.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/singleton.py` & `sympy-1.9rc1/sympy/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/symbol.py` & `sympy-1.9rc1/sympy/core/symbol.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/sympify.py` & `sympy-1.9rc1/sympy/core/sympify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_args.py` & `sympy-1.9rc1/sympy/core/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_arit.py` & `sympy-1.9rc1/sympy/core/tests/test_arit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_assumptions.py` & `sympy-1.9rc1/sympy/core/tests/test_assumptions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_basic.py` & `sympy-1.9rc1/sympy/core/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_cache.py` & `sympy-1.9rc1/sympy/core/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_compatibility.py` & `sympy-1.9rc1/sympy/core/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_complex.py` & `sympy-1.9rc1/sympy/core/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_constructor_postprocessor.py` & `sympy-1.9rc1/sympy/core/tests/test_constructor_postprocessor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_containers.py` & `sympy-1.9rc1/sympy/core/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_count_ops.py` & `sympy-1.9rc1/sympy/core/tests/test_count_ops.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_diff.py` & `sympy-1.9rc1/sympy/core/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_equal.py` & `sympy-1.9rc1/sympy/core/tests/test_equal.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_eval.py` & `sympy-1.9rc1/sympy/core/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_evalf.py` & `sympy-1.9rc1/sympy/core/tests/test_evalf.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_expand.py` & `sympy-1.9rc1/sympy/core/tests/test_expand.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_expr.py` & `sympy-1.9rc1/sympy/core/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_exprtools.py` & `sympy-1.9rc1/sympy/core/tests/test_exprtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_facts.py` & `sympy-1.9rc1/sympy/core/tests/test_facts.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_function.py` & `sympy-1.9rc1/sympy/core/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_kind.py` & `sympy-1.9rc1/sympy/core/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_logic.py` & `sympy-1.9rc1/sympy/core/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_match.py` & `sympy-1.9rc1/sympy/core/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_multidimensional.py` & `sympy-1.9rc1/sympy/core/tests/test_multidimensional.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_noncommutative.py` & `sympy-1.9rc1/sympy/core/tests/test_noncommutative.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_numbers.py` & `sympy-1.9rc1/sympy/core/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_operations.py` & `sympy-1.9rc1/sympy/core/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_parameters.py` & `sympy-1.9rc1/sympy/core/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_power.py` & `sympy-1.9rc1/sympy/core/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_priority.py` & `sympy-1.9rc1/sympy/core/tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_relational.py` & `sympy-1.9rc1/sympy/core/tests/test_relational.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_singleton.py` & `sympy-1.9rc1/sympy/core/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_subs.py` & `sympy-1.9rc1/sympy/core/tests/test_subs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_symbol.py` & `sympy-1.9rc1/sympy/core/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_sympify.py` & `sympy-1.9rc1/sympy/core/tests/test_sympify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_trace.py` & `sympy-1.9rc1/sympy/core/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_truediv.py` & `sympy-1.9rc1/sympy/core/tests/test_truediv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/tests/test_var.py` & `sympy-1.9rc1/sympy/core/tests/test_var.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/core/trace.py` & `sympy-1.9rc1/sympy/core/trace.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/crypto/__init__.py` & `sympy-1.9rc1/sympy/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/crypto/crypto.py` & `sympy-1.9rc1/sympy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/crypto/tests/test_crypto.py` & `sympy-1.9rc1/sympy/crypto/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/__init__.py` & `sympy-1.9rc1/sympy/diffgeom/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/diffgeom.py` & `sympy-1.9rc1/sympy/diffgeom/diffgeom.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/rn.py` & `sympy-1.9rc1/sympy/diffgeom/rn.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/tests/test_class_structure.py` & `sympy-1.9rc1/sympy/diffgeom/tests/test_class_structure.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/tests/test_diffgeom.py` & `sympy-1.9rc1/sympy/diffgeom/tests/test_diffgeom.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/tests/test_function_diffgeom_book.py` & `sympy-1.9rc1/sympy/diffgeom/tests/test_function_diffgeom_book.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/diffgeom/tests/test_hyperbolic_space.py` & `sympy-1.9rc1/sympy/diffgeom/tests/test_hyperbolic_space.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/__init__.py` & `sympy-1.9rc1/sympy/discrete/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/convolutions.py` & `sympy-1.9rc1/sympy/discrete/convolutions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/recurrences.py` & `sympy-1.9rc1/sympy/discrete/recurrences.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/tests/test_convolutions.py` & `sympy-1.9rc1/sympy/discrete/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/tests/test_recurrences.py` & `sympy-1.9rc1/sympy/discrete/tests/test_recurrences.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/tests/test_transforms.py` & `sympy-1.9rc1/sympy/discrete/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/discrete/transforms.py` & `sympy-1.9rc1/sympy/discrete/transforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/__init__.py` & `sympy-1.9rc1/sympy/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/gmpy.py` & `sympy-1.9rc1/sympy/external/gmpy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/importtools.py` & `sympy-1.9rc1/sympy/external/importtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/pythonmpq.py` & `sympy-1.9rc1/sympy/external/pythonmpq.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/tests/test_autowrap.py` & `sympy-1.9rc1/sympy/external/tests/test_autowrap.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/tests/test_codegen.py` & `sympy-1.9rc1/sympy/external/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/tests/test_importtools.py` & `sympy-1.9rc1/sympy/external/tests/test_importtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/tests/test_numpy.py` & `sympy-1.9rc1/sympy/external/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/tests/test_pythonmpq.py` & `sympy-1.9rc1/sympy/external/tests/test_pythonmpq.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/external/tests/test_scipy.py` & `sympy-1.9rc1/sympy/external/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/__init__.py` & `sympy-1.9rc1/sympy/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/combinatorial/factorials.py` & `sympy-1.9rc1/sympy/functions/combinatorial/factorials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/combinatorial/numbers.py` & `sympy-1.9rc1/sympy/functions/combinatorial/numbers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/combinatorial/tests/test_comb_factorials.py` & `sympy-1.9rc1/sympy/functions/combinatorial/tests/test_comb_factorials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/combinatorial/tests/test_comb_numbers.py` & `sympy-1.9rc1/sympy/functions/combinatorial/tests/test_comb_numbers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/complexes.py` & `sympy-1.9rc1/sympy/functions/elementary/complexes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/exponential.py` & `sympy-1.9rc1/sympy/functions/elementary/exponential.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/hyperbolic.py` & `sympy-1.9rc1/sympy/functions/elementary/hyperbolic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/integers.py` & `sympy-1.9rc1/sympy/functions/elementary/integers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/miscellaneous.py` & `sympy-1.9rc1/sympy/functions/elementary/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/piecewise.py` & `sympy-1.9rc1/sympy/functions/elementary/piecewise.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_complexes.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_complexes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_exponential.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_hyperbolic.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_hyperbolic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_integers.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_integers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_interface.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_miscellaneous.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_piecewise.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/tests/test_trigonometric.py` & `sympy-1.9rc1/sympy/functions/elementary/tests/test_trigonometric.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/elementary/trigonometric.py` & `sympy-1.9rc1/sympy/functions/elementary/trigonometric.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/bessel.py` & `sympy-1.9rc1/sympy/functions/special/bessel.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/beta_functions.py` & `sympy-1.9rc1/sympy/functions/special/beta_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/bsplines.py` & `sympy-1.9rc1/sympy/functions/special/bsplines.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/delta_functions.py` & `sympy-1.9rc1/sympy/functions/special/delta_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/elliptic_integrals.py` & `sympy-1.9rc1/sympy/functions/special/elliptic_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/error_functions.py` & `sympy-1.9rc1/sympy/functions/special/error_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/gamma_functions.py` & `sympy-1.9rc1/sympy/functions/special/gamma_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/hyper.py` & `sympy-1.9rc1/sympy/functions/special/hyper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/mathieu_functions.py` & `sympy-1.9rc1/sympy/functions/special/mathieu_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/polynomials.py` & `sympy-1.9rc1/sympy/functions/special/polynomials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/singularity_functions.py` & `sympy-1.9rc1/sympy/functions/special/singularity_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/spherical_harmonics.py` & `sympy-1.9rc1/sympy/functions/special/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tensor_functions.py` & `sympy-1.9rc1/sympy/functions/special/tensor_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_bessel.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_bessel.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_beta_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_beta_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_bsplines.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_bsplines.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_delta_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_delta_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_elliptic_integrals.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_elliptic_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_error_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_error_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_gamma_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_gamma_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_hyper.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_hyper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_mathieu.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_mathieu.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_singularity_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_singularity_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_spec_polynomials.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_spec_polynomials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_spherical_harmonics.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_tensor_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_tensor_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/tests/test_zeta_functions.py` & `sympy-1.9rc1/sympy/functions/special/tests/test_zeta_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/functions/special/zeta_functions.py` & `sympy-1.9rc1/sympy/functions/special/zeta_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/__init__.py` & `sympy-1.9rc1/sympy/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/curve.py` & `sympy-1.9rc1/sympy/geometry/curve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/ellipse.py` & `sympy-1.9rc1/sympy/geometry/ellipse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/entity.py` & `sympy-1.9rc1/sympy/geometry/entity.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/line.py` & `sympy-1.9rc1/sympy/geometry/line.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/parabola.py` & `sympy-1.9rc1/sympy/geometry/parabola.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/plane.py` & `sympy-1.9rc1/sympy/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/point.py` & `sympy-1.9rc1/sympy/geometry/point.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/polygon.py` & `sympy-1.9rc1/sympy/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_curve.py` & `sympy-1.9rc1/sympy/geometry/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_ellipse.py` & `sympy-1.9rc1/sympy/geometry/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_entity.py` & `sympy-1.9rc1/sympy/geometry/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_geometrysets.py` & `sympy-1.9rc1/sympy/geometry/tests/test_geometrysets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_line.py` & `sympy-1.9rc1/sympy/geometry/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_parabola.py` & `sympy-1.9rc1/sympy/geometry/tests/test_parabola.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_plane.py` & `sympy-1.9rc1/sympy/geometry/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_point.py` & `sympy-1.9rc1/sympy/geometry/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_polygon.py` & `sympy-1.9rc1/sympy/geometry/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/tests/test_util.py` & `sympy-1.9rc1/sympy/geometry/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/geometry/util.py` & `sympy-1.9rc1/sympy/geometry/util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/__init__.py` & `sympy-1.9rc1/sympy/holonomic/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/holonomic.py` & `sympy-1.9rc1/sympy/holonomic/holonomic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/holonomicerrors.py` & `sympy-1.9rc1/sympy/holonomic/holonomicerrors.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/numerical.py` & `sympy-1.9rc1/sympy/holonomic/numerical.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/recurrence.py` & `sympy-1.9rc1/sympy/holonomic/recurrence.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/tests/test_holonomic.py` & `sympy-1.9rc1/sympy/holonomic/tests/test_holonomic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/holonomic/tests/test_recurrence.py` & `sympy-1.9rc1/sympy/holonomic/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/__init__.py` & `sympy-1.9rc1/sympy/integrals/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/deltafunctions.py` & `sympy-1.9rc1/sympy/integrals/deltafunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/heurisch.py` & `sympy-1.9rc1/sympy/integrals/heurisch.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/integrals.py` & `sympy-1.9rc1/sympy/integrals/integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/intpoly.py` & `sympy-1.9rc1/sympy/integrals/intpoly.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/manualintegrate.py` & `sympy-1.9rc1/sympy/integrals/manualintegrate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/meijerint.py` & `sympy-1.9rc1/sympy/integrals/meijerint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/meijerint_doc.py` & `sympy-1.9rc1/sympy/integrals/meijerint_doc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/prde.py` & `sympy-1.9rc1/sympy/integrals/prde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/quadrature.py` & `sympy-1.9rc1/sympy/integrals/quadrature.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rationaltools.py` & `sympy-1.9rc1/sympy/integrals/rationaltools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rde.py` & `sympy-1.9rc1/sympy/integrals/rde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/risch.py` & `sympy-1.9rc1/sympy/integrals/risch.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/__init__.py` & `sympy-1.9rc1/sympy/integrals/rubi/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/constraints.py` & `sympy-1.9rc1/sympy/integrals/rubi/constraints.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/parsetools/generate_rules.py` & `sympy-1.9rc1/sympy/integrals/rubi/parsetools/generate_rules.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/parsetools/generate_tests.py` & `sympy-1.9rc1/sympy/integrals/rubi/parsetools/generate_tests.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/parsetools/header.py.txt` & `sympy-1.9rc1/sympy/integrals/rubi/parsetools/header.py.txt`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/parsetools/parse.py` & `sympy-1.9rc1/sympy/integrals/rubi/parsetools/parse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/parsetools/tests/test_parse.py` & `sympy-1.9rc1/sympy/integrals/rubi/parsetools/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_1_2.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_1_2.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_1_3.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_1_3.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_1_4.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_1_4.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_exponential.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_hyperbolic_sine.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_hyperbolic_sine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_inverse_hyperbolic_sine.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_inverse_hyperbolic_sine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_inverse_sine.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_inverse_sine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_logarithms.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_logarithms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_miscellaneous_algebra.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_miscellaneous_algebra.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_secant.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_secant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_sine.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_sine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_special_functions.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_special_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_tangent.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_tangent.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubi_tests/tests/test_trinomials.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubi_tests/tests/test_trinomials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rubimain.py` & `sympy-1.9rc1/sympy/integrals/rubi/rubimain.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/binomial_products.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/binomial_products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/exponential.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/exponential.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/hyperbolic.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/hyperbolic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/integrand_simplification.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/integrand_simplification.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/inverse_hyperbolic.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/inverse_hyperbolic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/inverse_trig.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/inverse_trig.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/linear_products.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/linear_products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/logarithms.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/logarithms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/miscellaneous_algebraic.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/miscellaneous_algebraic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/miscellaneous_integration.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/miscellaneous_integration.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/miscellaneous_trig.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/miscellaneous_trig.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/piecewise_linear.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/quadratic_products.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/quadratic_products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/secant.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/secant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/sine.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/sine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/special_functions.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/special_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/tangent.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/tangent.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/rules/trinomial_products.py` & `sympy-1.9rc1/sympy/integrals/rubi/rules/trinomial_products.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/symbol.py` & `sympy-1.9rc1/sympy/integrals/rubi/symbol.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/tests/test_rubi_integrate.py` & `sympy-1.9rc1/sympy/integrals/rubi/tests/test_rubi_integrate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/tests/test_utility_function.py` & `sympy-1.9rc1/sympy/integrals/rubi/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/rubi/utility_function.py` & `sympy-1.9rc1/sympy/integrals/rubi/utility_function.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/singularityfunctions.py` & `sympy-1.9rc1/sympy/integrals/singularityfunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_deltafunctions.py` & `sympy-1.9rc1/sympy/integrals/tests/test_deltafunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_failing_integrals.py` & `sympy-1.9rc1/sympy/integrals/tests/test_failing_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_heurisch.py` & `sympy-1.9rc1/sympy/integrals/tests/test_heurisch.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_integrals.py` & `sympy-1.9rc1/sympy/integrals/tests/test_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_intpoly.py` & `sympy-1.9rc1/sympy/integrals/tests/test_intpoly.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_manual.py` & `sympy-1.9rc1/sympy/integrals/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_meijerint.py` & `sympy-1.9rc1/sympy/integrals/tests/test_meijerint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_prde.py` & `sympy-1.9rc1/sympy/integrals/tests/test_prde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_quadrature.py` & `sympy-1.9rc1/sympy/integrals/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_rationaltools.py` & `sympy-1.9rc1/sympy/integrals/tests/test_rationaltools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_rde.py` & `sympy-1.9rc1/sympy/integrals/tests/test_rde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_risch.py` & `sympy-1.9rc1/sympy/integrals/tests/test_risch.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_singularityfunctions.py` & `sympy-1.9rc1/sympy/integrals/tests/test_singularityfunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_transforms.py` & `sympy-1.9rc1/sympy/integrals/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/tests/test_trigonometry.py` & `sympy-1.9rc1/sympy/integrals/tests/test_trigonometry.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/transforms.py` & `sympy-1.9rc1/sympy/integrals/transforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/integrals/trigonometry.py` & `sympy-1.9rc1/sympy/integrals/trigonometry.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/interactive/ipythonprinting.py` & `sympy-1.9rc1/sympy/interactive/ipythonprinting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/interactive/printing.py` & `sympy-1.9rc1/sympy/interactive/printing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/interactive/session.py` & `sympy-1.9rc1/sympy/interactive/session.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/interactive/tests/test_ipython.py` & `sympy-1.9rc1/sympy/interactive/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/interactive/tests/test_ipythonprinting.py` & `sympy-1.9rc1/sympy/interactive/tests/test_ipythonprinting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/cartan_matrix.py` & `sympy-1.9rc1/sympy/liealgebras/cartan_matrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/cartan_type.py` & `sympy-1.9rc1/sympy/liealgebras/cartan_type.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/dynkin_diagram.py` & `sympy-1.9rc1/sympy/liealgebras/dynkin_diagram.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/root_system.py` & `sympy-1.9rc1/sympy/liealgebras/root_system.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_root_system.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_root_system.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_A.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_A.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_B.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_B.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_C.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_C.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_D.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_D.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_E.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_E.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_F.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_F.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_type_G.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_type_G.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/tests/test_weyl_group.py` & `sympy-1.9rc1/sympy/liealgebras/tests/test_weyl_group.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_a.py` & `sympy-1.9rc1/sympy/liealgebras/type_a.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_b.py` & `sympy-1.9rc1/sympy/liealgebras/type_b.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_c.py` & `sympy-1.9rc1/sympy/liealgebras/type_c.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_d.py` & `sympy-1.9rc1/sympy/liealgebras/type_d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_e.py` & `sympy-1.9rc1/sympy/liealgebras/type_e.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_f.py` & `sympy-1.9rc1/sympy/liealgebras/type_f.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/type_g.py` & `sympy-1.9rc1/sympy/liealgebras/type_g.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/liealgebras/weyl_group.py` & `sympy-1.9rc1/sympy/liealgebras/weyl_group.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/algorithms/dpll.py` & `sympy-1.9rc1/sympy/logic/algorithms/dpll.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/algorithms/dpll2.py` & `sympy-1.9rc1/sympy/logic/algorithms/dpll2.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/algorithms/minisat22_wrapper.py` & `sympy-1.9rc1/sympy/logic/algorithms/minisat22_wrapper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/algorithms/pycosat_wrapper.py` & `sympy-1.9rc1/sympy/logic/algorithms/pycosat_wrapper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/boolalg.py` & `sympy-1.9rc1/sympy/logic/boolalg.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/inference.py` & `sympy-1.9rc1/sympy/logic/inference.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/tests/test_boolalg.py` & `sympy-1.9rc1/sympy/logic/tests/test_boolalg.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/tests/test_dimacs.py` & `sympy-1.9rc1/sympy/logic/tests/test_dimacs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/tests/test_inference.py` & `sympy-1.9rc1/sympy/logic/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/logic/utilities/dimacs.py` & `sympy-1.9rc1/sympy/logic/utilities/dimacs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/__init__.py` & `sympy-1.9rc1/sympy/matrices/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/common.py` & `sympy-1.9rc1/sympy/matrices/common.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/decompositions.py` & `sympy-1.9rc1/sympy/matrices/decompositions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/dense.py` & `sympy-1.9rc1/sympy/matrices/dense.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/densearith.py` & `sympy-1.9rc1/sympy/matrices/densearith.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/densesolve.py` & `sympy-1.9rc1/sympy/matrices/densesolve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/densetools.py` & `sympy-1.9rc1/sympy/matrices/densetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/determinant.py` & `sympy-1.9rc1/sympy/matrices/determinant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/eigen.py` & `sympy-1.9rc1/sympy/matrices/eigen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/__init__.py` & `sympy-1.9rc1/sympy/matrices/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/adjoint.py` & `sympy-1.9rc1/sympy/matrices/expressions/adjoint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/applyfunc.py` & `sympy-1.9rc1/sympy/matrices/expressions/applyfunc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/blockmatrix.py` & `sympy-1.9rc1/sympy/matrices/expressions/blockmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/companion.py` & `sympy-1.9rc1/sympy/matrices/expressions/companion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/determinant.py` & `sympy-1.9rc1/sympy/matrices/expressions/determinant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/diagonal.py` & `sympy-1.9rc1/sympy/matrices/expressions/diagonal.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/dotproduct.py` & `sympy-1.9rc1/sympy/matrices/expressions/dotproduct.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/factorizations.py` & `sympy-1.9rc1/sympy/matrices/expressions/factorizations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/fourier.py` & `sympy-1.9rc1/sympy/matrices/expressions/fourier.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/funcmatrix.py` & `sympy-1.9rc1/sympy/matrices/expressions/funcmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/hadamard.py` & `sympy-1.9rc1/sympy/matrices/expressions/hadamard.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/inverse.py` & `sympy-1.9rc1/sympy/matrices/expressions/inverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/kronecker.py` & `sympy-1.9rc1/sympy/matrices/expressions/kronecker.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/matadd.py` & `sympy-1.9rc1/sympy/matrices/expressions/matadd.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/matexpr.py` & `sympy-1.9rc1/sympy/matrices/expressions/matexpr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/matmul.py` & `sympy-1.9rc1/sympy/matrices/expressions/matmul.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/matpow.py` & `sympy-1.9rc1/sympy/matrices/expressions/matpow.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/permutation.py` & `sympy-1.9rc1/sympy/matrices/expressions/permutation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/sets.py` & `sympy-1.9rc1/sympy/matrices/expressions/sets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/slice.py` & `sympy-1.9rc1/sympy/matrices/expressions/slice.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/special.py` & `sympy-1.9rc1/sympy/matrices/expressions/special.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_adjoint.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_applyfunc.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_applyfunc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_blockmatrix.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_blockmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_companion.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_companion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_derivatives.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_determinant.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_determinant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_diagonal.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_diagonal.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_dotproduct.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_dotproduct.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_factorizations.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_factorizations.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_fourier.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_funcmatrix.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_funcmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_hadamard.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_indexing.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_inverse.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_kronecker.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_kronecker.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_matadd.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_matadd.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_matexpr.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_matexpr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_matmul.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_matmul.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_matpow.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_matpow.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_permutation.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_permutation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_sets.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_sets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_slice.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_special.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_special.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_trace.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/tests/test_transpose.py` & `sympy-1.9rc1/sympy/matrices/expressions/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/trace.py` & `sympy-1.9rc1/sympy/matrices/expressions/trace.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/expressions/transpose.py` & `sympy-1.9rc1/sympy/matrices/expressions/transpose.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/graph.py` & `sympy-1.9rc1/sympy/matrices/graph.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/immutable.py` & `sympy-1.9rc1/sympy/matrices/immutable.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/inverse.py` & `sympy-1.9rc1/sympy/matrices/inverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/matrices.py` & `sympy-1.9rc1/sympy/matrices/matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/normalforms.py` & `sympy-1.9rc1/sympy/matrices/normalforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/reductions.py` & `sympy-1.9rc1/sympy/matrices/reductions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/repmatrix.py` & `sympy-1.9rc1/sympy/matrices/repmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/solvers.py` & `sympy-1.9rc1/sympy/matrices/solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/sparse.py` & `sympy-1.9rc1/sympy/matrices/sparse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/sparsetools.py` & `sympy-1.9rc1/sympy/matrices/sparsetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/subspaces.py` & `sympy-1.9rc1/sympy/matrices/subspaces.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_commonmatrix.py` & `sympy-1.9rc1/sympy/matrices/tests/test_commonmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_decompositions.py` & `sympy-1.9rc1/sympy/matrices/tests/test_decompositions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_densearith.py` & `sympy-1.9rc1/sympy/matrices/tests/test_densearith.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_densesolve.py` & `sympy-1.9rc1/sympy/matrices/tests/test_densesolve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_densetools.py` & `sympy-1.9rc1/sympy/matrices/tests/test_densetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_determinant.py` & `sympy-1.9rc1/sympy/matrices/tests/test_determinant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_eigen.py` & `sympy-1.9rc1/sympy/matrices/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_graph.py` & `sympy-1.9rc1/sympy/matrices/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_immutable.py` & `sympy-1.9rc1/sympy/matrices/tests/test_immutable.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_interactions.py` & `sympy-1.9rc1/sympy/matrices/tests/test_interactions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_matrices.py` & `sympy-1.9rc1/sympy/matrices/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_normalforms.py` & `sympy-1.9rc1/sympy/matrices/tests/test_normalforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_reductions.py` & `sympy-1.9rc1/sympy/matrices/tests/test_reductions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_solvers.py` & `sympy-1.9rc1/sympy/matrices/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_sparse.py` & `sympy-1.9rc1/sympy/matrices/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_sparsetools.py` & `sympy-1.9rc1/sympy/matrices/tests/test_sparsetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/tests/test_subspaces.py` & `sympy-1.9rc1/sympy/matrices/tests/test_subspaces.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/matrices/utilities.py` & `sympy-1.9rc1/sympy/matrices/utilities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/conflict.py` & `sympy-1.9rc1/sympy/multipledispatch/conflict.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/core.py` & `sympy-1.9rc1/sympy/multipledispatch/core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/dispatcher.py` & `sympy-1.9rc1/sympy/multipledispatch/dispatcher.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/tests/test_conflict.py` & `sympy-1.9rc1/sympy/multipledispatch/tests/test_conflict.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/tests/test_core.py` & `sympy-1.9rc1/sympy/multipledispatch/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/tests/test_dispatcher.py` & `sympy-1.9rc1/sympy/multipledispatch/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/multipledispatch/utils.py` & `sympy-1.9rc1/sympy/multipledispatch/utils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/__init__.py` & `sympy-1.9rc1/sympy/ntheory/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/bbp_pi.py` & `sympy-1.9rc1/sympy/ntheory/bbp_pi.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/continued_fraction.py` & `sympy-1.9rc1/sympy/ntheory/continued_fraction.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/digits.py` & `sympy-1.9rc1/sympy/ntheory/digits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/ecm.py` & `sympy-1.9rc1/sympy/ntheory/ecm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/egyptian_fraction.py` & `sympy-1.9rc1/sympy/ntheory/egyptian_fraction.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/elliptic_curve.py` & `sympy-1.9rc1/sympy/ntheory/elliptic_curve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/factor_.py` & `sympy-1.9rc1/sympy/ntheory/factor_.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/generate.py` & `sympy-1.9rc1/sympy/ntheory/generate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/modular.py` & `sympy-1.9rc1/sympy/ntheory/modular.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/multinomial.py` & `sympy-1.9rc1/sympy/ntheory/multinomial.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/partitions_.py` & `sympy-1.9rc1/sympy/ntheory/partitions_.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/primetest.py` & `sympy-1.9rc1/sympy/ntheory/primetest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/qs.py` & `sympy-1.9rc1/sympy/ntheory/qs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/residue_ntheory.py` & `sympy-1.9rc1/sympy/ntheory/residue_ntheory.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_bbp_pi.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_bbp_pi.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_continued_fraction.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_continued_fraction.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_digits.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_digits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_ecm.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_ecm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_egyptian_fraction.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_egyptian_fraction.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_elliptic_curve.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_elliptic_curve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_factor_.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_factor_.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_generate.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_modular.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_multinomial.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_multinomial.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_primetest.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_primetest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_qs.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_qs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/ntheory/tests/test_residue.py` & `sympy-1.9rc1/sympy/ntheory/tests/test_residue.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/ast_parser.py` & `sympy-1.9rc1/sympy/parsing/ast_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/Autolev.g4` & `sympy-1.9rc1/sympy/parsing/autolev/Autolev.g4`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/__init__.py` & `sympy-1.9rc1/sympy/parsing/autolev/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/_antlr/autolevlexer.py` & `sympy-1.9rc1/sympy/parsing/autolev/_antlr/autolevlexer.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/_antlr/autolevlistener.py` & `sympy-1.9rc1/sympy/parsing/autolev/_antlr/autolevlistener.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/_antlr/autolevparser.py` & `sympy-1.9rc1/sympy/parsing/autolev/_antlr/autolevparser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/_listener_autolev_antlr.py` & `sympy-1.9rc1/sympy/parsing/autolev/_listener_autolev_antlr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/_parse_autolev_antlr.py` & `sympy-1.9rc1/sympy/parsing/autolev/_parse_autolev_antlr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/README.txt` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/README.txt`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/chaos_pendulum.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/double_pendulum.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/double_pendulum.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/mass_spring_damper.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/mass_spring_damper.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/pydy-example-repo/non_min_pendulum.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/pydy-example-repo/non_min_pendulum.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest1.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest1.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest10.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest10.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest10.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest10.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest2.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest2.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest3.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest3.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest4.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest4.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest5.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest5.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest5.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest5.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest6.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest6.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest6.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest6.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest7.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest7.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest7.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest7.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest8.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest8.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest8.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest8.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest9.al` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest9.al`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/autolev/test-examples/ruletest9.py` & `sympy-1.9rc1/sympy/parsing/autolev/test-examples/ruletest9.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/c/c_parser.py` & `sympy-1.9rc1/sympy/parsing/c/c_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/fortran/fortran_parser.py` & `sympy-1.9rc1/sympy/parsing/fortran/fortran_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/LICENSE.txt` & `sympy-1.9rc1/sympy/parsing/latex/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/LaTeX.g4` & `sympy-1.9rc1/sympy/parsing/latex/LaTeX.g4`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/__init__.py` & `sympy-1.9rc1/sympy/parsing/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/_antlr/latexlexer.py` & `sympy-1.9rc1/sympy/parsing/latex/_antlr/latexlexer.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/_antlr/latexparser.py` & `sympy-1.9rc1/sympy/parsing/latex/_antlr/latexparser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/_build_latex_antlr.py` & `sympy-1.9rc1/sympy/parsing/latex/_build_latex_antlr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/latex/_parse_latex_antlr.py` & `sympy-1.9rc1/sympy/parsing/latex/_parse_latex_antlr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/mathematica.py` & `sympy-1.9rc1/sympy/parsing/mathematica.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/maxima.py` & `sympy-1.9rc1/sympy/parsing/maxima.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/sym_expr.py` & `sympy-1.9rc1/sympy/parsing/sym_expr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/sympy_parser.py` & `sympy-1.9rc1/sympy/parsing/sympy_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_ast_parser.py` & `sympy-1.9rc1/sympy/parsing/tests/test_ast_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_autolev.py` & `sympy-1.9rc1/sympy/parsing/tests/test_autolev.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_c_parser.py` & `sympy-1.9rc1/sympy/parsing/tests/test_c_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_fortran_parser.py` & `sympy-1.9rc1/sympy/parsing/tests/test_fortran_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_implicit_multiplication_application.py` & `sympy-1.9rc1/sympy/parsing/tests/test_implicit_multiplication_application.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_latex.py` & `sympy-1.9rc1/sympy/parsing/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_mathematica.py` & `sympy-1.9rc1/sympy/parsing/tests/test_mathematica.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_maxima.py` & `sympy-1.9rc1/sympy/parsing/tests/test_maxima.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_sym_expr.py` & `sympy-1.9rc1/sympy/parsing/tests/test_sym_expr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/parsing/tests/test_sympy_parser.py` & `sympy-1.9rc1/sympy/parsing/tests/test_sympy_parser.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/continuum_mechanics/beam.py` & `sympy-1.9rc1/sympy/physics/continuum_mechanics/beam.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/continuum_mechanics/tests/test_beam.py` & `sympy-1.9rc1/sympy/physics/continuum_mechanics/tests/test_beam.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/control/__init__.py` & `sympy-1.9rc1/sympy/physics/control/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/control/control_plots.py` & `sympy-1.9rc1/sympy/physics/control/control_plots.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/control/lti.py` & `sympy-1.9rc1/sympy/physics/control/lti.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/control/tests/test_control_plots.py` & `sympy-1.9rc1/sympy/physics/control/tests/test_control_plots.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/control/tests/test_lti.py` & `sympy-1.9rc1/sympy/physics/control/tests/test_lti.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/gaussopt.py` & `sympy-1.9rc1/sympy/physics/gaussopt.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/hep/gamma_matrices.py` & `sympy-1.9rc1/sympy/physics/hep/gamma_matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/hep/tests/test_gamma_matrices.py` & `sympy-1.9rc1/sympy/physics/hep/tests/test_gamma_matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/hydrogen.py` & `sympy-1.9rc1/sympy/physics/hydrogen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/matrices.py` & `sympy-1.9rc1/sympy/physics/matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/__init__.py` & `sympy-1.9rc1/sympy/physics/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/body.py` & `sympy-1.9rc1/sympy/physics/mechanics/body.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/functions.py` & `sympy-1.9rc1/sympy/physics/mechanics/functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/joint.py` & `sympy-1.9rc1/sympy/physics/mechanics/joint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/jointsmethod.py` & `sympy-1.9rc1/sympy/physics/mechanics/jointsmethod.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/kane.py` & `sympy-1.9rc1/sympy/physics/mechanics/kane.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/lagrange.py` & `sympy-1.9rc1/sympy/physics/mechanics/lagrange.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/linearize.py` & `sympy-1.9rc1/sympy/physics/mechanics/linearize.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/method.py` & `sympy-1.9rc1/sympy/physics/mechanics/method.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/models.py` & `sympy-1.9rc1/sympy/physics/mechanics/models.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/particle.py` & `sympy-1.9rc1/sympy/physics/mechanics/particle.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/rigidbody.py` & `sympy-1.9rc1/sympy/physics/mechanics/rigidbody.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/system.py` & `sympy-1.9rc1/sympy/physics/mechanics/system.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_body.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_functions.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_joint.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_joint.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_jointsmethod.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_jointsmethod.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_kane.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_kane2.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane2.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_kane3.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane3.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_kane4.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_kane4.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_lagrange.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_lagrange.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_lagrange2.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_lagrange2.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_linearize.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_linearize.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_models.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_particle.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_particle.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_rigidbody.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_rigidbody.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/mechanics/tests/test_system.py` & `sympy-1.9rc1/sympy/physics/mechanics/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/__init__.py` & `sympy-1.9rc1/sympy/physics/optics/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/gaussopt.py` & `sympy-1.9rc1/sympy/physics/optics/gaussopt.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/medium.py` & `sympy-1.9rc1/sympy/physics/optics/medium.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/polarization.py` & `sympy-1.9rc1/sympy/physics/optics/polarization.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/tests/test_gaussopt.py` & `sympy-1.9rc1/sympy/physics/optics/tests/test_gaussopt.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/tests/test_medium.py` & `sympy-1.9rc1/sympy/physics/optics/tests/test_medium.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/tests/test_polarization.py` & `sympy-1.9rc1/sympy/physics/optics/tests/test_polarization.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/tests/test_utils.py` & `sympy-1.9rc1/sympy/physics/optics/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/tests/test_waves.py` & `sympy-1.9rc1/sympy/physics/optics/tests/test_waves.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/utils.py` & `sympy-1.9rc1/sympy/physics/optics/utils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/optics/waves.py` & `sympy-1.9rc1/sympy/physics/optics/waves.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/paulialgebra.py` & `sympy-1.9rc1/sympy/physics/paulialgebra.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/pring.py` & `sympy-1.9rc1/sympy/physics/pring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/qho_1d.py` & `sympy-1.9rc1/sympy/physics/qho_1d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/__init__.py` & `sympy-1.9rc1/sympy/physics/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/anticommutator.py` & `sympy-1.9rc1/sympy/physics/quantum/anticommutator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/boson.py` & `sympy-1.9rc1/sympy/physics/quantum/boson.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/cartesian.py` & `sympy-1.9rc1/sympy/physics/quantum/cartesian.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/cg.py` & `sympy-1.9rc1/sympy/physics/quantum/cg.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/circuitplot.py` & `sympy-1.9rc1/sympy/physics/quantum/circuitplot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/circuitutils.py` & `sympy-1.9rc1/sympy/physics/quantum/circuitutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/commutator.py` & `sympy-1.9rc1/sympy/physics/quantum/commutator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/constants.py` & `sympy-1.9rc1/sympy/physics/quantum/constants.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/dagger.py` & `sympy-1.9rc1/sympy/physics/quantum/dagger.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/density.py` & `sympy-1.9rc1/sympy/physics/quantum/density.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/fermion.py` & `sympy-1.9rc1/sympy/physics/quantum/fermion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/gate.py` & `sympy-1.9rc1/sympy/physics/quantum/gate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/grover.py` & `sympy-1.9rc1/sympy/physics/quantum/grover.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/hilbert.py` & `sympy-1.9rc1/sympy/physics/quantum/hilbert.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/identitysearch.py` & `sympy-1.9rc1/sympy/physics/quantum/identitysearch.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/innerproduct.py` & `sympy-1.9rc1/sympy/physics/quantum/innerproduct.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/matrixcache.py` & `sympy-1.9rc1/sympy/physics/quantum/matrixcache.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/matrixutils.py` & `sympy-1.9rc1/sympy/physics/quantum/matrixutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/operator.py` & `sympy-1.9rc1/sympy/physics/quantum/operator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/operatorordering.py` & `sympy-1.9rc1/sympy/physics/quantum/operatorordering.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/operatorset.py` & `sympy-1.9rc1/sympy/physics/quantum/operatorset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/pauli.py` & `sympy-1.9rc1/sympy/physics/quantum/pauli.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/piab.py` & `sympy-1.9rc1/sympy/physics/quantum/piab.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/qapply.py` & `sympy-1.9rc1/sympy/physics/quantum/qapply.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/qasm.py` & `sympy-1.9rc1/sympy/physics/quantum/qasm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/qexpr.py` & `sympy-1.9rc1/sympy/physics/quantum/qexpr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/qft.py` & `sympy-1.9rc1/sympy/physics/quantum/qft.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/qubit.py` & `sympy-1.9rc1/sympy/physics/quantum/qubit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/represent.py` & `sympy-1.9rc1/sympy/physics/quantum/represent.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/sho1d.py` & `sympy-1.9rc1/sympy/physics/quantum/sho1d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/shor.py` & `sympy-1.9rc1/sympy/physics/quantum/shor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/spin.py` & `sympy-1.9rc1/sympy/physics/quantum/spin.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/state.py` & `sympy-1.9rc1/sympy/physics/quantum/state.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tensorproduct.py` & `sympy-1.9rc1/sympy/physics/quantum/tensorproduct.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_anticommutator.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_anticommutator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_boson.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_boson.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_cartesian.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_cg.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_cg.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_circuitplot.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_circuitplot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_circuitutils.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_circuitutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_commutator.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_commutator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_dagger.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_dagger.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_density.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_fermion.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_fermion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_gate.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_grover.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_grover.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_hilbert.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_hilbert.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_identitysearch.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_identitysearch.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_innerproduct.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_innerproduct.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_matrixutils.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_matrixutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_operator.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_operatorordering.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_operatorordering.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_operatorset.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_operatorset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_pauli.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_pauli.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_piab.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_piab.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_printing.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_qapply.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_qapply.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_qasm.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_qasm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_qexpr.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_qexpr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_qft.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_qft.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_qubit.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_qubit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_represent.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_represent.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_sho1d.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_sho1d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_shor.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_shor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_spin.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_spin.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_state.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/quantum/tests/test_tensorproduct.py` & `sympy-1.9rc1/sympy/physics/quantum/tests/test_tensorproduct.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/secondquant.py` & `sympy-1.9rc1/sympy/physics/secondquant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/sho.py` & `sympy-1.9rc1/sympy/physics/sho.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_clebsch_gordan.py` & `sympy-1.9rc1/sympy/physics/tests/test_clebsch_gordan.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_hydrogen.py` & `sympy-1.9rc1/sympy/physics/tests/test_hydrogen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_paulialgebra.py` & `sympy-1.9rc1/sympy/physics/tests/test_paulialgebra.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_physics_matrices.py` & `sympy-1.9rc1/sympy/physics/tests/test_physics_matrices.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_pring.py` & `sympy-1.9rc1/sympy/physics/tests/test_pring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_qho_1d.py` & `sympy-1.9rc1/sympy/physics/tests/test_qho_1d.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_secondquant.py` & `sympy-1.9rc1/sympy/physics/tests/test_secondquant.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/tests/test_sho.py` & `sympy-1.9rc1/sympy/physics/tests/test_sho.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/__init__.py` & `sympy-1.9rc1/sympy/physics/units/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/definitions/__init__.py` & `sympy-1.9rc1/sympy/physics/units/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/definitions/dimension_definitions.py` & `sympy-1.9rc1/sympy/physics/units/definitions/dimension_definitions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/definitions/unit_definitions.py` & `sympy-1.9rc1/sympy/physics/units/definitions/unit_definitions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/dimensions.py` & `sympy-1.9rc1/sympy/physics/units/dimensions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/prefixes.py` & `sympy-1.9rc1/sympy/physics/units/prefixes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/quantities.py` & `sympy-1.9rc1/sympy/physics/units/quantities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/systems/cgs.py` & `sympy-1.9rc1/sympy/physics/units/systems/cgs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/systems/length_weight_time.py` & `sympy-1.9rc1/sympy/physics/units/systems/length_weight_time.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/systems/mks.py` & `sympy-1.9rc1/sympy/physics/units/systems/mks.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/systems/mksa.py` & `sympy-1.9rc1/sympy/physics/units/systems/mksa.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/systems/natural.py` & `sympy-1.9rc1/sympy/physics/units/systems/natural.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/systems/si.py` & `sympy-1.9rc1/sympy/physics/units/systems/si.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_dimensions.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_dimensionsystem.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_dimensionsystem.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_prefixes.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_prefixes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_quantities.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_unit_system_cgs_gauss.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_unit_system_cgs_gauss.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_unitsystem.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_unitsystem.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/tests/test_util.py` & `sympy-1.9rc1/sympy/physics/units/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/unitsystem.py` & `sympy-1.9rc1/sympy/physics/units/unitsystem.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/units/util.py` & `sympy-1.9rc1/sympy/physics/units/util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/__init__.py` & `sympy-1.9rc1/sympy/physics/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/dyadic.py` & `sympy-1.9rc1/sympy/physics/vector/dyadic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/fieldfunctions.py` & `sympy-1.9rc1/sympy/physics/vector/fieldfunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/frame.py` & `sympy-1.9rc1/sympy/physics/vector/frame.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/functions.py` & `sympy-1.9rc1/sympy/physics/vector/functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/point.py` & `sympy-1.9rc1/sympy/physics/vector/point.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/printing.py` & `sympy-1.9rc1/sympy/physics/vector/printing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_dyadic.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_dyadic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_fieldfunctions.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_fieldfunctions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_frame.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_functions.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_output.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_point.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_printing.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/tests/test_vector.py` & `sympy-1.9rc1/sympy/physics/vector/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/vector/vector.py` & `sympy-1.9rc1/sympy/physics/vector/vector.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/physics/wigner.py` & `sympy-1.9rc1/sympy/physics/wigner.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/experimental_lambdify.py` & `sympy-1.9rc1/sympy/plotting/experimental_lambdify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/intervalmath/interval_arithmetic.py` & `sympy-1.9rc1/sympy/plotting/intervalmath/interval_arithmetic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/intervalmath/interval_membership.py` & `sympy-1.9rc1/sympy/plotting/intervalmath/interval_membership.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/intervalmath/lib_interval.py` & `sympy-1.9rc1/sympy/plotting/intervalmath/lib_interval.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/intervalmath/tests/test_interval_functions.py` & `sympy-1.9rc1/sympy/plotting/intervalmath/tests/test_interval_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/intervalmath/tests/test_interval_membership.py` & `sympy-1.9rc1/sympy/plotting/intervalmath/tests/test_interval_membership.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/intervalmath/tests/test_intervalmath.py` & `sympy-1.9rc1/sympy/plotting/intervalmath/tests/test_intervalmath.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/plot.py` & `sympy-1.9rc1/sympy/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/plot_implicit.py` & `sympy-1.9rc1/sympy/plotting/plot_implicit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/__init__.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/color_scheme.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/color_scheme.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/managed_window.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/managed_window.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_axes.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_axes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_camera.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_camera.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_controller.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_controller.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_curve.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_curve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_interval.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_interval.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_mode.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_mode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_mode_base.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_mode_base.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_modes.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_modes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_rotation.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_rotation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_surface.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_surface.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/plot_window.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/plot_window.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/tests/test_plotting.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/pygletplot/util.py` & `sympy-1.9rc1/sympy/plotting/pygletplot/util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_experimental_lambdify.py` & `sympy-1.9rc1/sympy/plotting/tests/test_experimental_lambdify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_plot.py` & `sympy-1.9rc1/sympy/plotting/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_plot_implicit.py` & `sympy-1.9rc1/sympy/plotting/tests/test_plot_implicit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_region_and.png` & `sympy-1.9rc1/sympy/plotting/tests/test_region_and.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_region_not.png` & `sympy-1.9rc1/sympy/plotting/tests/test_region_not.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_region_or.png` & `sympy-1.9rc1/sympy/plotting/tests/test_region_or.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_region_xor.png` & `sympy-1.9rc1/sympy/plotting/tests/test_region_xor.png`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/tests/test_textplot.py` & `sympy-1.9rc1/sympy/plotting/tests/test_textplot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/plotting/textplot.py` & `sympy-1.9rc1/sympy/plotting/textplot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/__init__.py` & `sympy-1.9rc1/sympy/polys/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/extensions.py` & `sympy-1.9rc1/sympy/polys/agca/extensions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/homomorphisms.py` & `sympy-1.9rc1/sympy/polys/agca/homomorphisms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/ideals.py` & `sympy-1.9rc1/sympy/polys/agca/ideals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/modules.py` & `sympy-1.9rc1/sympy/polys/agca/modules.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/tests/test_extensions.py` & `sympy-1.9rc1/sympy/polys/agca/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/tests/test_homomorphisms.py` & `sympy-1.9rc1/sympy/polys/agca/tests/test_homomorphisms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/tests/test_ideals.py` & `sympy-1.9rc1/sympy/polys/agca/tests/test_ideals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/agca/tests/test_modules.py` & `sympy-1.9rc1/sympy/polys/agca/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/benchmarks/bench_galoispolys.py` & `sympy-1.9rc1/sympy/polys/benchmarks/bench_galoispolys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/benchmarks/bench_groebnertools.py` & `sympy-1.9rc1/sympy/polys/benchmarks/bench_groebnertools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/benchmarks/bench_solvers.py` & `sympy-1.9rc1/sympy/polys/benchmarks/bench_solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/compatibility.py` & `sympy-1.9rc1/sympy/polys/compatibility.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/constructor.py` & `sympy-1.9rc1/sympy/polys/constructor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/densearith.py` & `sympy-1.9rc1/sympy/polys/densearith.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/densebasic.py` & `sympy-1.9rc1/sympy/polys/densebasic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/densetools.py` & `sympy-1.9rc1/sympy/polys/densetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/dispersion.py` & `sympy-1.9rc1/sympy/polys/dispersion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/distributedmodules.py` & `sympy-1.9rc1/sympy/polys/distributedmodules.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/__init__.py` & `sympy-1.9rc1/sympy/polys/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/algebraicfield.py` & `sympy-1.9rc1/sympy/polys/domains/algebraicfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/complexfield.py` & `sympy-1.9rc1/sympy/polys/domains/complexfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/compositedomain.py` & `sympy-1.9rc1/sympy/polys/domains/compositedomain.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/domain.py` & `sympy-1.9rc1/sympy/polys/domains/domain.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/domainelement.py` & `sympy-1.9rc1/sympy/polys/domains/domainelement.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/expressiondomain.py` & `sympy-1.9rc1/sympy/polys/domains/expressiondomain.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/expressionrawdomain.py` & `sympy-1.9rc1/sympy/polys/domains/expressionrawdomain.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/field.py` & `sympy-1.9rc1/sympy/polys/domains/field.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/finitefield.py` & `sympy-1.9rc1/sympy/polys/domains/finitefield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/fractionfield.py` & `sympy-1.9rc1/sympy/polys/domains/fractionfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/gaussiandomains.py` & `sympy-1.9rc1/sympy/polys/domains/gaussiandomains.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/gmpyintegerring.py` & `sympy-1.9rc1/sympy/polys/domains/gmpyintegerring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/gmpyrationalfield.py` & `sympy-1.9rc1/sympy/polys/domains/gmpyrationalfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/groundtypes.py` & `sympy-1.9rc1/sympy/polys/domains/groundtypes.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/integerring.py` & `sympy-1.9rc1/sympy/polys/domains/integerring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/modularinteger.py` & `sympy-1.9rc1/sympy/polys/domains/modularinteger.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/mpelements.py` & `sympy-1.9rc1/sympy/polys/domains/mpelements.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/old_fractionfield.py` & `sympy-1.9rc1/sympy/polys/domains/old_fractionfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/old_polynomialring.py` & `sympy-1.9rc1/sympy/polys/domains/old_polynomialring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/polynomialring.py` & `sympy-1.9rc1/sympy/polys/domains/polynomialring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/pythonintegerring.py` & `sympy-1.9rc1/sympy/polys/domains/pythonintegerring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/pythonrational.py` & `sympy-1.9rc1/sympy/polys/domains/pythonrational.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/pythonrationalfield.py` & `sympy-1.9rc1/sympy/polys/domains/pythonrationalfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/quotientring.py` & `sympy-1.9rc1/sympy/polys/domains/quotientring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/rationalfield.py` & `sympy-1.9rc1/sympy/polys/domains/rationalfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/realfield.py` & `sympy-1.9rc1/sympy/polys/domains/realfield.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/ring.py` & `sympy-1.9rc1/sympy/polys/domains/ring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/tests/test_domains.py` & `sympy-1.9rc1/sympy/polys/domains/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/tests/test_polynomialring.py` & `sympy-1.9rc1/sympy/polys/domains/tests/test_polynomialring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/domains/tests/test_quotientring.py` & `sympy-1.9rc1/sympy/polys/domains/tests/test_quotientring.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/euclidtools.py` & `sympy-1.9rc1/sympy/polys/euclidtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/factortools.py` & `sympy-1.9rc1/sympy/polys/factortools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/fglmtools.py` & `sympy-1.9rc1/sympy/polys/fglmtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/fields.py` & `sympy-1.9rc1/sympy/polys/fields.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/galoistools.py` & `sympy-1.9rc1/sympy/polys/galoistools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/groebnertools.py` & `sympy-1.9rc1/sympy/polys/groebnertools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/heuristicgcd.py` & `sympy-1.9rc1/sympy/polys/heuristicgcd.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/ddm.py` & `sympy-1.9rc1/sympy/polys/matrices/ddm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/dense.py` & `sympy-1.9rc1/sympy/polys/matrices/dense.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/domainmatrix.py` & `sympy-1.9rc1/sympy/polys/matrices/domainmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/domainscalar.py` & `sympy-1.9rc1/sympy/polys/matrices/domainscalar.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/eigen.py` & `sympy-1.9rc1/sympy/polys/matrices/eigen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/exceptions.py` & `sympy-1.9rc1/sympy/polys/matrices/exceptions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/linsolve.py` & `sympy-1.9rc1/sympy/polys/matrices/linsolve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/normalforms.py` & `sympy-1.9rc1/sympy/polys/matrices/normalforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/sdm.py` & `sympy-1.9rc1/sympy/polys/matrices/sdm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_ddm.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_ddm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_dense.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_dense.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_domainmatrix.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_domainmatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_domainscalar.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_domainscalar.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_eigen.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_linsolve.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_linsolve.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_normalforms.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_normalforms.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/matrices/tests/test_sdm.py` & `sympy-1.9rc1/sympy/polys/matrices/tests/test_sdm.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/modulargcd.py` & `sympy-1.9rc1/sympy/polys/modulargcd.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/monomials.py` & `sympy-1.9rc1/sympy/polys/monomials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/multivariate_resultants.py` & `sympy-1.9rc1/sympy/polys/multivariate_resultants.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/numberfields.py` & `sympy-1.9rc1/sympy/polys/numberfields.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/orderings.py` & `sympy-1.9rc1/sympy/polys/orderings.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/orthopolys.py` & `sympy-1.9rc1/sympy/polys/orthopolys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/partfrac.py` & `sympy-1.9rc1/sympy/polys/partfrac.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyclasses.py` & `sympy-1.9rc1/sympy/polys/polyclasses.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyconfig.py` & `sympy-1.9rc1/sympy/polys/polyconfig.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyerrors.py` & `sympy-1.9rc1/sympy/polys/polyerrors.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyfuncs.py` & `sympy-1.9rc1/sympy/polys/polyfuncs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polymatrix.py` & `sympy-1.9rc1/sympy/polys/polymatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyoptions.py` & `sympy-1.9rc1/sympy/polys/polyoptions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyquinticconst.py` & `sympy-1.9rc1/sympy/polys/polyquinticconst.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyroots.py` & `sympy-1.9rc1/sympy/polys/polyroots.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polytools.py` & `sympy-1.9rc1/sympy/polys/polytools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/polyutils.py` & `sympy-1.9rc1/sympy/polys/polyutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/rationaltools.py` & `sympy-1.9rc1/sympy/polys/rationaltools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/ring_series.py` & `sympy-1.9rc1/sympy/polys/ring_series.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/rings.py` & `sympy-1.9rc1/sympy/polys/rings.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/rootisolation.py` & `sympy-1.9rc1/sympy/polys/rootisolation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/rootoftools.py` & `sympy-1.9rc1/sympy/polys/rootoftools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/solvers.py` & `sympy-1.9rc1/sympy/polys/solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/specialpolys.py` & `sympy-1.9rc1/sympy/polys/specialpolys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/sqfreetools.py` & `sympy-1.9rc1/sympy/polys/sqfreetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/subresultants_qq_zz.py` & `sympy-1.9rc1/sympy/polys/subresultants_qq_zz.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_constructor.py` & `sympy-1.9rc1/sympy/polys/tests/test_constructor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_densearith.py` & `sympy-1.9rc1/sympy/polys/tests/test_densearith.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_densebasic.py` & `sympy-1.9rc1/sympy/polys/tests/test_densebasic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_densetools.py` & `sympy-1.9rc1/sympy/polys/tests/test_densetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_dispersion.py` & `sympy-1.9rc1/sympy/polys/tests/test_dispersion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_distributedmodules.py` & `sympy-1.9rc1/sympy/polys/tests/test_distributedmodules.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_euclidtools.py` & `sympy-1.9rc1/sympy/polys/tests/test_euclidtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_factortools.py` & `sympy-1.9rc1/sympy/polys/tests/test_factortools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_fields.py` & `sympy-1.9rc1/sympy/polys/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_galoistools.py` & `sympy-1.9rc1/sympy/polys/tests/test_galoistools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_groebnertools.py` & `sympy-1.9rc1/sympy/polys/tests/test_groebnertools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_heuristicgcd.py` & `sympy-1.9rc1/sympy/polys/tests/test_heuristicgcd.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_injections.py` & `sympy-1.9rc1/sympy/polys/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_modulargcd.py` & `sympy-1.9rc1/sympy/polys/tests/test_modulargcd.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_monomials.py` & `sympy-1.9rc1/sympy/polys/tests/test_monomials.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_multivariate_resultants.py` & `sympy-1.9rc1/sympy/polys/tests/test_multivariate_resultants.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_numberfields.py` & `sympy-1.9rc1/sympy/polys/tests/test_numberfields.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_orderings.py` & `sympy-1.9rc1/sympy/polys/tests/test_orderings.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_orthopolys.py` & `sympy-1.9rc1/sympy/polys/tests/test_orthopolys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_partfrac.py` & `sympy-1.9rc1/sympy/polys/tests/test_partfrac.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polyclasses.py` & `sympy-1.9rc1/sympy/polys/tests/test_polyclasses.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polyfuncs.py` & `sympy-1.9rc1/sympy/polys/tests/test_polyfuncs.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polymatrix.py` & `sympy-1.9rc1/sympy/polys/tests/test_polymatrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polyoptions.py` & `sympy-1.9rc1/sympy/polys/tests/test_polyoptions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polyroots.py` & `sympy-1.9rc1/sympy/polys/tests/test_polyroots.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polytools.py` & `sympy-1.9rc1/sympy/polys/tests/test_polytools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_polyutils.py` & `sympy-1.9rc1/sympy/polys/tests/test_polyutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_pythonrational.py` & `sympy-1.9rc1/sympy/polys/tests/test_pythonrational.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_rationaltools.py` & `sympy-1.9rc1/sympy/polys/tests/test_rationaltools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_ring_series.py` & `sympy-1.9rc1/sympy/polys/tests/test_ring_series.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_rings.py` & `sympy-1.9rc1/sympy/polys/tests/test_rings.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_rootisolation.py` & `sympy-1.9rc1/sympy/polys/tests/test_rootisolation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_rootoftools.py` & `sympy-1.9rc1/sympy/polys/tests/test_rootoftools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_solvers.py` & `sympy-1.9rc1/sympy/polys/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_specialpolys.py` & `sympy-1.9rc1/sympy/polys/tests/test_specialpolys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_sqfreetools.py` & `sympy-1.9rc1/sympy/polys/tests/test_sqfreetools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/polys/tests/test_subresultants_qq_zz.py` & `sympy-1.9rc1/sympy/polys/tests/test_subresultants_qq_zz.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/__init__.py` & `sympy-1.9rc1/sympy/printing/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/aesaracode.py` & `sympy-1.9rc1/sympy/printing/aesaracode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/c.py` & `sympy-1.9rc1/sympy/printing/c.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/ccode.py` & `sympy-1.9rc1/sympy/printing/ccode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/codeprinter.py` & `sympy-1.9rc1/sympy/printing/codeprinter.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/conventions.py` & `sympy-1.9rc1/sympy/printing/conventions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/cxx.py` & `sympy-1.9rc1/sympy/printing/cxx.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/dot.py` & `sympy-1.9rc1/sympy/printing/dot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/fortran.py` & `sympy-1.9rc1/sympy/printing/fortran.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/glsl.py` & `sympy-1.9rc1/sympy/printing/glsl.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/jscode.py` & `sympy-1.9rc1/sympy/printing/jscode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/julia.py` & `sympy-1.9rc1/sympy/printing/julia.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/lambdarepr.py` & `sympy-1.9rc1/sympy/printing/lambdarepr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/latex.py` & `sympy-1.9rc1/sympy/printing/latex.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/llvmjitcode.py` & `sympy-1.9rc1/sympy/printing/llvmjitcode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/maple.py` & `sympy-1.9rc1/sympy/printing/maple.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/mathematica.py` & `sympy-1.9rc1/sympy/printing/mathematica.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/mathml.py` & `sympy-1.9rc1/sympy/printing/mathml.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/numpy.py` & `sympy-1.9rc1/sympy/printing/numpy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/octave.py` & `sympy-1.9rc1/sympy/printing/octave.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/precedence.py` & `sympy-1.9rc1/sympy/printing/precedence.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/pretty/pretty.py` & `sympy-1.9rc1/sympy/printing/pretty/pretty.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/pretty/pretty_symbology.py` & `sympy-1.9rc1/sympy/printing/pretty/pretty_symbology.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/pretty/stringpict.py` & `sympy-1.9rc1/sympy/printing/pretty/stringpict.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/pretty/tests/test_pretty.py` & `sympy-1.9rc1/sympy/printing/pretty/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/preview.py` & `sympy-1.9rc1/sympy/printing/preview.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/printer.py` & `sympy-1.9rc1/sympy/printing/printer.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/pycode.py` & `sympy-1.9rc1/sympy/printing/pycode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/python.py` & `sympy-1.9rc1/sympy/printing/python.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/rcode.py` & `sympy-1.9rc1/sympy/printing/rcode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/repr.py` & `sympy-1.9rc1/sympy/printing/repr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/rust.py` & `sympy-1.9rc1/sympy/printing/rust.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/str.py` & `sympy-1.9rc1/sympy/printing/str.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tableform.py` & `sympy-1.9rc1/sympy/printing/tableform.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tensorflow.py` & `sympy-1.9rc1/sympy/printing/tensorflow.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_aesaracode.py` & `sympy-1.9rc1/sympy/printing/tests/test_aesaracode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_c.py` & `sympy-1.9rc1/sympy/printing/tests/test_c.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_codeprinter.py` & `sympy-1.9rc1/sympy/printing/tests/test_codeprinter.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_conventions.py` & `sympy-1.9rc1/sympy/printing/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_cupy.py` & `sympy-1.9rc1/sympy/printing/tests/test_cupy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_cxx.py` & `sympy-1.9rc1/sympy/printing/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_dot.py` & `sympy-1.9rc1/sympy/printing/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_fortran.py` & `sympy-1.9rc1/sympy/printing/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_glsl.py` & `sympy-1.9rc1/sympy/printing/tests/test_glsl.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_jscode.py` & `sympy-1.9rc1/sympy/printing/tests/test_jscode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_julia.py` & `sympy-1.9rc1/sympy/printing/tests/test_julia.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_lambdarepr.py` & `sympy-1.9rc1/sympy/printing/tests/test_lambdarepr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_latex.py` & `sympy-1.9rc1/sympy/printing/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_llvmjit.py` & `sympy-1.9rc1/sympy/printing/tests/test_llvmjit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_maple.py` & `sympy-1.9rc1/sympy/printing/tests/test_maple.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_mathematica.py` & `sympy-1.9rc1/sympy/printing/tests/test_mathematica.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_mathml.py` & `sympy-1.9rc1/sympy/printing/tests/test_mathml.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_numpy.py` & `sympy-1.9rc1/sympy/printing/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_octave.py` & `sympy-1.9rc1/sympy/printing/tests/test_octave.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_precedence.py` & `sympy-1.9rc1/sympy/printing/tests/test_precedence.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_preview.py` & `sympy-1.9rc1/sympy/printing/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_pycode.py` & `sympy-1.9rc1/sympy/printing/tests/test_pycode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_python.py` & `sympy-1.9rc1/sympy/printing/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_rcode.py` & `sympy-1.9rc1/sympy/printing/tests/test_rcode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_repr.py` & `sympy-1.9rc1/sympy/printing/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_rust.py` & `sympy-1.9rc1/sympy/printing/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_str.py` & `sympy-1.9rc1/sympy/printing/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_tableform.py` & `sympy-1.9rc1/sympy/printing/tests/test_tableform.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_tensorflow.py` & `sympy-1.9rc1/sympy/printing/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_theanocode.py` & `sympy-1.9rc1/sympy/printing/tests/test_theanocode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tests/test_tree.py` & `sympy-1.9rc1/sympy/printing/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/theanocode.py` & `sympy-1.9rc1/sympy/printing/theanocode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/printing/tree.py` & `sympy-1.9rc1/sympy/printing/tree.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sandbox/indexed_integrals.py` & `sympy-1.9rc1/sympy/sandbox/indexed_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sandbox/tests/test_indexed_integrals.py` & `sympy-1.9rc1/sympy/sandbox/tests/test_indexed_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/__init__.py` & `sympy-1.9rc1/sympy/series/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/acceleration.py` & `sympy-1.9rc1/sympy/series/acceleration.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/approximants.py` & `sympy-1.9rc1/sympy/series/approximants.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/formal.py` & `sympy-1.9rc1/sympy/series/formal.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/fourier.py` & `sympy-1.9rc1/sympy/series/fourier.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/gruntz.py` & `sympy-1.9rc1/sympy/series/gruntz.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/kauers.py` & `sympy-1.9rc1/sympy/series/kauers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/limits.py` & `sympy-1.9rc1/sympy/series/limits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/limitseq.py` & `sympy-1.9rc1/sympy/series/limitseq.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/order.py` & `sympy-1.9rc1/sympy/series/order.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/residues.py` & `sympy-1.9rc1/sympy/series/residues.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/sequences.py` & `sympy-1.9rc1/sympy/series/sequences.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/series.py` & `sympy-1.9rc1/sympy/series/series.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/series_class.py` & `sympy-1.9rc1/sympy/series/series_class.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_approximants.py` & `sympy-1.9rc1/sympy/series/tests/test_approximants.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_aseries.py` & `sympy-1.9rc1/sympy/series/tests/test_aseries.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_demidovich.py` & `sympy-1.9rc1/sympy/series/tests/test_demidovich.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_formal.py` & `sympy-1.9rc1/sympy/series/tests/test_formal.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_fourier.py` & `sympy-1.9rc1/sympy/series/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_gruntz.py` & `sympy-1.9rc1/sympy/series/tests/test_gruntz.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_kauers.py` & `sympy-1.9rc1/sympy/series/tests/test_kauers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_limits.py` & `sympy-1.9rc1/sympy/series/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_limitseq.py` & `sympy-1.9rc1/sympy/series/tests/test_limitseq.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_lseries.py` & `sympy-1.9rc1/sympy/series/tests/test_lseries.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_nseries.py` & `sympy-1.9rc1/sympy/series/tests/test_nseries.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_order.py` & `sympy-1.9rc1/sympy/series/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_residues.py` & `sympy-1.9rc1/sympy/series/tests/test_residues.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_sequences.py` & `sympy-1.9rc1/sympy/series/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/series/tests/test_series.py` & `sympy-1.9rc1/sympy/series/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/__init__.py` & `sympy-1.9rc1/sympy/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/conditionset.py` & `sympy-1.9rc1/sympy/sets/conditionset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/contains.py` & `sympy-1.9rc1/sympy/sets/contains.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/fancysets.py` & `sympy-1.9rc1/sympy/sets/fancysets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/add.py` & `sympy-1.9rc1/sympy/sets/handlers/add.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/comparison.py` & `sympy-1.9rc1/sympy/sets/handlers/comparison.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/functions.py` & `sympy-1.9rc1/sympy/sets/handlers/functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/intersection.py` & `sympy-1.9rc1/sympy/sets/handlers/intersection.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/issubset.py` & `sympy-1.9rc1/sympy/sets/handlers/issubset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/mul.py` & `sympy-1.9rc1/sympy/sets/handlers/mul.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/power.py` & `sympy-1.9rc1/sympy/sets/handlers/power.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/handlers/union.py` & `sympy-1.9rc1/sympy/sets/handlers/union.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/ordinals.py` & `sympy-1.9rc1/sympy/sets/ordinals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/powerset.py` & `sympy-1.9rc1/sympy/sets/powerset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/setexpr.py` & `sympy-1.9rc1/sympy/sets/setexpr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/sets.py` & `sympy-1.9rc1/sympy/sets/sets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_conditionset.py` & `sympy-1.9rc1/sympy/sets/tests/test_conditionset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_contains.py` & `sympy-1.9rc1/sympy/sets/tests/test_contains.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_fancysets.py` & `sympy-1.9rc1/sympy/sets/tests/test_fancysets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_ordinals.py` & `sympy-1.9rc1/sympy/sets/tests/test_ordinals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_powerset.py` & `sympy-1.9rc1/sympy/sets/tests/test_powerset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_setexpr.py` & `sympy-1.9rc1/sympy/sets/tests/test_setexpr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/sets/tests/test_sets.py` & `sympy-1.9rc1/sympy/sets/tests/test_sets.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/__init__.py` & `sympy-1.9rc1/sympy/simplify/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/combsimp.py` & `sympy-1.9rc1/sympy/simplify/combsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/cse_main.py` & `sympy-1.9rc1/sympy/simplify/cse_main.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/cse_opts.py` & `sympy-1.9rc1/sympy/simplify/cse_opts.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/epathtools.py` & `sympy-1.9rc1/sympy/simplify/epathtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/fu.py` & `sympy-1.9rc1/sympy/simplify/fu.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/gammasimp.py` & `sympy-1.9rc1/sympy/simplify/gammasimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/hyperexpand.py` & `sympy-1.9rc1/sympy/simplify/hyperexpand.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/powsimp.py` & `sympy-1.9rc1/sympy/simplify/powsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/radsimp.py` & `sympy-1.9rc1/sympy/simplify/radsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/ratsimp.py` & `sympy-1.9rc1/sympy/simplify/ratsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/simplify.py` & `sympy-1.9rc1/sympy/simplify/simplify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/sqrtdenest.py` & `sympy-1.9rc1/sympy/simplify/sqrtdenest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_combsimp.py` & `sympy-1.9rc1/sympy/simplify/tests/test_combsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_cse.py` & `sympy-1.9rc1/sympy/simplify/tests/test_cse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_epathtools.py` & `sympy-1.9rc1/sympy/simplify/tests/test_epathtools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_fu.py` & `sympy-1.9rc1/sympy/simplify/tests/test_fu.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_function.py` & `sympy-1.9rc1/sympy/simplify/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_gammasimp.py` & `sympy-1.9rc1/sympy/simplify/tests/test_gammasimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_hyperexpand.py` & `sympy-1.9rc1/sympy/simplify/tests/test_hyperexpand.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_powsimp.py` & `sympy-1.9rc1/sympy/simplify/tests/test_powsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_radsimp.py` & `sympy-1.9rc1/sympy/simplify/tests/test_radsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_ratsimp.py` & `sympy-1.9rc1/sympy/simplify/tests/test_ratsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_rewrite.py` & `sympy-1.9rc1/sympy/simplify/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_simplify.py` & `sympy-1.9rc1/sympy/simplify/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_sqrtdenest.py` & `sympy-1.9rc1/sympy/simplify/tests/test_sqrtdenest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_traversaltools.py` & `sympy-1.9rc1/sympy/simplify/tests/test_traversaltools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/tests/test_trigsimp.py` & `sympy-1.9rc1/sympy/simplify/tests/test_trigsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/traversaltools.py` & `sympy-1.9rc1/sympy/simplify/traversaltools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/simplify/trigsimp.py` & `sympy-1.9rc1/sympy/simplify/trigsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/__init__.py` & `sympy-1.9rc1/sympy/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/bivariate.py` & `sympy-1.9rc1/sympy/solvers/bivariate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/decompogen.py` & `sympy-1.9rc1/sympy/solvers/decompogen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/deutils.py` & `sympy-1.9rc1/sympy/solvers/deutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/diophantine/diophantine.py` & `sympy-1.9rc1/sympy/solvers/diophantine/diophantine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/diophantine/tests/test_diophantine.py` & `sympy-1.9rc1/sympy/solvers/diophantine/tests/test_diophantine.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/inequalities.py` & `sympy-1.9rc1/sympy/solvers/inequalities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/hypergeometric.py` & `sympy-1.9rc1/sympy/solvers/ode/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/lie_group.py` & `sympy-1.9rc1/sympy/solvers/ode/lie_group.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/nonhomogeneous.py` & `sympy-1.9rc1/sympy/solvers/ode/nonhomogeneous.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/ode.py` & `sympy-1.9rc1/sympy/solvers/ode/ode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/riccati.py` & `sympy-1.9rc1/sympy/solvers/ode/riccati.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/single.py` & `sympy-1.9rc1/sympy/solvers/ode/single.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/subscheck.py` & `sympy-1.9rc1/sympy/solvers/ode/subscheck.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/systems.py` & `sympy-1.9rc1/sympy/solvers/ode/systems.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/tests/test_lie_group.py` & `sympy-1.9rc1/sympy/solvers/ode/tests/test_lie_group.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/tests/test_ode.py` & `sympy-1.9rc1/sympy/solvers/ode/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/tests/test_riccati.py` & `sympy-1.9rc1/sympy/solvers/ode/tests/test_riccati.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/tests/test_single.py` & `sympy-1.9rc1/sympy/solvers/ode/tests/test_single.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/tests/test_subscheck.py` & `sympy-1.9rc1/sympy/solvers/ode/tests/test_subscheck.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/ode/tests/test_systems.py` & `sympy-1.9rc1/sympy/solvers/ode/tests/test_systems.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/pde.py` & `sympy-1.9rc1/sympy/solvers/pde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/polysys.py` & `sympy-1.9rc1/sympy/solvers/polysys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/recurr.py` & `sympy-1.9rc1/sympy/solvers/recurr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/solvers.py` & `sympy-1.9rc1/sympy/solvers/solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/solveset.py` & `sympy-1.9rc1/sympy/solvers/solveset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_constantsimp.py` & `sympy-1.9rc1/sympy/solvers/tests/test_constantsimp.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_decompogen.py` & `sympy-1.9rc1/sympy/solvers/tests/test_decompogen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_inequalities.py` & `sympy-1.9rc1/sympy/solvers/tests/test_inequalities.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_numeric.py` & `sympy-1.9rc1/sympy/solvers/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_pde.py` & `sympy-1.9rc1/sympy/solvers/tests/test_pde.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_polysys.py` & `sympy-1.9rc1/sympy/solvers/tests/test_polysys.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_recurr.py` & `sympy-1.9rc1/sympy/solvers/tests/test_recurr.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_solvers.py` & `sympy-1.9rc1/sympy/solvers/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/solvers/tests/test_solveset.py` & `sympy-1.9rc1/sympy/solvers/tests/test_solveset.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/__init__.py` & `sympy-1.9rc1/sympy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/compound_rv.py` & `sympy-1.9rc1/sympy/stats/compound_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/crv.py` & `sympy-1.9rc1/sympy/stats/crv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/crv_types.py` & `sympy-1.9rc1/sympy/stats/crv_types.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/drv.py` & `sympy-1.9rc1/sympy/stats/drv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/drv_types.py` & `sympy-1.9rc1/sympy/stats/drv_types.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/error_prop.py` & `sympy-1.9rc1/sympy/stats/error_prop.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/frv.py` & `sympy-1.9rc1/sympy/stats/frv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/frv_types.py` & `sympy-1.9rc1/sympy/stats/frv_types.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/joint_rv.py` & `sympy-1.9rc1/sympy/stats/joint_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/joint_rv_types.py` & `sympy-1.9rc1/sympy/stats/joint_rv_types.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/matrix_distributions.py` & `sympy-1.9rc1/sympy/stats/matrix_distributions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/random_matrix.py` & `sympy-1.9rc1/sympy/stats/random_matrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/random_matrix_models.py` & `sympy-1.9rc1/sympy/stats/random_matrix_models.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/rv.py` & `sympy-1.9rc1/sympy/stats/rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/rv_interface.py` & `sympy-1.9rc1/sympy/stats/rv_interface.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/sampling/sample_numpy.py` & `sympy-1.9rc1/sympy/stats/sampling/sample_numpy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/sampling/sample_pymc3.py` & `sympy-1.9rc1/sympy/stats/sampling/sample_pymc3.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/sampling/sample_scipy.py` & `sympy-1.9rc1/sympy/stats/sampling/sample_scipy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/sampling/tests/test_sample_continuous_rv.py` & `sympy-1.9rc1/sympy/stats/sampling/tests/test_sample_continuous_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/sampling/tests/test_sample_discrete_rv.py` & `sympy-1.9rc1/sympy/stats/sampling/tests/test_sample_discrete_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/sampling/tests/test_sample_finite_rv.py` & `sympy-1.9rc1/sympy/stats/sampling/tests/test_sample_finite_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/stochastic_process.py` & `sympy-1.9rc1/sympy/stats/stochastic_process.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/stochastic_process_types.py` & `sympy-1.9rc1/sympy/stats/stochastic_process_types.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/symbolic_multivariate_probability.py` & `sympy-1.9rc1/sympy/stats/symbolic_multivariate_probability.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/symbolic_probability.py` & `sympy-1.9rc1/sympy/stats/symbolic_probability.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_compound_rv.py` & `sympy-1.9rc1/sympy/stats/tests/test_compound_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_continuous_rv.py` & `sympy-1.9rc1/sympy/stats/tests/test_continuous_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_discrete_rv.py` & `sympy-1.9rc1/sympy/stats/tests/test_discrete_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_error_prop.py` & `sympy-1.9rc1/sympy/stats/tests/test_error_prop.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_finite_rv.py` & `sympy-1.9rc1/sympy/stats/tests/test_finite_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_joint_rv.py` & `sympy-1.9rc1/sympy/stats/tests/test_joint_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_matrix_distributions.py` & `sympy-1.9rc1/sympy/stats/tests/test_matrix_distributions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_mix.py` & `sympy-1.9rc1/sympy/stats/tests/test_mix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_random_matrix.py` & `sympy-1.9rc1/sympy/stats/tests/test_random_matrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_rv.py` & `sympy-1.9rc1/sympy/stats/tests/test_rv.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_stochastic_process.py` & `sympy-1.9rc1/sympy/stats/tests/test_stochastic_process.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_symbolic_multivariate.py` & `sympy-1.9rc1/sympy/stats/tests/test_symbolic_multivariate.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/stats/tests/test_symbolic_probability.py` & `sympy-1.9rc1/sympy/stats/tests/test_symbolic_probability.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/__init__.py` & `sympy-1.9rc1/sympy/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/branch/core.py` & `sympy-1.9rc1/sympy/strategies/branch/core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/branch/tests/test_core.py` & `sympy-1.9rc1/sympy/strategies/branch/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/branch/tests/test_tools.py` & `sympy-1.9rc1/sympy/strategies/branch/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/branch/tests/test_traverse.py` & `sympy-1.9rc1/sympy/strategies/branch/tests/test_traverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/branch/traverse.py` & `sympy-1.9rc1/sympy/strategies/branch/traverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/core.py` & `sympy-1.9rc1/sympy/strategies/core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/rl.py` & `sympy-1.9rc1/sympy/strategies/rl.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tests/test_core.py` & `sympy-1.9rc1/sympy/strategies/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tests/test_rl.py` & `sympy-1.9rc1/sympy/strategies/tests/test_rl.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tests/test_tools.py` & `sympy-1.9rc1/sympy/strategies/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tests/test_traverse.py` & `sympy-1.9rc1/sympy/strategies/tests/test_traverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tests/test_tree.py` & `sympy-1.9rc1/sympy/strategies/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tools.py` & `sympy-1.9rc1/sympy/strategies/tools.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/traverse.py` & `sympy-1.9rc1/sympy/strategies/traverse.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/strategies/tree.py` & `sympy-1.9rc1/sympy/strategies/tree.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/__init__.py` & `sympy-1.9rc1/sympy/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/__init__.py` & `sympy-1.9rc1/sympy/tensor/array/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/array_comprehension.py` & `sympy-1.9rc1/sympy/tensor/array/array_comprehension.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/array_derivatives.py` & `sympy-1.9rc1/sympy/tensor/array/array_derivatives.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/arrayop.py` & `sympy-1.9rc1/sympy/tensor/array/arrayop.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/dense_ndim_array.py` & `sympy-1.9rc1/sympy/tensor/array/dense_ndim_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/array_expressions.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/array_expressions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/arrayexpr_derivatives.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/arrayexpr_derivatives.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/conv_array_to_matrix.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/conv_array_to_matrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/conv_indexed_to_array.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/conv_indexed_to_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/conv_matrix_to_array.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/conv_matrix_to_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/tests/test_array_expressions.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_array_expressions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/tests/test_arrayexpr_derivatives.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_arrayexpr_derivatives.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/tests/test_as_explicit.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_as_explicit.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/tests/test_convert_array_to_matrix.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_convert_array_to_matrix.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/tests/test_convert_index_to_array.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_convert_index_to_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/tests/test_convert_matrix_to_array.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/tests/test_convert_matrix_to_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/expressions/utils.py` & `sympy-1.9rc1/sympy/tensor/array/expressions/utils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/ndim_array.py` & `sympy-1.9rc1/sympy/tensor/array/ndim_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/sparse_ndim_array.py` & `sympy-1.9rc1/sympy/tensor/array/sparse_ndim_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_array_comprehension.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_array_comprehension.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_array_derivatives.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_array_derivatives.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_arrayop.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_arrayop.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_immutable_ndim_array.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_immutable_ndim_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_mutable_ndim_array.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_mutable_ndim_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_ndim_array.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_ndim_array.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/array/tests/test_ndim_array_conversions.py` & `sympy-1.9rc1/sympy/tensor/array/tests/test_ndim_array_conversions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/functions.py` & `sympy-1.9rc1/sympy/tensor/functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/index_methods.py` & `sympy-1.9rc1/sympy/tensor/index_methods.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/indexed.py` & `sympy-1.9rc1/sympy/tensor/indexed.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tensor.py` & `sympy-1.9rc1/sympy/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tests/test_functions.py` & `sympy-1.9rc1/sympy/tensor/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tests/test_index_methods.py` & `sympy-1.9rc1/sympy/tensor/tests/test_index_methods.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tests/test_indexed.py` & `sympy-1.9rc1/sympy/tensor/tests/test_indexed.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tests/test_tensor.py` & `sympy-1.9rc1/sympy/tensor/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tests/test_tensor_element.py` & `sympy-1.9rc1/sympy/tensor/tests/test_tensor_element.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/tests/test_tensor_operators.py` & `sympy-1.9rc1/sympy/tensor/tests/test_tensor_operators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/tensor/toperators.py` & `sympy-1.9rc1/sympy/tensor/toperators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/benchmarking.py` & `sympy-1.9rc1/sympy/testing/benchmarking.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/pytest.py` & `sympy-1.9rc1/sympy/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/quality_unicode.py` & `sympy-1.9rc1/sympy/testing/quality_unicode.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/randtest.py` & `sympy-1.9rc1/sympy/testing/randtest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/runtests.py` & `sympy-1.9rc1/sympy/testing/runtests.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/tests/diagnose_imports.py` & `sympy-1.9rc1/sympy/testing/tests/diagnose_imports.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/tests/test_code_quality.py` & `sympy-1.9rc1/sympy/testing/tests/test_code_quality.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/tests/test_module_imports.py` & `sympy-1.9rc1/sympy/testing/tests/test_module_imports.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/tests/test_pytest.py` & `sympy-1.9rc1/sympy/testing/tests/test_pytest.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/testing/tmpfiles.py` & `sympy-1.9rc1/sympy/testing/tmpfiles.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/this.py` & `sympy-1.9rc1/sympy/this.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/unify/core.py` & `sympy-1.9rc1/sympy/unify/core.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/unify/rewrite.py` & `sympy-1.9rc1/sympy/unify/rewrite.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/unify/tests/test_rewrite.py` & `sympy-1.9rc1/sympy/unify/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/unify/tests/test_sympy.py` & `sympy-1.9rc1/sympy/unify/tests/test_sympy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/unify/tests/test_unify.py` & `sympy-1.9rc1/sympy/unify/tests/test_unify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/unify/usympy.py` & `sympy-1.9rc1/sympy/unify/usympy.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/__init__.py` & `sympy-1.9rc1/sympy/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/_compilation/__init__.py` & `sympy-1.9rc1/sympy/utilities/_compilation/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/_compilation/availability.py` & `sympy-1.9rc1/sympy/utilities/_compilation/availability.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/_compilation/compilation.py` & `sympy-1.9rc1/sympy/utilities/_compilation/compilation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/_compilation/runners.py` & `sympy-1.9rc1/sympy/utilities/_compilation/runners.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/_compilation/tests/test_compilation.py` & `sympy-1.9rc1/sympy/utilities/_compilation/tests/test_compilation.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/_compilation/util.py` & `sympy-1.9rc1/sympy/utilities/_compilation/util.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/autowrap.py` & `sympy-1.9rc1/sympy/utilities/autowrap.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/codegen.py` & `sympy-1.9rc1/sympy/utilities/codegen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/decorator.py` & `sympy-1.9rc1/sympy/utilities/decorator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/enumerative.py` & `sympy-1.9rc1/sympy/utilities/enumerative.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/exceptions.py` & `sympy-1.9rc1/sympy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/iterables.py` & `sympy-1.9rc1/sympy/utilities/iterables.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/lambdify.py` & `sympy-1.9rc1/sympy/utilities/lambdify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/matchpy_connector.py` & `sympy-1.9rc1/sympy/utilities/matchpy_connector.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/mathml/__init__.py` & `sympy-1.9rc1/sympy/utilities/mathml/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/mathml/data/mmlctop.xsl` & `sympy-1.9rc1/sympy/utilities/mathml/data/mmlctop.xsl`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/mathml/data/mmltex.xsl` & `sympy-1.9rc1/sympy/utilities/mathml/data/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/mathml/data/simple_mmlctop.xsl` & `sympy-1.9rc1/sympy/utilities/mathml/data/simple_mmlctop.xsl`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/memoization.py` & `sympy-1.9rc1/sympy/utilities/memoization.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/misc.py` & `sympy-1.9rc1/sympy/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/pkgdata.py` & `sympy-1.9rc1/sympy/utilities/pkgdata.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/source.py` & `sympy-1.9rc1/sympy/utilities/source.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_autowrap.py` & `sympy-1.9rc1/sympy/utilities/tests/test_autowrap.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_codegen.py` & `sympy-1.9rc1/sympy/utilities/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_codegen_julia.py` & `sympy-1.9rc1/sympy/utilities/tests/test_codegen_julia.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_codegen_octave.py` & `sympy-1.9rc1/sympy/utilities/tests/test_codegen_octave.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_codegen_rust.py` & `sympy-1.9rc1/sympy/utilities/tests/test_codegen_rust.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_decorator.py` & `sympy-1.9rc1/sympy/utilities/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_deprecated.py` & `sympy-1.9rc1/sympy/utilities/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_enumerative.py` & `sympy-1.9rc1/sympy/utilities/tests/test_enumerative.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_iterables.py` & `sympy-1.9rc1/sympy/utilities/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_lambdify.py` & `sympy-1.9rc1/sympy/utilities/tests/test_lambdify.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_matchpy_connector.py` & `sympy-1.9rc1/sympy/utilities/tests/test_matchpy_connector.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_misc.py` & `sympy-1.9rc1/sympy/utilities/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_pickling.py` & `sympy-1.9rc1/sympy/utilities/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_source.py` & `sympy-1.9rc1/sympy/utilities/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/tests/test_wester.py` & `sympy-1.9rc1/sympy/utilities/tests/test_wester.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/utilities/timeutils.py` & `sympy-1.9rc1/sympy/utilities/timeutils.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/__init__.py` & `sympy-1.9rc1/sympy/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/basisdependent.py` & `sympy-1.9rc1/sympy/vector/basisdependent.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/coordsysrect.py` & `sympy-1.9rc1/sympy/vector/coordsysrect.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/deloperator.py` & `sympy-1.9rc1/sympy/vector/deloperator.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/dyadic.py` & `sympy-1.9rc1/sympy/vector/dyadic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/functions.py` & `sympy-1.9rc1/sympy/vector/functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/implicitregion.py` & `sympy-1.9rc1/sympy/vector/implicitregion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/integrals.py` & `sympy-1.9rc1/sympy/vector/integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/operators.py` & `sympy-1.9rc1/sympy/vector/operators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/orienters.py` & `sympy-1.9rc1/sympy/vector/orienters.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/parametricregion.py` & `sympy-1.9rc1/sympy/vector/parametricregion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/point.py` & `sympy-1.9rc1/sympy/vector/point.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/scalar.py` & `sympy-1.9rc1/sympy/vector/scalar.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_coordsysrect.py` & `sympy-1.9rc1/sympy/vector/tests/test_coordsysrect.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_dyadic.py` & `sympy-1.9rc1/sympy/vector/tests/test_dyadic.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_field_functions.py` & `sympy-1.9rc1/sympy/vector/tests/test_field_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_functions.py` & `sympy-1.9rc1/sympy/vector/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_implicitregion.py` & `sympy-1.9rc1/sympy/vector/tests/test_implicitregion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_integrals.py` & `sympy-1.9rc1/sympy/vector/tests/test_integrals.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_operators.py` & `sympy-1.9rc1/sympy/vector/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_parametricregion.py` & `sympy-1.9rc1/sympy/vector/tests/test_parametricregion.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_printing.py` & `sympy-1.9rc1/sympy/vector/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/tests/test_vector.py` & `sympy-1.9rc1/sympy/vector/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `sympy-1.9/sympy/vector/vector.py` & `sympy-1.9rc1/sympy/vector/vector.py`

 * *Files identical despite different names*

