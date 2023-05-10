# Comparing `tmp/stmaterial-0.0.4.tar.gz` & `tmp/stmaterial-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmaterial-0.0.4.tar", last modified: Sat May  6 04:25:01 2023, max compression
+gzip compressed data, was "stmaterial-0.0.5.tar", last modified: Wed May 10 05:46:17 2023, max compression
```

## Comparing `stmaterial-0.0.4.tar` & `stmaterial-0.0.5.tar`

### file list

```diff
@@ -1,201 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:25:01.071255 stmaterial-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-06 04:24:42.834728 stmaterial-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-06 04:24:42.834728 stmaterial-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-06 04:24:42.834728 stmaterial-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-06 04:24:42.834728 stmaterial-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/a.png
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/b.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/books/
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/books/benders分解.png
--rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/books/内点法.png
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/c.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.838728 stmaterial-0.0.4/docs/_images/links/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/jupyter_book.png
--rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/matplotlib.png
--rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/pandas.png
--rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_images/links/gallery/sphinx_design.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/links/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/links/gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/blog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-06 04:24:42.842728 stmaterial-0.0.4/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2021-python-pathlib.md
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2022-pytest-tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2022-python-setup.md
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/posts/plangs/2022-python-typing.md
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/edit-button.md
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/fonts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/header.md
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/logo.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/sidebar-title.md
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/sidebar.md
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/user_guide/toc.md
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-06 04:24:42.846728 stmaterial-0.0.4/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-06 04:24:42.846728 stmaterial-0.0.4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-06 04:24:42.846728 stmaterial-0.0.4/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-06 04:24:42.846728 stmaterial-0.0.4/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 04:24:42.846728 stmaterial-0.0.4/postcss.config.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-06 04:24:42.846728 stmaterial-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/gumshoe-patched.js
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/materialize.js
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/scripts/stmaterial.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/base/_typography.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_breadcrumb.sass
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_edit-update-meta.scss
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/components/_table-of-contents.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_lists.sass
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_myst-nb.scss
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_tippy.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_legacy.sass
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_patch.scss
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_test.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_article.sass
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_headnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/stmaterial.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-06 04:24:42.846728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/stmaterial theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3333 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/headnav-items.html
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/postnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/sidenav-brand.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/images/github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/theme/stmaterial/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-06 04:24:42.850728 stmaterial-0.0.4/src/stmaterial/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:24:42.850728 stmaterial-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-06 04:24:42.850728 stmaterial-0.0.4/webpack.config.js
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 stmaterial-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:46:17.492102 stmaterial-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-10 05:45:45.148052 stmaterial-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 05:45:45.148052 stmaterial-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-10 05:45:45.148052 stmaterial-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-10 05:45:45.148052 stmaterial-0.0.5/docs/_images/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-10 05:45:45.148052 stmaterial-0.0.5/docs/_images/b.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/books/
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/books/benders分解.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/books/内点法.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/c.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/links/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/jupyter_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/pandas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/sphinx_design.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/links/gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/logo-.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/blog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2021-python-pathlib.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2022-pytest-tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2022-python-setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2022-python-typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/sidenav.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/edit-button.md
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/fonts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/index1.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/logo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/sidebar-title.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/sidebar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/toc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-10 05:45:45.160052 stmaterial-0.0.5/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-10 05:45:45.160052 stmaterial-0.0.5/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 05:45:45.160052 stmaterial-0.0.5/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 05:45:45.160052 stmaterial-0.0.5/postcss.config.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-10 05:45:45.160052 stmaterial-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/gumshoe-patched.js
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/materialize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/stmaterial.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/_theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_breadcrumb.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_edit-update-meta.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_searchbox.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_table-of-contents.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_api.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_code.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_lists.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_spans.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_myst-nb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_tippy.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_legacy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_patch.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_test.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_article.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_headnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/stmaterial.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/stmaterial theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3333 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/headnav-items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/postnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-10 05:45:45.168052 stmaterial-0.0.5/webpack.config.js
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 stmaterial-0.0.5/PKG-INFO
```

### Comparing `stmaterial-0.0.4/LICENSE` & `stmaterial-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/README.md` & `stmaterial-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/a.png` & `stmaterial-0.0.5/docs/_images/a.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/b.png` & `stmaterial-0.0.5/docs/_images/b.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/books/benders分解.png` & `stmaterial-0.0.5/docs/_images/books/benders分解.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/books/内点法.png` & `stmaterial-0.0.5/docs/_images/books/内点法.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/c.png` & `stmaterial-0.0.5/docs/_images/c.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/links/gallery/jupyter_book.png` & `stmaterial-0.0.5/docs/_images/links/gallery/jupyter_book.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/links/gallery/matplotlib.png` & `stmaterial-0.0.5/docs/_images/links/gallery/matplotlib.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/links/gallery/pandas.png` & `stmaterial-0.0.5/docs/_images/links/gallery/pandas.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_images/links/gallery/sphinx_design.png` & `stmaterial-0.0.5/docs/_images/links/gallery/sphinx_design.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_static/favicon.png` & `stmaterial-0.0.5/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_static/links/gallery.yaml` & `stmaterial-0.0.5/docs/_static/links/gallery.yaml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/_static/logo.png` & `stmaterial-0.0.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/conf.py` & `stmaterial-0.0.5/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,55 +31,59 @@
 
 myst_enable_extensions = ["colon_fence", "deflist"]
 exclude_patterns = [
     "_build", 
     "Thumbs.db", 
     ".DS_Store",
     "contributing",
-    "user_guide/*"
+    "user_guide_tmp/*"
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.7", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master", None),
     "markdown_it": ("https://markdown-it-py.readthedocs.io/en/latest", None),
 }
 
 templates_path = ["_templates"]
 html_static_path = ["_static"]
 html_theme = "stmaterial"
 html_title = "sphinx theme of material"
 html_favicon = "_static/favicon.png"
 html_last_updated_fmt = ""
