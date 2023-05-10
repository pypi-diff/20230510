# Comparing `tmp/types-openpyxl-3.1.0.5.tar.gz` & `tmp/types-openpyxl-3.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-openpyxl-3.1.0.5.tar", last modified: Mon May  1 15:15:18 2023, max compression
+gzip compressed data, was "types-openpyxl-3.1.0.6.tar", last modified: Wed May 10 09:14:51 2023, max compression
```

## Comparing `types-openpyxl-3.1.0.5.tar` & `types-openpyxl-3.1.0.6.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.810914 types-openpyxl-3.1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.794914 types-openpyxl-3.1.0.5/openpyxl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/_constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.794914 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/rich_text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/cell/text.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.794914 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/area_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/bar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/bubble_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/chartspace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/data_source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/error_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/legend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/line_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/marker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/pie_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/pivot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/plotarea.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/radar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/scatter_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/series.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/series_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/shapes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/stock_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/surface_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/title.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/trendline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chart/updown_bars.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.794914 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/chartsheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/publish.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.798914 types-openpyxl-3.1.0.5/openpyxl-stubs/comments/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/comments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/comments/author.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/comments/comment_sheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/comments/comments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/comments/shape_writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.798914 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/product.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/singleton.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/compat/strings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.798914 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/nested.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/serialisable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/slots.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.798914 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/connector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/effect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/fill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/graphic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/line.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/xdr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.798914 types-openpyxl-3.1.0.5/openpyxl-stubs/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/formatting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/formatting/formatting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/formatting/rule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.798914 types-openpyxl-3.1.0.5/openpyxl-stubs/formula/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/formula/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/formula/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/formula/translate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.802914 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/extended.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/interface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/relationship.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.802914 types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18243 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.802914 types-openpyxl-3.1.0.5/openpyxl-stubs/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/reader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/reader/drawings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/reader/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/reader/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/reader/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.802914 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/alignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/borders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/cell_style.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/differential.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/fills.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/named_styles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/styleable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/stylesheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/styles/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.802914 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/bound_dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/dataframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/escape.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/formulas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/indexed_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/inference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/utils/units.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/child.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/defined_name.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/external_link/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/external_link/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/external_link/external.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/external_reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/function_group.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/smart_tags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/web.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_write_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/cell_range.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/cell_watch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/controls.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/copier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/datavalidation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/dimensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/formula.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/header_footer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/hyperlink.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/ole.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/page.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/pagebreak.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/related.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/scenario.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/smart_tag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/worksheet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/openpyxl-stubs/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/writer/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/writer/theme.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/openpyxl-stubs/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/xml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/xml/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-01 15:14:47.000000 types-openpyxl-3.1.0.5/openpyxl-stubs/xml/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:15:18.810914 types-openpyxl-3.1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:18.806914 types-openpyxl-3.1.0.5/types_openpyxl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/types_openpyxl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/types_openpyxl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/types_openpyxl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 15:15:18.000000 types-openpyxl-3.1.0.5/types_openpyxl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.406629 types-openpyxl-3.1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-10 09:14:49.000000 types-openpyxl-3.1.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 09:14:49.000000 types-openpyxl-3.1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 09:14:51.406629 types-openpyxl-3.1.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.386629 types-openpyxl-3.1.0.6/openpyxl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 09:14:49.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/_constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.386629 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/rich_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/cell/text.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.390629 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/area_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/bar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/bubble_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/chartspace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/data_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/error_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/line_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/marker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/pie_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/pivot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/plotarea.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/radar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/scatter_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/series.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/series_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/shapes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/stock_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/surface_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/title.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/trendline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chart/updown_bars.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.390629 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/chartsheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/publish.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.394629 types-openpyxl-3.1.0.6/openpyxl-stubs/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/comments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/comments/author.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/comments/comment_sheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/comments/comments.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/comments/shape_writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.394629 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/singleton.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/compat/strings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.394629 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/nested.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/serialisable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/slots.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.394629 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/connector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/effect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/fill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/graphic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18284 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/xdr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.394629 types-openpyxl-3.1.0.6/openpyxl-stubs/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/formatting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/formatting/formatting.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/formatting/rule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.394629 types-openpyxl-3.1.0.6/openpyxl-stubs/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/formula/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/formula/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/formula/translate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.398629 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/extended.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/interface.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/relationship.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.398629 types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/record.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34488 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.398629 types-openpyxl-3.1.0.6/openpyxl-stubs/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/reader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/reader/drawings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/reader/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/reader/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/reader/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.398629 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/alignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/borders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/cell_style.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/differential.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/fills.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/named_styles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/styleable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/stylesheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/styles/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.398629 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/bound_dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/dataframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/escape.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/formulas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/indexed_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/inference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/utils/units.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.402629 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/child.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/defined_name.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.402629 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/external_link/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/external_link/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/external_link/external.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/external_reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/function_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/smart_tags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/web.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.402629 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_write_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/cell_range.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/cell_watch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/controls.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/copier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/datavalidation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/dimensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/formula.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/header_footer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/hyperlink.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/ole.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/page.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/pagebreak.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/scenario.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/smart_tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/worksheet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.402629 types-openpyxl-3.1.0.6/openpyxl-stubs/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/writer/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/writer/theme.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.406629 types-openpyxl-3.1.0.6/openpyxl-stubs/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/xml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/xml/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 09:14:33.000000 types-openpyxl-3.1.0.6/openpyxl-stubs/xml/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:14:51.406629 types-openpyxl-3.1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-10 09:14:49.000000 types-openpyxl-3.1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:51.406629 types-openpyxl-3.1.0.6/types_openpyxl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 09:14:51.000000 types-openpyxl-3.1.0.6/types_openpyxl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-10 09:14:51.000000 types-openpyxl-3.1.0.6/types_openpyxl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:14:51.000000 types-openpyxl-3.1.0.6/types_openpyxl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 09:14:51.000000 types-openpyxl-3.1.0.6/types_openpyxl.egg-info/top_level.txt
```

### Comparing `types-openpyxl-3.1.0.5/CHANGELOG.md` & `types-openpyxl-3.1.0.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.1.0.6 (2023-05-10)
+
+[openpyxl] Complete base descriptors (#10001)
+
 ## 3.1.0.5 (2023-05-01)
 
 Remove unnecessary F821 noqas (#10123)
 
 ## 3.1.0.4 (2023-04-13)
 
 [openpyxl] Annotate _WorkbookChild.title property (#10043)
```

### Comparing `types-openpyxl-3.1.0.5/PKG-INFO` & `types-openpyxl-3.1.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.5
+Version: 3.1.0.6
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e816acffddf9d984bac131224b0eb0f6a3e1c9fc`.
+This package was generated from typeshed commit `1221b4711818d3c5e17c56619fc049e5dbc2fd00`.
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/cell/cell.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/cell/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/cell/read_only.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/cell/read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/cell/rich_text.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/cell/rich_text.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections.abc import Iterable
 from typing import overload
-from typing_extensions import Self
+from typing_extensions import Literal, Self
 
+from openpyxl.cell.text import InlineFont
 from openpyxl.descriptors import Strict, String, Typed
 
 class TextBlock(Strict):
-    font: Typed
-    text: String
+    font: Typed[InlineFont, Literal[False]]
+    text: String[Literal[False]]
 
-    def __init__(self, font: Typed, text: String) -> None: ...
+    def __init__(self, font: InlineFont, text: str) -> None: ...
     def __eq__(self, other: TextBlock) -> bool: ...  # type: ignore[override]
 
 class CellRichText(list[str | TextBlock]):
     @overload
     def __init__(self, __args: list[str] | list[TextBlock] | list[str | TextBlock] | tuple[str | TextBlock, ...]) -> None: ...
     @overload
     def __init__(self, *args: str | TextBlock) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/cell/text.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/label.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,86 @@
-from _typeshed import Incomplete
-
-from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.styles.fonts import Font
-
-class PhoneticProperties(Serialisable):
-    tagname: str
-    fontId: Incomplete
-    type: Incomplete
-    alignment: Incomplete
-    def __init__(
-        self, fontId: Incomplete | None = None, type: Incomplete | None = None, alignment: Incomplete | None = None
-    ) -> None: ...
-
-class PhoneticText(Serialisable):
-    tagname: str
-    sb: Incomplete
-    eb: Incomplete
-    t: Incomplete
-    text: Incomplete
-    def __init__(self, sb: Incomplete | None = None, eb: Incomplete | None = None, t: Incomplete | None = None) -> None: ...
-
-class InlineFont(Font):
-    tagname: str
-    rFont: Incomplete
-    charset: Incomplete
-    family: Incomplete
-    b: Incomplete
-    i: Incomplete
-    strike: Incomplete
-    outline: Incomplete
-    shadow: Incomplete
-    condense: Incomplete
-    extend: Incomplete
-    color: Incomplete
-    sz: Incomplete
-    u: Incomplete
-    vertAlign: Incomplete
-    scheme: Incomplete
+from _typeshed import Incomplete, Unused
+from abc import abstractmethod
+from typing_extensions import Literal
+
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.serialisable import Serialisable as Serialisable
+
+class _DataLabelBase(Serialisable):
+    numFmt: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    textProperties: Alias
+    dLblPos: Incomplete
+    position: Alias
+    showLegendKey: Incomplete
+    showVal: Incomplete
+    showCatName: Incomplete
+    showSerName: Incomplete
+    showPercent: Incomplete
+    showBubbleSize: Incomplete
+    showLeaderLines: Incomplete
+    separator: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        rFont: Incomplete | None = None,
-        charset: Incomplete | None = None,
-        family: Incomplete | None = None,
-        b: Incomplete | None = None,
-        i: Incomplete | None = None,
-        strike: Incomplete | None = None,
-        outline: Incomplete | None = None,
-        shadow: Incomplete | None = None,
-        condense: Incomplete | None = None,
-        extend: Incomplete | None = None,
-        color: Incomplete | None = None,
-        sz: Incomplete | None = None,
-        u: Incomplete | None = None,
-        vertAlign: Incomplete | None = None,
-        scheme: Incomplete | None = None,
+        numFmt: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        dLblPos: Incomplete | None = None,
+        showLegendKey: Incomplete | None = None,
+        showVal: Incomplete | None = None,
+        showCatName: Incomplete | None = None,
+        showSerName: Incomplete | None = None,
+        showPercent: Incomplete | None = None,
+        showBubbleSize: Incomplete | None = None,
+        showLeaderLines: Incomplete | None = None,
+        separator: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
+    @property
+    @abstractmethod
+    def tagname(self) -> str: ...
 
-class RichText(Serialisable):
+class DataLabel(_DataLabelBase):
     tagname: str
-    rPr: Incomplete
-    font: Incomplete
-    t: Incomplete
-    text: Incomplete
+    idx: Incomplete
+    numFmt: Incomplete
+    spPr: Incomplete
+    txPr: Incomplete
+    dLblPos: Incomplete
+    showLegendKey: Incomplete
+    showVal: Incomplete
+    showCatName: Incomplete
+    showSerName: Incomplete
+    showPercent: Incomplete
+    showBubbleSize: Incomplete
+    showLeaderLines: Incomplete
+    separator: Incomplete
+    extLst: Incomplete
     __elements__: Incomplete
-    def __init__(self, rPr: Incomplete | None = None, t: Incomplete | None = None) -> None: ...
+    def __init__(self, idx: int = 0, **kw) -> None: ...
 
-class Text(Serialisable):
+class DataLabelList(_DataLabelBase):
     tagname: str
-    t: Incomplete
-    plain: Incomplete
-    r: Incomplete
-    formatted: Incomplete
-    rPh: Incomplete
-    phonetic: Incomplete
-    phoneticPr: Incomplete
-    PhoneticProperties: Incomplete
+    dLbl: Incomplete
+    delete: Incomplete
+    numFmt: Incomplete
+    spPr: Incomplete
+    txPr: Incomplete
+    dLblPos: Incomplete
+    showLegendKey: Incomplete
+    showVal: Incomplete
+    showCatName: Incomplete
+    showSerName: Incomplete
+    showPercent: Incomplete
+    showBubbleSize: Incomplete
+    showLeaderLines: Incomplete
+    separator: Incomplete
+    extLst: Incomplete
     __elements__: Incomplete
-    def __init__(self, t: Incomplete | None = None, r=(), rPh=(), phoneticPr: Incomplete | None = None) -> None: ...
-    @property
-    def content(self): ...
+    def __init__(self, dLbl=(), delete: Incomplete | None = None, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/_3d.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/trendline.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,63 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.chart.data_source import NumFmt
+from openpyxl.chart.layout import Layout
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText, Text
+from openpyxl.descriptors.base import Alias, String, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class View3D(Serialisable):
+class TrendlineLabel(Serialisable):
     tagname: str
-    rotX: Incomplete
-    x_rotation: Incomplete
-    hPercent: Incomplete
-    height_percent: Incomplete
-    rotY: Incomplete
-    y_rotation: Incomplete
-    depthPercent: Incomplete
-    rAngAx: Incomplete
-    right_angle_axes: Incomplete
-    perspective: Incomplete
-    extLst: Incomplete
+    layout: Typed[Layout, Literal[True]]
+    tx: Typed[Text, Literal[True]]
+    numFmt: Typed[NumFmt, Literal[True]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    textProperties: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        rotX: int = 15,
-        hPercent: Incomplete | None = None,
-        rotY: int = 20,
-        depthPercent: Incomplete | None = None,
-        rAngAx: bool = True,
-        perspective: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        layout: Layout | None = None,
+        tx: Text | None = None,
+        numFmt: NumFmt | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
-class Surface(Serialisable):
+class Trendline(Serialisable):
     tagname: str
-    thickness: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    pictureOptions: Incomplete
-    extLst: Incomplete
+    name: String[Literal[True]]
+    spPr: Typed[ExtensionList, Literal[True]]
+    graphicalProperties: Alias
+    trendlineType: Incomplete
+    order: Incomplete
+    period: Incomplete
+    forward: Incomplete
+    backward: Incomplete
+    intercept: Incomplete
+    dispRSqr: Incomplete
+    dispEq: Incomplete
+    trendlineLbl: Typed[ExtensionList, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        thickness: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        pictureOptions: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-    ) -> None: ...
-
-class _3DBase(Serialisable):
-    tagname: str
-    view3D: Incomplete
-    floor: Incomplete
-    sideWall: Incomplete
-    backWall: Incomplete
-    def __init__(
-        self,
-        view3D: Incomplete | None = None,
-        floor: Incomplete | None = None,
-        sideWall: Incomplete | None = None,
-        backWall: Incomplete | None = None,
+        name: str | None = None,
+        spPr: ExtensionList | None = None,
+        trendlineType: str = "linear",
+        order: Incomplete | None = None,
+        period: Incomplete | None = None,
+        forward: Incomplete | None = None,
+        backward: Incomplete | None = None,
+        intercept: Incomplete | None = None,
+        dispRSqr: Incomplete | None = None,
+        dispEq: Incomplete | None = None,
+        trendlineLbl: ExtensionList | None = None,
+        extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/__init__.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/area_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/radar_chart.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,31 @@
-from _typeshed import Incomplete
-from abc import abstractmethod
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
+
+from openpyxl.chart.axis import NumericAxis, TextAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 
 from ._chart import ChartBase
 
-class _AreaChartBase(ChartBase):
-    grouping: Incomplete
+class RadarChart(ChartBase):
+    tagname: str
+    radarStyle: Incomplete
+    type: Alias
     varyColors: Incomplete
     ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
-    dropLines: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: Incomplete
     def __init__(
         self,
-        grouping: str = "standard",
+        radarStyle: str = "standard",
         varyColors: Incomplete | None = None,
         ser=(),
-        dLbls: Incomplete | None = None,
-        dropLines: Incomplete | None = None,
+        dLbls: DataLabelList | None = None,
+        extLst: Unused = None,
+        **kw,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
-
-class AreaChart(_AreaChartBase):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(self, axId: Incomplete | None = None, extLst: Incomplete | None = None, **kw) -> None: ...
-
-class AreaChart3D(AreaChart):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    gapDepth: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
-    z_axis: Incomplete
-    __elements__: Incomplete
-    def __init__(self, gapDepth: Incomplete | None = None, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/axis.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/axis.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,116 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing_extensions import Literal
 
+from openpyxl.chart.layout import Layout
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText, Text
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class ChartLines(Serialisable):
     tagname: str
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    def __init__(self, spPr: Incomplete | None = None) -> None: ...
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    def __init__(self, spPr: GraphicalProperties | None = None) -> None: ...
 
 class Scaling(Serialisable):
     tagname: str
     logBase: Incomplete
     orientation: Incomplete
     max: Incomplete
     min: Incomplete
-    extLst: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         logBase: Incomplete | None = None,
         orientation: str = "minMax",
         max: Incomplete | None = None,
         min: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
 class _BaseAxis(Serialisable):
     axId: Incomplete
-    scaling: Incomplete
+    scaling: Typed[Scaling, Literal[False]]
     delete: Incomplete
     axPos: Incomplete
-    majorGridlines: Incomplete
-    minorGridlines: Incomplete
+    majorGridlines: Typed[ChartLines, Literal[True]]
+    minorGridlines: Typed[ChartLines, Literal[True]]
     title: Incomplete
     numFmt: Incomplete
-    number_format: Incomplete
+    number_format: Alias
     majorTickMark: Incomplete
     minorTickMark: Incomplete
     tickLblPos: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    textProperties: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    textProperties: Alias
     crossAx: Incomplete
     crosses: Incomplete
     crossesAt: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
         axId: Incomplete | None = None,
-        scaling: Incomplete | None = None,
+        scaling: Scaling | None = None,
         delete: Incomplete | None = None,
         axPos: str = "l",
-        majorGridlines: Incomplete | None = None,
-        minorGridlines: Incomplete | None = None,
+        majorGridlines: ChartLines | None = None,
+        minorGridlines: ChartLines | None = None,
         title: Incomplete | None = None,
         numFmt: Incomplete | None = None,
         majorTickMark: Incomplete | None = None,
         minorTickMark: Incomplete | None = None,
         tickLblPos: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
         crossAx: Incomplete | None = None,
         crosses: Incomplete | None = None,
         crossesAt: Incomplete | None = None,
     ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
 class DisplayUnitsLabel(Serialisable):
     tagname: str
-    layout: Incomplete
-    tx: Incomplete
-    text: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    textPropertes: Incomplete
+    layout: Typed[Layout, Literal[True]]
+    tx: Typed[Text, Literal[True]]
+    text: Alias
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    textPropertes: Alias
     __elements__: Incomplete
     def __init__(
         self,
-        layout: Incomplete | None = None,
-        tx: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
+        layout: Layout | None = None,
+        tx: Text | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
     ) -> None: ...
 
 class DisplayUnitsLabelList(Serialisable):
     tagname: str
     custUnit: Incomplete
     builtInUnit: Incomplete
-    dispUnitsLbl: Incomplete
-    extLst: Incomplete
+    dispUnitsLbl: Typed[DisplayUnitsLabel, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         custUnit: Incomplete | None = None,
         builtInUnit: Incomplete | None = None,
-        dispUnitsLbl: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        dispUnitsLbl: DisplayUnitsLabel | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
 class NumericAxis(_BaseAxis):
     tagname: str
     axId: Incomplete
     scaling: Incomplete
     delete: Incomplete
@@ -120,24 +126,24 @@
     txPr: Incomplete
     crossAx: Incomplete
     crosses: Incomplete
     crossesAt: Incomplete
     crossBetween: Incomplete
     majorUnit: Incomplete
     minorUnit: Incomplete
-    dispUnits: Incomplete
-    extLst: Incomplete
+    dispUnits: Typed[DisplayUnitsLabelList, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         crossBetween: Incomplete | None = None,
         majorUnit: Incomplete | None = None,
         minorUnit: Incomplete | None = None,
-        dispUnits: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        dispUnits: DisplayUnitsLabelList | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
     @classmethod
     def from_tree(cls, node): ...
 
 class TextAxis(_BaseAxis):
     tagname: str
@@ -159,25 +165,25 @@
     crossesAt: Incomplete
     auto: Incomplete
     lblAlgn: Incomplete
     lblOffset: Incomplete
     tickLblSkip: Incomplete
     tickMarkSkip: Incomplete
     noMultiLvlLbl: Incomplete
-    extLst: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         auto: Incomplete | None = None,
         lblAlgn: Incomplete | None = None,
         lblOffset: int = 100,
         tickLblSkip: Incomplete | None = None,
         tickMarkSkip: Incomplete | None = None,
         noMultiLvlLbl: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class DateAxis(TextAxis):
     tagname: str
     axId: Incomplete
     scaling: Incomplete
@@ -198,26 +204,26 @@
     auto: Incomplete
     lblOffset: Incomplete
     baseTimeUnit: Incomplete
     majorUnit: Incomplete
     majorTimeUnit: Incomplete
     minorUnit: Incomplete
     minorTimeUnit: Incomplete
-    extLst: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         auto: Incomplete | None = None,
         lblOffset: Incomplete | None = None,
         baseTimeUnit: Incomplete | None = None,
         majorUnit: Incomplete | None = None,
         majorTimeUnit: Incomplete | None = None,
         minorUnit: Incomplete | None = None,
         minorTimeUnit: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class SeriesAxis(_BaseAxis):
     tagname: str
     axId: Incomplete
     scaling: Incomplete
@@ -233,16 +239,12 @@
     spPr: Incomplete
     txPr: Incomplete
     crossAx: Incomplete
     crosses: Incomplete
     crossesAt: Incomplete
     tickLblSkip: Incomplete
     tickMarkSkip: Incomplete
-    extLst: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
-        self,
-        tickLblSkip: Incomplete | None = None,
-        tickMarkSkip: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-        **kw,
+        self, tickLblSkip: Incomplete | None = None, tickMarkSkip: Incomplete | None = None, extLst: Unused = None, **kw
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/bar_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/bar_chart.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing_extensions import Literal
+
+from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 
 from ._3d import _3DBase
 from ._chart import ChartBase
 
 class _BarChartBase(ChartBase):
     barDir: Incomplete
-    type: Incomplete
+    type: Alias
     grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
     __elements__: Incomplete
     def __init__(
         self,
         barDir: str = "col",
         grouping: str = "clustered",
         varyColors: Incomplete | None = None,
         ser=(),
-        dLbls: Incomplete | None = None,
+        dLbls: DataLabelList | None = None,
         **kw,
     ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
 class BarChart(_BarChartBase):
@@ -31,26 +37,26 @@
     barDir: Incomplete
     grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
     gapWidth: Incomplete
     overlap: Incomplete
-    serLines: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
+    serLines: Typed[ChartLines, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: Incomplete
     legend: Incomplete
     def __init__(
         self,
         gapWidth: int = 150,
         overlap: Incomplete | None = None,
-        serLines: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        serLines: ChartLines | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class BarChart3D(_BarChartBase, _3DBase):
     tagname: str
     barDir: Incomplete
     grouping: Incomplete
@@ -60,22 +66,22 @@
     view3D: Incomplete
     floor: Incomplete
     sideWall: Incomplete
     backWall: Incomplete
     gapWidth: Incomplete
     gapDepth: Incomplete
     shape: Incomplete
-    serLines: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
-    z_axis: Incomplete
+    serLines: Typed[ChartLines, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    z_axis: Typed[SeriesAxis, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         gapWidth: int = 150,
         gapDepth: int = 150,
         shape: Incomplete | None = None,
-        serLines: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        serLines: ChartLines | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/bubble_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/bubble_chart.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
+
+from openpyxl.chart.axis import NumericAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 
 from ._chart import ChartBase
 
 class BubbleChart(ChartBase):
     tagname: str
     varyColors: Incomplete
     ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
     bubble3D: Incomplete
     bubbleScale: Incomplete
     showNegBubbles: Incomplete
     sizeRepresents: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[NumericAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: Incomplete
     def __init__(
         self,
         varyColors: Incomplete | None = None,
         ser=(),
-        dLbls: Incomplete | None = None,
+        dLbls: DataLabelList | None = None,
         bubble3D: Incomplete | None = None,
         bubbleScale: Incomplete | None = None,
         showNegBubbles: Incomplete | None = None,
         sizeRepresents: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/chartspace.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/cell/text.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,92 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal, TypeAlias
 
+from openpyxl.descriptors.base import Alias, Integer, NoneSet, Typed, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.fonts import Font
 
-class ChartContainer(Serialisable):
+_PhoneticPropertiesType: TypeAlias = Literal["halfwidthKatakana", "fullwidthKatakana", "Hiragana", "noConversion"]
+_PhoneticPropertiesAlignment: TypeAlias = Literal["noControl", "left", "center", "distributed"]
+
+class PhoneticProperties(Serialisable):
     tagname: str
-    title: Incomplete
-    autoTitleDeleted: Incomplete
-    pivotFmts: Incomplete
-    view3D: Incomplete
-    floor: Incomplete
-    sideWall: Incomplete
-    backWall: Incomplete
-    plotArea: Incomplete
-    legend: Incomplete
-    plotVisOnly: Incomplete
-    dispBlanksAs: Incomplete
-    showDLblsOverMax: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
+    fontId: Integer[Literal[False]]
+    type: NoneSet[_PhoneticPropertiesType]
+    alignment: NoneSet[_PhoneticPropertiesAlignment]
     def __init__(
         self,
-        title: Incomplete | None = None,
-        autoTitleDeleted: Incomplete | None = None,
-        pivotFmts=(),
-        view3D: Incomplete | None = None,
-        floor: Incomplete | None = None,
-        sideWall: Incomplete | None = None,
-        backWall: Incomplete | None = None,
-        plotArea: Incomplete | None = None,
-        legend: Incomplete | None = None,
-        plotVisOnly: bool = True,
-        dispBlanksAs: str = "gap",
-        showDLblsOverMax: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        fontId: _ConvertibleToInt,
+        type: _PhoneticPropertiesType | Literal["none"] | None = None,
+        alignment: _PhoneticPropertiesAlignment | Literal["none"] | None = None,
     ) -> None: ...
 
-class Protection(Serialisable):
+_PhoneticProperties: TypeAlias = PhoneticProperties
+
+class PhoneticText(Serialisable):
+    tagname: str
+    sb: Integer[Literal[False]]
+    eb: Integer[Literal[False]]
+    t: Incomplete
+    text: Alias
+    def __init__(self, sb: _ConvertibleToInt, eb: _ConvertibleToInt, t: Incomplete | None = None) -> None: ...
+
+class InlineFont(Font):
     tagname: str
-    chartObject: Incomplete
-    data: Incomplete
-    formatting: Incomplete
-    selection: Incomplete
-    userInterface: Incomplete
+    rFont: Incomplete
+    charset: Incomplete
+    family: Incomplete
+    b: Incomplete
+    i: Incomplete
+    strike: Incomplete
+    outline: Incomplete
+    shadow: Incomplete
+    condense: Incomplete
+    extend: Incomplete
+    color: Incomplete
+    sz: Incomplete
+    u: Incomplete
+    vertAlign: Incomplete
+    scheme: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        chartObject: Incomplete | None = None,
-        data: Incomplete | None = None,
-        formatting: Incomplete | None = None,
-        selection: Incomplete | None = None,
-        userInterface: Incomplete | None = None,
+        rFont: Incomplete | None = None,
+        charset: Incomplete | None = None,
+        family: Incomplete | None = None,
+        b: Incomplete | None = None,
+        i: Incomplete | None = None,
+        strike: Incomplete | None = None,
+        outline: Incomplete | None = None,
+        shadow: Incomplete | None = None,
+        condense: Incomplete | None = None,
+        extend: Incomplete | None = None,
+        color: Incomplete | None = None,
+        sz: Incomplete | None = None,
+        u: Incomplete | None = None,
+        vertAlign: Incomplete | None = None,
+        scheme: Incomplete | None = None,
     ) -> None: ...
 
-class ExternalData(Serialisable):
+class RichText(Serialisable):
     tagname: str
-    autoUpdate: Incomplete
-    id: Incomplete
-    def __init__(self, autoUpdate: Incomplete | None = None, id: Incomplete | None = None) -> None: ...
+    rPr: Typed[InlineFont, Literal[True]]
+    font: Alias
+    t: Incomplete
+    text: Alias
+    __elements__: Incomplete
+    def __init__(self, rPr: InlineFont | None = None, t: Incomplete | None = None) -> None: ...
 
-class ChartSpace(Serialisable):
+class Text(Serialisable):
     tagname: str
-    date1904: Incomplete
-    lang: Incomplete
-    roundedCorners: Incomplete
-    style: Incomplete
-    clrMapOvr: Incomplete
-    pivotSource: Incomplete
-    protection: Incomplete
-    chart: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    textProperties: Incomplete
-    externalData: Incomplete
-    printSettings: Incomplete
-    userShapes: Incomplete
-    extLst: Incomplete
+    t: Incomplete
+    plain: Alias
+    r: Incomplete
+    formatted: Alias
+    rPh: Incomplete
+    phonetic: Alias
+    phoneticPr: Typed[_PhoneticProperties, Literal[True]]
+    PhoneticProperties: Alias
     __elements__: Incomplete
-    def __init__(
-        self,
-        date1904: Incomplete | None = None,
-        lang: Incomplete | None = None,
-        roundedCorners: Incomplete | None = None,
-        style: Incomplete | None = None,
-        clrMapOvr: Incomplete | None = None,
-        pivotSource: Incomplete | None = None,
-        protection: Incomplete | None = None,
-        chart: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
-        externalData: Incomplete | None = None,
-        printSettings: Incomplete | None = None,
-        userShapes: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-    ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    def __init__(self, t: Incomplete | None = None, r=(), rPh=(), phoneticPr: _PhoneticProperties | None = None) -> None: ...
+    @property
+    def content(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/data_source.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/spreadsheet_drawing.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,114 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.nested import NestedText
+from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
-
-class NumFmt(Serialisable):  # type: ignore[misc]
-    formatCode: Incomplete
-    sourceLinked: Incomplete
-    def __init__(self, formatCode: Incomplete | None = None, sourceLinked: bool = False) -> None: ...
-
-class NumberValueDescriptor(NestedText):
-    allow_none: bool
-    expected_type: Incomplete
-    def __set__(self, instance, value) -> None: ...
-
-class NumVal(Serialisable):  # type: ignore[misc]
-    idx: Incomplete
-    formatCode: Incomplete
-    v: Incomplete
-    def __init__(
-        self, idx: Incomplete | None = None, formatCode: Incomplete | None = None, v: Incomplete | None = None
-    ) -> None: ...
-
-class NumData(Serialisable):  # type: ignore[misc]
-    formatCode: Incomplete
-    ptCount: Incomplete
-    pt: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self, formatCode: Incomplete | None = None, ptCount: Incomplete | None = None, pt=(), extLst: Incomplete | None = None
-    ) -> None: ...
-
-class NumRef(Serialisable):  # type: ignore[misc]
-    f: Incomplete
-    ref: Incomplete
-    numCache: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self, f: Incomplete | None = None, numCache: Incomplete | None = None, extLst: Incomplete | None = None
-    ) -> None: ...
-
-class StrVal(Serialisable):
-    tagname: str
-    idx: Incomplete
-    v: Incomplete
-    def __init__(self, idx: int = 0, v: Incomplete | None = None) -> None: ...
-
-class StrData(Serialisable):
-    tagname: str
-    ptCount: Incomplete
-    pt: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(self, ptCount: Incomplete | None = None, pt=(), extLst: Incomplete | None = None) -> None: ...
-
-class StrRef(Serialisable):
-    tagname: str
-    f: Incomplete
-    strCache: Incomplete
-    extLst: Incomplete
+from openpyxl.drawing.connector import Shape
+from openpyxl.drawing.graphic import GraphicFrame, GroupShape
+from openpyxl.drawing.picture import PictureFrame
+from openpyxl.drawing.xdr import XDRPoint2D, XDRPositiveSize2D
+
+_TwoCellAnchorEditAs: TypeAlias = Literal["twoCell", "oneCell", "absolute"]
+
+class AnchorClientData(Serialisable):
+    fLocksWithSheet: Bool[Literal[True]]
+    fPrintsWithSheet: Bool[Literal[True]]
+    def __init__(
+        self, fLocksWithSheet: _ConvertibleToBool | None = None, fPrintsWithSheet: _ConvertibleToBool | None = None
+    ) -> None: ...
+
+class AnchorMarker(Serialisable):
+    tagname: str
+    col: Incomplete
+    colOff: Incomplete
+    row: Incomplete
+    rowOff: Incomplete
+    def __init__(self, col: int = 0, colOff: int = 0, row: int = 0, rowOff: int = 0) -> None: ...
+
+class _AnchorBase(Serialisable):
+    sp: Typed[Shape, Literal[True]]
+    shape: Alias
+    grpSp: Typed[GroupShape, Literal[True]]
+    groupShape: Alias
+    graphicFrame: Typed[GraphicFrame, Literal[True]]
+    cxnSp: Typed[Shape, Literal[True]]
+    connectionShape: Alias
+    pic: Typed[PictureFrame, Literal[True]]
+    contentPart: Incomplete
+    clientData: Typed[AnchorClientData, Literal[False]]
     __elements__: Incomplete
     def __init__(
-        self, f: Incomplete | None = None, strCache: Incomplete | None = None, extLst: Incomplete | None = None
-    ) -> None: ...
-
-class NumDataSource(Serialisable):  # type: ignore[misc]
-    numRef: Incomplete
-    numLit: Incomplete
-    def __init__(self, numRef: Incomplete | None = None, numLit: Incomplete | None = None) -> None: ...
-
-class Level(Serialisable):
-    tagname: str
-    pt: Incomplete
-    __elements__: Incomplete
-    def __init__(self, pt=()) -> None: ...
-
-class MultiLevelStrData(Serialisable):
-    tagname: str
-    ptCount: Incomplete
-    lvl: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(self, ptCount: Incomplete | None = None, lvl=(), extLst: Incomplete | None = None) -> None: ...
-
-class MultiLevelStrRef(Serialisable):
-    tagname: str
-    f: Incomplete
-    multiLvlStrCache: Incomplete
-    extLst: Incomplete
+        self,
+        clientData: AnchorClientData | None = None,
+        sp: Shape | None = None,
+        grpSp: GroupShape | None = None,
+        graphicFrame: GraphicFrame | None = None,
+        cxnSp: Shape | None = None,
+        pic: PictureFrame | None = None,
+        contentPart: Incomplete | None = None,
+    ) -> None: ...
+
+class AbsoluteAnchor(_AnchorBase):
+    tagname: str
+    pos: Typed[XDRPoint2D, Literal[False]]
+    ext: Typed[XDRPositiveSize2D, Literal[False]]
+    sp: Incomplete
+    grpSp: Incomplete
+    graphicFrame: Incomplete
+    cxnSp: Incomplete
+    pic: Incomplete
+    contentPart: Incomplete
+    clientData: Incomplete
+    __elements__: Incomplete
+    def __init__(self, pos: XDRPoint2D | None = None, ext: XDRPositiveSize2D | None = None, **kw) -> None: ...
+
+class OneCellAnchor(_AnchorBase):
+    tagname: str
+    _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
+    ext: Typed[XDRPositiveSize2D, Literal[False]]
+    sp: Incomplete
+    grpSp: Incomplete
+    graphicFrame: Incomplete
+    cxnSp: Incomplete
+    pic: Incomplete
+    contentPart: Incomplete
+    clientData: Incomplete
+    __elements__: Incomplete
+    def __init__(self, _from: AnchorMarker | None = None, ext: XDRPositiveSize2D | None = None, **kw) -> None: ...
+
+class TwoCellAnchor(_AnchorBase):
+    tagname: str
+    editAs: NoneSet[_TwoCellAnchorEditAs]
+    _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
+    to: Typed[AnchorMarker, Literal[False]]
+    sp: Incomplete
+    grpSp: Incomplete
+    graphicFrame: Incomplete
+    cxnSp: Incomplete
+    pic: Incomplete
+    contentPart: Incomplete
+    clientData: Incomplete
     __elements__: Incomplete
     def __init__(
-        self, f: Incomplete | None = None, multiLvlStrCache: Incomplete | None = None, extLst: Incomplete | None = None
-    ) -> None: ...
-
-class AxDataSource(Serialisable):
-    tagname: str
-    numRef: Incomplete
-    numLit: Incomplete
-    strRef: Incomplete
-    strLit: Incomplete
-    multiLvlStrRef: Incomplete
-    def __init__(
         self,
-        numRef: Incomplete | None = None,
-        numLit: Incomplete | None = None,
-        strRef: Incomplete | None = None,
-        strLit: Incomplete | None = None,
-        multiLvlStrRef: Incomplete | None = None,
-    ) -> None: ...
+        editAs: _TwoCellAnchorEditAs | Literal["none"] | None = None,
+        _from: AnchorMarker | None = None,
+        to: AnchorMarker | None = None,
+        **kw,
+    ) -> None: ...
+
+class SpreadsheetDrawing(Serialisable):
+    tagname: str
+    mime_type: str
+    PartName: str
+    twoCellAnchor: Incomplete
+    oneCellAnchor: Incomplete
+    absoluteAnchor: Incomplete
+    __elements__: Incomplete
+    charts: Incomplete
+    images: Incomplete
+    def __init__(self, twoCellAnchor=(), oneCellAnchor=(), absoluteAnchor=()) -> None: ...
+    def __hash__(self) -> int: ...
+    def __bool__(self) -> bool: ...
+    @property
+    def path(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/label.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/line_chart.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from abc import abstractmethod
+from typing_extensions import Literal
 
-from openpyxl.descriptors.serialisable import Serialisable as Serialisable
+from openpyxl.chart.axis import ChartLines, NumericAxis, _BaseAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.chart.updown_bars import UpDownBars
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 
-class _DataLabelBase(Serialisable):
-    numFmt: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    textProperties: Incomplete
-    dLblPos: Incomplete
-    position: Incomplete
-    showLegendKey: Incomplete
-    showVal: Incomplete
-    showCatName: Incomplete
-    showSerName: Incomplete
-    showPercent: Incomplete
-    showBubbleSize: Incomplete
-    showLeaderLines: Incomplete
-    separator: Incomplete
-    extLst: Incomplete
+from ._chart import ChartBase
+
+class _LineChartBase(ChartBase):
+    grouping: Incomplete
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
+    dropLines: Typed[ChartLines, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        numFmt: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
-        dLblPos: Incomplete | None = None,
-        showLegendKey: Incomplete | None = None,
-        showVal: Incomplete | None = None,
-        showCatName: Incomplete | None = None,
-        showSerName: Incomplete | None = None,
-        showPercent: Incomplete | None = None,
-        showBubbleSize: Incomplete | None = None,
-        showLeaderLines: Incomplete | None = None,
-        separator: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        grouping: str = "standard",
+        varyColors: Incomplete | None = None,
+        ser=(),
+        dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
+        **kw,
     ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
-class DataLabel(_DataLabelBase):
+class LineChart(_LineChartBase):
     tagname: str
-    idx: Incomplete
-    numFmt: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    dLblPos: Incomplete
-    showLegendKey: Incomplete
-    showVal: Incomplete
-    showCatName: Incomplete
-    showSerName: Incomplete
-    showPercent: Incomplete
-    showBubbleSize: Incomplete
-    showLeaderLines: Incomplete
-    separator: Incomplete
-    extLst: Incomplete
+    grouping: Incomplete
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    dropLines: Incomplete
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
+    marker: Incomplete
+    smooth: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[_BaseAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: Incomplete
-    def __init__(self, idx: int = 0, **kw) -> None: ...
+    def __init__(
+        self,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
+        marker: Incomplete | None = None,
+        smooth: Incomplete | None = None,
+        extLst: Unused = None,
+        **kw,
+    ) -> None: ...
 
-class DataLabelList(_DataLabelBase):
+class LineChart3D(_LineChartBase):
     tagname: str
-    dLbl: Incomplete
-    delete: Incomplete
-    numFmt: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    dLblPos: Incomplete
-    showLegendKey: Incomplete
-    showVal: Incomplete
-    showCatName: Incomplete
-    showSerName: Incomplete
-    showPercent: Incomplete
-    showBubbleSize: Incomplete
-    showLeaderLines: Incomplete
-    separator: Incomplete
-    extLst: Incomplete
+    grouping: Incomplete
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    dropLines: Incomplete
+    gapDepth: Incomplete
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
+    marker: Incomplete
+    smooth: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[ExtensionList, Literal[False]]
+    y_axis: Typed[ExtensionList, Literal[False]]
+    z_axis: Typed[ExtensionList, Literal[False]]
     __elements__: Incomplete
-    def __init__(self, dLbl=(), delete: Incomplete | None = None, **kw) -> None: ...
+    def __init__(
+        self,
+        gapDepth: Incomplete | None = None,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
+        marker: Incomplete | None = None,
+        smooth: Incomplete | None = None,
+        **kw,
+    ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/layout.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/layout.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class ManualLayout(Serialisable):
     tagname: str
     layoutTarget: Incomplete
     xMode: Incomplete
     yMode: Incomplete
     wMode: Incomplete
     hMode: Incomplete
     x: Incomplete
     y: Incomplete
     w: Incomplete
-    width: Incomplete
+    width: Alias
     h: Incomplete
-    height: Incomplete
-    extLst: Incomplete
+    height: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         layoutTarget: Incomplete | None = None,
         xMode: Incomplete | None = None,
         yMode: Incomplete | None = None,
         wMode: str = "factor",
         hMode: str = "factor",
         x: Incomplete | None = None,
         y: Incomplete | None = None,
         w: Incomplete | None = None,
         h: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
 class Layout(Serialisable):
     tagname: str
-    manualLayout: Incomplete
-    extLst: Incomplete
+    manualLayout: Typed[ManualLayout, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(self, manualLayout: Incomplete | None = None, extLst: Incomplete | None = None) -> None: ...
+    def __init__(self, manualLayout: ManualLayout | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/legend.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/formula.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from _typeshed import Incomplete
+from collections.abc import Iterator
+from typing import ClassVar
 
-from openpyxl.descriptors.serialisable import Serialisable
+class DataTableFormula:
+    t: ClassVar[str]
 
-class LegendEntry(Serialisable):
-    tagname: str
-    idx: Incomplete
-    delete: Incomplete
-    txPr: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self, idx: int = 0, delete: bool = False, txPr: Incomplete | None = None, extLst: Incomplete | None = None
-    ) -> None: ...
+    ref: Incomplete
+    ca: bool
+    dt2D: bool
+    dtr: bool
+    r1: Incomplete | None
+    r2: Incomplete | None
+    del1: bool
+    del2: bool
 
-class Legend(Serialisable):
-    tagname: str
-    legendPos: Incomplete
-    position: Incomplete
-    legendEntry: Incomplete
-    layout: Incomplete
-    overlay: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    textProperties: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
     def __init__(
         self,
-        legendPos: str = "r",
-        legendEntry=(),
-        layout: Incomplete | None = None,
-        overlay: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        ref,
+        ca: bool = False,
+        dt2D: bool = False,
+        dtr: bool = False,
+        r1: Incomplete | None = None,
+        r2: Incomplete | None = None,
+        del1: bool = False,
+        del2: bool = False,
+        **kw,
     ) -> None: ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
+
+class ArrayFormula:
+    t: ClassVar[str]
+    ref: Incomplete
+    text: Incomplete | None
+
+    def __init__(self, ref, text: Incomplete | None = None) -> None: ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/line_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/plotarea.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,72 @@
-from _typeshed import Incomplete
-from abc import abstractmethod
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
-from ._chart import ChartBase
+from openpyxl.chart.layout import Layout
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.serialisable import Serialisable
 
-class _LineChartBase(ChartBase):
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
-    dropLines: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self,
-        grouping: str = "standard",
-        varyColors: Incomplete | None = None,
-        ser=(),
-        dLbls: Incomplete | None = None,
-        dropLines: Incomplete | None = None,
-        **kw,
-    ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
-
-class LineChart(_LineChartBase):
+class DataTable(Serialisable):
     tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    hiLowLines: Incomplete
-    upDownBars: Incomplete
-    marker: Incomplete
-    smooth: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
+    showHorzBorder: Incomplete
+    showVertBorder: Incomplete
+    showOutline: Incomplete
+    showKeys: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        hiLowLines: Incomplete | None = None,
-        upDownBars: Incomplete | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-        **kw,
+        showHorzBorder: Incomplete | None = None,
+        showVertBorder: Incomplete | None = None,
+        showOutline: Incomplete | None = None,
+        showKeys: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
-class LineChart3D(_LineChartBase):
+class PlotArea(Serialisable):
     tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    gapDepth: Incomplete
-    hiLowLines: Incomplete
-    upDownBars: Incomplete
-    marker: Incomplete
-    smooth: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
-    z_axis: Incomplete
+    layout: Typed[Layout, Literal[True]]
+    dTable: Typed[DataTable, Literal[True]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
+    areaChart: Incomplete
+    area3DChart: Incomplete
+    lineChart: Incomplete
+    line3DChart: Incomplete
+    stockChart: Incomplete
+    radarChart: Incomplete
+    scatterChart: Incomplete
+    pieChart: Incomplete
+    pie3DChart: Incomplete
+    doughnutChart: Incomplete
+    barChart: Incomplete
+    bar3DChart: Incomplete
+    ofPieChart: Incomplete
+    surfaceChart: Incomplete
+    surface3DChart: Incomplete
+    bubbleChart: Incomplete
+    valAx: Incomplete
+    catAx: Incomplete
+    dateAx: Incomplete
+    serAx: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        gapDepth: Incomplete | None = None,
-        hiLowLines: Incomplete | None = None,
-        upDownBars: Incomplete | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
-        **kw,
+        layout: Layout | None = None,
+        dTable: DataTable | None = None,
+        spPr: GraphicalProperties | None = None,
+        _charts=(),
+        _axes=(),
+        extLst: Unused = None,
     ) -> None: ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    @classmethod
+    def from_tree(cls, node): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/marker.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/marker.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.chart.picture import PictureOptions
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Marker(Serialisable):
     tagname: str
     symbol: Incomplete
     size: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    extLst: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         symbol: Incomplete | None = None,
         size: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
 class DataPoint(Serialisable):
     tagname: str
     idx: Incomplete
     invertIfNegative: Incomplete
-    marker: Incomplete
+    marker: Typed[Marker, Literal[True]]
     bubble3D: Incomplete
     explosion: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    pictureOptions: Incomplete
-    extLst: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    pictureOptions: Typed[PictureOptions, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         idx: Incomplete | None = None,
         invertIfNegative: Incomplete | None = None,
-        marker: Incomplete | None = None,
+        marker: Marker | None = None,
         bubble3D: Incomplete | None = None,
         explosion: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        pictureOptions: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        pictureOptions: PictureOptions | None = None,
+        extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/picture.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/picture.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/pie_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/extended.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from _typeshed import Incomplete
-from abc import abstractmethod
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.serialisable import Serialisable
 
-from ._chart import ChartBase
+def get_version(): ...
 
-class _PieChartBase(ChartBase):
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
+class DigSigBlob(Serialisable):
     __elements__: Incomplete
-    def __init__(self, varyColors: bool = True, ser=(), dLbls: Incomplete | None = None) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
+    __attrs__: Incomplete
 
-class PieChart(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    firstSliceAng: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(self, firstSliceAng: int = 0, extLst: Incomplete | None = None, **kw) -> None: ...
-
-class PieChart3D(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    extLst: Incomplete
+class VectorLpstr(Serialisable):
     __elements__: Incomplete
+    __attrs__: Incomplete
 
-class DoughnutChart(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    firstSliceAng: Incomplete
-    holeSize: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(self, firstSliceAng: int = 0, holeSize: int = 10, extLst: Incomplete | None = None, **kw) -> None: ...
-
-class CustomSplit(Serialisable):
-    tagname: str
-    secondPiePt: Incomplete
+class VectorVariant(Serialisable):
     __elements__: Incomplete
-    def __init__(self, secondPiePt=()) -> None: ...
+    __attrs__: Incomplete
 
-class ProjectedPieChart(_PieChartBase):
+class ExtendedProperties(Serialisable):
     tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    ofPieType: Incomplete
-    type: Incomplete
-    gapWidth: Incomplete
-    splitType: Incomplete
-    splitPos: Incomplete
-    custSplit: Incomplete
-    secondPieSize: Incomplete
-    serLines: Incomplete
-    join_lines: Incomplete
-    extLst: Incomplete
+    Template: Incomplete
+    Manager: Incomplete
+    Company: Incomplete
+    Pages: Incomplete
+    Words: Incomplete
+    Characters: Incomplete
+    PresentationFormat: Incomplete
+    Lines: Incomplete
+    Paragraphs: Incomplete
+    Slides: Incomplete
+    Notes: Incomplete
+    TotalTime: Incomplete
+    HiddenSlides: Incomplete
+    MMClips: Incomplete
+    ScaleCrop: Incomplete
+    HeadingPairs: Typed[VectorVariant, Literal[True]]
+    TitlesOfParts: Typed[VectorLpstr, Literal[True]]
+    LinksUpToDate: Incomplete
+    CharactersWithSpaces: Incomplete
+    SharedDoc: Incomplete
+    HyperlinkBase: Incomplete
+    HLinks: Typed[VectorVariant, Literal[True]]
+    HyperlinksChanged: Incomplete
+    DigSig: Typed[DigSigBlob, Literal[True]]
+    Application: Incomplete
+    AppVersion: Incomplete
+    DocSecurity: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        ofPieType: str = "pie",
-        gapWidth: Incomplete | None = None,
-        splitType: str = "auto",
-        splitPos: Incomplete | None = None,
-        custSplit: Incomplete | None = None,
-        secondPieSize: int = 75,
-        serLines: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-        **kw,
+        Template: Incomplete | None = None,
+        Manager: Incomplete | None = None,
+        Company: Incomplete | None = None,
+        Pages: Incomplete | None = None,
+        Words: Incomplete | None = None,
+        Characters: Incomplete | None = None,
+        PresentationFormat: Incomplete | None = None,
+        Lines: Incomplete | None = None,
+        Paragraphs: Incomplete | None = None,
+        Slides: Incomplete | None = None,
+        Notes: Incomplete | None = None,
+        TotalTime: Incomplete | None = None,
+        HiddenSlides: Incomplete | None = None,
+        MMClips: Incomplete | None = None,
+        ScaleCrop: Incomplete | None = None,
+        HeadingPairs: Unused = None,
+        TitlesOfParts: Unused = None,
+        LinksUpToDate: Incomplete | None = None,
+        CharactersWithSpaces: Incomplete | None = None,
+        SharedDoc: Incomplete | None = None,
+        HyperlinkBase: Incomplete | None = None,
+        HLinks: Unused = None,
+        HyperlinksChanged: Incomplete | None = None,
+        DigSig: Unused = None,
+        Application: str = "Microsoft Excel",
+        AppVersion: Incomplete | None = None,
+        DocSecurity: Incomplete | None = None,
     ) -> None: ...
+    def to_tree(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/pivot.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/pivot.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.chart.label import DataLabel as _DataLabel
+from openpyxl.chart.marker import Marker
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class PivotSource(Serialisable):
     tagname: str
     name: Incomplete
     fmtId: Incomplete
-    extLst: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(
-        self, name: Incomplete | None = None, fmtId: Incomplete | None = None, extLst: Incomplete | None = None
-    ) -> None: ...
+    def __init__(self, name: str | None = None, fmtId: Incomplete | None = None, extLst: Unused = None) -> None: ...
 
 class PivotFormat(Serialisable):
     tagname: str
     idx: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    TextBody: Incomplete
-    marker: Incomplete
-    dLbl: Incomplete
-    DataLabel: Incomplete
-    extLst: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    TextBody: Alias
+    marker: Typed[Marker, Literal[True]]
+    dLbl: Typed[_DataLabel, Literal[True]]
+    DataLabel: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
         idx: int = 0,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
-        marker: Incomplete | None = None,
-        dLbl: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        marker: Marker | None = None,
+        dLbl: _DataLabel | None = None,
+        extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/plotarea.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/styles/differential.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,42 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles import Alignment, Border, Fill, Font, Protection
+from openpyxl.styles.numbers import NumberFormat
 
-class DataTable(Serialisable):
+class DifferentialStyle(Serialisable):
     tagname: str
-    showHorzBorder: Incomplete
-    showVertBorder: Incomplete
-    showOutline: Incomplete
-    showKeys: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    extLst: Incomplete
     __elements__: Incomplete
+    font: Typed[Font, Literal[True]]
+    numFmt: Typed[NumberFormat, Literal[True]]
+    fill: Typed[Fill, Literal[True]]
+    alignment: Typed[Alignment, Literal[True]]
+    border: Typed[Border, Literal[True]]
+    protection: Typed[Protection, Literal[True]]
+    extLst: ExtensionList | None
     def __init__(
         self,
-        showHorzBorder: Incomplete | None = None,
-        showVertBorder: Incomplete | None = None,
-        showOutline: Incomplete | None = None,
-        showKeys: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        font: Font | None = None,
+        numFmt: NumberFormat | None = None,
+        fill: Fill | None = None,
+        alignment: Alignment | None = None,
+        border: Border | None = None,
+        protection: Protection | None = None,
+        extLst: ExtensionList | None = None,
     ) -> None: ...
 
-class PlotArea(Serialisable):
+class DifferentialStyleList(Serialisable):
     tagname: str
-    layout: Incomplete
-    dTable: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    extLst: Incomplete
-    areaChart: Incomplete
-    area3DChart: Incomplete
-    lineChart: Incomplete
-    line3DChart: Incomplete
-    stockChart: Incomplete
-    radarChart: Incomplete
-    scatterChart: Incomplete
-    pieChart: Incomplete
-    pie3DChart: Incomplete
-    doughnutChart: Incomplete
-    barChart: Incomplete
-    bar3DChart: Incomplete
-    ofPieChart: Incomplete
-    surfaceChart: Incomplete
-    surface3DChart: Incomplete
-    bubbleChart: Incomplete
-    valAx: Incomplete
-    catAx: Incomplete
-    dateAx: Incomplete
-    serAx: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self,
-        layout: Incomplete | None = None,
-        dTable: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        _charts=(),
-        _axes=(),
-        extLst: Incomplete | None = None,
-    ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
-    @classmethod
-    def from_tree(cls, node): ...
+    dxf: Incomplete
+    styles: Alias
+    __attrs__: Incomplete
+    def __init__(self, dxf=(), count: Incomplete | None = None) -> None: ...
+    def append(self, dxf) -> None: ...
+    def add(self, dxf): ...
+    def __bool__(self) -> bool: ...
+    def __getitem__(self, idx): ...
+    @property
+    def count(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/radar_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/scatter_chart.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
-from ._chart import ChartBase
+from openpyxl.chart.axis import NumericAxis, TextAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 
-class RadarChart(ChartBase):
+from ._chart import ChartBase as ChartBase
+
+class ScatterChart(ChartBase):
     tagname: str
-    radarStyle: Incomplete
-    type: Incomplete
+    scatterStyle: Incomplete
     varyColors: Incomplete
     ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[NumericAxis | TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: Incomplete
     def __init__(
         self,
-        radarStyle: str = "standard",
+        scatterStyle: Incomplete | None = None,
         varyColors: Incomplete | None = None,
         ser=(),
-        dLbls: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        dLbls: DataLabelList | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/reference.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_write_only.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 from _typeshed import Incomplete
-from collections.abc import Generator
 
-from openpyxl.descriptors import Strict
+from openpyxl.workbook.child import _WorkbookChild
 
-class DummyWorksheet:
-    title: Incomplete
-    def __init__(self, title) -> None: ...
-
-class Reference(Strict):
-    min_row: Incomplete
-    max_row: Incomplete
-    min_col: Incomplete
-    max_col: Incomplete
-    range_string: Incomplete
-    worksheet: Incomplete
-    def __init__(
-        self,
-        worksheet: Incomplete | None = None,
-        min_col: Incomplete | None = None,
-        min_row: Incomplete | None = None,
-        max_col: Incomplete | None = None,
-        max_row: Incomplete | None = None,
-        range_string: Incomplete | None = None,
-    ) -> None: ...
-    def __len__(self) -> int: ...
-    def __eq__(self, other): ...
+class WriteOnlyWorksheet(_WorkbookChild):
+    mime_type: Incomplete
+    add_chart: Incomplete
+    add_image: Incomplete
+    add_table: Incomplete
+    @property
+    def tables(self): ...
     @property
-    def rows(self) -> Generator[Incomplete, None, None]: ...
+    def print_titles(self): ...
+    print_title_cols: Incomplete
+    print_title_rows: Incomplete
+    freeze_panes: Incomplete
+    print_area: Incomplete
     @property
-    def cols(self) -> Generator[Incomplete, None, None]: ...
-    def pop(self): ...
+    def sheet_view(self): ...
+    def __init__(self, parent, title) -> None: ...
     @property
-    def sheetname(self): ...
+    def closed(self): ...
+    def close(self) -> None: ...
+    def append(self, row) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/series.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/core.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,57 @@
 from _typeshed import Incomplete
 
+from openpyxl.descriptors import DateTime
+from openpyxl.descriptors.base import Alias
+from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 
-attribute_mapping: Incomplete
+# Does not reimplement the relevant methods, so runtime also has incompatible supertypes
+class NestedDateTime(DateTime[Incomplete], NestedText):  # type: ignore[misc]
+    expected_type: type[Incomplete]
+    def to_tree(
+        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
+    ): ...
 
-class SeriesLabel(Serialisable):
-    tagname: str
-    strRef: Incomplete
-    v: Incomplete
-    value: Incomplete
-    __elements__: Incomplete
-    def __init__(self, strRef: Incomplete | None = None, v: Incomplete | None = None) -> None: ...
+class QualifiedDateTime(NestedDateTime):
+    def to_tree(
+        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
+    ): ...
 
-class Series(Serialisable):
+class DocumentProperties(Serialisable):
     tagname: str
-    idx: Incomplete
-    order: Incomplete
-    tx: Incomplete
+    namespace: Incomplete
+    category: Incomplete
+    contentStatus: Incomplete
+    keywords: Incomplete
+    lastModifiedBy: Incomplete
+    lastPrinted: Incomplete
+    revision: Incomplete
+    version: Incomplete
+    last_modified_by: Alias
+    subject: Incomplete
     title: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    pictureOptions: Incomplete
-    dPt: Incomplete
-    data_points: Incomplete
-    dLbls: Incomplete
-    labels: Incomplete
-    trendline: Incomplete
-    errBars: Incomplete
-    cat: Incomplete
-    identifiers: Incomplete
-    val: Incomplete
-    extLst: Incomplete
-    invertIfNegative: Incomplete
-    shape: Incomplete
-    xVal: Incomplete
-    yVal: Incomplete
-    bubbleSize: Incomplete
-    zVal: Incomplete
-    bubble3D: Incomplete
-    marker: Incomplete
-    smooth: Incomplete
-    explosion: Incomplete
+    creator: Incomplete
+    description: Incomplete
+    identifier: Incomplete
+    language: Incomplete
+    created: Incomplete
+    modified: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        idx: int = 0,
-        order: int = 0,
-        tx: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        pictureOptions: Incomplete | None = None,
-        dPt=(),
-        dLbls: Incomplete | None = None,
-        trendline: Incomplete | None = None,
-        errBars: Incomplete | None = None,
-        cat: Incomplete | None = None,
-        val: Incomplete | None = None,
-        invertIfNegative: Incomplete | None = None,
-        shape: Incomplete | None = None,
-        xVal: Incomplete | None = None,
-        yVal: Incomplete | None = None,
-        bubbleSize: Incomplete | None = None,
-        bubble3D: Incomplete | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
-        explosion: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        category: Incomplete | None = None,
+        contentStatus: Incomplete | None = None,
+        keywords: Incomplete | None = None,
+        lastModifiedBy: Incomplete | None = None,
+        lastPrinted: Incomplete | None = None,
+        revision: Incomplete | None = None,
+        version: Incomplete | None = None,
+        created=None,
+        creator: str = "openpyxl",
+        description: Incomplete | None = None,
+        identifier: Incomplete | None = None,
+        language: Incomplete | None = None,
+        modified=None,
+        subject: Incomplete | None = None,
+        title: Incomplete | None = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
-
-class XYSeries(Series):
-    idx: Incomplete
-    order: Incomplete
-    tx: Incomplete
-    spPr: Incomplete
-    dPt: Incomplete
-    dLbls: Incomplete
-    trendline: Incomplete
-    errBars: Incomplete
-    xVal: Incomplete
-    yVal: Incomplete
-    invertIfNegative: Incomplete
-    bubbleSize: Incomplete
-    bubble3D: Incomplete
-    marker: Incomplete
-    smooth: Incomplete
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/shapes.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/pivot/record.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class GraphicalProperties(Serialisable):
+class Record(Serialisable):
     tagname: str
-    bwMode: Incomplete
-    xfrm: Incomplete
-    transform: Incomplete
-    custGeom: Incomplete
-    prstGeom: Incomplete
-    noFill: Incomplete
-    solidFill: Incomplete
-    gradFill: Incomplete
-    pattFill: Incomplete
-    ln: Incomplete
-    line: Incomplete
-    scene3d: Incomplete
-    sp3d: Incomplete
-    shape3D: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
+    m: Incomplete
+    n: Incomplete
+    b: Incomplete
+    e: Incomplete
+    s: Incomplete
+    d: Incomplete
+    x: Incomplete
     def __init__(
         self,
-        bwMode: Incomplete | None = None,
-        xfrm: Incomplete | None = None,
-        noFill: Incomplete | None = None,
-        solidFill: Incomplete | None = None,
-        gradFill: Incomplete | None = None,
-        pattFill: Incomplete | None = None,
-        ln: Incomplete | None = None,
-        scene3d: Incomplete | None = None,
-        custGeom: Incomplete | None = None,
-        prstGeom: Incomplete | None = None,
-        sp3d: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        _fields=(),
+        m: Incomplete | None = None,
+        n: Incomplete | None = None,
+        b: Incomplete | None = None,
+        e: Incomplete | None = None,
+        s: Incomplete | None = None,
+        d: Incomplete | None = None,
+        x: Incomplete | None = None,
     ) -> None: ...
+
+class RecordList(Serialisable):
+    mime_type: str
+    rel_type: str
+    tagname: str
+    r: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    __attrs__: Incomplete
+    def __init__(self, count: Unused = None, r=(), extLst: ExtensionList | None = None) -> None: ...
+    @property
+    def count(self): ...
+    def to_tree(self): ...
+    @property
+    def path(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/stock_chart.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/styles/fonts.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,59 @@
 from _typeshed import Incomplete
 
-from ._chart import ChartBase
+from openpyxl.descriptors.base import Alias
+from openpyxl.descriptors.serialisable import Serialisable
 
-class StockChart(ChartBase):
+class Font(Serialisable):
+    UNDERLINE_DOUBLE: str
+    UNDERLINE_DOUBLE_ACCOUNTING: str
+    UNDERLINE_SINGLE: str
+    UNDERLINE_SINGLE_ACCOUNTING: str
+    name: Incomplete
+    charset: Incomplete
+    family: Incomplete
+    sz: Incomplete
+    size: Alias
+    b: Incomplete
+    bold: Alias
+    i: Incomplete
+    italic: Alias
+    strike: Incomplete
+    strikethrough: Alias
+    outline: Incomplete
+    shadow: Incomplete
+    condense: Incomplete
+    extend: Incomplete
+    u: Incomplete
+    underline: Alias
+    vertAlign: Incomplete
+    color: Incomplete
+    scheme: Incomplete
     tagname: str
-    ser: Incomplete
-    dLbls: Incomplete
-    dataLabels: Incomplete
-    dropLines: Incomplete
-    hiLowLines: Incomplete
-    upDownBars: Incomplete
-    extLst: Incomplete
-    x_axis: Incomplete
-    y_axis: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        ser=(),
-        dLbls: Incomplete | None = None,
-        dropLines: Incomplete | None = None,
-        hiLowLines: Incomplete | None = None,
-        upDownBars: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-        **kw,
+        name: Incomplete | None = None,
+        sz: Incomplete | None = None,
+        b: Incomplete | None = None,
+        i: Incomplete | None = None,
+        charset: Incomplete | None = None,
+        u: Incomplete | None = None,
+        strike: Incomplete | None = None,
+        color: Incomplete | None = None,
+        scheme: Incomplete | None = None,
+        family: Incomplete | None = None,
+        size: Incomplete | None = None,
+        bold: Incomplete | None = None,
+        italic: Incomplete | None = None,
+        strikethrough: Incomplete | None = None,
+        underline: Incomplete | None = None,
+        vertAlign: Incomplete | None = None,
+        outline: Incomplete | None = None,
+        shadow: Incomplete | None = None,
+        condense: Incomplete | None = None,
+        extend: Incomplete | None = None,
     ) -> None: ...
+    @classmethod
+    def from_tree(cls, node): ...
+
+DEFAULT_FONT: Incomplete
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/text.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/serialisable.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from _typeshed import Incomplete
 
-from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.descriptors import MetaSerialisable
 
-class RichText(Serialisable):
-    tagname: str
-    bodyPr: Incomplete
-    properties: Incomplete
-    lstStyle: Incomplete
-    p: Incomplete
-    paragraphs: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self, bodyPr: Incomplete | None = None, lstStyle: Incomplete | None = None, p: Incomplete | None = None
-    ) -> None: ...
+KEYWORDS: Incomplete
+seq_types: Incomplete
 
-class Text(Serialisable):
-    tagname: str
-    strRef: Incomplete
-    rich: Incomplete
+class Serialisable(metaclass=MetaSerialisable):
+    __attrs__: Incomplete
+    __nested__: Incomplete
     __elements__: Incomplete
-    def __init__(self, strRef: Incomplete | None = None, rich: Incomplete | None = None) -> None: ...
+    __namespaced__: Incomplete
+    idx_base: int
+    @property
+    # TODO: needs overrides in many sub-classes
+    # @abstractmethod
+    def tagname(self) -> str: ...
+    namespace: Incomplete
+    @classmethod
+    def from_tree(cls, node): ...
     def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    def __iter__(self): ...
+    def __eq__(self, other): ...
+    def __ne__(self, other): ...
+    def __hash__(self) -> int: ...
+    def __add__(self, other): ...
+    def __copy__(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chart/title.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/error_bar.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
-from openpyxl.descriptors import Typed
+from openpyxl.chart.data_source import NumDataSource
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class Title(Serialisable):
+class ErrorBars(Serialisable):
     tagname: str
-    tx: Incomplete
-    text: Incomplete
-    layout: Incomplete
-    overlay: Incomplete
-    spPr: Incomplete
-    graphicalProperties: Incomplete
-    txPr: Incomplete
-    body: Incomplete
-    extLst: Incomplete
+    errDir: Incomplete
+    direction: Alias
+    errBarType: Incomplete
+    style: Alias
+    errValType: Incomplete
+    size: Alias
+    noEndCap: Incomplete
+    plus: Typed[NumDataSource, Literal[True]]
+    minus: Typed[NumDataSource, Literal[True]]
+    val: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        tx: Incomplete | None = None,
-        layout: Incomplete | None = None,
-        overlay: Incomplete | None = None,
-        spPr: Incomplete | None = None,
-        txPr: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        errDir: Incomplete | None = None,
+        errBarType: str = "both",
+        errValType: str = "fixedVal",
+        noEndCap: Incomplete | None = None,
+        plus: NumDataSource | None = None,
+        minus: NumDataSource | None = None,
+        val: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        extLst: Unused = None,
     ) -> None: ...
-
-def title_maker(text): ...
-
-class TitleDescriptor(Typed):
-    expected_type: Incomplete
-    allow_none: bool
-    def __set__(self, instance, value) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/custom.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/protection.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.worksheet.protection import _Protected
 
-class CustomChartsheetView(Serialisable):
+class ChartsheetProtection(Serialisable, _Protected):
     tagname: str
-    guid: Incomplete
-    scale: Incomplete
-    state: Incomplete
-    zoomToFit: Incomplete
-    pageMargins: Incomplete
-    pageSetup: Incomplete
-    headerFooter: Incomplete
-    __elements__: Incomplete
+    algorithmName: String[Literal[True]]
+    hashValue: Incomplete
+    saltValue: Incomplete
+    spinCount: Integer[Literal[True]]
+    content: Bool[Literal[True]]
+    objects: Bool[Literal[True]]
+    __attrs__: Incomplete
+    password: Incomplete
     def __init__(
         self,
-        guid: Incomplete | None = None,
-        scale: Incomplete | None = None,
-        state: str = "visible",
-        zoomToFit: Incomplete | None = None,
-        pageMargins: Incomplete | None = None,
-        pageSetup: Incomplete | None = None,
-        headerFooter: Incomplete | None = None,
+        content: _ConvertibleToBool | None = None,
+        objects: _ConvertibleToBool | None = None,
+        hashValue: Incomplete | None = None,
+        spinCount: _ConvertibleToInt | None = None,
+        saltValue: Incomplete | None = None,
+        algorithmName: str | None = None,
+        password: Incomplete | None = None,
     ) -> None: ...
-
-class CustomChartsheetViews(Serialisable):
-    tagname: str
-    customSheetView: Incomplete
-    __elements__: Incomplete
-    def __init__(self, customSheetView: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/protection.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/merge.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.protection import _Protected
 
-class ChartsheetProtection(Serialisable, _Protected):
+from .cell_range import CellRange
+
+class MergeCell(CellRange):
     tagname: str
-    algorithmName: Incomplete
-    hashValue: Incomplete
-    saltValue: Incomplete
-    spinCount: Incomplete
-    content: Incomplete
-    objects: Incomplete
+    @property
+    def ref(self): ...
     __attrs__: Incomplete
-    password: Incomplete
-    def __init__(
-        self,
-        content: Incomplete | None = None,
-        objects: Incomplete | None = None,
-        hashValue: Incomplete | None = None,
-        spinCount: Incomplete | None = None,
-        saltValue: Incomplete | None = None,
-        algorithmName: Incomplete | None = None,
-        password: Incomplete | None = None,
-    ) -> None: ...
+    def __init__(self, ref: Incomplete | None = None) -> None: ...
+    def __copy__(self): ...
+
+class MergeCells(Serialisable):
+    tagname: str
+    # Overwritten by property below
+    # count: Integer
+    mergeCell: Incomplete
+    __elements__: Incomplete
+    __attrs__: Incomplete
+    def __init__(self, count: Unused = None, mergeCell=()) -> None: ...
+    @property
+    def count(self): ...
+
+class MergedCellRange(CellRange):
+    ws: Incomplete
+    start_cell: Incomplete
+    def __init__(self, worksheet, coord) -> None: ...
+    def format(self) -> None: ...
+    def __contains__(self, coord): ...
+    def __copy__(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/chartsheet/relation.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/protection.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
-class SheetBackgroundPicture(Serialisable):
+class WorkbookProtection(Serialisable):
     tagname: str
-    id: Incomplete
-    def __init__(self, id) -> None: ...
+    workbook_password: Alias
+    workbookPasswordCharacterSet: String[Literal[True]]
+    revision_password: Alias
+    revisionsPasswordCharacterSet: String[Literal[True]]
+    lockStructure: Bool[Literal[True]]
+    lock_structure: Alias
+    lockWindows: Bool[Literal[True]]
+    lock_windows: Alias
+    lockRevision: Bool[Literal[True]]
+    lock_revision: Alias
+    revisionsAlgorithmName: String[Literal[True]]
+    revisionsHashValue: Incomplete
+    revisionsSaltValue: Incomplete
+    revisionsSpinCount: Integer[Literal[True]]
+    workbookAlgorithmName: String[Literal[True]]
+    workbookHashValue: Incomplete
+    workbookSaltValue: Incomplete
+    workbookSpinCount: Integer[Literal[True]]
+    __attrs__: Incomplete
+    def __init__(
+        self,
+        workbookPassword: Incomplete | None = None,
+        workbookPasswordCharacterSet: str | None = None,
+        revisionsPassword: Incomplete | None = None,
+        revisionsPasswordCharacterSet: str | None = None,
+        lockStructure: _ConvertibleToBool | None = None,
+        lockWindows: _ConvertibleToBool | None = None,
+        lockRevision: _ConvertibleToBool | None = None,
+        revisionsAlgorithmName: str | None = None,
+        revisionsHashValue: Incomplete | None = None,
+        revisionsSaltValue: Incomplete | None = None,
+        revisionsSpinCount: _ConvertibleToInt | None = None,
+        workbookAlgorithmName: str | None = None,
+        workbookHashValue: Incomplete | None = None,
+        workbookSaltValue: Incomplete | None = None,
+        workbookSpinCount: _ConvertibleToInt | None = None,
+    ) -> None: ...
+    def set_workbook_password(self, value: str = "", already_hashed: bool = False) -> None: ...
+    @property
+    def workbookPassword(self): ...
+    @workbookPassword.setter
+    def workbookPassword(self, value) -> None: ...
+    def set_revisions_password(self, value: str = "", already_hashed: bool = False) -> None: ...
+    @property
+    def revisionsPassword(self): ...
+    @revisionsPassword.setter
+    def revisionsPassword(self, value) -> None: ...
+    @classmethod
+    def from_tree(cls, node): ...
 
-class DrawingHF(Serialisable):
-    id: Incomplete
-    lho: Incomplete
-    leftHeaderOddPages: Incomplete
-    lhe: Incomplete
-    leftHeaderEvenPages: Incomplete
-    lhf: Incomplete
-    leftHeaderFirstPage: Incomplete
-    cho: Incomplete
-    centerHeaderOddPages: Incomplete
-    che: Incomplete
-    centerHeaderEvenPages: Incomplete
-    chf: Incomplete
-    centerHeaderFirstPage: Incomplete
-    rho: Incomplete
-    rightHeaderOddPages: Incomplete
-    rhe: Incomplete
-    rightHeaderEvenPages: Incomplete
-    rhf: Incomplete
-    rightHeaderFirstPage: Incomplete
-    lfo: Incomplete
-    leftFooterOddPages: Incomplete
-    lfe: Incomplete
-    leftFooterEvenPages: Incomplete
-    lff: Incomplete
-    leftFooterFirstPage: Incomplete
-    cfo: Incomplete
-    centerFooterOddPages: Incomplete
-    cfe: Incomplete
-    centerFooterEvenPages: Incomplete
-    cff: Incomplete
-    centerFooterFirstPage: Incomplete
-    rfo: Incomplete
-    rightFooterOddPages: Incomplete
-    rfe: Incomplete
-    rightFooterEvenPages: Incomplete
-    rff: Incomplete
-    rightFooterFirstPage: Incomplete
+DocumentSecurity = WorkbookProtection
+
+class FileSharing(Serialisable):
+    tagname: str
+    readOnlyRecommended: Bool[Literal[True]]
+    userName: String[Literal[True]]
+    reservationPassword: Incomplete
+    algorithmName: String[Literal[True]]
+    hashValue: Incomplete
+    saltValue: Incomplete
+    spinCount: Integer[Literal[True]]
     def __init__(
         self,
-        id: Incomplete | None = None,
-        lho: Incomplete | None = None,
-        lhe: Incomplete | None = None,
-        lhf: Incomplete | None = None,
-        cho: Incomplete | None = None,
-        che: Incomplete | None = None,
-        chf: Incomplete | None = None,
-        rho: Incomplete | None = None,
-        rhe: Incomplete | None = None,
-        rhf: Incomplete | None = None,
-        lfo: Incomplete | None = None,
-        lfe: Incomplete | None = None,
-        lff: Incomplete | None = None,
-        cfo: Incomplete | None = None,
-        cfe: Incomplete | None = None,
-        cff: Incomplete | None = None,
-        rfo: Incomplete | None = None,
-        rfe: Incomplete | None = None,
-        rff: Incomplete | None = None,
+        readOnlyRecommended: _ConvertibleToBool | None = None,
+        userName: str | None = None,
+        reservationPassword: Incomplete | None = None,
+        algorithmName: str | None = None,
+        hashValue: Incomplete | None = None,
+        saltValue: Incomplete | None = None,
+        spinCount: _ConvertibleToInt | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/comments/comment_sheet.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/pie_chart.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,86 @@
-from _typeshed import Incomplete
-from collections.abc import Generator
+from _typeshed import Incomplete, Unused
+from abc import abstractmethod
+from typing_extensions import Literal
 
+from openpyxl.chart.axis import ChartLines
+from openpyxl.chart.label import DataLabelList
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class Properties(Serialisable):
-    locked: Incomplete
-    defaultSize: Incomplete
-    disabled: Incomplete
-    uiObject: Incomplete
-    autoFill: Incomplete
-    autoLine: Incomplete
-    altText: Incomplete
-    textHAlign: Incomplete
-    textVAlign: Incomplete
-    lockText: Incomplete
-    justLastX: Incomplete
-    autoScale: Incomplete
-    rowHidden: Incomplete
-    colHidden: Incomplete
+from ._chart import ChartBase
+
+class _PieChartBase(ChartBase):
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
     __elements__: Incomplete
-    anchor: Incomplete
-    def __init__(
-        self,
-        locked: Incomplete | None = None,
-        defaultSize: Incomplete | None = None,
-        _print: Incomplete | None = None,
-        disabled: Incomplete | None = None,
-        uiObject: Incomplete | None = None,
-        autoFill: Incomplete | None = None,
-        autoLine: Incomplete | None = None,
-        altText: Incomplete | None = None,
-        textHAlign: Incomplete | None = None,
-        textVAlign: Incomplete | None = None,
-        lockText: Incomplete | None = None,
-        justLastX: Incomplete | None = None,
-        autoScale: Incomplete | None = None,
-        rowHidden: Incomplete | None = None,
-        colHidden: Incomplete | None = None,
-        anchor: Incomplete | None = None,
-    ) -> None: ...
+    def __init__(self, varyColors: bool = True, ser=(), dLbls: DataLabelList | None = None) -> None: ...
+    @property
+    @abstractmethod
+    def tagname(self) -> str: ...
 
-class CommentRecord(Serialisable):
+class PieChart(_PieChartBase):
     tagname: str
-    ref: Incomplete
-    authorId: Incomplete
-    guid: Incomplete
-    shapeId: Incomplete
-    text: Incomplete
-    commentPr: Incomplete
-    author: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
-    height: Incomplete
-    width: Incomplete
-    def __init__(
-        self,
-        ref: str = "",
-        authorId: int = 0,
-        guid: Incomplete | None = None,
-        shapeId: int = 0,
-        text: Incomplete | None = None,
-        commentPr: Incomplete | None = None,
-        author: Incomplete | None = None,
-        height: int = 79,
-        width: int = 144,
-    ) -> None: ...
-    @classmethod
-    def from_cell(cls, cell): ...
-    @property
-    def content(self): ...
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    firstSliceAng: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, firstSliceAng: int = 0, extLst: Unused = None, **kw) -> None: ...
+
+class PieChart3D(_PieChartBase):
+    tagname: str
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+
+class DoughnutChart(_PieChartBase):
+    tagname: str
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    firstSliceAng: Incomplete
+    holeSize: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, firstSliceAng: int = 0, holeSize: int = 10, extLst: Unused = None, **kw) -> None: ...
 
-class CommentSheet(Serialisable):
+class CustomSplit(Serialisable):
     tagname: str
-    authors: Incomplete
-    commentList: Incomplete
-    extLst: Incomplete
-    mime_type: str
+    secondPiePt: Incomplete
+    __elements__: Incomplete
+    def __init__(self, secondPiePt=()) -> None: ...
+
+class ProjectedPieChart(_PieChartBase):
+    tagname: str
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    ofPieType: Incomplete
+    type: Alias
+    gapWidth: Incomplete
+    splitType: Incomplete
+    splitPos: Incomplete
+    custSplit: Typed[CustomSplit, Literal[True]]
+    secondPieSize: Incomplete
+    serLines: Typed[ChartLines, Literal[True]]
+    join_lines: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
-        self, authors: Incomplete | None = None, commentList: Incomplete | None = None, extLst: Incomplete | None = None
+        self,
+        ofPieType: str = "pie",
+        gapWidth: Incomplete | None = None,
+        splitType: str = "auto",
+        splitPos: Incomplete | None = None,
+        custSplit: CustomSplit | None = None,
+        secondPieSize: int = 75,
+        serLines: ChartLines | None = None,
+        extLst: Unused = None,
+        **kw,
     ) -> None: ...
-    def to_tree(self): ...
-    @property
-    def comments(self) -> Generator[Incomplete, None, None]: ...
-    @classmethod
-    def from_comments(cls, comments): ...
-    def write_shapes(self, vml: Incomplete | None = None): ...
-    @property
-    def path(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/descriptors/nested.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/descriptors/nested.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from _typeshed import Incomplete
 
-from .base import Bool, Convertible, Descriptor, Float, Integer, MinMax, NoneSet, Set, String
+from openpyxl.descriptors import Strict
+from openpyxl.descriptors.base import Bool, Convertible, Descriptor, Float, Integer, MinMax, NoneSet, Set, String
+from openpyxl.descriptors.serialisable import Serialisable
 
-class Nested(Descriptor):
+# NOTE: # type: ignore[misc]: Class does not reimplement the relevant methods, so runtime also has incompatible supertypes
+
+class Nested(Descriptor[Incomplete]):
     nested: bool
     attribute: str
-    def __set__(self, instance, value) -> None: ...
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
     def from_tree(self, node): ...
     def to_tree(
         self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
     ): ...
 
-class NestedValue(Nested, Convertible): ...
+class NestedValue(Nested, Convertible[Incomplete, Incomplete]): ...  # type: ignore[misc]
 
 class NestedText(NestedValue):
     def from_tree(self, node): ...
     def to_tree(
         self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
     ): ...
 
-class NestedFloat(NestedValue, Float): ...
-class NestedInteger(NestedValue, Integer): ...
-class NestedString(NestedValue, String): ...
+class NestedFloat(NestedValue, Float[Incomplete]): ...  # type: ignore[misc]
+class NestedInteger(NestedValue, Integer[Incomplete]): ...  # type: ignore[misc]
+class NestedString(NestedValue, String[Incomplete]): ...  # type: ignore[misc]
 
-class NestedBool(NestedValue, Bool):
+class NestedBool(NestedValue, Bool[Incomplete]):  # type: ignore[misc]
     def from_tree(self, node): ...
 
-class NestedNoneSet(Nested, NoneSet): ...
-class NestedSet(Nested, Set): ...
-class NestedMinMax(Nested, MinMax): ...
+class NestedNoneSet(Nested, NoneSet[Incomplete]): ...
+class NestedSet(Nested, Set[Incomplete]): ...
+class NestedMinMax(Nested, MinMax[Incomplete, Incomplete]): ...  # type: ignore[misc]
 
-class EmptyTag(Nested, Bool):
+class EmptyTag(Nested, Bool[Incomplete]):  # type: ignore[misc]
     def from_tree(self, node): ...
     def to_tree(
         self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
     ): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/drawing.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/drawing/drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/graphic.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/series.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,96 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.chart.data_source import AxDataSource, NumDataSource, StrRef
+from openpyxl.chart.error_bar import ErrorBars
+from openpyxl.chart.label import DataLabelList
+from openpyxl.chart.marker import Marker
+from openpyxl.chart.picture import PictureOptions
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.trendline import Trendline
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class GraphicFrameLocking(Serialisable):
-    noGrp: Incomplete
-    noDrilldown: Incomplete
-    noSelect: Incomplete
-    noChangeAspect: Incomplete
-    noMove: Incomplete
-    noResize: Incomplete
-    extLst: Incomplete
-    def __init__(
-        self,
-        noGrp: Incomplete | None = None,
-        noDrilldown: Incomplete | None = None,
-        noSelect: Incomplete | None = None,
-        noChangeAspect: Incomplete | None = None,
-        noMove: Incomplete | None = None,
-        noResize: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-    ) -> None: ...
+attribute_mapping: Incomplete
 
-class NonVisualGraphicFrameProperties(Serialisable):
+class SeriesLabel(Serialisable):
     tagname: str
-    graphicFrameLocks: Incomplete
-    extLst: Incomplete
-    def __init__(self, graphicFrameLocks: Incomplete | None = None, extLst: Incomplete | None = None) -> None: ...
-
-class NonVisualGraphicFrame(Serialisable):
-    tagname: str
-    cNvPr: Incomplete
-    cNvGraphicFramePr: Incomplete
+    strRef: Typed[StrRef, Literal[True]]
+    v: Incomplete
+    value: Alias
     __elements__: Incomplete
-    def __init__(self, cNvPr: Incomplete | None = None, cNvGraphicFramePr: Incomplete | None = None) -> None: ...
-
-class GraphicData(Serialisable):
-    tagname: str
-    namespace: Incomplete
-    uri: Incomplete
-    chart: Incomplete
-    def __init__(self, uri: str = ..., chart: Incomplete | None = None) -> None: ...
-
-class GraphicObject(Serialisable):
-    tagname: str
-    namespace: Incomplete
-    graphicData: Incomplete
-    def __init__(self, graphicData: Incomplete | None = None) -> None: ...
+    def __init__(self, strRef: StrRef | None = None, v: Incomplete | None = None) -> None: ...
 
-class GraphicFrame(Serialisable):
+class Series(Serialisable):
     tagname: str
-    nvGraphicFramePr: Incomplete
-    xfrm: Incomplete
-    graphic: Incomplete
-    macro: Incomplete
-    fPublished: Incomplete
+    idx: Incomplete
+    order: Incomplete
+    tx: Typed[SeriesLabel, Literal[True]]
+    title: Alias
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Incomplete
+    pictureOptions: Typed[PictureOptions, Literal[True]]
+    dPt: Incomplete
+    data_points: Alias
+    dLbls: Typed[DataLabelList, Literal[True]]
+    labels: Alias
+    trendline: Typed[Trendline, Literal[True]]
+    errBars: Typed[ErrorBars, Literal[True]]
+    cat: Typed[AxDataSource, Literal[True]]
+    identifiers: Alias
+    val: Typed[NumDataSource, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    invertIfNegative: Incomplete
+    shape: Incomplete
+    xVal: Typed[AxDataSource, Literal[True]]
+    yVal: Typed[NumDataSource, Literal[True]]
+    bubbleSize: Typed[NumDataSource, Literal[True]]
+    zVal: Alias
+    bubble3D: Incomplete
+    marker: Typed[Marker, Literal[True]]
+    smooth: Incomplete
+    explosion: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        nvGraphicFramePr: Incomplete | None = None,
-        xfrm: Incomplete | None = None,
-        graphic: Incomplete | None = None,
-        macro: Incomplete | None = None,
-        fPublished: Incomplete | None = None,
+        idx: int = 0,
+        order: int = 0,
+        tx: SeriesLabel | None = None,
+        spPr: GraphicalProperties | None = None,
+        pictureOptions: PictureOptions | None = None,
+        dPt=(),
+        dLbls: DataLabelList | None = None,
+        trendline: Trendline | None = None,
+        errBars: ErrorBars | None = None,
+        cat: AxDataSource | None = None,
+        val: NumDataSource | None = None,
+        invertIfNegative: Incomplete | None = None,
+        shape: Incomplete | None = None,
+        xVal: AxDataSource | None = None,
+        yVal: NumDataSource | None = None,
+        bubbleSize: NumDataSource | None = None,
+        bubble3D: Incomplete | None = None,
+        marker: Marker | None = None,
+        smooth: Incomplete | None = None,
+        explosion: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
 
-class GroupShape(Serialisable):
-    nvGrpSpPr: Incomplete
-    nonVisualProperties: Incomplete
-    grpSpPr: Incomplete
-    visualProperties: Incomplete
-    pic: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self, nvGrpSpPr: Incomplete | None = None, grpSpPr: Incomplete | None = None, pic: Incomplete | None = None
-    ) -> None: ...
+class XYSeries(Series):
+    idx: Incomplete
+    order: Incomplete
+    tx: Incomplete
+    spPr: Incomplete
+    dPt: Incomplete
+    dLbls: Incomplete
+    trendline: Incomplete
+    errBars: Incomplete
+    xVal: Incomplete
+    yVal: Incomplete
+    invertIfNegative: Incomplete
+    bubbleSize: Incomplete
+    bubble3D: Incomplete
+    marker: Incomplete
+    smooth: Incomplete
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/line.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/external_link/external.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,81 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal, TypeAlias
 
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.packaging.relationship import Relationship
 
-class LineEndProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
-    type: Incomplete
-    w: Incomplete
-    len: Incomplete
-    def __init__(self, type: Incomplete | None = None, w: Incomplete | None = None, len: Incomplete | None = None) -> None: ...
+_ExternalCellType: TypeAlias = Literal["b", "d", "n", "e", "s", "str", "inlineStr"]
+
+class ExternalCell(Serialisable):
+    r: String[Literal[False]]
+    t: NoneSet[_ExternalCellType]
+    vm: Integer[Literal[True]]
+    v: Incomplete
+    def __init__(
+        self,
+        r: str,
+        t: _ExternalCellType | Literal["none"] | None = None,
+        vm: _ConvertibleToInt | None = None,
+        v: Incomplete | None = None,
+    ) -> None: ...
 
-class DashStop(Serialisable):
+class ExternalRow(Serialisable):
+    r: Integer[Literal[False]]
+    cell: Incomplete
+    __elements__: Incomplete
+    def __init__(self, r: _ConvertibleToInt, cell: Incomplete | None = None) -> None: ...
+
+class ExternalSheetData(Serialisable):
+    sheetId: Integer[Literal[False]]
+    refreshError: Bool[Literal[True]]
+    row: Incomplete
+    __elements__: Incomplete
+    def __init__(self, sheetId: _ConvertibleToInt, refreshError: _ConvertibleToBool | None = None, row=()) -> None: ...
+
+class ExternalSheetDataSet(Serialisable):
+    sheetData: Incomplete
+    __elements__: Incomplete
+    def __init__(self, sheetData: Incomplete | None = None) -> None: ...
+
+class ExternalSheetNames(Serialisable):
+    sheetName: Incomplete
+    __elements__: Incomplete
+    def __init__(self, sheetName=()) -> None: ...
+
+class ExternalDefinedName(Serialisable):
     tagname: str
-    namespace: Incomplete
-    d: Incomplete
-    length: Incomplete
-    sp: Incomplete
-    space: Incomplete
-    def __init__(self, d: int = 0, sp: int = 0) -> None: ...
-
-class DashStopList(Serialisable):
-    ds: Incomplete
-    def __init__(self, ds: Incomplete | None = None) -> None: ...
+    name: String[Literal[False]]
+    refersTo: String[Literal[True]]
+    sheetId: Integer[Literal[True]]
+    def __init__(self, name: str, refersTo: str | None = None, sheetId: _ConvertibleToInt | None = None) -> None: ...
 
-class LineProperties(Serialisable):
+class ExternalBook(Serialisable):
     tagname: str
-    namespace: Incomplete
-    w: Incomplete
-    width: Incomplete
-    cap: Incomplete
-    cmpd: Incomplete
-    algn: Incomplete
-    noFill: Incomplete
-    solidFill: Incomplete
-    gradFill: Incomplete
-    pattFill: Incomplete
-    prstDash: Incomplete
-    dashStyle: Incomplete
-    custDash: Incomplete
-    round: Incomplete
-    bevel: Incomplete
-    miter: Incomplete
-    headEnd: Incomplete
-    tailEnd: Incomplete
-    extLst: Incomplete
+    sheetNames: Typed[ExternalSheetNames, Literal[True]]
+    definedNames: Incomplete
+    sheetDataSet: Typed[ExternalSheetDataSet, Literal[True]]
+    id: Incomplete
     __elements__: Incomplete
     def __init__(
         self,
-        w: Incomplete | None = None,
-        cap: Incomplete | None = None,
-        cmpd: Incomplete | None = None,
-        algn: Incomplete | None = None,
-        noFill: Incomplete | None = None,
-        solidFill: Incomplete | None = None,
-        gradFill: Incomplete | None = None,
-        pattFill: Incomplete | None = None,
-        prstDash: Incomplete | None = None,
-        custDash: Incomplete | None = None,
-        round: Incomplete | None = None,
-        bevel: Incomplete | None = None,
-        miter: Incomplete | None = None,
-        headEnd: Incomplete | None = None,
-        tailEnd: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        sheetNames: ExternalSheetNames | None = None,
+        definedNames=(),
+        sheetDataSet: ExternalSheetDataSet | None = None,
+        id: Incomplete | None = None,
     ) -> None: ...
+
+class ExternalLink(Serialisable):
+    tagname: str
+    mime_type: str
+    externalBook: Typed[ExternalBook, Literal[True]]
+    file_link: Typed[Relationship, Literal[True]]
+    __elements__: Incomplete
+    def __init__(
+        self, externalBook: ExternalBook | None = None, ddeLink: Unused = None, oleLink: Unused = None, extLst: Unused = None
+    ) -> None: ...
+    def to_tree(self): ...
+    @property
+    def path(self): ...
+
+def read_external_link(archive, book_path): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/drawing/properties.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/_3d.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,63 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.chart.picture import PictureOptions
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class GroupShapeProperties(Serialisable):
+class View3D(Serialisable):
     tagname: str
-    bwMode: Incomplete
-    xfrm: Incomplete
-    scene3d: Incomplete
-    extLst: Incomplete
-    def __init__(
-        self,
-        bwMode: Incomplete | None = None,
-        xfrm: Incomplete | None = None,
-        scene3d: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-    ) -> None: ...
-
-class GroupLocking(Serialisable):
-    tagname: str
-    namespace: Incomplete
-    noGrp: Incomplete
-    noUngrp: Incomplete
-    noSelect: Incomplete
-    noRot: Incomplete
-    noChangeAspect: Incomplete
-    noMove: Incomplete
-    noResize: Incomplete
-    noChangeArrowheads: Incomplete
-    noEditPoints: Incomplete
-    noAdjustHandles: Incomplete
-    noChangeShapeType: Incomplete
-    extLst: Incomplete
+    rotX: Incomplete
+    x_rotation: Alias
+    hPercent: Incomplete
+    height_percent: Alias
+    rotY: Incomplete
+    y_rotation: Alias
+    depthPercent: Incomplete
+    rAngAx: Incomplete
+    right_angle_axes: Alias
+    perspective: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        noGrp: Incomplete | None = None,
-        noUngrp: Incomplete | None = None,
-        noSelect: Incomplete | None = None,
-        noRot: Incomplete | None = None,
-        noChangeAspect: Incomplete | None = None,
-        noChangeArrowheads: Incomplete | None = None,
-        noMove: Incomplete | None = None,
-        noResize: Incomplete | None = None,
-        noEditPoints: Incomplete | None = None,
-        noAdjustHandles: Incomplete | None = None,
-        noChangeShapeType: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        rotX: int = 15,
+        hPercent: Incomplete | None = None,
+        rotY: int = 20,
+        depthPercent: Incomplete | None = None,
+        rAngAx: bool = True,
+        perspective: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
-class NonVisualGroupDrawingShapeProps(Serialisable):
+class Surface(Serialisable):
     tagname: str
-    grpSpLocks: Incomplete
-    extLst: Incomplete
+    thickness: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    pictureOptions: Typed[PictureOptions, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(self, grpSpLocks: Incomplete | None = None, extLst: Incomplete | None = None) -> None: ...
-
-class NonVisualDrawingShapeProps(Serialisable):
-    tagname: str
-    spLocks: Incomplete
-    txBax: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    txBox: Incomplete
     def __init__(
-        self, spLocks: Incomplete | None = None, txBox: Incomplete | None = None, extLst: Incomplete | None = None
+        self,
+        thickness: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        pictureOptions: PictureOptions | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
-class NonVisualDrawingProps(Serialisable):
+class _3DBase(Serialisable):
     tagname: str
-    id: Incomplete
-    name: Incomplete
-    descr: Incomplete
-    hidden: Incomplete
-    title: Incomplete
-    hlinkClick: Incomplete
-    hlinkHover: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
+    view3D: Typed[View3D, Literal[True]]
+    floor: Typed[Surface, Literal[True]]
+    sideWall: Typed[Surface, Literal[True]]
+    backWall: Typed[Surface, Literal[True]]
     def __init__(
         self,
-        id: Incomplete | None = None,
-        name: Incomplete | None = None,
-        descr: Incomplete | None = None,
-        hidden: Incomplete | None = None,
-        title: Incomplete | None = None,
-        hlinkClick: Incomplete | None = None,
-        hlinkHover: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        view3D: View3D | None = None,
+        floor: Surface | None = None,
+        sideWall: Surface | None = None,
+        backWall: Surface | None = None,
     ) -> None: ...
-
-class NonVisualGroupShape(Serialisable):
-    tagname: str
-    cNvPr: Incomplete
-    cNvGrpSpPr: Incomplete
-    __elements__: Incomplete
-    def __init__(self, cNvPr: Incomplete | None = None, cNvGrpSpPr: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/formatting/formatting.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/formatting/formatting.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Alias, Bool, Convertible, _ConvertibleToBool, _ConvertibleToMultiCellRange
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.worksheet.cell_range import MultiCellRange
 
 class ConditionalFormatting(Serialisable):
     tagname: str
-    sqref: Incomplete
-    cells: Incomplete
-    pivot: Incomplete
+    sqref: Convertible[MultiCellRange, Literal[False]]
+    cells: Alias
+    pivot: Bool[Literal[True]]
     cfRule: Incomplete
-    rules: Incomplete
-    def __init__(self, sqref=(), pivot: Incomplete | None = None, cfRule=(), extLst: Incomplete | None = None) -> None: ...
+    rules: Alias
+    def __init__(
+        self, sqref: _ConvertibleToMultiCellRange = (), pivot: _ConvertibleToBool | None = None, cfRule=(), extLst: Unused = None
+    ) -> None: ...
     def __eq__(self, other): ...
     def __hash__(self) -> int: ...
     def __contains__(self, coord): ...
 
 class ConditionalFormattingList:
     max_priority: int
     def __init__(self) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/formatting/rule.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/workbook.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,102 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors import Float
+from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.workbook.defined_name import DefinedNameList
+from openpyxl.workbook.function_group import FunctionGroupList
+from openpyxl.workbook.properties import CalcProperties, FileVersion, WorkbookProperties
+from openpyxl.workbook.protection import FileSharing, WorkbookProtection
+from openpyxl.workbook.smart_tags import SmartTagList, SmartTagProperties
+from openpyxl.workbook.web import WebPublishing, WebPublishObjectList
 
-class ValueDescriptor(Float):
-    expected_type: Incomplete
-    def __set__(self, instance, value) -> None: ...
+_ChildSheetState: TypeAlias = Literal["visible", "hidden", "veryHidden"]
+_WorkbookPackageConformance: TypeAlias = Literal["strict", "transitional"]
 
-class FormatObject(Serialisable):
+class FileRecoveryProperties(Serialisable):
     tagname: str
-    type: Incomplete
-    val: Incomplete
-    gte: Incomplete
-    extLst: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self, type, val: Incomplete | None = None, gte: Incomplete | None = None, extLst: Incomplete | None = None
-    ) -> None: ...
-
-class RuleType(Serialisable):  # type: ignore[misc]
-    cfvo: Incomplete
-
-class IconSet(RuleType):
-    tagname: str
-    iconSet: Incomplete
-    showValue: Incomplete
-    percent: Incomplete
-    reverse: Incomplete
-    __elements__: Incomplete
-    cfvo: Incomplete
+    autoRecover: Bool[Literal[True]]
+    crashSave: Bool[Literal[True]]
+    dataExtractLoad: Bool[Literal[True]]
+    repairLoad: Bool[Literal[True]]
     def __init__(
         self,
-        iconSet: Incomplete | None = None,
-        showValue: Incomplete | None = None,
-        percent: Incomplete | None = None,
-        reverse: Incomplete | None = None,
-        cfvo: Incomplete | None = None,
+        autoRecover: _ConvertibleToBool | None = None,
+        crashSave: _ConvertibleToBool | None = None,
+        dataExtractLoad: _ConvertibleToBool | None = None,
+        repairLoad: _ConvertibleToBool | None = None,
     ) -> None: ...
 
-class DataBar(RuleType):
+class ChildSheet(Serialisable):
     tagname: str
-    minLength: Incomplete
-    maxLength: Incomplete
-    showValue: Incomplete
-    color: Incomplete
-    __elements__: Incomplete
-    cfvo: Incomplete
+    name: String[Literal[False]]
+    sheetId: Integer[Literal[False]]
+    state: NoneSet[_ChildSheetState]
+    id: Incomplete
     def __init__(
         self,
-        minLength: Incomplete | None = None,
-        maxLength: Incomplete | None = None,
-        showValue: Incomplete | None = None,
-        cfvo: Incomplete | None = None,
-        color: Incomplete | None = None,
+        name: str,
+        sheetId: _ConvertibleToInt,
+        state: _ChildSheetState | Literal["none"] | None = "visible",
+        id: Incomplete | None = None,
     ) -> None: ...
 
-class ColorScale(RuleType):
+class PivotCache(Serialisable):
     tagname: str
-    color: Incomplete
-    __elements__: Incomplete
-    cfvo: Incomplete
-    def __init__(self, cfvo: Incomplete | None = None, color: Incomplete | None = None) -> None: ...
+    cacheId: Integer[Literal[False]]
+    id: Incomplete
+    def __init__(self, cacheId: _ConvertibleToInt, id: Incomplete | None = None) -> None: ...
 
-class Rule(Serialisable):
+class WorkbookPackage(Serialisable):
     tagname: str
-    type: Incomplete
-    dxfId: Incomplete
-    priority: Incomplete
-    stopIfTrue: Incomplete
-    aboveAverage: Incomplete
-    percent: Incomplete
-    bottom: Incomplete
-    operator: Incomplete
-    text: Incomplete
-    timePeriod: Incomplete
-    rank: Incomplete
-    stdDev: Incomplete
-    equalAverage: Incomplete
-    formula: Incomplete
-    colorScale: Incomplete
-    dataBar: Incomplete
-    iconSet: Incomplete
-    extLst: Incomplete
-    dxf: Incomplete
+    conformance: NoneSet[_WorkbookPackageConformance]
+    fileVersion: Typed[FileVersion, Literal[True]]
+    fileSharing: Typed[FileSharing, Literal[True]]
+    workbookPr: Typed[WorkbookProperties, Literal[True]]
+    properties: Alias
+    workbookProtection: Typed[WorkbookProtection, Literal[True]]
+    bookViews: Incomplete
+    sheets: Incomplete
+    functionGroups: Typed[FunctionGroupList, Literal[True]]
+    externalReferences: Incomplete
+    definedNames: Typed[DefinedNameList, Literal[True]]
+    calcPr: Typed[CalcProperties, Literal[True]]
+    oleSize: Incomplete
+    customWorkbookViews: Incomplete
+    pivotCaches: Incomplete
+    smartTagPr: Typed[SmartTagProperties, Literal[True]]
+    smartTagTypes: Typed[SmartTagList, Literal[True]]
+    webPublishing: Typed[WebPublishing, Literal[True]]
+    fileRecoveryPr: Typed[FileRecoveryProperties, Literal[True]]
+    webPublishObjects: Typed[WebPublishObjectList, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    Ignorable: Incomplete
     __elements__: Incomplete
-    __attrs__: Incomplete
     def __init__(
         self,
-        type,
-        dxfId: Incomplete | None = None,
-        priority: int = 0,
-        stopIfTrue: Incomplete | None = None,
-        aboveAverage: Incomplete | None = None,
-        percent: Incomplete | None = None,
-        bottom: Incomplete | None = None,
-        operator: Incomplete | None = None,
-        text: Incomplete | None = None,
-        timePeriod: Incomplete | None = None,
-        rank: Incomplete | None = None,
-        stdDev: Incomplete | None = None,
-        equalAverage: Incomplete | None = None,
-        formula=(),
-        colorScale: Incomplete | None = None,
-        dataBar: Incomplete | None = None,
-        iconSet: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-        dxf: Incomplete | None = None,
+        conformance: _WorkbookPackageConformance | Literal["none"] | None = None,
+        fileVersion: FileVersion | None = None,
+        fileSharing: FileSharing | None = None,
+        workbookPr: WorkbookProperties | None = None,
+        workbookProtection: WorkbookProtection | None = None,
+        bookViews=(),
+        sheets=(),
+        functionGroups: FunctionGroupList | None = None,
+        externalReferences=(),
+        definedNames: DefinedNameList | None = None,
+        calcPr: CalcProperties | None = None,
+        oleSize: Incomplete | None = None,
+        customWorkbookViews=(),
+        pivotCaches=(),
+        smartTagPr: SmartTagProperties | None = None,
+        smartTagTypes: SmartTagList | None = None,
+        webPublishing: WebPublishing | None = None,
+        fileRecoveryPr: FileRecoveryProperties | None = None,
+        webPublishObjects: WebPublishObjectList | None = None,
+        extLst: Unused = None,
+        Ignorable: Unused = None,
     ) -> None: ...
-
-def ColorScaleRule(
-    start_type: Incomplete | None = None,
-    start_value: Incomplete | None = None,
-    start_color: Incomplete | None = None,
-    mid_type: Incomplete | None = None,
-    mid_value: Incomplete | None = None,
-    mid_color: Incomplete | None = None,
-    end_type: Incomplete | None = None,
-    end_value: Incomplete | None = None,
-    end_color: Incomplete | None = None,
-): ...
-def FormulaRule(
-    formula: Incomplete | None = None,
-    stopIfTrue: Incomplete | None = None,
-    font: Incomplete | None = None,
-    border: Incomplete | None = None,
-    fill: Incomplete | None = None,
-): ...
-def CellIsRule(
-    operator: Incomplete | None = None,
-    formula: Incomplete | None = None,
-    stopIfTrue: Incomplete | None = None,
-    font: Incomplete | None = None,
-    border: Incomplete | None = None,
-    fill: Incomplete | None = None,
-): ...
-def IconSetRule(
-    icon_style: Incomplete | None = None,
-    type: Incomplete | None = None,
-    values: Incomplete | None = None,
-    showValue: Incomplete | None = None,
-    percent: Incomplete | None = None,
-    reverse: Incomplete | None = None,
-): ...
-def DataBarRule(
-    start_type: Incomplete | None = None,
-    start_value: Incomplete | None = None,
-    end_type: Incomplete | None = None,
-    end_value: Incomplete | None = None,
-    color: Incomplete | None = None,
-    showValue: Incomplete | None = None,
-    minLength: Incomplete | None = None,
-    maxLength: Incomplete | None = None,
-): ...
+    def to_tree(self): ...
+    @property
+    def active(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/formula/tokenizer.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/formula/tokenizer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/formula/translate.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/formula/translate.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/packaging/core.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/legend.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,42 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
-from openpyxl.descriptors import DateTime
-from openpyxl.descriptors.nested import NestedText
+from openpyxl.chart.layout import Layout
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class NestedDateTime(DateTime, NestedText):
-    expected_type: Incomplete
-    def to_tree(
-        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
-    ): ...
-
-class QualifiedDateTime(NestedDateTime):
-    def to_tree(
-        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
-    ): ...
+class LegendEntry(Serialisable):
+    tagname: str
+    idx: Incomplete
+    delete: Incomplete
+    txPr: Typed[RichText, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, idx: int = 0, delete: bool = False, txPr: RichText | None = None, extLst: Unused = None) -> None: ...
 
-class DocumentProperties(Serialisable):
+class Legend(Serialisable):
     tagname: str
-    namespace: Incomplete
-    category: Incomplete
-    contentStatus: Incomplete
-    keywords: Incomplete
-    lastModifiedBy: Incomplete
-    lastPrinted: Incomplete
-    revision: Incomplete
-    version: Incomplete
-    last_modified_by: Incomplete
-    subject: Incomplete
-    title: Incomplete
-    creator: Incomplete
-    description: Incomplete
-    identifier: Incomplete
-    language: Incomplete
-    created: Incomplete
-    modified: Incomplete
+    legendPos: Incomplete
+    position: Alias
+    legendEntry: Incomplete
+    layout: Typed[Layout, Literal[True]]
+    overlay: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    textProperties: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        category: Incomplete | None = None,
-        contentStatus: Incomplete | None = None,
-        keywords: Incomplete | None = None,
-        lastModifiedBy: Incomplete | None = None,
-        lastPrinted: Incomplete | None = None,
-        revision: Incomplete | None = None,
-        version: Incomplete | None = None,
-        created=None,
-        creator: str = "openpyxl",
-        description: Incomplete | None = None,
-        identifier: Incomplete | None = None,
-        language: Incomplete | None = None,
-        modified=None,
-        subject: Incomplete | None = None,
-        title: Incomplete | None = None,
+        legendPos: str = "r",
+        legendEntry=(),
+        layout: Layout | None = None,
+        overlay: Incomplete | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/pivot/fields.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/data_source.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,115 @@
-from _typeshed import Incomplete
-
+from _typeshed import Incomplete, Unused
+from typing import NoReturn, overload
+from typing_extensions import Literal
+
+from openpyxl.descriptors import Strict
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 
-class Index(Serialisable):
-    tagname: str
-    v: Incomplete
-    def __init__(self, v: int = 0) -> None: ...
+class NumFmt(Serialisable):
+    formatCode: String[Literal[False]]
+    sourceLinked: Bool[Literal[False]]
+    def __init__(self, formatCode: str, sourceLinked: _ConvertibleToBool = False) -> None: ...
 
-class Tuple(Serialisable):  # type: ignore[misc]
-    fld: Incomplete
-    hier: Incomplete
-    item: Incomplete
-    def __init__(self, fld: Incomplete | None = None, hier: Incomplete | None = None, item: Incomplete | None = None) -> None: ...
+class NumberValueDescriptor(NestedText):
+    allow_none: bool
+    expected_type: type[Incomplete]
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...  # type: ignore[override]
 
-class TupleList(Serialisable):  # type: ignore[misc]
-    c: Incomplete
-    tpl: Incomplete
-    __elements__: Incomplete
-    def __init__(self, c: Incomplete | None = None, tpl: Incomplete | None = None) -> None: ...
+class NumVal(Serialisable):
+    idx: Integer[Literal[False]]
+    formatCode: Incomplete
+    v: Incomplete
+    def __init__(self, idx: _ConvertibleToInt, formatCode: Incomplete | None = None, v: Incomplete | None = None) -> None: ...
 
-class Missing(Serialisable):
-    tagname: str
-    tpls: Incomplete
-    x: Incomplete
-    u: Incomplete
-    f: Incomplete
-    c: Incomplete
-    cp: Incomplete
-    bc: Incomplete
-    fc: Incomplete
-    i: Incomplete
-    un: Incomplete
-    st: Incomplete
-    b: Incomplete
+class NumData(Serialisable):
+    formatCode: Incomplete
+    ptCount: Incomplete
+    pt: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
-        self,
-        tpls=(),
-        x=(),
-        u: Incomplete | None = None,
-        f: Incomplete | None = None,
-        c: Incomplete | None = None,
-        cp: Incomplete | None = None,
-        _in: Incomplete | None = None,
-        bc: Incomplete | None = None,
-        fc: Incomplete | None = None,
-        i: Incomplete | None = None,
-        un: Incomplete | None = None,
-        st: Incomplete | None = None,
-        b: Incomplete | None = None,
+        self, formatCode: Incomplete | None = None, ptCount: Incomplete | None = None, pt=(), extLst: Unused = None
     ) -> None: ...
 
-class Number(Serialisable):
-    tagname: str
-    tpls: Incomplete
-    x: Incomplete
-    v: Incomplete
-    u: Incomplete
+class NumRef(Serialisable):
     f: Incomplete
-    c: Incomplete
-    cp: Incomplete
-    bc: Incomplete
-    fc: Incomplete
-    i: Incomplete
-    un: Incomplete
-    st: Incomplete
-    b: Incomplete
+    ref: Alias
+    numCache: Typed[NumData, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(
-        self,
-        tpls=(),
-        x=(),
-        v: Incomplete | None = None,
-        u: Incomplete | None = None,
-        f: Incomplete | None = None,
-        c: Incomplete | None = None,
-        cp: Incomplete | None = None,
-        _in: Incomplete | None = None,
-        bc: Incomplete | None = None,
-        fc: Incomplete | None = None,
-        i: Incomplete | None = None,
-        un: Incomplete | None = None,
-        st: Incomplete | None = None,
-        b: Incomplete | None = None,
-    ) -> None: ...
+    def __init__(self, f: Incomplete | None = None, numCache: NumData | None = None, extLst: Unused = None) -> None: ...
 
-class Error(Serialisable):
+class StrVal(Serialisable):
     tagname: str
-    tpls: Incomplete
-    x: Incomplete
+    idx: Integer[Literal[False]]
     v: Incomplete
-    u: Incomplete
-    f: Incomplete
-    c: Incomplete
-    cp: Incomplete
-    bc: Incomplete
-    fc: Incomplete
-    i: Incomplete
-    un: Incomplete
-    st: Incomplete
-    b: Incomplete
+    def __init__(self, idx: _ConvertibleToInt = 0, v: Incomplete | None = None) -> None: ...
+
+class StrData(Serialisable):
+    tagname: str
+    ptCount: Incomplete
+    pt: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(
-        self,
-        tpls: Incomplete | None = None,
-        x=(),
-        v: Incomplete | None = None,
-        u: Incomplete | None = None,
-        f: Incomplete | None = None,
-        c: Incomplete | None = None,
-        cp: Incomplete | None = None,
-        _in: Incomplete | None = None,
-        bc: Incomplete | None = None,
-        fc: Incomplete | None = None,
-        i: Incomplete | None = None,
-        un: Incomplete | None = None,
-        st: Incomplete | None = None,
-        b: Incomplete | None = None,
-    ) -> None: ...
+    def __init__(self, ptCount: Incomplete | None = None, pt=(), extLst: Unused = None) -> None: ...
 
-class Boolean(Serialisable):
+class StrRef(Serialisable):
     tagname: str
-    x: Incomplete
-    v: Incomplete
-    u: Incomplete
     f: Incomplete
-    c: Incomplete
-    cp: Incomplete
+    strCache: Typed[StrData, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(
-        self,
-        x=(),
-        v: Incomplete | None = None,
-        u: Incomplete | None = None,
-        f: Incomplete | None = None,
-        c: Incomplete | None = None,
-        cp: Incomplete | None = None,
-    ) -> None: ...
+    def __init__(self, f: Incomplete | None = None, strCache: StrData | None = None, extLst: Unused = None) -> None: ...
 
-class Text(Serialisable):
+class NumDataSource(Serialisable):
+    numRef: Typed[NumRef, Literal[True]]
+    numLit: Typed[NumData, Literal[True]]
+    def __init__(self, numRef: NumRef | None = None, numLit: NumData | None = None) -> None: ...
+
+class Level(Serialisable):
+    tagname: str
+    pt: Incomplete
+    __elements__: Incomplete
+    def __init__(self, pt=()) -> None: ...
+
+class MultiLevelStrData(Serialisable):
+    tagname: str
+    ptCount: Integer[Literal[True]]
+    lvl: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, ptCount: _ConvertibleToInt | None = None, lvl=(), extLst: Unused = None) -> None: ...
+
+class MultiLevelStrRef(Serialisable):
     tagname: str
-    tpls: Incomplete
-    x: Incomplete
-    v: Incomplete
-    u: Incomplete
     f: Incomplete
-    c: Incomplete
-    cp: Incomplete
-    bc: Incomplete
-    fc: Incomplete
-    i: Incomplete
-    un: Incomplete
-    st: Incomplete
-    b: Incomplete
+    multiLvlStrCache: Typed[MultiLevelStrData, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
-        self,
-        tpls=(),
-        x=(),
-        v: Incomplete | None = None,
-        u: Incomplete | None = None,
-        f: Incomplete | None = None,
-        c: Incomplete | None = None,
-        cp: Incomplete | None = None,
-        _in: Incomplete | None = None,
-        bc: Incomplete | None = None,
-        fc: Incomplete | None = None,
-        i: Incomplete | None = None,
-        un: Incomplete | None = None,
-        st: Incomplete | None = None,
-        b: Incomplete | None = None,
+        self, f: Incomplete | None = None, multiLvlStrCache: MultiLevelStrData | None = None, extLst: Unused = None
     ) -> None: ...
 
-class DateTimeField(Serialisable):
+class AxDataSource(Serialisable):
     tagname: str
-    x: Incomplete
-    v: Incomplete
-    u: Incomplete
-    f: Incomplete
-    c: Incomplete
-    cp: Incomplete
-    __elements__: Incomplete
+    numRef: Typed[NumRef, Literal[True]]
+    numLit: Typed[NumData, Literal[True]]
+    strRef: Typed[StrRef, Literal[True]]
+    strLit: Typed[StrData, Literal[True]]
+    multiLvlStrRef: Typed[MultiLevelStrRef, Literal[True]]
+    @overload
+    def __init__(
+        self, numRef: None = None, numLit: None = None, strRef: None = None, strLit: None = None, multiLvlStrRef: None = None
+    ) -> NoReturn: ...
+    @overload
     def __init__(
         self,
-        x=(),
-        v: Incomplete | None = None,
-        u: Incomplete | None = None,
-        f: Incomplete | None = None,
-        c: Incomplete | None = None,
-        cp: Incomplete | None = None,
+        numRef: NumRef | None = None,
+        numLit: NumData | None = None,
+        strRef: StrRef | None = None,
+        strLit: StrData | None = None,
+        multiLvlStrRef: MultiLevelStrRef | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/reader/excel.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/reader/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/reader/workbook.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/reader/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/__init__.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/styles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/builtins.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/styles/builtins.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/differential.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/text.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal
 
+from openpyxl.chart.data_source import StrRef
+from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.text import ListStyle, RichTextProperties
 
-class DifferentialStyle(Serialisable):
+class RichText(Serialisable):
     tagname: str
+    bodyPr: Typed[RichTextProperties, Literal[False]]
+    properties: Alias
+    lstStyle: Typed[ListStyle, Literal[True]]
+    p: Incomplete
+    paragraphs: Alias
     __elements__: Incomplete
-    font: Incomplete
-    numFmt: Incomplete
-    fill: Incomplete
-    alignment: Incomplete
-    border: Incomplete
-    protection: Incomplete
-    extLst: Incomplete
     def __init__(
-        self,
-        font: Incomplete | None = None,
-        numFmt: Incomplete | None = None,
-        fill: Incomplete | None = None,
-        alignment: Incomplete | None = None,
-        border: Incomplete | None = None,
-        protection: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        self, bodyPr: RichTextProperties | None = None, lstStyle: ListStyle | None = None, p: Incomplete | None = None
     ) -> None: ...
 
-class DifferentialStyleList(Serialisable):
+class Text(Serialisable):
     tagname: str
-    dxf: Incomplete
-    styles: Incomplete
-    __attrs__: Incomplete
-    def __init__(self, dxf=(), count: Incomplete | None = None) -> None: ...
-    def append(self, dxf) -> None: ...
-    def add(self, dxf): ...
-    def __bool__(self) -> bool: ...
-    def __getitem__(self, idx): ...
-    @property
-    def count(self): ...
+    strRef: Typed[StrRef, Literal[True]]
+    rich: Typed[RichText, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, strRef: StrRef | None = None, rich: RichText | None = None) -> None: ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/fills.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/surface_chart.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,57 @@
 from _typeshed import Incomplete
+from abc import abstractmethod
+from typing_extensions import Literal
 
-from openpyxl.descriptors import Sequence
+from openpyxl.chart.axis import NumericAxis, SeriesAxis, TextAxis
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-FILL_NONE: str
-FILL_SOLID: str
-FILL_PATTERN_DARKDOWN: str
-FILL_PATTERN_DARKGRAY: str
-FILL_PATTERN_DARKGRID: str
-FILL_PATTERN_DARKHORIZONTAL: str
-FILL_PATTERN_DARKTRELLIS: str
-FILL_PATTERN_DARKUP: str
-FILL_PATTERN_DARKVERTICAL: str
-FILL_PATTERN_GRAY0625: str
-FILL_PATTERN_GRAY125: str
-FILL_PATTERN_LIGHTDOWN: str
-FILL_PATTERN_LIGHTGRAY: str
-FILL_PATTERN_LIGHTGRID: str
-FILL_PATTERN_LIGHTHORIZONTAL: str
-FILL_PATTERN_LIGHTTRELLIS: str
-FILL_PATTERN_LIGHTUP: str
-FILL_PATTERN_LIGHTVERTICAL: str
-FILL_PATTERN_MEDIUMGRAY: str
-fills: Incomplete
+from ._3d import _3DBase
+from ._chart import ChartBase
 
-class Fill(Serialisable):
+class BandFormat(Serialisable):
     tagname: str
-    @classmethod
-    def from_tree(cls, el): ...
+    idx: Incomplete
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    __elements__: Incomplete
+    def __init__(self, idx: int = 0, spPr: GraphicalProperties | None = None) -> None: ...
 
-class PatternFill(Fill):
+class BandFormatList(Serialisable):
     tagname: str
+    bandFmt: Incomplete
     __elements__: Incomplete
-    patternType: Incomplete
-    fill_type: Incomplete
-    fgColor: Incomplete
-    start_color: Incomplete
-    bgColor: Incomplete
-    end_color: Incomplete
-    def __init__(
-        self,
-        patternType: Incomplete | None = None,
-        fgColor=...,
-        bgColor=...,
-        fill_type: Incomplete | None = None,
-        start_color: Incomplete | None = None,
-        end_color: Incomplete | None = None,
-    ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
+    def __init__(self, bandFmt=()) -> None: ...
 
-DEFAULT_EMPTY_FILL: Incomplete
-DEFAULT_GRAY_FILL: Incomplete
+class _SurfaceChartBase(ChartBase):
+    wireframe: Incomplete
+    ser: Incomplete
+    bandFmts: Typed[BandFormatList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, wireframe: Incomplete | None = None, ser=(), bandFmts: BandFormatList | None = None, **kw) -> None: ...
+    @property
+    @abstractmethod
+    def tagname(self) -> str: ...
 
-class Stop(Serialisable):
+class SurfaceChart3D(_SurfaceChartBase, _3DBase):
     tagname: str
-    position: Incomplete
-    color: Incomplete
-    def __init__(self, color, position) -> None: ...
-
-class StopList(Sequence):
-    expected_type: Incomplete
-    def __set__(self, obj, values) -> None: ...
+    wireframe: Incomplete
+    ser: Incomplete
+    bandFmts: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    z_axis: Typed[SeriesAxis, Literal[False]]
+    __elements__: Incomplete
+    def __init__(self, **kw) -> None: ...
 
-class GradientFill(Fill):
+class SurfaceChart(SurfaceChart3D):
     tagname: str
-    type: Incomplete
-    fill_type: Incomplete
-    degree: Incomplete
-    left: Incomplete
-    right: Incomplete
-    top: Incomplete
-    bottom: Incomplete
-    stop: Incomplete
-    def __init__(
-        self, type: str = "linear", degree: int = 0, left: int = 0, right: int = 0, top: int = 0, bottom: int = 0, stop=()
-    ) -> None: ...
-    def __iter__(self): ...
-    def to_tree(self, tagname: Incomplete | None = None, namespace: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
+    wireframe: Incomplete
+    ser: Incomplete
+    bandFmts: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/fonts.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chartsheet/custom.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 from _typeshed import Incomplete
+from typing import overload
+from typing_extensions import Literal, TypeAlias
 
+from openpyxl.descriptors.base import Bool, Integer, Set, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.worksheet.header_footer import HeaderFooter
+from openpyxl.worksheet.page import PageMargins, PrintPageSetup
 
-class Font(Serialisable):
-    UNDERLINE_DOUBLE: str
-    UNDERLINE_DOUBLE_ACCOUNTING: str
-    UNDERLINE_SINGLE: str
-    UNDERLINE_SINGLE_ACCOUNTING: str
-    name: Incomplete
-    charset: Incomplete
-    family: Incomplete
-    sz: Incomplete
-    size: Incomplete
-    b: Incomplete
-    bold: Incomplete
-    i: Incomplete
-    italic: Incomplete
-    strike: Incomplete
-    strikethrough: Incomplete
-    outline: Incomplete
-    shadow: Incomplete
-    condense: Incomplete
-    extend: Incomplete
-    u: Incomplete
-    underline: Incomplete
-    vertAlign: Incomplete
-    color: Incomplete
-    scheme: Incomplete
+_CustomChartsheetViewState: TypeAlias = Literal["visible", "hidden", "veryHidden"]
+
+class CustomChartsheetView(Serialisable):
     tagname: str
+    guid: Incomplete
+    scale: Integer[Literal[False]]
+    state: Set[_CustomChartsheetViewState]
+    zoomToFit: Bool[Literal[True]]
+    pageMargins: Typed[PageMargins, Literal[True]]
+    pageSetup: Typed[PrintPageSetup, Literal[True]]
+    headerFooter: Typed[HeaderFooter, Literal[True]]
     __elements__: Incomplete
+    @overload
+    def __init__(
+        self,
+        guid: Incomplete | None = None,
+        *,
+        scale: _ConvertibleToInt,
+        state: _CustomChartsheetViewState = "visible",
+        zoomToFit: _ConvertibleToBool | None = None,
+        pageMargins: PageMargins | None = None,
+        pageSetup: PrintPageSetup | None = None,
+        headerFooter: HeaderFooter | None = None,
+    ) -> None: ...
+    @overload
     def __init__(
         self,
-        name: Incomplete | None = None,
-        sz: Incomplete | None = None,
-        b: Incomplete | None = None,
-        i: Incomplete | None = None,
-        charset: Incomplete | None = None,
-        u: Incomplete | None = None,
-        strike: Incomplete | None = None,
-        color: Incomplete | None = None,
-        scheme: Incomplete | None = None,
-        family: Incomplete | None = None,
-        size: Incomplete | None = None,
-        bold: Incomplete | None = None,
-        italic: Incomplete | None = None,
-        strikethrough: Incomplete | None = None,
-        underline: Incomplete | None = None,
-        vertAlign: Incomplete | None = None,
-        outline: Incomplete | None = None,
-        shadow: Incomplete | None = None,
-        condense: Incomplete | None = None,
-        extend: Incomplete | None = None,
+        guid: Incomplete | None,
+        scale: _ConvertibleToInt,
+        state: _CustomChartsheetViewState = "visible",
+        zoomToFit: _ConvertibleToBool | None = None,
+        pageMargins: PageMargins | None = None,
+        pageSetup: PrintPageSetup | None = None,
+        headerFooter: HeaderFooter | None = None,
     ) -> None: ...
-    @classmethod
-    def from_tree(cls, node): ...
 
-DEFAULT_FONT: Incomplete
+class CustomChartsheetViews(Serialisable):
+    tagname: str
+    customSheetView: Incomplete
+    __elements__: Incomplete
+    def __init__(self, customSheetView: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/named_styles.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/styles/named_styles.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.alignment import Alignment
+from openpyxl.styles.borders import Border
+from openpyxl.styles.fills import Fill
+from openpyxl.styles.fonts import Font
+from openpyxl.styles.protection import Protection
 
-class NamedStyle(Serialisable):  # type: ignore[misc]
-    font: Incomplete
-    fill: Incomplete
-    border: Incomplete
-    alignment: Incomplete
+class NamedStyle(Serialisable):
+    font: Typed[Font, Literal[False]]
+    fill: Typed[Fill, Literal[False]]
+    border: Typed[Border, Literal[False]]
+    alignment: Typed[Alignment, Literal[False]]
     number_format: Incomplete
-    protection: Incomplete
-    builtinId: Incomplete
-    hidden: Incomplete
+    protection: Typed[Protection, Literal[False]]
+    builtinId: Integer[Literal[True]]
+    hidden: Bool[Literal[True]]
     # Overwritten by property below
     # xfId: Integer
-    name: Incomplete
+    name: String[Literal[False]]
     def __init__(
         self,
         name: str = "Normal",
-        font=None,
-        fill=None,
-        border=None,
-        alignment=None,
+        font: Font | None = None,
+        fill: Fill | None = None,
+        border: Border | None = None,
+        alignment: Alignment | None = None,
         number_format: Incomplete | None = None,
-        protection=None,
-        builtinId: Incomplete | None = None,
-        hidden: bool = False,
-        xfId: Incomplete | None = None,
+        protection: Protection | None = None,
+        builtinId: _ConvertibleToInt | None = None,
+        hidden: _ConvertibleToBool | None = False,
+        xfId: Unused = None,
     ) -> None: ...
     def __setattr__(self, attr: str, value) -> None: ...
     def __iter__(self): ...
     @property
     def xfId(self): ...
     def bind(self, wb) -> None: ...
     def as_tuple(self): ...
@@ -40,37 +48,37 @@
     @property
     def names(self): ...
     def __getitem__(self, key): ...
     def append(self, style) -> None: ...
 
 class _NamedCellStyle(Serialisable):
     tagname: str
-    name: Incomplete
-    xfId: Incomplete
-    builtinId: Incomplete
-    iLevel: Incomplete
-    hidden: Incomplete
-    customBuiltin: Incomplete
-    extLst: Incomplete
+    name: String[Literal[False]]
+    xfId: Integer[Literal[False]]
+    builtinId: Integer[Literal[True]]
+    iLevel: Integer[Literal[True]]
+    hidden: Bool[Literal[True]]
+    customBuiltin: Bool[Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
     def __init__(
         self,
-        name: Incomplete | None = None,
-        xfId: Incomplete | None = None,
-        builtinId: Incomplete | None = None,
-        iLevel: Incomplete | None = None,
-        hidden: Incomplete | None = None,
-        customBuiltin: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        name: str,
+        xfId: _ConvertibleToInt,
+        builtinId: _ConvertibleToInt | None = None,
+        iLevel: _ConvertibleToInt | None = None,
+        hidden: _ConvertibleToBool | None = None,
+        customBuiltin: _ConvertibleToBool | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
 class _NamedCellStyleList(Serialisable):
     tagname: str
     # Overwritten by property below
     # count: Integer
     cellStyle: Incomplete
     __attrs__: Incomplete
-    def __init__(self, count: Incomplete | None = None, cellStyle=()) -> None: ...
+    def __init__(self, count: Unused = None, cellStyle=()) -> None: ...
     @property
     def count(self): ...
     @property
     def names(self): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/styleable.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/manifest.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from _typeshed import Incomplete
-from warnings import warn as warn
+from collections.abc import Generator
+from typing_extensions import Literal
 
-class StyleDescriptor:
-    collection: Incomplete
-    key: Incomplete
-    def __init__(self, collection, key) -> None: ...
-    def __set__(self, instance, value) -> None: ...
-    def __get__(self, instance, cls): ...
-
-class NumberFormatDescriptor:
-    key: str
-    collection: str
-    def __set__(self, instance, value) -> None: ...
-    def __get__(self, instance, cls): ...
-
-class NamedStyleDescriptor:
-    key: str
-    collection: str
-    def __set__(self, instance, value) -> None: ...
-    def __get__(self, instance, cls): ...
-
-class StyleArrayDescriptor:
-    key: Incomplete
-    def __init__(self, key) -> None: ...
-    def __set__(self, instance, value) -> None: ...
-    def __get__(self, instance, cls): ...
-
-class StyleableObject:
-    font: Incomplete
-    fill: Incomplete
-    border: Incomplete
-    number_format: Incomplete
-    protection: Incomplete
-    alignment: Incomplete
-    style: Incomplete
-    quotePrefix: Incomplete
-    pivotButton: Incomplete
-    parent: Incomplete
-    def __init__(self, sheet, style_array: Incomplete | None = None) -> None: ...
+from openpyxl.descriptors.base import String
+from openpyxl.descriptors.serialisable import Serialisable
+
+mimetypes: Incomplete
+
+class FileExtension(Serialisable):
+    tagname: str
+    Extension: String[Literal[False]]
+    ContentType: String[Literal[False]]
+    def __init__(self, Extension: str, ContentType: str) -> None: ...
+
+class Override(Serialisable):
+    tagname: str
+    PartName: String[Literal[False]]
+    ContentType: String[Literal[False]]
+    def __init__(self, PartName: str, ContentType: str) -> None: ...
+
+DEFAULT_TYPES: Incomplete
+DEFAULT_OVERRIDE: Incomplete
+
+class Manifest(Serialisable):
+    tagname: str
+    Default: Incomplete
+    Override: Incomplete
+    path: str
+    __elements__: Incomplete
+    def __init__(self, Default=(), Override=()) -> None: ...
     @property
-    def style_id(self): ...
+    def filenames(self): ...
     @property
-    def has_style(self): ...
+    def extensions(self): ...
+    def to_tree(self): ...
+    def __contains__(self, content_type): ...
+    def find(self, content_type): ...
+    def findall(self, content_type) -> Generator[Incomplete, None, None]: ...
+    def append(self, obj) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/stylesheet.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/area_chart.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from abc import abstractmethod
+from typing_extensions import Literal
 
-from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.excel import ExtensionList
 
-class Stylesheet(Serialisable):
-    tagname: str
-    numFmts: Incomplete
-    fonts: Incomplete
-    fills: Incomplete
-    borders: Incomplete
-    cellStyleXfs: Incomplete
-    cellXfs: Incomplete
-    cellStyles: Incomplete
-    dxfs: Incomplete
-    tableStyles: Incomplete
-    colors: Incomplete
-    extLst: Incomplete
+from ._chart import ChartBase
+
+class _AreaChartBase(ChartBase):
+    grouping: Incomplete
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
+    dropLines: Typed[ChartLines, Literal[True]]
     __elements__: Incomplete
-    number_formats: Incomplete
-    cell_styles: Incomplete
-    alignments: Incomplete
-    protections: Incomplete
-    named_styles: Incomplete
     def __init__(
         self,
-        numFmts: Incomplete | None = None,
-        fonts=(),
-        fills=(),
-        borders=(),
-        cellStyleXfs: Incomplete | None = None,
-        cellXfs: Incomplete | None = None,
-        cellStyles: Incomplete | None = None,
-        dxfs=(),
-        tableStyles: Incomplete | None = None,
-        colors: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        grouping: str = "standard",
+        varyColors: Incomplete | None = None,
+        ser=(),
+        dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
     ) -> None: ...
-    @classmethod
-    def from_tree(cls, node): ...
     @property
-    def custom_formats(self): ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    @abstractmethod
+    def tagname(self) -> str: ...
 
-def apply_stylesheet(archive, wb): ...
-def write_stylesheet(wb): ...
+class AreaChart(_AreaChartBase):
+    tagname: str
+    grouping: Incomplete
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    dropLines: Incomplete
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, axId: Unused = None, extLst: Unused = None, **kw) -> None: ...
+
+class AreaChart3D(AreaChart):
+    tagname: str
+    grouping: Incomplete
+    varyColors: Incomplete
+    ser: Incomplete
+    dLbls: Incomplete
+    dropLines: Incomplete
+    gapDepth: Incomplete
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    z_axis: Typed[SeriesAxis, Literal[True]]
+    __elements__: Incomplete
+    def __init__(self, gapDepth: Incomplete | None = None, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/styles/table.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/packaging/relationship.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from collections.abc import Generator
+from typing import overload
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Alias, String
 from openpyxl.descriptors.serialisable import Serialisable
 
-class TableStyleElement(Serialisable):
+class Relationship(Serialisable):
     tagname: str
-    type: Incomplete
-    size: Incomplete
-    dxfId: Incomplete
+    Type: String[Literal[False]]
+    Target: String[Literal[False]]
+    target: Alias
+    TargetMode: String[Literal[True]]
+    Id: String[Literal[True]]
+    id: Alias
+    @overload
     def __init__(
-        self, type: Incomplete | None = None, size: Incomplete | None = None, dxfId: Incomplete | None = None
+        self, Id: str, Type: Unused = None, *, type: str, Target: str | None = None, TargetMode: str | None = None
     ) -> None: ...
-
-class TableStyle(Serialisable):
-    tagname: str
-    name: Incomplete
-    pivot: Incomplete
-    table: Incomplete
-    count: Incomplete
-    tableStyleElement: Incomplete
-    __elements__: Incomplete
+    @overload
+    def __init__(self, Id: str, Type: Unused, type: str, Target: str | None = None, TargetMode: str | None = None) -> None: ...
+    @overload
     def __init__(
-        self,
-        name: Incomplete | None = None,
-        pivot: Incomplete | None = None,
-        table: Incomplete | None = None,
-        count: Incomplete | None = None,
-        tableStyleElement=(),
+        self, Id: str, Type: str, type: None = None, Target: str | None = None, TargetMode: str | None = None
     ) -> None: ...
 
-class TableStyleList(Serialisable):
+class RelationshipList(Serialisable):
     tagname: str
-    defaultTableStyle: Incomplete
-    defaultPivotStyle: Incomplete
-    tableStyle: Incomplete
-    __elements__: Incomplete
-    __attrs__: Incomplete
-    def __init__(
-        self,
-        count: Incomplete | None = None,
-        defaultTableStyle: str = "TableStyleMedium9",
-        defaultPivotStyle: str = "PivotStyleLight16",
-        tableStyle=(),
-    ) -> None: ...
-    @property
-    def count(self): ...
+    Relationship: Incomplete
+    def __init__(self, Relationship=()) -> None: ...
+    def append(self, value) -> None: ...
+    def __len__(self) -> int: ...
+    def __bool__(self) -> bool: ...
+    def find(self, content_type) -> Generator[Incomplete, None, None]: ...
+    def __getitem__(self, key): ...
+    def to_tree(self): ...
+
+def get_rels_path(path): ...
+def get_dependents(archive, filename): ...
+def get_rel(archive, deps, id: Incomplete | None = None, cls: Incomplete | None = None): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/utils/cell.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/utils/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/utils/datetime.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/utils/datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/utils/units.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/utils/units.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/_writer.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/child.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/child.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/external_link/external.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/styles/stylesheet.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,53 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.cell_style import CellStyleList
+from openpyxl.styles.colors import ColorList
+from openpyxl.styles.named_styles import _NamedCellStyleList
+from openpyxl.styles.numbers import NumberFormatList
+from openpyxl.styles.table import TableStyleList
 
-class ExternalCell(Serialisable):  # type: ignore[misc]
-    r: Incomplete
-    t: Incomplete
-    vm: Incomplete
-    v: Incomplete
-    def __init__(
-        self, r: Incomplete | None = None, t: Incomplete | None = None, vm: Incomplete | None = None, v: Incomplete | None = None
-    ) -> None: ...
-
-class ExternalRow(Serialisable):  # type: ignore[misc]
-    r: Incomplete
-    cell: Incomplete
-    __elements__: Incomplete
-    def __init__(self, r=(), cell: Incomplete | None = None) -> None: ...
-
-class ExternalSheetData(Serialisable):  # type: ignore[misc]
-    sheetId: Incomplete
-    refreshError: Incomplete
-    row: Incomplete
-    __elements__: Incomplete
-    def __init__(self, sheetId: Incomplete | None = None, refreshError: Incomplete | None = None, row=()) -> None: ...
-
-class ExternalSheetDataSet(Serialisable):  # type: ignore[misc]
-    sheetData: Incomplete
-    __elements__: Incomplete
-    def __init__(self, sheetData: Incomplete | None = None) -> None: ...
-
-class ExternalSheetNames(Serialisable):  # type: ignore[misc]
-    sheetName: Incomplete
-    __elements__: Incomplete
-    def __init__(self, sheetName=()) -> None: ...
-
-class ExternalDefinedName(Serialisable):
+class Stylesheet(Serialisable):
     tagname: str
-    name: Incomplete
-    refersTo: Incomplete
-    sheetId: Incomplete
-    def __init__(
-        self, name: Incomplete | None = None, refersTo: Incomplete | None = None, sheetId: Incomplete | None = None
-    ) -> None: ...
-
-class ExternalBook(Serialisable):
-    tagname: str
-    sheetNames: Incomplete
-    definedNames: Incomplete
-    sheetDataSet: Incomplete
-    id: Incomplete
-    __elements__: Incomplete
-    def __init__(
-        self,
-        sheetNames: Incomplete | None = None,
-        definedNames=(),
-        sheetDataSet: Incomplete | None = None,
-        id: Incomplete | None = None,
-    ) -> None: ...
-
-class ExternalLink(Serialisable):
-    tagname: str
-    mime_type: str
-    externalBook: Incomplete
-    file_link: Incomplete
-    __elements__: Incomplete
+    numFmts: Typed[NumberFormatList, Literal[False]]
+    fonts: Incomplete
+    fills: Incomplete
+    borders: Incomplete
+    cellStyleXfs: Typed[CellStyleList, Literal[False]]
+    cellXfs: Typed[CellStyleList, Literal[False]]
+    cellStyles: Typed[_NamedCellStyleList, Literal[False]]
+    dxfs: Incomplete
+    tableStyles: Typed[TableStyleList, Literal[True]]
+    colors: Typed[ColorList, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    number_formats: Incomplete
+    cell_styles: Incomplete
+    alignments: Incomplete
+    protections: Incomplete
+    named_styles: Incomplete
     def __init__(
         self,
-        externalBook: Incomplete | None = None,
-        ddeLink: Incomplete | None = None,
-        oleLink: Incomplete | None = None,
-        extLst: Incomplete | None = None,
+        numFmts: NumberFormatList | None = None,
+        fonts=(),
+        fills=(),
+        borders=(),
+        cellStyleXfs: CellStyleList | None = None,
+        cellXfs: CellStyleList | None = None,
+        cellStyles: _NamedCellStyleList | None = None,
+        dxfs=(),
+        tableStyles: TableStyleList | None = None,
+        colors: ColorList | None = None,
+        extLst: Unused = None,
     ) -> None: ...
-    def to_tree(self): ...
+    @classmethod
+    def from_tree(cls, node): ...
     @property
-    def path(self): ...
+    def custom_formats(self): ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
 
-def read_external_link(archive, book_path): ...
+def apply_stylesheet(archive, wb): ...
+def write_stylesheet(wb): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/properties.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/chart/chartspace.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,132 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from typing import overload
+from typing_extensions import Literal
 
+from openpyxl.chart.legend import Legend
+from openpyxl.chart.pivot import PivotSource
+from openpyxl.chart.plotarea import PlotArea
+from openpyxl.chart.print_settings import PrintSettings
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
+from openpyxl.chart.title import Title
+from openpyxl.descriptors.base import Alias, String, Typed
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.colors import ColorMapping
 
-class WorkbookProperties(Serialisable):
+class ChartContainer(Serialisable):
     tagname: str
-    date1904: Incomplete
-    dateCompatibility: Incomplete
-    showObjects: Incomplete
-    showBorderUnselectedTables: Incomplete
-    filterPrivacy: Incomplete
-    promptedSolutions: Incomplete
-    showInkAnnotation: Incomplete
-    backupFile: Incomplete
-    saveExternalLinkValues: Incomplete
-    updateLinks: Incomplete
-    codeName: Incomplete
-    hidePivotFieldList: Incomplete
-    showPivotChartFilter: Incomplete
-    allowRefreshQuery: Incomplete
-    publishItems: Incomplete
-    checkCompatibility: Incomplete
-    autoCompressPictures: Incomplete
-    refreshAllConnections: Incomplete
-    defaultThemeVersion: Incomplete
+    title: Typed[Title, Literal[True]]
+    autoTitleDeleted: Incomplete
+    pivotFmts: Incomplete
+    view3D: Incomplete
+    floor: Incomplete
+    sideWall: Incomplete
+    backWall: Incomplete
+    plotArea: Typed[PlotArea, Literal[False]]
+    legend: Typed[Legend, Literal[True]]
+    plotVisOnly: Incomplete
+    dispBlanksAs: Incomplete
+    showDLblsOverMax: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
     def __init__(
         self,
-        date1904: Incomplete | None = None,
-        dateCompatibility: Incomplete | None = None,
-        showObjects: Incomplete | None = None,
-        showBorderUnselectedTables: Incomplete | None = None,
-        filterPrivacy: Incomplete | None = None,
-        promptedSolutions: Incomplete | None = None,
-        showInkAnnotation: Incomplete | None = None,
-        backupFile: Incomplete | None = None,
-        saveExternalLinkValues: Incomplete | None = None,
-        updateLinks: Incomplete | None = None,
-        codeName: Incomplete | None = None,
-        hidePivotFieldList: Incomplete | None = None,
-        showPivotChartFilter: Incomplete | None = None,
-        allowRefreshQuery: Incomplete | None = None,
-        publishItems: Incomplete | None = None,
-        checkCompatibility: Incomplete | None = None,
-        autoCompressPictures: Incomplete | None = None,
-        refreshAllConnections: Incomplete | None = None,
-        defaultThemeVersion: Incomplete | None = None,
+        title: Title | None = None,
+        autoTitleDeleted: Incomplete | None = None,
+        pivotFmts=(),
+        view3D: Incomplete | None = None,
+        floor: Incomplete | None = None,
+        sideWall: Incomplete | None = None,
+        backWall: Incomplete | None = None,
+        plotArea: PlotArea | None = None,
+        legend: Legend | None = None,
+        plotVisOnly: bool = True,
+        dispBlanksAs: str = "gap",
+        showDLblsOverMax: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
 
-class CalcProperties(Serialisable):
+class Protection(Serialisable):
     tagname: str
-    calcId: Incomplete
-    calcMode: Incomplete
-    fullCalcOnLoad: Incomplete
-    refMode: Incomplete
-    iterate: Incomplete
-    iterateCount: Incomplete
-    iterateDelta: Incomplete
-    fullPrecision: Incomplete
-    calcCompleted: Incomplete
-    calcOnSave: Incomplete
-    concurrentCalc: Incomplete
-    concurrentManualCount: Incomplete
-    forceFullCalc: Incomplete
+    chartObject: Incomplete
+    data: Incomplete
+    formatting: Incomplete
+    selection: Incomplete
+    userInterface: Incomplete
+    __elements__: Incomplete
     def __init__(
         self,
-        calcId: int = 124519,
-        calcMode: Incomplete | None = None,
-        fullCalcOnLoad: bool = True,
-        refMode: Incomplete | None = None,
-        iterate: Incomplete | None = None,
-        iterateCount: Incomplete | None = None,
-        iterateDelta: Incomplete | None = None,
-        fullPrecision: Incomplete | None = None,
-        calcCompleted: Incomplete | None = None,
-        calcOnSave: Incomplete | None = None,
-        concurrentCalc: Incomplete | None = None,
-        concurrentManualCount: Incomplete | None = None,
-        forceFullCalc: Incomplete | None = None,
+        chartObject: Incomplete | None = None,
+        data: Incomplete | None = None,
+        formatting: Incomplete | None = None,
+        selection: Incomplete | None = None,
+        userInterface: Incomplete | None = None,
     ) -> None: ...
 
-class FileVersion(Serialisable):
+class ExternalData(Serialisable):
     tagname: str
-    appName: Incomplete
-    lastEdited: Incomplete
-    lowestEdited: Incomplete
-    rupBuild: Incomplete
-    codeName: Incomplete
+    autoUpdate: Incomplete
+    id: String[Literal[False]]
+    @overload
+    def __init__(self, autoUpdate: Incomplete | None = None, *, id: str) -> None: ...
+    @overload
+    def __init__(self, autoUpdate: Incomplete | None, id: str) -> None: ...
+
+class ChartSpace(Serialisable):
+    tagname: str
+    date1904: Incomplete
+    lang: Incomplete
+    roundedCorners: Incomplete
+    style: Incomplete
+    clrMapOvr: Typed[ColorMapping, Literal[True]]
+    pivotSource: Typed[PivotSource, Literal[True]]
+    protection: Typed[Protection, Literal[True]]
+    chart: Typed[ChartContainer, Literal[False]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    textProperties: Alias
+    externalData: Typed[ExternalData, Literal[True]]
+    printSettings: Typed[PrintSettings, Literal[True]]
+    userShapes: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: Incomplete
+    @overload
+    def __init__(
+        self,
+        date1904: Incomplete | None = None,
+        lang: Incomplete | None = None,
+        roundedCorners: Incomplete | None = None,
+        style: Incomplete | None = None,
+        clrMapOvr: ColorMapping | None = None,
+        pivotSource: PivotSource | None = None,
+        protection: Protection | None = None,
+        *,
+        chart: ChartContainer,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        externalData: ExternalData | None = None,
+        printSettings: PrintSettings | None = None,
+        userShapes: Incomplete | None = None,
+        extLst: Unused = None,
+    ) -> None: ...
+    @overload
     def __init__(
         self,
-        appName: Incomplete | None = None,
-        lastEdited: Incomplete | None = None,
-        lowestEdited: Incomplete | None = None,
-        rupBuild: Incomplete | None = None,
-        codeName: Incomplete | None = None,
+        date1904: Incomplete | None,
+        lang: Incomplete | None,
+        roundedCorners: Incomplete | None,
+        style: Incomplete | None,
+        clrMapOvr: ColorMapping | None,
+        pivotSource: PivotSource | None,
+        protection: Protection | None,
+        chart: ChartContainer,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        externalData: ExternalData | None = None,
+        printSettings: PrintSettings | None = None,
+        userShapes: Incomplete | None = None,
+        extLst: Unused = None,
     ) -> None: ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/workbook/workbook.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/workbook/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_read_only.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_reader.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_reader.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/_writer.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/ole.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/errors.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,49 @@
 from _typeshed import Incomplete
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
-class ObjectAnchor(Serialisable):
+class Extension(Serialisable):
     tagname: str
-    to: Incomplete
-    moveWithCells: Incomplete
-    sizeWithCells: Incomplete
-    z_order: Incomplete
-    def __init__(
-        self,
-        _from: Incomplete | None = None,
-        to: Incomplete | None = None,
-        moveWithCells: bool = False,
-        sizeWithCells: bool = False,
-        z_order: Incomplete | None = None,
-    ) -> None: ...
+    uri: String[Literal[True]]
+    def __init__(self, uri: str | None = None) -> None: ...
 
-class ObjectPr(Serialisable):
+class ExtensionList(Serialisable):
     tagname: str
-    anchor: Incomplete
-    locked: Incomplete
-    defaultSize: Incomplete
-    disabled: Incomplete
-    uiObject: Incomplete
-    autoFill: Incomplete
-    autoLine: Incomplete
-    autoPict: Incomplete
-    macro: Incomplete
-    altText: Incomplete
-    dde: Incomplete
+    ext: Incomplete
     __elements__: Incomplete
-    def __init__(
-        self,
-        anchor: Incomplete | None = None,
-        locked: bool = True,
-        defaultSize: bool = True,
-        _print: bool = True,
-        disabled: bool = False,
-        uiObject: bool = False,
-        autoFill: bool = True,
-        autoLine: bool = True,
-        autoPict: bool = True,
-        macro: Incomplete | None = None,
-        altText: Incomplete | None = None,
-        dde: bool = False,
-    ) -> None: ...
+    def __init__(self, ext=()) -> None: ...
 
-class OleObject(Serialisable):
+class IgnoredError(Serialisable):
     tagname: str
-    objectPr: Incomplete
-    progId: Incomplete
-    dvAspect: Incomplete
-    link: Incomplete
-    oleUpdate: Incomplete
-    autoLoad: Incomplete
-    shapeId: Incomplete
-    __elements__: Incomplete
+    sqref: Incomplete
+    evalError: Bool[Literal[True]]
+    twoDigitTextYear: Bool[Literal[True]]
+    numberStoredAsText: Bool[Literal[True]]
+    formula: Bool[Literal[True]]
+    formulaRange: Bool[Literal[True]]
+    unlockedFormula: Bool[Literal[True]]
+    emptyCellReference: Bool[Literal[True]]
+    listDataValidation: Bool[Literal[True]]
+    calculatedColumn: Bool[Literal[True]]
     def __init__(
         self,
-        objectPr: Incomplete | None = None,
-        progId: Incomplete | None = None,
-        dvAspect: str = "DVASPECT_CONTENT",
-        link: Incomplete | None = None,
-        oleUpdate: Incomplete | None = None,
-        autoLoad: bool = False,
-        shapeId: Incomplete | None = None,
+        sqref: Incomplete | None = None,
+        evalError: _ConvertibleToBool | None = False,
+        twoDigitTextYear: _ConvertibleToBool | None = False,
+        numberStoredAsText: _ConvertibleToBool | None = False,
+        formula: _ConvertibleToBool | None = False,
+        formulaRange: _ConvertibleToBool | None = False,
+        unlockedFormula: _ConvertibleToBool | None = False,
+        emptyCellReference: _ConvertibleToBool | None = False,
+        listDataValidation: _ConvertibleToBool | None = False,
+        calculatedColumn: _ConvertibleToBool | None = False,
     ) -> None: ...
 
-class OleObjects(Serialisable):
+class IgnoredErrors(Serialisable):
     tagname: str
-    oleObject: Incomplete
+    ignoredError: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: Incomplete
-    def __init__(self, oleObject=()) -> None: ...
+    def __init__(self, ignoredError=(), extLst: ExtensionList | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/print_settings.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/print_settings.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from re import Pattern
-from typing_extensions import Self
+from typing import overload
+from typing_extensions import Literal, Self
 
 from openpyxl.descriptors import Integer, Strict, String
+from openpyxl.descriptors.base import Typed, _ConvertibleToInt
 from openpyxl.utils.cell import SHEETRANGE_RE as SHEETRANGE_RE
 
 from .cell_range import MultiCellRange
 
 COL_RANGE: str
 COL_RANGE_RE: Pattern[str]
 ROW_RANGE: str
 ROW_RANGE_RE: Pattern[str]
 TITLES_REGEX: Pattern[str]
 PRINT_AREA_RE: Pattern[str]
 
 class ColRange(Strict):
-    min_col: String
-    max_col: String
-    def __init__(
-        self, range_string: Incomplete | None = None, min_col: Incomplete | None = None, max_col: Incomplete | None = None
-    ) -> None: ...
+    min_col: String[Literal[False]]
+    max_col: String[Literal[False]]
+    @overload
+    def __init__(self, range_string: None = None, *, min_col: str, max_col: str) -> None: ...
+    @overload
+    def __init__(self, range_string: Incomplete, min_col: Unused = None, max_col: Unused = None) -> None: ...
     def __eq__(self, other: object) -> bool: ...
 
 class RowRange(Strict):
-    min_row: Integer
-    max_row: Integer
-    def __init__(
-        self, range_string: Incomplete | None = None, min_row: Incomplete | None = None, max_row: Incomplete | None = None
-    ) -> None: ...
+    min_row: Integer[Literal[False]]
+    max_row: Integer[Literal[False]]
+    @overload
+    def __init__(self, range_string: None, min_row: _ConvertibleToInt, max_row: _ConvertibleToInt) -> None: ...
+    @overload
+    def __init__(self, range_string: Incomplete, min_row: Unused = None, max_row: Unused = None) -> None: ...
     def __eq__(self, other: object) -> bool: ...
 
 class PrintTitles(Strict):
-    cols: Incomplete
-    rows: Incomplete
-    title: String
-    def __init__(self, cols: Incomplete | None = None, rows: Incomplete | None = None, title: str = "") -> None: ...
+    cols: Typed[ColRange, Literal[True]]
+    rows: Typed[RowRange, Literal[True]]
+    title: String[Literal[False]]
+    def __init__(self, cols: ColRange | None = None, rows: RowRange | None = None, title: str = "") -> None: ...
     @classmethod
     def from_string(cls, value) -> Self: ...
     def __eq__(self, other: object) -> bool: ...
 
 class PrintArea(MultiCellRange):
     title: str
     @classmethod
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/scenario.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/controls.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 from _typeshed import Incomplete
+from typing import overload
+from typing_extensions import Literal
 
+from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.worksheet.ole import ObjectAnchor
 
-class InputCells(Serialisable):
+class ControlProperty(Serialisable):
     tagname: str
-    r: Incomplete
-    deleted: Incomplete
-    undone: Incomplete
-    val: Incomplete
-    numFmtId: Incomplete
+    anchor: Typed[ObjectAnchor, Literal[False]]
+    locked: Bool[Literal[True]]
+    defaultSize: Bool[Literal[True]]
+    _print: Bool[Literal[True]]  # Not private. Avoids name clash
+    disabled: Bool[Literal[True]]
+    recalcAlways: Bool[Literal[True]]
+    uiObject: Bool[Literal[True]]
+    autoFill: Bool[Literal[True]]
+    autoLine: Bool[Literal[True]]
+    autoPict: Bool[Literal[True]]
+    macro: String[Literal[True]]
+    altText: String[Literal[True]]
+    linkedCell: String[Literal[True]]
+    listFillRange: String[Literal[True]]
+    cf: String[Literal[True]]
+    id: Incomplete
+    __elements__: Incomplete
     def __init__(
         self,
-        r: Incomplete | None = None,
-        deleted: bool = False,
-        undone: bool = False,
-        val: Incomplete | None = None,
-        numFmtId: Incomplete | None = None,
+        anchor: ObjectAnchor,
+        locked: _ConvertibleToBool | None = True,
+        defaultSize: _ConvertibleToBool | None = True,
+        _print: _ConvertibleToBool | None = True,
+        disabled: _ConvertibleToBool | None = False,
+        recalcAlways: _ConvertibleToBool | None = False,
+        uiObject: _ConvertibleToBool | None = False,
+        autoFill: _ConvertibleToBool | None = True,
+        autoLine: _ConvertibleToBool | None = True,
+        autoPict: _ConvertibleToBool | None = True,
+        macro: str | None = None,
+        altText: str | None = None,
+        linkedCell: str | None = None,
+        listFillRange: str | None = None,
+        cf: str | None = "pict",
+        id: Incomplete | None = None,
     ) -> None: ...
 
-class Scenario(Serialisable):
+class Control(Serialisable):
     tagname: str
-    inputCells: Incomplete
-    name: Incomplete
-    locked: Incomplete
-    hidden: Incomplete
-    user: Incomplete
-    comment: Incomplete
+    controlPr: Typed[ControlProperty, Literal[True]]
+    shapeId: Integer[Literal[False]]
+    name: String[Literal[True]]
     __elements__: Incomplete
-    __attrs__: Incomplete
+    @overload
     def __init__(
-        self,
-        inputCells=(),
-        name: Incomplete | None = None,
-        locked: bool = False,
-        hidden: bool = False,
-        count: Incomplete | None = None,
-        user: Incomplete | None = None,
-        comment: Incomplete | None = None,
+        self, controlPr: ControlProperty | None = None, *, shapeId: _ConvertibleToInt, name: str | None = None
     ) -> None: ...
-    @property
-    def count(self): ...
+    @overload
+    def __init__(self, controlPr: ControlProperty | None, shapeId: _ConvertibleToInt, name: str | None = None) -> None: ...
 
-class ScenarioList(Serialisable):
+class Controls(Serialisable):
     tagname: str
-    scenario: Incomplete
-    current: Incomplete
-    show: Incomplete
-    sqref: Incomplete
+    control: Incomplete
     __elements__: Incomplete
-    def __init__(
-        self, scenario=(), current: Incomplete | None = None, show: Incomplete | None = None, sqref: Incomplete | None = None
-    ) -> None: ...
-    def append(self, scenario) -> None: ...
-    def __bool__(self) -> bool: ...
+    def __init__(self, control=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/worksheet/worksheet.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/worksheet/worksheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/openpyxl-stubs/xml/constants.pyi` & `types-openpyxl-3.1.0.6/openpyxl-stubs/xml/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.5/setup.py` & `types-openpyxl-3.1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e816acffddf9d984bac131224b0eb0f6a3e1c9fc`.
+This package was generated from typeshed commit `1221b4711818d3c5e17c56619fc049e5dbc2fd00`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.1.0.5",
+      version="3.1.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md",
```

### Comparing `types-openpyxl-3.1.0.5/types_openpyxl.egg-info/PKG-INFO` & `types-openpyxl-3.1.0.6/types_openpyxl.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.5
+Version: 3.1.0.6
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e816acffddf9d984bac131224b0eb0f6a3e1c9fc`.
+This package was generated from typeshed commit `1221b4711818d3c5e17c56619fc049e5dbc2fd00`.
```

### Comparing `types-openpyxl-3.1.0.5/types_openpyxl.egg-info/SOURCES.txt` & `types-openpyxl-3.1.0.6/types_openpyxl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

