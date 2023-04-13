# Comparing `tmp/types-openpyxl-3.1.0.3.tar.gz` & `tmp/types-openpyxl-3.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-openpyxl-3.1.0.3.tar", last modified: Sun Mar 26 21:12:31 2023, max compression
+gzip compressed data, was "types-openpyxl-3.1.0.4.tar", last modified: Thu Apr 13 12:30:55 2023, max compression
```

## Comparing `types-openpyxl-3.1.0.3.tar` & `types-openpyxl-3.1.0.4.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.169631 types-openpyxl-3.1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-26 21:12:29.000000 types-openpyxl-3.1.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-26 21:12:29.000000 types-openpyxl-3.1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-26 21:12:31.169631 types-openpyxl-3.1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.141630 types-openpyxl-3.1.0.3/openpyxl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-26 21:12:29.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/_constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.141630 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/rich_text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/cell/text.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.149630 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/area_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/bar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/bubble_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/chartspace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/data_source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/error_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/legend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/line_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/marker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/pie_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/pivot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/plotarea.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/radar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/scatter_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/series.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/series_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/shapes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/stock_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/surface_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/title.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/trendline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chart/updown_bars.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.149630 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/chartsheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/publish.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.153630 types-openpyxl-3.1.0.3/openpyxl-stubs/comments/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/comments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/comments/author.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/comments/comment_sheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/comments/comments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/comments/shape_writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.153630 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/product.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/singleton.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/compat/strings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.153630 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/nested.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/serialisable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/slots.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.153630 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/connector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/effect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/fill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/graphic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/line.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/xdr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.153630 types-openpyxl-3.1.0.3/openpyxl-stubs/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/formatting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/formatting/formatting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/formatting/rule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.157630 types-openpyxl-3.1.0.3/openpyxl-stubs/formula/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/formula/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/formula/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/formula/translate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.157630 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/extended.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/interface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/relationship.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.157630 types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18243 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.157630 types-openpyxl-3.1.0.3/openpyxl-stubs/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/reader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/reader/drawings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/reader/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/reader/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/reader/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.161631 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/alignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/borders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/cell_style.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/differential.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/fills.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/named_styles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/styleable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/stylesheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/styles/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.161631 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/bound_dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/dataframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/escape.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/formulas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/indexed_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/inference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/utils/units.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.161631 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/child.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/defined_name.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.161631 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/external_link/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/external_link/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/external_link/external.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/external_reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/function_group.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/smart_tags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/web.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.165631 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_write_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/cell_range.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/cell_watch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/controls.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/copier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/datavalidation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/dimensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/formula.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/header_footer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/hyperlink.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/ole.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/page.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/pagebreak.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/related.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/scenario.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/smart_tag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/worksheet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.165631 types-openpyxl-3.1.0.3/openpyxl-stubs/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/writer/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/writer/theme.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.169631 types-openpyxl-3.1.0.3/openpyxl-stubs/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/xml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/xml/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-26 21:12:17.000000 types-openpyxl-3.1.0.3/openpyxl-stubs/xml/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 21:12:31.169631 types-openpyxl-3.1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-26 21:12:29.000000 types-openpyxl-3.1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:12:31.169631 types-openpyxl-3.1.0.3/types_openpyxl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-26 21:12:31.000000 types-openpyxl-3.1.0.3/types_openpyxl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-03-26 21:12:31.000000 types-openpyxl-3.1.0.3/types_openpyxl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 21:12:31.000000 types-openpyxl-3.1.0.3/types_openpyxl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-26 21:12:31.000000 types-openpyxl-3.1.0.3/types_openpyxl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-13 12:30:53.000000 types-openpyxl-3.1.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 12:30:53.000000 types-openpyxl-3.1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.804139 types-openpyxl-3.1.0.4/openpyxl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 12:30:53.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/_constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.804139 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/rich_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/cell/text.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.812140 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/area_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/bar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/bubble_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/chartspace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/data_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/error_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/line_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/marker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/pie_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/pivot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/plotarea.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/radar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/scatter_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/series.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/series_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/shapes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/stock_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/surface_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/title.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/trendline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chart/updown_bars.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.812140 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/chartsheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/publish.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.816140 types-openpyxl-3.1.0.4/openpyxl-stubs/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/comments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/comments/author.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/comments/comment_sheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/comments/comments.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/comments/shape_writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.816140 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/singleton.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/compat/strings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.816140 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/nested.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/serialisable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/slots.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.820140 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/connector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/effect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/fill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/graphic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/xdr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.820140 types-openpyxl-3.1.0.4/openpyxl-stubs/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/formatting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/formatting/formatting.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/formatting/rule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.824140 types-openpyxl-3.1.0.4/openpyxl-stubs/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/formula/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/formula/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/formula/translate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.824140 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/extended.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/interface.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/relationship.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.824140 types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18243 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/record.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.828140 types-openpyxl-3.1.0.4/openpyxl-stubs/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/reader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/reader/drawings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/reader/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/reader/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/reader/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.828140 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/alignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/borders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/cell_style.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/differential.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/fills.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/named_styles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/styleable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/stylesheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/styles/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.832140 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/bound_dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/dataframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/escape.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/formulas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/indexed_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/inference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/utils/units.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.836140 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/child.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/defined_name.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.836140 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/external_link/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/external_link/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/external_link/external.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/external_reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/function_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/smart_tags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/web.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_write_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/cell_range.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/cell_watch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/controls.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/copier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/datavalidation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/dimensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/formula.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/header_footer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/hyperlink.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/ole.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/page.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/pagebreak.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/scenario.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/smart_tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/worksheet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/openpyxl-stubs/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/writer/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/writer/theme.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/openpyxl-stubs/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/xml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/xml/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 12:30:41.000000 types-openpyxl-3.1.0.4/openpyxl-stubs/xml/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-13 12:30:53.000000 types-openpyxl-3.1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:30:55.844140 types-openpyxl-3.1.0.4/types_openpyxl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 12:30:55.000000 types-openpyxl-3.1.0.4/types_openpyxl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-04-13 12:30:55.000000 types-openpyxl-3.1.0.4/types_openpyxl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:30:55.000000 types-openpyxl-3.1.0.4/types_openpyxl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 12:30:55.000000 types-openpyxl-3.1.0.4/types_openpyxl.egg-info/top_level.txt
```

### Comparing `types-openpyxl-3.1.0.3/CHANGELOG.md` & `types-openpyxl-3.1.0.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.1.0.4 (2023-04-13)
+
+[openpyxl] Annotate _WorkbookChild.title property (#10043)
+
 ## 3.1.0.3 (2023-03-26)
 
 Ran stubdefaulter for `stubs/openpyxl` (#9946)
 
 ## 3.1.0.2 (2023-03-24)
 
 openpyxl: add baseline stubs for new modules (#9921)
```

### Comparing `types-openpyxl-3.1.0.3/PKG-INFO` & `types-openpyxl-3.1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.3
+Version: 3.1.0.4
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
-This package was generated from typeshed commit `ccbe46173e1c4ed8b165f72e6f0edcc6af2fe15a`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
```

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/cell/cell.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/cell/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/cell/read_only.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/cell/read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/cell/rich_text.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/cell/rich_text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/cell/text.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/cell/text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/_3d.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/_3d.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/__init__.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/area_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/area_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/axis.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/axis.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/bar_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/bar_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/bubble_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/bubble_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/chartspace.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/chartspace.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/data_source.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/data_source.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/error_bar.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/error_bar.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/label.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/label.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/layout.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/layout.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/legend.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/legend.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/line_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/line_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/marker.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/marker.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/picture.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/picture.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/pie_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/pie_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/pivot.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/pivot.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/plotarea.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/plotarea.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/print_settings.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/print_settings.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/radar_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/radar_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/reference.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/reference.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/scatter_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/scatter_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/series.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/series.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/shapes.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/shapes.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/stock_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/stock_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/surface_chart.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/surface_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/text.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/title.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/title.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chart/trendline.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chart/trendline.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/chartsheet.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/chartsheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/custom.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/custom.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/protection.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/protection.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/publish.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/publish.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/relation.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/relation.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/chartsheet/views.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/chartsheet/views.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/comments/comment_sheet.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/comments/comment_sheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/base.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/base.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/excel.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/nested.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/nested.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/sequence.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/sequence.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/descriptors/serialisable.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/descriptors/serialisable.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/colors.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/colors.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/connector.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/connector.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/drawing.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/effect.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/effect.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/fill.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/fill.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/geometry.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/geometry.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/graphic.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/graphic.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/line.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/line.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/picture.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/picture.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/properties.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/spreadsheet_drawing.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/spreadsheet_drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/drawing/text.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/drawing/text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/formatting/formatting.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/formatting/formatting.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/formatting/rule.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/formatting/rule.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/formula/tokenizer.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/formula/tokenizer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/formula/translate.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/formula/translate.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/core.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/core.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/custom.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/custom.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/extended.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/extended.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/manifest.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/relationship.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/relationship.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/packaging/workbook.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/packaging/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/cache.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/cache.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/fields.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/fields.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/record.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/record.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/pivot/table.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/pivot/table.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/reader/excel.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/reader/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/reader/workbook.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/reader/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/__init__.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/alignment.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/alignment.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/borders.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/borders.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/builtins.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/builtins.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/cell_style.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/cell_style.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/colors.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/colors.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/differential.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/differential.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/fills.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/fills.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/fonts.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/fonts.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/named_styles.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/named_styles.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/numbers.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/numbers.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/styleable.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/styleable.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/stylesheet.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/stylesheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/styles/table.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/styles/table.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/utils/cell.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/utils/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/utils/datetime.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/utils/datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/utils/units.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/utils/units.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/_writer.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/child.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/child.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     HeaderFooter: Incomplete
     def __init__(self, parent: Incomplete | None = None, title: Incomplete | None = None) -> None: ...
     @property
     def parent(self): ...
     @property
     def encoding(self): ...
     @property
-    def title(self): ...
+    def title(self) -> str: ...
     @title.setter
-    def title(self, value) -> None: ...
+    def title(self, value: str | bytes) -> None: ...
     @property
     def oddHeader(self): ...
     @oddHeader.setter
     def oddHeader(self, value) -> None: ...
     @property
     def oddFooter(self): ...
     @oddFooter.setter
```

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/defined_name.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/defined_name.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/external_link/external.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/external_link/external.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/properties.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/protection.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/protection.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/smart_tags.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/smart_tags.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/views.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/views.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/web.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/web.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/workbook/workbook.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/workbook/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_read_only.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_reader.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_reader.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_write_only.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_write_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/_writer.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/cell_range.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/cell_range.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/controls.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/controls.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/datavalidation.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/datavalidation.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/dimensions.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/dimensions.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/errors.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/filters.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/filters.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/formula.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/formula.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/header_footer.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/header_footer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/hyperlink.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/hyperlink.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/merge.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/merge.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/ole.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/ole.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/page.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/page.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/pagebreak.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/pagebreak.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/print_settings.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/print_settings.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/properties.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/protection.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/protection.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/scenario.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/scenario.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/smart_tag.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/smart_tag.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/table.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/table.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/views.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/views.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/worksheet/worksheet.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/worksheet/worksheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/openpyxl-stubs/xml/constants.pyi` & `types-openpyxl-3.1.0.4/openpyxl-stubs/xml/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.3/setup.py` & `types-openpyxl-3.1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ccbe46173e1c4ed8b165f72e6f0edcc6af2fe15a`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.1.0.3",
+      version="3.1.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md",
```

### Comparing `types-openpyxl-3.1.0.3/types_openpyxl.egg-info/PKG-INFO` & `types-openpyxl-3.1.0.4/types_openpyxl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.3
+Version: 3.1.0.4
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
-This package was generated from typeshed commit `ccbe46173e1c4ed8b165f72e6f0edcc6af2fe15a`.
+This package was generated from typeshed commit `8db375c3a96441ac94dc6e1aec9a0b1e61cc7763`.
```

### Comparing `types-openpyxl-3.1.0.3/types_openpyxl.egg-info/SOURCES.txt` & `types-openpyxl-3.1.0.4/types_openpyxl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