-html_logo = "_static/logo.png"
+html_logo = "_static/logo-.png"
 
 todo_include_todos = True
 
 
 html_theme_options = {
     "header_links_before_dropdown": 4,
     "source_repository": "https://github.com/zclab/stmaterial",
     "source_branch": "main",
     "source_directory": "docs/",
     "show_back_to_top": True,
     "fix_header_nav": False,
     "logo":{
-        "text": "Logo",
+        "text": "Stmaterial",
         "logo": "_static/logo.png"
     },
     "external_links": [
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
         {"name": "Sphinx book theme", "url": "https://sphinx-book-theme.readthedocs.io/en/latest/"},
         {"name": "Pydata sphinx theme", "url": "https://pydata-sphinx-theme.readthedocs.io/"},
     ],
     "show_toc_level": 1,
     "header_icons": [
-        # {"name":"Github", "url": "http://github.com/zclab/stmaterial", "svg":"github.svg"},
         {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
-        {"name":"Email", "url": "example@example.com", "material_icons":"email"},
+        # {"name":"Email", "url": "example@example.com", "material_icons":"email"},
+    ],
+    "footer_icons": [
+        {"name":"PyPi", "url": "https://pypi.org/project/stmaterial/", "image":"https://img.shields.io/pypi/dw/stmaterial"},
+        {"name":"Licence", "url": "https://github.com/zclab/stmaterial/blob/main/LICENSE", "fontawesome":"fa-solid fa-file"},
+        {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
     ],
     "use_edit_page_button": True,
     "toc_title": "On this page",
     "custom_fonts": {
         "name": 'LXGWWenKaiLite',
         "type": 'truetype',
         "src": [
@@ -117,10 +121,10 @@
     "blog/**": [
         "search-field.html", "ablog/categories.html","ablog/tagcloud.html","ablog/archives.html","ablog/recentposts.html",
     ],
 }
 
 # https://github.com/hung1001/font-awesome-pro-v6
 html_css_files = [
-      "https://cdn.staticaly.com/gh/hung1001/font-awesome-pro-v6/44659d9/css/all.min.css",
+      "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
 ]
 fontawesome_included = True
```

### Comparing `stmaterial-0.0.4/docs/develop.md` & `stmaterial-0.0.5/docs/develop.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/admonitions.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/api.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/blocks.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/generic.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/images.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/index.md` & `stmaterial-0.0.5/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/lists.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/really-long.md` & `stmaterial-0.0.5/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/sphinx-design.md` & `stmaterial-0.0.5/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/structure.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/tables.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/kitchen-sink/typography.rst` & `stmaterial-0.0.5/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/admonitions.md` & `stmaterial-0.0.5/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/api.md` & `stmaterial-0.0.5/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/code-blocks.md` & `stmaterial-0.0.5/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/hyperlinks.md` & `stmaterial-0.0.5/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/images.md` & `stmaterial-0.0.5/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/index.md` & `stmaterial-0.0.5/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/lists.md` & `stmaterial-0.0.5/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/tables.md` & `stmaterial-0.0.5/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/tabs.md` & `stmaterial-0.0.5/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/examples/reference/text-formatting.md` & `stmaterial-0.0.5/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/posts/plangs/2021-python-pathlib.md` & `stmaterial-0.0.5/docs/posts/plangs/2021-python-pathlib.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/posts/plangs/2022-pytest-tutorial.md` & `stmaterial-0.0.5/docs/posts/plangs/2022-pytest-tutorial.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/posts/plangs/2022-python-setup.md` & `stmaterial-0.0.5/docs/posts/plangs/2022-python-setup.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/posts/plangs/2022-python-typing.md` & `stmaterial-0.0.5/docs/posts/plangs/2022-python-typing.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/edit-button.md` & `stmaterial-0.0.5/docs/user_guide_tmp/edit-button.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/fonts.md` & `stmaterial-0.0.5/docs/user_guide_tmp/fonts.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/header.md` & `stmaterial-0.0.5/docs/user_guide_tmp/header.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/index.md` & `stmaterial-0.0.5/docs/user_guide_tmp/index1.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/landing-page.md` & `stmaterial-0.0.5/docs/user_guide_tmp/landing-page.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/logo.md` & `stmaterial-0.0.5/docs/user_guide_tmp/logo.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/sidebar.md` & `stmaterial-0.0.5/docs/user_guide_tmp/sidebar.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/user_guide/toc.md` & `stmaterial-0.0.5/docs/user_guide_tmp/toc.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/docs/web-components.rst` & `stmaterial-0.0.5/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/noxfile.py` & `stmaterial-0.0.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/package-lock.json` & `stmaterial-0.0.5/package-lock.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/package.json` & `stmaterial-0.0.5/package.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/pyproject.toml` & `stmaterial-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/__init__.py` & `stmaterial-0.0.5/src/stmaterial/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sphinx.locale import get_translation
 from ._navigation import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
 from .utils import get_theme_options, config_provided_by_user
 from .directives import GalleryDirective
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 logger = logging.getLogger(__name__)
 
 MESSAGE_CATALOG_NAME = "stmaterial"
 _KNOWN_STYLES_IN_USE: Dict[str, Optional[Style]] = {
     "light": None,
     "dark": None,
 }
```

### Comparing `stmaterial-0.0.4/src/stmaterial/_navigation.py` & `stmaterial-0.0.5/src/stmaterial/_navigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
         # Add external links defined in configuration as sibling list items
         for external_link in context["theme_external_links"]:
             links_html.append(
                 f"""
                 <li class="md-tabs__item">
                   <a class="md-tabs__link nav-external" href="{ external_link["url"] }">
-                    { external_link["name"] } <span class="material-icons">open_in_new</span>
+                    { external_link["name"] } 
                   </a>
                 </li>
                 """
             )
 
         # The first links will always be visible
         links_solo = links_html[:n_links_before_dropdown]
```

### Comparing `stmaterial-0.0.4/src/stmaterial/_transforms.py` & `stmaterial-0.0.5/src/stmaterial/_transforms.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/_translations.py` & `stmaterial-0.0.5/src/stmaterial/_translations.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/scripts/gumshoe-patched.js` & `stmaterial-0.0.5/src/stmaterial/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/scripts/stmaterial.js` & `stmaterial-0.0.5/src/stmaterial/assets/scripts/stmaterial.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/base/_typography.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/components/_back-to-top.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/components/_prev-next.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/components/_table-of-contents.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_table-of-contents.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_admonitions.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_api.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_code.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_footnotes.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_images.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_lists.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_misc.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_sidebar.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_tables.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/content/_target.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_ablog.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/extensions/_timeline.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_timeline.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_legacy.sass` & `stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_legacy.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/patch/_test.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_test.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_footer.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_footer.scss`

 * *Files 26% similar despite different names*

```diff
@@ -24,7 +24,29 @@
 .stm-content-footer {
   margin-top: auto;
   padding: 10px var(--footer-horizontal-spacing);
   border-top: 1px solid var(--separator-color);
   background-color: var(--background-color);
   color: var(--font-color-medium);
 }
+
+.stm-bottom-footer {
+  display: flex;
+  align-items: center;
+  justify-content: space-between;
+}
+
+.stm-right-footer {
+  display: flex;
+  align-items: center;
+  gap: 1.2rem;
+  font-size: 24px;
+
+  a {
+    display: contents;
+    color: var(--font-color-medium);
+  }
+
+  i.material-icons {
+    font-size: 28px;
+  }
+}
```

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_headnav.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_headnav.scss`

 * *Files 19% similar despite different names*

```diff
@@ -53,28 +53,14 @@
     display: flex;
 
     @media (max-width: $medium-screen-up) {
       padding-left: 0
     }
   }
 
-  .stm-doc-logo {
-    @media (min-width: $medium-screen-up) {
-      padding-left: 15px;
-    }
-
-    height: $navbar-height;
-    width: $sidenav-width;
-
-    img {
-      max-width: calc($sidenav-width - var(--header-horizontal-spacing)*2); // $sidenav-width - 30px; 
-      max-height: $navbar-height;
-    }
-  }
-
   ul {
     a {
       display: flex;
       padding: 0 var(--header-horizontal-spacing);
     }
 
     li {
@@ -101,7 +87,16 @@
           align-items: center;
           gap: 0.25rem;
         }
       }
     }
   }
 }
+
+
+a {
+  &.nav-external:after {
+    color: unset;
+    content: "\e89e";
+    font-family: Material Icons;
+  }
+}
```

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss`

 * *Files 5% similar despite different names*

```diff
@@ -106,9 +106,10 @@
 
 nav label.sidebar-toggle {
   align-items: center;
   color: var(--pst-color-muted);
   cursor: pointer;
   display: flex;
   font-size: var(--pst-font-size-icon);
-  margin-bottom: 0
+  margin-bottom: 0;
+  padding-left: 15px;
 }
```

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/sections/_stm-sidenav.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_stm-sidenav.scss`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,9 @@
 .sidenav-logo {
-  padding: 0 0 0 var(--header-horizontal-spacing);
-}
-
-.stm-sidenav-logo {
   display: flex;
-  height: $navbar-height;
-
-  img {
-    max-height: $navbar-height;
-    padding-right: 15px;
-  }
 }
 
 aside.stm-sidenav {
   border-right: 1px solid var(--separator-color);
   clip-path: inset(0);
   display: block;
   background-color: var(--background-color-sidenav);
```

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_admonitions.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_colors.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_colors.scss`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
   --color-api-paren: var(--font-color-medium);
   --color-api-keyword: var(--font-color-main);
 
   // GUI Labels
   --color-guilabel-background: #ddeeff80;
   --color-guilabel-border: #bedaf580;
   --color-guilabel-text: var(--font-color-main);
+  // Dropdown colors
+  --dropdown-color: var(--primary-color);
 }
 
 @mixin colors-dark {
   // primary and secondary color
   --primary-color: #B39DDB;
   --primary-color-dark: #9575CD;
   --primary-color-numeric: 179, 157, 219;
@@ -135,8 +137,8 @@
   --color-background-border: #303335;
   --color-highlight-on-target: #333300;
   --color-api-keyword: var(--font-color-medium);
 
   // GUI Labels
   --color-guilabel-background: #08356380;
   --color-guilabel-border: #13395f80;
-}
+}
```

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/styles/variables/_icons.scss` & `stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/translations/README.md` & `stmaterial-0.0.5/src/stmaterial/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/Edit this page.json` & `stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/assets/translations/jsons/On this page.json` & `stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/demo/module.py` & `stmaterial-0.0.5/src/stmaterial/demo/module.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/demo/sphinxext.py` & `stmaterial-0.0.5/src/stmaterial/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/directives.py` & `stmaterial-0.0.5/src/stmaterial/directives.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/base.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/base.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/breadcrumbs.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/edit-this-page.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/postnav.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/postnav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/prev-next.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/components/search-field.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-field.html`

 * *Files 19% similar despite different names*

```diff
@@ -3,8 +3,7 @@
     <input class="search-docs" placeholder="{{ theme_search_bar_text }}" name="q"
         aria-label="{{ theme_search_bar_text }}" autocomplete="off" autocorrect="off" autocapitalize="off"
         spellcheck="false">
     <input type="hidden" name="check_keywords" value="yes">
     <input type="hidden" name="area" value="default">
     <span class="search-button__kbd-shortcut"><kbd class="kbd-shortcut__modifier">Ctrl</kbd>+<kbd>K</kbd></span>
 </form>
-<div id="searchbox"></div>
```

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/domainindex.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/domainindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/genindex.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/genindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/layout.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/layout.html`

 * *Files 16% similar despite different names*

```diff
@@ -93,146 +93,224 @@
 000005c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
 000005d0: 6469 7620 636c 6173 733d 2273 746d 2d61  div class="stm-a
 000005e0: 7274 6963 6c65 2073 6563 7469 6f6e 2063  rticle section c
 000005f0: 6f6c 2073 3132 207b 2520 6966 206e 6f74  ol s12 {% if not
 00000600: 2068 6964 655f 746f 636e 6176 2025 7d20   hide_tocnav %} 
 00000610: 6d31 3020 786c 3920 7b25 2065 6e64 6966  m10 xl9 {% endif
 00000620: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-00000630: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-00000640: 7274 6963 6c65 2072 6f6c 653d 226d 6169  rticle role="mai
-00000650: 6e22 2063 6c61 7373 3d22 7365 6374 696f  n" class="sectio
-00000660: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
+00000630: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00000640: 2069 6e63 6c75 6465 2022 636f 6d70 6f6e   include "compon
+00000650: 656e 7473 2f73 6561 7263 6862 6f78 2e68  ents/searchbox.h
+00000660: 746d 6c22 2025 7d0a 2020 2020 2020 2020  tml" %}.        
 00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 7b25 2062 6c6f 636b 2062 6f64 7920 257d  {% block body %}
-00000690: 7b7b 2062 6f64 7920 7d7d 7b25 2065 6e64  {{ body }}{% end
-000006a0: 626c 6f63 6b20 257d 0a20 2020 2020 2020  block %}.       
+00000680: 3c61 7274 6963 6c65 2072 6f6c 653d 226d  <article role="m
+00000690: 6169 6e22 2063 6c61 7373 3d22 7365 6374  ain" class="sect
+000006a0: 696f 6e22 3e0a 2020 2020 2020 2020 2020  ion">.          
 000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006c0: 203c 2f61 7274 6963 6c65 3e0a 0a20 2020   </article>..   
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000006f0: 2273 746d 2d65 6469 742d 7570 6461 7465  "stm-edit-update
-00000700: 2d6d 6574 6122 3e0a 2020 2020 2020 2020  -meta">.        
+000006c0: 2020 7b25 2062 6c6f 636b 2062 6f64 7920    {% block body 
+000006d0: 257d 7b7b 2062 6f64 7920 7d7d 7b25 2065  %}{{ body }}{% e
+000006e0: 6e64 626c 6f63 6b20 257d 0a20 2020 2020  ndblock %}.     
+000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000700: 2020 203c 2f61 7274 6963 6c65 3e0a 0a20     </article>.. 
 00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 7b25 2069 6e63 6c75 6465 2022      {% include "
-00000730: 636f 6d70 6f6e 656e 7473 2f6c 6173 742d  components/last-
-00000740: 7570 6461 7465 642e 6874 6d6c 2220 257d  updated.html" %}
-00000750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000760: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00000770: 6966 2074 6865 6d65 5f75 7365 5f65 6469  if theme_use_edi
-00000780: 745f 7061 6765 5f62 7574 746f 6e20 257d  t_page_button %}
-00000790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007a0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000007b0: 696e 636c 7564 6520 2263 6f6d 706f 6e65  include "compone
-000007c0: 6e74 732f 6564 6974 2d74 6869 732d 7061  nts/edit-this-pa
-000007d0: 6765 2e68 746d 6c22 2025 7d0a 2020 2020  ge.html" %}.    
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00000800: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000810: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000820: 763e 0a0a 2020 2020 2020 2020 2020 2020  v>..            
-00000830: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000840: 2063 6c61 7373 3d22 7374 6d2d 6172 7469   class="stm-arti
-00000850: 636c 652d 666f 6f74 6572 223e 0a20 2020  cle-footer">.   
-00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000870: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000880: 6173 733d 2270 7265 762d 6e65 7874 2d61  ass="prev-next-a
-00000890: 7265 6122 3e0a 2020 2020 2020 2020 2020  rea">.          
+00000720: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000730: 733d 2273 746d 2d65 6469 742d 7570 6461  s="stm-edit-upda
+00000740: 7465 2d6d 6574 6122 3e0a 2020 2020 2020  te-meta">.      
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+00000770: 2022 636f 6d70 6f6e 656e 7473 2f6c 6173   "components/las
+00000780: 742d 7570 6461 7465 642e 6874 6d6c 2220  t-updated.html" 
+00000790: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000007a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000007b0: 2520 6966 2074 6865 6d65 5f75 7365 5f65  % if theme_use_e
+000007c0: 6469 745f 7061 6765 5f62 7574 746f 6e20  dit_page_button 
+000007d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000007e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000007f0: 2520 696e 636c 7564 6520 2263 6f6d 706f  % include "compo
+00000800: 6e65 6e74 732f 6564 6974 2d74 6869 732d  nents/edit-this-
+00000810: 7061 6765 2e68 746d 6c22 2025 7d0a 2020  page.html" %}.  
+00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000830: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00000840: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00000850: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000860: 6469 763e 0a0a 2020 2020 2020 2020 2020  div>..          
+00000870: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000880: 6976 2063 6c61 7373 3d22 7374 6d2d 6172  iv class="stm-ar
+00000890: 7469 636c 652d 666f 6f74 6572 223e 0a20  ticle-footer">. 
 000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2020 7b25 2069 6620 7468 656d        {% if them
-000008c0: 655f 7368 6f77 5f70 7265 765f 6e65 7874  e_show_prev_next
-000008d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000008b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000008c0: 636c 6173 733d 2270 7265 762d 6e65 7874  class="prev-next
+000008d0: 2d61 7265 6122 3e0a 2020 2020 2020 2020  -area">.        
 000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 7b25 2069 6e63 6c75 6465 2022      {% include "
-00000900: 636f 6d70 6f6e 656e 7473 2f70 7265 762d  components/prev-
-00000910: 6e65 7874 2e68 746d 6c22 2025 7d0a 2020  next.html" %}.  
+000008f0: 2020 2020 2020 2020 7b25 2069 6620 7468          {% if th
+00000900: 656d 655f 7368 6f77 5f70 7265 765f 6e65  eme_show_prev_ne
+00000910: 7874 2025 7d0a 2020 2020 2020 2020 2020  xt %}.          
 00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000930: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000940: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 2020 2020 2020 2020 2020 7b25 2069 6e63            {% inc
-00000970: 6c75 6465 2022 636f 6d70 6f6e 656e 7473  lude "components
-00000980: 2f70 6f73 746e 6176 2e68 746d 6c22 2025  /postnav.html" %
-00000990: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000009a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000009b0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000009c0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-000009d0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000009e0: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 7b25 2069 6620 6e6f 7420 6869      {% if not hi
-00000a10: 6465 5f74 6f63 6e61 7620 257d 0a20 2020  de_tocnav %}.   
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 207b 2520 7365 7420 7061 6765 5f74 6f63   {% set page_toc
-00000a40: 203d 2067 656e 6572 6174 655f 746f 635f   = generate_toc_
-00000a50: 6874 6d6c 2829 2025 7d0a 2020 2020 2020  html() %}.      
-00000a60: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000a70: 2d20 6966 2070 6167 655f 746f 6320 7c20  - if page_toc | 
-00000a80: 6c65 6e67 7468 203e 3d20 3120 257d 0a20  length >= 1 %}. 
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000aa0: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-00000ab0: 746d 2d74 6f63 2063 6f6c 206d 3220 786c  tm-toc col m2 xl
-00000ac0: 3320 7b25 2069 6620 6869 6465 5f74 6f63  3 {% if hide_toc
-00000ad0: 2025 7d20 6869 6465 207b 2520 656c 7365   %} hide {% else
-00000ae0: 2025 7d20 6869 6465 2d6f 6e2d 736d 616c   %} hide-on-smal
-00000af0: 6c2d 6f6e 6c79 207b 2520 656e 6469 6620  l-only {% endif 
-00000b00: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-00000b10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00000b20: 7620 636c 6173 733d 2274 6f63 2d77 7261  v class="toc-wra
-00000b30: 7070 6572 2074 6f63 2d73 6372 6f6c 6c22  pper toc-scroll"
-00000b40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000b50: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000b60: 2069 6620 7468 656d 655f 746f 635f 7469   if theme_toc_ti
-00000b70: 746c 6520 257d 0a20 2020 2020 2020 2020  tle %}.         
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 203c 6469 7620 636c 6173 733d 2274     <div class="t
-00000ba0: 6f63 2d74 6974 6c65 223e 0a20 2020 2020  oc-title">.     
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00000bd0: 2063 6c61 7373 3d22 6d61 7465 7269 616c   class="material
-00000be0: 2d69 636f 6e73 223e 6c69 7374 3c2f 7370  -icons">list</sp
-00000bf0: 616e 3e20 7b7b 2074 6865 6d65 5f74 6f63  an> {{ theme_toc
-00000c00: 5f74 6974 6c65 207d 7d0a 2020 2020 2020  _title }}.      
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c40: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-00000c50: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
-00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 207b 7b20 7061 6765 5f74 6f63 207d 7d0a   {{ page_toc }}.
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000930: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+00000940: 2022 636f 6d70 6f6e 656e 7473 2f70 7265   "components/pre
+00000950: 762d 6e65 7874 2e68 746d 6c22 2025 7d0a  v-next.html" %}.
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009a0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+000009b0: 6e63 6c75 6465 2022 636f 6d70 6f6e 656e  nclude "componen
+000009c0: 7473 2f70 6f73 746e 6176 2e68 746d 6c22  ts/postnav.html"
+000009d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000a00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000a10: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00000a20: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000a30: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000a40: 2020 2020 2020 7b25 2069 6620 6e6f 7420        {% if not 
+00000a50: 6869 6465 5f74 6f63 6e61 7620 257d 0a20  hide_tocnav %}. 
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 2020 207b 2520 7365 7420 7061 6765 5f74     {% set page_t
+00000a80: 6f63 203d 2067 656e 6572 6174 655f 746f  oc = generate_to
+00000a90: 635f 6874 6d6c 2829 2025 7d0a 2020 2020  c_html() %}.    
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 7b25 2d20 6966 2070 6167 655f 746f 6320  {%- if page_toc 
+00000ac0: 7c20 6c65 6e67 7468 203e 3d20 3120 257d  | length >= 1 %}
+00000ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ae0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000af0: 2273 746d 2d74 6f63 2063 6f6c 206d 3220  "stm-toc col m2 
+00000b00: 786c 3320 7b25 2069 6620 6869 6465 5f74  xl3 {% if hide_t
+00000b10: 6f63 2025 7d20 6869 6465 207b 2520 656c  oc %} hide {% el
+00000b20: 7365 2025 7d20 6869 6465 2d6f 6e2d 736d  se %} hide-on-sm
+00000b30: 616c 6c2d 6f6e 6c79 207b 2520 656e 6469  all-only {% endi
+00000b40: 6620 257d 223e 0a20 2020 2020 2020 2020  f %}">.         
+00000b50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000b60: 6469 7620 636c 6173 733d 2274 6f63 2d77  div class="toc-w
+00000b70: 7261 7070 6572 2074 6f63 2d73 6372 6f6c  rapper toc-scrol
+00000b80: 6c22 3e0a 2020 2020 2020 2020 2020 2020  l">.            
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 7b25 2069 6620 7468 656d 655f 746f 635f  {% if theme_toc_
+00000bb0: 7469 746c 6520 257d 0a20 2020 2020 2020  title %}.       
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000be0: 2274 6f63 2d74 6974 6c65 223e 0a20 2020  "toc-title">.   
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
+00000c10: 616e 2063 6c61 7373 3d22 6d61 7465 7269  an class="materi
+00000c20: 616c 2d69 636f 6e73 223e 6c69 7374 3c2f  al-icons">list</
+00000c30: 7370 616e 3e20 7b7b 2074 6865 6d65 5f74  span> {{ theme_t
+00000c40: 6f63 5f74 6974 6c65 207d 7d0a 2020 2020  oc_title }}.    
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c80: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000c90: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
 00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000cd0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000cf0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000d00: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000d10: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-00000d20: 6976 3e0a 0a20 2020 2020 2020 2020 2020  iv>..           
-00000d30: 207b 2520 6966 2074 6865 6d65 5f66 6f6f   {% if theme_foo
-00000d40: 7465 725f 636f 6e74 656e 7420 257d 0a20  ter_content %}. 
-00000d50: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000d60: 636c 6173 733d 2273 746d 2d63 6f6e 7465  class="stm-conte
-00000d70: 6e74 2d66 6f6f 7465 7222 3e0a 2020 2020  nt-footer">.    
-00000d80: 2020 2020 2020 2020 2020 2020 7b25 2d20              {%- 
-00000d90: 666f 7220 666f 6f74 6572 5f69 7465 6d20  for footer_item 
-00000da0: 696e 2074 6865 6d65 5f66 6f6f 7465 725f  in theme_footer_
-00000db0: 636f 6e74 656e 7420 257d 0a20 2020 2020  content %}.     
-00000dc0: 2020 2020 2020 2020 2020 207b 252d 2069             {%- i
-00000dd0: 6e63 6c75 6465 2066 6f6f 7465 725f 6974  nclude footer_it
-00000de0: 656d 2025 7d0a 2020 2020 2020 2020 2020  em %}.          
-00000df0: 2020 2020 2020 7b25 2d20 656e 6466 6f72        {%- endfor
-00000e00: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000e10: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000e20: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
-00000e30: 2020 2020 2020 2020 3c2f 6d61 696e 3e0a          </main>.
-00000e40: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
-00000e50: 3e0a 0a7b 2520 626c 6f63 6b20 666f 6f74  >..{% block foot
-00000e60: 6572 2025 7d0a 7b25 2069 6620 7468 656d  er %}.{% if them
-00000e70: 655f 666f 6f74 6572 2025 7d0a 7b25 2069  e_footer %}.{% i
-00000e80: 6e63 6c75 6465 2022 7365 6374 696f 6e73  nclude "sections
-00000e90: 2f66 6f6f 7465 722e 6874 6d6c 2220 257d  /footer.html" %}
-00000ea0: 0a7b 2520 656e 6469 6620 257d 0a7b 2520  .{% endif %}.{% 
-00000eb0: 656e 6462 6c6f 636b 2025 7d0a 0a7b 252d  endblock %}..{%-
-00000ec0: 2065 6e64 626c 6f63 6b20 257d 0a7b 252d   endblock %}.{%-
-00000ed0: 2065 6e64 626c 6f63 6b20 257d 0a          endblock %}.
+00000cb0: 2020 207b 7b20 7061 6765 5f74 6f63 207d     {{ page_toc }
+00000cc0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000cd0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cf0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000d40: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000d50: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
+00000d60: 2f64 6976 3e0a 0a20 2020 2020 2020 2020  /div>..         
+00000d70: 2020 207b 2520 6966 2074 6865 6d65 5f66     {% if theme_f
+00000d80: 6f6f 7465 725f 636f 6e74 656e 7420 257d  ooter_content %}
+00000d90: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00000da0: 7620 636c 6173 733d 2273 746d 2d63 6f6e  v class="stm-con
+00000db0: 7465 6e74 2d66 6f6f 7465 7222 3e0a 2020  tent-footer">.  
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000dd0: 6976 2063 6c61 7373 3d22 7374 6d2d 626f  iv class="stm-bo
+00000de0: 7474 6f6d 2d66 6f6f 7465 7222 3e0a 2020  ttom-footer">.  
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 2020 3c64 6976 2063 6c61 7373 3d22 7374    <div class="st
+00000e10: 6d2d 6c65 6674 2d66 6f6f 7465 7222 3e0a  m-left-footer">.
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2020 2020 2020 7b25 2d20 666f 7220          {%- for 
+00000e40: 666f 6f74 6572 5f69 7465 6d20 696e 2074  footer_item in t
+00000e50: 6865 6d65 5f66 6f6f 7465 725f 636f 6e74  heme_footer_cont
+00000e60: 656e 7420 257d 0a20 2020 2020 2020 2020  ent %}.         
+00000e70: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000e80: 252d 2069 6e63 6c75 6465 2066 6f6f 7465  %- include foote
+00000e90: 725f 6974 656d 2025 7d0a 2020 2020 2020  r_item %}.      
+00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000eb0: 2020 7b25 2d20 656e 6466 6f72 2025 7d0a    {%- endfor %}.
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000ef0: 6469 7620 636c 6173 733d 2273 746d 2d72  div class="stm-r
+00000f00: 6967 6874 2d66 6f6f 7465 7222 3e0a 2020  ight-footer">.  
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 2020 2020 7b25 2069 6620 7468 656d        {% if them
+00000f30: 655f 666f 6f74 6572 5f69 636f 6e73 202d  e_footer_icons -
+00000f40: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000f50: 2020 2020 2020 2020 2020 207b 2520 666f             {% fo
+00000f60: 7220 6963 6f6e 5f64 6963 7420 696e 2074  r icon_dict in t
+00000f70: 6865 6d65 5f66 6f6f 7465 725f 6963 6f6e  heme_footer_icon
+00000f80: 7320 2d25 7d0a 2020 2020 2020 2020 2020  s -%}.          
+00000f90: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
+00000fa0: 2068 7265 663d 227b 7b20 6963 6f6e 5f64   href="{{ icon_d
+00000fb0: 6963 742e 7572 6c20 7d7d 2220 7461 7267  ict.url }}" targ
+00000fc0: 6574 3d22 5f62 6c61 6e6b 2220 7469 746c  et="_blank" titl
+00000fd0: 653d 227b 7b20 6963 6f6e 5f64 6963 742e  e="{{ icon_dict.
+00000fe0: 6e61 6d65 207d 7d22 2063 6c61 7373 3d22  name }}" class="
+00000ff0: 6578 742d 6c69 6e6b 223e 0a20 2020 2020  ext-link">.     
+00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001010: 2020 2020 2020 207b 2520 6966 2069 636f         {% if ico
+00001020: 6e5f 6469 6374 2e63 6c61 7373 2025 7d0a  n_dict.class %}.
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 2020 2020 3c69 2063              <i c
+00001050: 6c61 7373 3d22 7b7b 2069 636f 6e5f 6469  lass="{{ icon_di
+00001060: 6374 2e63 6c61 7373 207d 7d22 3e3c 2f69  ct.class }}"></i
+00001070: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001080: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00001090: 2065 6c69 6620 6963 6f6e 5f64 6963 742e   elif icon_dict.
+000010a0: 6d61 7465 7269 616c 5f69 636f 6e73 2025  material_icons %
+000010b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000010c0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+000010d0: 2063 6c61 7373 3d22 6d61 7465 7269 616c   class="material
+000010e0: 2d69 636f 6e73 223e 7b7b 2069 636f 6e5f  -icons">{{ icon_
+000010f0: 6469 6374 2e6d 6174 6572 6961 6c5f 6963  dict.material_ic
+00001100: 6f6e 7320 7d7d 3c2f 693e 0a20 2020 2020  ons }}</i>.     
+00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001120: 2020 2020 2020 207b 2520 656c 6966 2069         {% elif i
+00001130: 636f 6e5f 6469 6374 2e66 6f6e 7461 7765  con_dict.fontawe
+00001140: 736f 6d65 2025 7d0a 2020 2020 2020 2020  some %}.        
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 3c69 2063 6c61 7373 3d22 7b7b      <i class="{{
+00001170: 2069 636f 6e5f 6469 6374 2e66 6f6e 7461   icon_dict.fonta
+00001180: 7765 736f 6d65 207d 7d22 3e3c 2f69 3e0a  wesome }}"></i>.
+00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011a0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000011b0: 6c69 6620 6963 6f6e 5f64 6963 742e 696d  lif icon_dict.im
+000011c0: 6167 6520 257d 0a20 2020 2020 2020 2020  age %}.         
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 2020 203c 696d 6720 7372 633d 227b 7b20     <img src="{{ 
+000011f0: 6963 6f6e 5f64 6963 742e 696d 6167 6520  icon_dict.image 
+00001200: 7d7d 2220 636c 6173 733d 2273 746d 2d69  }}" class="stm-i
+00001210: 636f 6e2d 696d 6167 6522 3e0a 2020 2020  con-image">.    
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00001240: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001250: 2020 2020 2020 2020 2020 2020 3c2f 613e              </a>
+00001260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001270: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
+00001280: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
+00001290: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000012a0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+000012b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000012c0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000012d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000012e0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+000012f0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00001300: 6469 6620 257d 0a0a 2020 2020 2020 2020  dif %}..        
+00001310: 3c2f 6d61 696e 3e0a 2020 2020 3c2f 6469  </main>.    </di
+00001320: 763e 0a3c 2f64 6976 3e0a 0a7b 2520 626c  v>.</div>..{% bl
+00001330: 6f63 6b20 666f 6f74 6572 2025 7d0a 7b25  ock footer %}.{%
+00001340: 2069 6620 7468 656d 655f 666f 6f74 6572   if theme_footer
+00001350: 2025 7d0a 7b25 2069 6e63 6c75 6465 2022   %}.{% include "
+00001360: 7365 6374 696f 6e73 2f66 6f6f 7465 722e  sections/footer.
+00001370: 6874 6d6c 2220 257d 0a7b 2520 656e 6469  html" %}.{% endi
+00001380: 6620 257d 0a7b 2520 656e 6462 6c6f 636b  f %}.{% endblock
+00001390: 2025 7d0a 0a7b 252d 2065 6e64 626c 6f63   %}..{%- endbloc
+000013a0: 6b20 257d 0a7b 252d 2065 6e64 626c 6f63  k %}.{%- endbloc
+000013b0: 6b20 257d 0a                             k %}.
```

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/search.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/search.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/headnav.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/headnav.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 <div class="nav-wrapper">
     <label class="sidebar-toggle primary-toggle" for="__primary">
         <i class="material-icons">menu</i>
     </label>
     <div class="headnav-items__start">
-        <div class="headnav-item">
-            <a class="stm-doc-logo" href="{{ pathto(root_doc) }}"><img src="{{ logo_url }}" alt="Logo" /></a>
+        <div class="headnav-item hide-on-small-only">
+            {%- include "brand-logo.html" %}
         </div>
     </div>
     <div class="headnav-items__content">
         <div class="me-auto headnav-items__center">
             {% include "components/headnav-items.html" %}
         </div>
         <div class="headnav-items__end">
             <div class="headnav-item">
                 <ul>
                     <li>
-                        {% include "components/search-button.html" %}
+                        {% include "search-button.html" %}
                     </li>
                     <li>
                         <a id="theme-switch" href="#"><i class="material-icons">dark_mode</i></a>
                     </li>
                     {% if theme_header_icons -%}
                     {% for icon_dict in theme_header_icons -%}
                     <li>
                         <a href="{{ icon_dict.url }}" target="_blank" title="{{ icon_dict.name }}" class="ext-link">
                             {% if icon_dict.class %}
                             <i class="{{ icon_dict.class }}"></i>
-                            {% elif icon_dict.svg %}
-                            <img src="{{ pathto(icon_dict.svg, 1) }}" style="transform: scale(0.8);">
                             {% elif icon_dict.material_icons %}
                             <i class="material-icons">{{ icon_dict.material_icons }}</i>
                             {% elif icon_dict.fontawesome %}
                             <i class="{{ icon_dict.fontawesome }}"></i>
+                            {% elif icon_dict.image %}
+                            <img src="{{ icon_dict.image }}" class="stm-icon-image">
                             {% endif %}
                         </a>
                     </li>
                     {% endfor %}
                     {% endif %}
                 </ul>
             </div>
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
  menu
-[Logo]
+{%- include "brand-logo.html" %}
 {% include "components/headnav-items.html" %}
-    * {% include "components/search-button.html" %}
+    * {% include "search-button.html" %}
     * dark_mode
     * {% if theme_header_icons -%} {% for icon_dict in theme_header_icons -%}
-    * {%_if_icon_dict.class_%}__{%_elif_icon_dict.svg_%}_[{{_pathto
-      (icon_dict.svg,_1)_}}]_{%_elif_icon_dict.material_icons_%}_{
-      {_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_endif
-      %}
+    * {%_if_icon_dict.class_%}__{%_elif_icon_dict.material_icons_%}_{
+      {_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_elif
+      icon_dict.image_%}_[{{_icon_dict.image_}}]_{%_endif_%}
     * {% endfor %} {% endif %}
     * {%- include "search-button.html" %}
     * dark_mode
```

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/sections/sidenav.html` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/sidenav.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div class="sidenav-drawer">
     <div class="sidenav-logo">
-        {%- include "sidenav-brand.html" %}
+        {%- include "brand-logo.html" %}
     </div>
     <div class="sidenav-header-items hide-on-large-only">
         <div class="sidenav-header-items__center">
             <div class="headnav-item">
                 <ul>
                     {{ head_nav_html[1] }}
                 </ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{%- include "sidenav-brand.html" %}
+{%- include "brand-logo.html" %}
     * {{ head_nav_html[1] }}
     * {% if theme_header_icons -%} {% for icon_dict in theme_header_icons -%}
     * {%_if_icon_dict.class_%}__{%_elif_icon_dict.svg_%}_[{{_pathto
       (icon_dict.svg,_1)_}}]_{%_elif_icon_dict.material_icons_%}_{
       {_icon_dict.material_icons_}}_{%_elif_icon_dict.fontawesome_%}__{%_endif
       %}
     * {% endfor %} {% endif %}
```

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/static/images/github.svg` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/images/github.svg`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/src/stmaterial/theme/stmaterial/theme.conf` & `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/theme.conf`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 [options]
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
 logo = 
 header_links_before_dropdown = 4
 external_links = 
-header_icons = []
+header_icons =
+footer_icons = 
 use_edit_page_button=
 source_repository=
 source_branch =
 source_directory =
 source_edit_link =
 custom_fonts =
 show_prev_next = True
```

### Comparing `stmaterial-0.0.4/src/stmaterial/utils.py` & `stmaterial-0.0.5/src/stmaterial/utils.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/webpack.config.js` & `stmaterial-0.0.5/webpack.config.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.4/PKG-INFO` & `stmaterial-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmaterial
-Version: 0.0.4
+Version: 0.0.5
 Summary: A sphinx theme of materializecss.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

