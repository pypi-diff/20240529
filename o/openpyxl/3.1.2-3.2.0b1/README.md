# Comparing `tmp/openpyxl-3.1.2.tar.gz` & `tmp/openpyxl-3.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpyxl-3.1.2.tar", last modified: Sat Mar 11 16:54:22 2023, max compression
+gzip compressed data, was "openpyxl-3.2.0b1.tar", last modified: Thu May 19 15:22:22 2022, max compression
```

## Comparing `openpyxl-3.1.2.tar` & `openpyxl-3.2.0b1.tar`

### file list

```diff
@@ -1,223 +1,224 @@
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.283453 openpyxl-3.1.2/
--rw-r--r--   0 charlieclark   (501) staff       (20)     1773 2023-01-31 14:42:06.000000 openpyxl-3.1.2/AUTHORS.rst
--rw-r--r--   0 charlieclark   (501) staff       (20)     1131 2021-10-07 16:20:11.000000 openpyxl-3.1.2/LICENCE.rst
--rw-r--r--   0 charlieclark   (501) staff       (20)      113 2021-10-07 16:20:11.000000 openpyxl-3.1.2/MANIFEST.in
--rw-r--r--   0 charlieclark   (501) staff       (20)     2484 2023-03-11 16:54:22.283666 openpyxl-3.1.2/PKG-INFO
--rw-r--r--   0 charlieclark   (501) staff       (20)     1388 2021-10-07 16:20:11.000000 openpyxl-3.1.2/README.rst
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.174456 openpyxl-3.1.2/openpyxl/
--rw-r--r--   0 charlieclark   (501) staff       (20)      603 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      306 2023-03-11 16:50:56.000000 openpyxl-3.1.2/openpyxl/_constants.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.181964 openpyxl-3.1.2/openpyxl/cell/
--rw-r--r--   0 charlieclark   (501) staff       (20)      122 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/cell/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4950 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/cell/_writer.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     8948 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/cell/cell.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3113 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/cell/read_only.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4818 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/cell/rich_text.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4367 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/cell/text.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.202983 openpyxl-3.1.2/openpyxl/chart/
--rw-r--r--   0 charlieclark   (501) staff       (20)     3104 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/_3d.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      564 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5776 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/chart/_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2925 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/area_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    12657 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/axis.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4175 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/bar_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2021 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/chart/bubble_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6085 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/chartspace.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5809 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/chart/data_source.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      764 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/descriptors.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1832 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/error_bar.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4167 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/label.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2040 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/layout.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2040 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/legend.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3986 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/chart/line_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2600 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/marker.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1156 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/picture.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4868 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/chart/pie_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1741 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/pivot.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5832 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/plotarea.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1454 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/print_settings.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1537 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/radar_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      802 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/chart/reader.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3098 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/chart/reference.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1581 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/scatter_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5908 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/series.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1368 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/series_factory.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2815 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/shapes.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1620 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/stock_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2955 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/surface_chart.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1857 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/text.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1973 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/title.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3053 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/trendline.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      897 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chart/updown_bars.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.209948 openpyxl-3.1.2/openpyxl/chartsheet/
--rw-r--r--   0 charlieclark   (501) staff       (20)       71 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chartsheet/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3943 2023-02-13 16:42:21.000000 openpyxl-3.1.2/openpyxl/chartsheet/chartsheet.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1691 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chartsheet/custom.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      679 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chartsheet/properties.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1265 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/chartsheet/protection.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1587 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chartsheet/publish.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2731 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/chartsheet/relation.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1341 2023-02-13 16:42:21.000000 openpyxl-3.1.2/openpyxl/chartsheet/views.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.212774 openpyxl-3.1.2/openpyxl/comments/
--rw-r--r--   0 charlieclark   (501) staff       (20)       67 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/comments/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      388 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/comments/author.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5771 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/comments/comment_sheet.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1474 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/comments/comments.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3817 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/comments/shape_writer.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.216247 openpyxl-3.1.2/openpyxl/compat/
--rw-r--r--   0 charlieclark   (501) staff       (20)     1592 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/compat/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      155 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/compat/abc.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1617 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/compat/numbers.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      264 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/compat/product.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1083 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/compat/singleton.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      604 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/compat/strings.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.219321 openpyxl-3.1.2/openpyxl/descriptors/
--rw-r--r--   0 charlieclark   (501) staff       (20)     1952 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/descriptors/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     7359 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/descriptors/base.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2443 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/descriptors/excel.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      313 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/descriptors/namespace.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2656 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/descriptors/nested.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3490 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/descriptors/sequence.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     7361 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/descriptors/serialisable.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      824 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/descriptors/slots.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.226120 openpyxl-3.1.2/openpyxl/drawing/
--rw-r--r--   0 charlieclark   (501) staff       (20)       66 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/drawing/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    15278 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/colors.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3863 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/connector.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2347 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/drawing/drawing.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     9515 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/effect.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    13092 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/fill.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    17523 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/geometry.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4811 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/graphic.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1463 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/image.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3904 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/drawing/line.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4205 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/picture.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4948 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/properties.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      344 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/drawing/relation.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    10762 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/spreadsheet_drawing.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    22421 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/drawing/text.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      626 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/drawing/xdr.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.227553 openpyxl-3.1.2/openpyxl/formatting/
--rw-r--r--   0 charlieclark   (501) staff       (20)       59 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/formatting/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2709 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/formatting/formatting.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     9309 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/formatting/rule.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.228750 openpyxl-3.1.2/openpyxl/formula/
--rw-r--r--   0 charlieclark   (501) staff       (20)       69 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/formula/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    15104 2022-08-24 15:09:39.000000 openpyxl-3.1.2/openpyxl/formula/tokenizer.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6661 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/formula/translate.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.232765 openpyxl-3.1.2/openpyxl/packaging/
--rw-r--r--   0 charlieclark   (501) staff       (20)       90 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/packaging/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3955 2023-02-13 16:42:21.000000 openpyxl-3.1.2/openpyxl/packaging/core.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6725 2023-03-11 16:50:56.000000 openpyxl-3.1.2/openpyxl/packaging/custom.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4755 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/packaging/extended.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      920 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/packaging/interface.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5380 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/packaging/manifest.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4319 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/packaging/relationship.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6516 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/packaging/workbook.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.235465 openpyxl-3.1.2/openpyxl/pivot/
--rw-r--r--   0 charlieclark   (501) staff       (20)       35 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/pivot/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    30587 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/pivot/cache.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6984 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/pivot/fields.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2687 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/pivot/record.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    40777 2023-03-11 16:50:56.000000 openpyxl-3.1.2/openpyxl/pivot/table.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.238545 openpyxl-3.1.2/openpyxl/reader/
--rw-r--r--   0 charlieclark   (501) staff       (20)       35 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/reader/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2188 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/reader/drawings.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    12286 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/reader/excel.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1113 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/reader/strings.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4338 2023-03-11 16:50:56.000000 openpyxl-3.1.2/openpyxl/reader/workbook.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.248260 openpyxl-3.1.2/openpyxl/styles/
--rw-r--r--   0 charlieclark   (501) staff       (20)      363 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2512 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/alignment.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3594 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/borders.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    31182 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/builtins.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5304 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/cell_style.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4653 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/colors.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2267 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/differential.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6412 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/fills.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3525 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/fonts.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     7464 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/named_styles.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5122 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/numbers.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      394 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/protection.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1456 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/proxy.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4565 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/styleable.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     8535 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/stylesheet.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2801 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/styles/table.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.255999 openpyxl-3.1.2/openpyxl/utils/
--rw-r--r--   0 charlieclark   (501) staff       (20)      324 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      759 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/bound_dictionary.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6536 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/cell.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2957 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/dataframe.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4529 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/utils/datetime.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      790 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/escape.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      889 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/exceptions.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4240 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/formulas.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1257 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/indexed_list.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1583 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/inference.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      830 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/protection.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2642 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/utils/units.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.261704 openpyxl-3.1.2/openpyxl/workbook/
--rw-r--r--   0 charlieclark   (501) staff       (20)       68 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6506 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/workbook/_writer.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4060 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/child.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5394 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/defined_name.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.262677 openpyxl-3.1.2/openpyxl/workbook/external_link/
--rw-r--r--   0 charlieclark   (501) staff       (20)       71 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/external_link/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4555 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/external_link/external.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      348 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/external_reference.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      803 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/function_group.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5261 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/properties.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6031 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/protection.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1181 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/smart_tags.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5214 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/views.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2642 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/workbook/web.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    13240 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/workbook/workbook.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.279494 openpyxl-3.1.2/openpyxl/worksheet/
--rw-r--r--   0 charlieclark   (501) staff       (20)       35 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5545 2023-03-11 16:50:56.000000 openpyxl-3.1.2/openpyxl/worksheet/_read_only.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    16383 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/worksheet/_reader.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4256 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/_write_only.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    10318 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/worksheet/_writer.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    15013 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/cell_range.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      608 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/worksheet/cell_watch.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2735 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/worksheet/controls.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2327 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/copier.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      639 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/worksheet/custom.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     6156 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/datavalidation.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     8877 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/dimensions.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      275 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/drawing.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2435 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/worksheet/errors.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    11556 2023-03-07 16:22:57.000000 openpyxl-3.1.2/openpyxl/worksheet/filters.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1045 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/formula.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     7886 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/header_footer.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1391 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/worksheet/hyperlink.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4140 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/merge.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3530 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/worksheet/ole.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4920 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/page.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1811 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/pagebreak.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      185 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/worksheet/picture.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     5215 2023-03-11 16:50:56.000000 openpyxl-3.1.2/openpyxl/worksheet/print_settings.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3087 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/properties.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     3787 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/protection.py
--rw-r--r--   0 charlieclark   (501) staff       (20)      348 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/related.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2401 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/scenario.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     1608 2021-10-07 16:20:11.000000 openpyxl-3.1.2/openpyxl/worksheet/smart_tag.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    11740 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/table.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4632 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/worksheet/views.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    27508 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/worksheet/worksheet.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.281334 openpyxl-3.1.2/openpyxl/writer/
--rw-r--r--   0 charlieclark   (501) staff       (20)       35 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/writer/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     9539 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/writer/excel.py
--rw-r--r--   0 charlieclark   (501) staff       (20)    10320 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/writer/theme.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.283031 openpyxl-3.1.2/openpyxl/xml/
--rw-r--r--   0 charlieclark   (501) staff       (20)     1016 2023-02-01 15:19:11.000000 openpyxl-3.1.2/openpyxl/xml/__init__.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     4833 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/xml/constants.py
--rw-r--r--   0 charlieclark   (501) staff       (20)     2025 2023-03-11 16:16:45.000000 openpyxl-3.1.2/openpyxl/xml/functions.py
-drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2023-03-11 16:54:22.177901 openpyxl-3.1.2/openpyxl.egg-info/
--rw-r--r--   0 charlieclark   (501) staff       (20)     2484 2023-03-11 16:54:22.000000 openpyxl-3.1.2/openpyxl.egg-info/PKG-INFO
--rw-r--r--   0 charlieclark   (501) staff       (20)     5718 2023-03-11 16:54:22.000000 openpyxl-3.1.2/openpyxl.egg-info/SOURCES.txt
--rw-r--r--   0 charlieclark   (501) staff       (20)        1 2023-03-11 16:54:22.000000 openpyxl-3.1.2/openpyxl.egg-info/dependency_links.txt
--rw-r--r--   0 charlieclark   (501) staff       (20)       11 2023-03-11 16:54:22.000000 openpyxl-3.1.2/openpyxl.egg-info/requires.txt
--rw-r--r--   0 charlieclark   (501) staff       (20)        9 2023-03-11 16:54:22.000000 openpyxl-3.1.2/openpyxl.egg-info/top_level.txt
--rw-r--r--   0 charlieclark   (501) staff       (20)      106 2023-03-11 16:54:22.284206 openpyxl-3.1.2/setup.cfg
--rwxr-xr-x   0 charlieclark   (501) staff       (20)     2893 2023-02-01 15:19:11.000000 openpyxl-3.1.2/setup.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.680154 openpyxl-3.2.0b1/
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1773 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/AUTHORS.rst
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1131 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/LICENCE.rst
+-rw-r--r--   0 charlieclark   (501) staff       (20)      113 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/MANIFEST.in
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2404 2022-05-19 15:22:22.680315 openpyxl-3.2.0b1/PKG-INFO
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1388 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/README.rst
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.601801 openpyxl-3.2.0b1/openpyxl/
+-rw-r--r--   0 charlieclark   (501) staff       (20)      589 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      308 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/_constants.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.606860 openpyxl-3.2.0b1/openpyxl/cell/
+-rw-r--r--   0 charlieclark   (501) staff       (20)      122 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/cell/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4950 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/cell/_writer.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     8948 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/cell/cell.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3113 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/cell/read_only.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4818 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/cell/rich_text.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4367 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/cell/text.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.622599 openpyxl-3.2.0b1/openpyxl/chart/
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3104 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/_3d.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      564 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6032 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/chart/_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2925 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/area_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    12657 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/axis.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4175 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/bar_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2021 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/chart/bubble_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6085 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/chart/chartspace.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5809 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/chart/data_source.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      764 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/descriptors.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1832 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/error_bar.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4167 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/label.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2040 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/layout.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2040 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/legend.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3986 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/chart/line_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2600 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/marker.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1156 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/picture.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4868 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/chart/pie_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1741 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/pivot.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5832 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/plotarea.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1454 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/print_settings.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1537 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/radar_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      851 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/chart/reader.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3089 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/chart/reference.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1559 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/scatter_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5908 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/series.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1368 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/series_factory.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2815 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/shapes.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1620 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/stock_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2955 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/surface_chart.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1857 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/text.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1973 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/title.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3053 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/trendline.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      897 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chart/updown_bars.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.625242 openpyxl-3.2.0b1/openpyxl/chartsheet/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       71 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4042 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/chartsheet.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1691 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/custom.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      679 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/properties.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1265 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/protection.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1587 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/publish.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2731 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/relation.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1341 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/chartsheet/views.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.626828 openpyxl-3.2.0b1/openpyxl/comments/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       67 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/comments/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      388 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/comments/author.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5874 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/comments/comment_sheet.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1474 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/comments/comments.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4063 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/comments/shape_writer.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.628440 openpyxl-3.2.0b1/openpyxl/compat/
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1592 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/compat/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      155 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/compat/abc.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1617 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/compat/numbers.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      264 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/compat/product.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1083 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/compat/singleton.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      604 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/compat/strings.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.632417 openpyxl-3.2.0b1/openpyxl/descriptors/
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1816 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/descriptors/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     7142 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/descriptors/base.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2438 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/descriptors/excel.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      309 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/descriptors/namespace.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2651 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/descriptors/nested.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3380 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/descriptors/sequence.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     7343 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/descriptors/serialisable.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      824 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/descriptors/slots.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.637194 openpyxl-3.2.0b1/openpyxl/drawing/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       66 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5428 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/anchor.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    15255 2022-05-19 15:20:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/colors.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3982 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/connector.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2785 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/drawing.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     9589 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/effect.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    13285 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/fill.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    19642 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/geometry.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4876 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/graphic.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2419 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/image.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      675 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/legacy.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4105 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/line.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4338 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/picture.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5030 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/properties.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      344 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/relation.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     9302 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/spreadsheet_drawing.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    22454 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/drawing/text.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      626 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/drawing/xdr.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.638255 openpyxl-3.2.0b1/openpyxl/formatting/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       59 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/formatting/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2805 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/formatting/formatting.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     9308 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/formatting/rule.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.639431 openpyxl-3.2.0b1/openpyxl/formula/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       69 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/formula/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    15104 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/formula/tokenizer.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6661 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/formula/translate.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.642124 openpyxl-3.2.0b1/openpyxl/packaging/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       90 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/packaging/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4011 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/packaging/core.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5407 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/packaging/custom.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4755 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/packaging/extended.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      920 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/packaging/interface.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5817 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/packaging/manifest.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4824 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/packaging/relationship.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     7024 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/packaging/workbook.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.644603 openpyxl-3.2.0b1/openpyxl/pivot/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       35 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/pivot/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    30587 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/pivot/cache.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6984 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/pivot/fields.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2687 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/pivot/record.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    37786 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/pivot/table.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.647387 openpyxl-3.2.0b1/openpyxl/reader/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       35 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/reader/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2330 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/reader/drawings.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    15274 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/reader/excel.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1113 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/reader/strings.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3921 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/reader/workbook.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.655105 openpyxl-3.2.0b1/openpyxl/styles/
+-rw-r--r--   0 charlieclark   (501) staff       (20)      363 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2512 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/alignment.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3594 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/borders.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    31182 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/builtins.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5304 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/cell_style.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4653 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/colors.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2267 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/differential.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6443 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/fills.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3525 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/fonts.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     7464 2022-05-19 15:16:25.000000 openpyxl-3.2.0b1/openpyxl/styles/named_styles.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5120 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/numbers.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      394 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/protection.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1456 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/proxy.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4565 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/styleable.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     8535 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/stylesheet.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2801 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/styles/table.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.660163 openpyxl-3.2.0b1/openpyxl/utils/
+-rw-r--r--   0 charlieclark   (501) staff       (20)      324 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      759 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/bound_dictionary.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6535 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/cell.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2596 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/dataframe.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4529 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/datetime.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      790 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/escape.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      889 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/exceptions.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3733 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/formulas.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1257 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/indexed_list.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1582 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/inference.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      830 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/protection.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2674 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/utils/units.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.665901 openpyxl-3.2.0b1/openpyxl/workbook/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       68 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6699 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/workbook/_writer.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4060 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/child.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     7444 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/defined_name.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.666650 openpyxl-3.2.0b1/openpyxl/workbook/external_link/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       71 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/external_link/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4555 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/external_link/external.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      348 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/external_reference.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      803 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/function_group.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5261 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/properties.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6031 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/protection.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1181 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/smart_tags.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5214 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/views.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2642 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/workbook/web.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    14091 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/workbook/workbook.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.677674 openpyxl-3.2.0b1/openpyxl/worksheet/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       35 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5439 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/_read_only.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    16555 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/worksheet/_reader.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4256 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/_write_only.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    11565 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/worksheet/_writer.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    14642 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/cell_range.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      608 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/worksheet/cell_watch.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     9584 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/worksheet/controls.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2327 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/copier.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      639 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/worksheet/custom.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     6136 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/datavalidation.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     8877 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/dimensions.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      275 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/drawing.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2435 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/worksheet/errors.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    11439 2022-05-19 15:16:26.000000 openpyxl-3.2.0b1/openpyxl/worksheet/filters.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1045 2022-05-19 15:16:26.000000 openpyxl-3.2.0b1/openpyxl/worksheet/formula.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     7886 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/header_footer.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1391 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/worksheet/hyperlink.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4140 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/merge.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3871 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/worksheet/ole.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4920 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/page.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1811 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/pagebreak.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      185 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/worksheet/picture.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3087 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/properties.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     3787 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/protection.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)      348 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/related.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2401 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/scenario.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1608 2021-10-07 16:20:11.000000 openpyxl-3.2.0b1/openpyxl/worksheet/smart_tag.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    11716 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/table.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     4632 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/worksheet/views.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    27528 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/worksheet/worksheet.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.678612 openpyxl-3.2.0b1/openpyxl/writer/
+-rw-r--r--   0 charlieclark   (501) staff       (20)       35 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/writer/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    12184 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/writer/excel.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)    10320 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/writer/theme.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.679920 openpyxl-3.2.0b1/openpyxl/xml/
+-rw-r--r--   0 charlieclark   (501) staff       (20)     1016 2022-05-19 15:13:48.000000 openpyxl-3.2.0b1/openpyxl/xml/__init__.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5088 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/xml/constants.py
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2042 2022-05-19 15:20:49.000000 openpyxl-3.2.0b1/openpyxl/xml/functions.py
+drwxr-xr-x   0 charlieclark   (501) staff       (20)        0 2022-05-19 15:22:22.603403 openpyxl-3.2.0b1/openpyxl.egg-info/
+-rw-r--r--   0 charlieclark   (501) staff       (20)     2404 2022-05-19 15:22:22.000000 openpyxl-3.2.0b1/openpyxl.egg-info/PKG-INFO
+-rw-r--r--   0 charlieclark   (501) staff       (20)     5735 2022-05-19 15:22:22.000000 openpyxl-3.2.0b1/openpyxl.egg-info/SOURCES.txt
+-rw-r--r--   0 charlieclark   (501) staff       (20)        1 2022-05-19 15:22:22.000000 openpyxl-3.2.0b1/openpyxl.egg-info/dependency_links.txt
+-rw-r--r--   0 charlieclark   (501) staff       (20)       11 2022-05-19 15:22:22.000000 openpyxl-3.2.0b1/openpyxl.egg-info/requires.txt
+-rw-r--r--   0 charlieclark   (501) staff       (20)        9 2022-05-19 15:22:22.000000 openpyxl-3.2.0b1/openpyxl.egg-info/top_level.txt
+-rw-r--r--   0 charlieclark   (501) staff       (20)      106 2022-05-19 15:22:22.680769 openpyxl-3.2.0b1/setup.cfg
+-rwxr-xr-x   0 charlieclark   (501) staff       (20)     2775 2022-03-08 15:06:53.000000 openpyxl-3.2.0b1/setup.py
```

### Comparing `openpyxl-3.1.2/AUTHORS.rst` & `openpyxl-3.2.0b1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/LICENCE.rst` & `openpyxl-3.2.0b1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/PKG-INFO` & `openpyxl-3.2.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: openpyxl
-Version: 3.1.2
+Version: 3.2.0b1
 Summary: A Python library to read/write Excel 2010 xlsx/xlsm files
 Home-page: https://openpyxl.readthedocs.io
 Author: See AUTHORS
 Author-email: charlie.clark@clark-consulting.eu
 License: MIT
 Project-URL: Documentation, https://openpyxl.readthedocs.io/en/stable/
 Project-URL: Source, https://foss.heptapod.net/openpyxl/openpyxl
 Project-URL: Tracker, https://foss.heptapod.net/openpyxl/openpyxl/-/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENCE.rst
 
 .. image:: https://coveralls.io/repos/bitbucket/openpyxl/openpyxl/badge.svg?branch=default
     :target: https://coveralls.io/bitbucket/openpyxl/openpyxl?branch=default
     :alt: coverage status
 
 Introduction
@@ -79,7 +78,9 @@
 The documentation is at: https://openpyxl.readthedocs.io
 
 * installation methods
 * code examples
 * instructions for contributing
 
 Release notes: https://openpyxl.readthedocs.io/en/stable/changes.html
+
+
```

### Comparing `openpyxl-3.1.2/README.rst` & `openpyxl-3.2.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/__init__.py` & `openpyxl-3.2.0b1/openpyxl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
-DEBUG = False
 
 from openpyxl.compat.numbers import NUMPY
 from openpyxl.xml import DEFUSEDXML, LXML
 from openpyxl.workbook import Workbook
 from openpyxl.reader.excel import load_workbook as open
 from openpyxl.reader.excel import load_workbook
 import openpyxl._constants as constants
```

### Comparing `openpyxl-3.1.2/openpyxl/cell/_writer.py` & `openpyxl-3.2.0b1/openpyxl/cell/_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.compat import safe_string
 from openpyxl.xml.functions import Element, SubElement, whitespace, XML_NS, REL_NS
 from openpyxl import LXML
 from openpyxl.utils.datetime import to_excel, to_ISO8601
 from datetime import timedelta
```

### Comparing `openpyxl-3.1.2/openpyxl/cell/cell.py` & `openpyxl-3.2.0b1/openpyxl/cell/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Manage individual cells in a spreadsheet.
 
 The Cell class is required to know its value and type, display options,
 and any other features of an Excel cell.  Utilities for referencing
 cells using Excel's 'A1' column/row nomenclature are also provided.
```

### Comparing `openpyxl-3.1.2/openpyxl/cell/read_only.py` & `openpyxl-3.2.0b1/openpyxl/cell/read_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.cell import Cell
 from openpyxl.utils import get_column_letter
 from openpyxl.utils.datetime import from_excel
 from openpyxl.styles import is_date_format
 from openpyxl.styles.numbers import BUILTIN_FORMATS, BUILTIN_FORMATS_MAX_SIZE
```

### Comparing `openpyxl-3.1.2/openpyxl/cell/rich_text.py` & `openpyxl-3.2.0b1/openpyxl/cell/rich_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 RichText definition
 """
 from copy import copy
 from openpyxl.cell.text import InlineFont, Text
 from openpyxl.descriptors import (
```

### Comparing `openpyxl-3.1.2/openpyxl/cell/text.py` & `openpyxl-3.2.0b1/openpyxl/cell/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 Richtext definition
 """
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/_3d.py` & `openpyxl-3.2.0b1/openpyxl/chart/_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import Typed, Alias
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors.nested import (
     NestedBool,
     NestedInteger,
     NestedMinMax,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/__init__.py` & `openpyxl-3.2.0b1/openpyxl/chart/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from .area_chart import AreaChart, AreaChart3D
 from .bar_chart import BarChart, BarChart3D
 from .bubble_chart import BubbleChart
 from .line_chart import LineChart, LineChart3D
 from .pie_chart import (
     PieChart,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/_chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from collections import OrderedDict
 from operator import attrgetter
 
 from openpyxl.descriptors import (
     Typed,
     Integer,
@@ -59,14 +59,16 @@
     width = 15 # in cm, approx 5 rows
     height = 7.5 # in cm, approx 14 rows
     _id = 1
     _path = "/xl/charts/chart{0}.xml"
     style = MinMax(allow_none=True, min=1, max=48)
     mime_type = "application/vnd.openxmlformats-officedocument.drawingml.chart+xml"
     graphical_properties = Typed(expected_type=GraphicalProperties, allow_none=True) # mapped to chartspace
+    hidden = Bool(allow_none=True) # mapped to GraphicFrame in parent drawing
+    hide_title = Bool(allow_none=True) # mapped to Chart Container
 
     __elements__ = ()
 
 
     def __init__(self, axId=(), **kw):
         self._charts = [self]
         self.title = None
@@ -79,14 +81,16 @@
         self.axId = axId
         self.display_blanks = 'gap'
         self.pivotSource = None
         self.pivotFormats = ()
         self.visible_cells_only = True
         self.idx_base = 0
         self.graphical_properties = None
+        self.hidden = None
+        self.hide_title = None
         super(ChartBase, self).__init__()
 
 
     def __hash__(self):
         """
         Just need to check for identity
         """
@@ -138,14 +142,15 @@
             container.view3D = chart.view3D
             container.floor = chart.floor
             container.sideWall = chart.sideWall
             container.backWall = chart.backWall
         container.plotVisOnly = self.visible_cells_only
         container.dispBlanksAs = self.display_blanks
         container.pivotFmts = self.pivotFormats
+        container.autoTitleDeleted = self.hide_title
         cs = ChartSpace(chart=container)
         cs.style = self.style
         cs.roundedCorners = self.roundedCorners
         cs.pivotSource = self.pivotSource
         cs.spPr = self.graphical_properties
         return cs.to_tree()
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/area_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/area_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Set,
     Bool,
     Integer,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/axis.py` & `openpyxl-3.2.0b1/openpyxl/chart/axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Float,
     NoneSet,
     Bool,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/bar_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/bar_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Bool,
     Integer,
     Sequence,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/bubble_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/bubble_chart.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/chart/chartspace.py` & `openpyxl-3.2.0b1/openpyxl/chart/chartspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 Enclosing chart object. The various chart types are actually child objects.
 Will probably need to call this indirectly
 """
 
 from openpyxl.descriptors.serialisable import Serialisable
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/data_source.py` & `openpyxl-3.2.0b1/openpyxl/chart/data_source.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/chart/descriptors.py` & `openpyxl-3.2.0b1/openpyxl/chart/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 
 from openpyxl.descriptors.nested import (
     NestedMinMax
     )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/error_bar.py` & `openpyxl-3.2.0b1/openpyxl/chart/error_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Float,
     Set,
     Alias
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/label.py` & `openpyxl-3.2.0b1/openpyxl/chart/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Sequence,
     Alias,
     Typed
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/layout.py` & `openpyxl-3.2.0b1/openpyxl/chart/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     NoneSet,
     Float,
     Typed,
     Alias,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/legend.py` & `openpyxl-3.2.0b1/openpyxl/chart/legend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Integer,
     Alias,
     Sequence,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/line_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/line_chart.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/chart/marker.py` & `openpyxl-3.2.0b1/openpyxl/chart/marker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Alias,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/picture.py` & `openpyxl-3.2.0b1/openpyxl/chart/picture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 
 from openpyxl.descriptors.nested import (
     NestedBool,
     NestedFloat,
     NestedMinMax,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/pie_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/pie_chart.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/chart/pivot.py` & `openpyxl-3.2.0b1/openpyxl/chart/pivot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Typed,
 )
 from openpyxl.descriptors.nested import NestedInteger, NestedText
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/plotarea.py` & `openpyxl-3.2.0b1/openpyxl/chart/plotarea.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Alias,
 )
 from openpyxl.descriptors.excel import (
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/print_settings.py` & `openpyxl-3.2.0b1/openpyxl/chart/print_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Float,
     Typed,
     Alias,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/radar_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/radar_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Sequence,
     Typed,
     Alias,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/reader.py` & `openpyxl-3.2.0b1/openpyxl/chart/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 Read a chart
 """
 
 def read_chart(chartspace):
     cs = chartspace
@@ -12,14 +12,15 @@
     chart._charts = plot._charts
 
     chart.title = cs.chart.title
     chart.display_blanks = cs.chart.dispBlanksAs
     chart.visible_cells_only = cs.chart.plotVisOnly
     chart.layout = plot.layout
     chart.legend = cs.chart.legend
+    chart.hide_title = cs.chart.autoTitleDeleted
 
     # 3d attributes
     chart.floor = cs.chart.floor
     chart.sideWall = cs.chart.sideWall
     chart.backWall = cs.chart.backWall
     chart.pivotSource = cs.pivotSource
     chart.pivotFormats = cs.chart.pivotFmts
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/reference.py` & `openpyxl-3.2.0b1/openpyxl/chart/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
-from itertools import chain
+#from itertools import chain
 
-from openpyxl.descriptors.serialisable import Serialisable
+#from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     MinMax,
-    Typed,
     String,
     Strict,
 )
-from openpyxl.worksheet.worksheet import Worksheet
+#from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.utils import (
     get_column_letter,
     range_to_tuple,
     quote_sheetname
 )
 
 
@@ -74,15 +73,14 @@
                           get_column_letter(self.max_col), self.max_row
                           )
 
 
     __str__ = __str__
 
 
-
     def __len__(self):
         if self.min_row == self.max_row:
             return 1 + self.max_col - self.min_col
         return 1 + self.max_row - self.min_row
 
 
     def __eq__(self, other):
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/scatter_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/scatter_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Sequence,
     Alias
 )
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.nested import (
     NestedNoneSet,
     NestedBool,
 )
 
 from ._chart import ChartBase
-from .axis import NumericAxis, TextAxis
+from .axis import NumericAxis
 from .series import XYSeries
 from .label import DataLabelList
 
 
 class ScatterChart(ChartBase):
 
     tagname = "scatterChart"
@@ -25,15 +25,15 @@
     scatterStyle = NestedNoneSet(values=(['line', 'lineMarker', 'marker', 'smooth', 'smoothMarker']))
     varyColors = NestedBool(allow_none=True)
     ser = Sequence(expected_type=XYSeries, allow_none=True)
     dLbls = Typed(expected_type=DataLabelList, allow_none=True)
     dataLabels = Alias("dLbls")
     extLst = Typed(expected_type=ExtensionList, allow_none=True)
 
-    x_axis = Typed(expected_type=(NumericAxis, TextAxis))
+    x_axis = Typed(expected_type=NumericAxis)
     y_axis = Typed(expected_type=NumericAxis)
 
     _series_type = "scatter"
 
     __elements__ = ('scatterStyle', 'varyColors', 'ser', 'dLbls', 'axId',)
 
     def __init__(self,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/series.py` & `openpyxl-3.2.0b1/openpyxl/chart/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     String,
     Integer,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/series_factory.py` & `openpyxl-3.2.0b1/openpyxl/chart/series_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from .data_source import NumDataSource, NumRef, AxDataSource
 from .reference import Reference
 from .series import Series, XYSeries, SeriesLabel, StrRef
 from  openpyxl.utils import rows_from_range, quote_sheetname
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/shapes.py` & `openpyxl-3.2.0b1/openpyxl/chart/shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Alias
 )
 from openpyxl.descriptors.nested import (
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/stock_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/stock_chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Sequence,
     Alias,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/surface_chart.py` & `openpyxl-3.2.0b1/openpyxl/chart/surface_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Integer,
     Bool,
     Alias,
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/text.py` & `openpyxl-3.2.0b1/openpyxl/chart/text.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Alias,
     Sequence,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/title.py` & `openpyxl-3.2.0b1/openpyxl/chart/title.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Alias,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/trendline.py` & `openpyxl-3.2.0b1/openpyxl/chart/trendline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     String,
     Alias
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/chart/updown_bars.py` & `openpyxl-3.2.0b1/openpyxl/chart/updown_bars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import Typed
 from openpyxl.descriptors.excel import ExtensionList
 
 from .shapes import GraphicalProperties
 from .axis import ChartLines
```

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/chartsheet.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/chartsheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
+from weakref import ref
 
 from openpyxl.descriptors import Typed, Set, Alias
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.spreadsheet_drawing import (
     AbsoluteAnchor,
     SpreadsheetDrawing,
 )
 from openpyxl.worksheet.page import (
     PageMargins,
     PrintPageSetup
 )
+from openpyxl.packaging.relationship import Relationship, RelationshipList
 from openpyxl.worksheet.drawing import Drawing
 from openpyxl.worksheet.header_footer import HeaderFooter
 from openpyxl.workbook.child import _WorkbookChild
 from openpyxl.xml.constants import SHEET_MAIN_NS, REL_NS
 
 from .relation import DrawingHF, SheetBackgroundPicture
 from .properties import ChartsheetProperties
```

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/custom.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.worksheet.header_footer import HeaderFooter
 
 from openpyxl.descriptors import (
     Bool,
     Integer,
     Set,
```

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/properties.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/properties.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Bool,
     String,
     Typed
 )
 from openpyxl.descriptors.serialisable import Serialisable
```

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/protection.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/protection.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/publish.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/publish.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Bool,
     Integer,
     String,
     Set,
     Sequence
```

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/relation.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Integer,
     Alias
 )
 from openpyxl.descriptors.excel import Relation
 from openpyxl.descriptors.serialisable import Serialisable
```

### Comparing `openpyxl-3.1.2/openpyxl/chartsheet/views.py` & `openpyxl-3.2.0b1/openpyxl/chartsheet/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Bool,
     Integer,
     Typed,
     Sequence
 )
@@ -21,15 +21,15 @@
 
     __elements__ = ()
 
     def __init__(self,
                  tabSelected=None,
                  zoomScale=None,
                  workbookViewId=0,
-                 zoomToFit=True,
+                 zoomToFit=None,
                  extLst=None,
                  ):
         self.tabSelected = tabSelected
         self.zoomScale = zoomScale
         self.workbookViewId = workbookViewId
         self.zoomToFit = zoomToFit
```

### Comparing `openpyxl-3.1.2/openpyxl/comments/comment_sheet.py` & `openpyxl-3.2.0b1/openpyxl/comments/comment_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 ## Incomplete!
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
+    Float,
     Integer,
     Set,
     String,
     Bool,
 )
 from openpyxl.descriptors.excel import Guid, ExtensionList
 from openpyxl.descriptors.sequence import NestedSequence
 
 from openpyxl.utils.indexed_list import IndexedList
 from openpyxl.xml.constants import SHEET_MAIN_NS
+from openpyxl.xml.functions import tostring
 
 from openpyxl.cell.text import Text
+#from openpyxl.worksheet.ole import ObjectAnchor
 from .author import AuthorList
 from .comments import Comment
 from .shape_writer import ShapeWriter
 
 
 class Properties(Serialisable):
 
@@ -34,15 +37,15 @@
     textHAlign = Set(values=(['left', 'center', 'right', 'justify', 'distributed']))
     textVAlign = Set(values=(['top', 'center', 'bottom', 'justify', 'distributed']))
     lockText = Bool(allow_none=True)
     justLastX = Bool(allow_none=True)
     autoScale = Bool(allow_none=True)
     rowHidden = Bool(allow_none=True)
     colHidden = Bool(allow_none=True)
-    # anchor = Typed(expected_type=ObjectAnchor, )
+    #anchor = Typed(expected_type=ObjectAnchor, )
 
     __elements__ = ('anchor',)
 
     def __init__(self,
                  locked=None,
                  defaultSize=None,
                  _print=None,
```

### Comparing `openpyxl-3.1.2/openpyxl/comments/comments.py` & `openpyxl-3.2.0b1/openpyxl/comments/comments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 class Comment(object):
 
     _parent = None
 
     def __init__(self, text, author, height=79, width=144):
```

### Comparing `openpyxl-3.1.2/openpyxl/comments/shape_writer.py` & `openpyxl-3.2.0b1/openpyxl/comments/shape_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.xml.functions import (
     Element,
     SubElement,
     tostring,
+    fromstring,
 )
 
-from openpyxl.utils import coordinate_to_tuple
+from openpyxl.utils import (
+    coordinate_to_tuple,
+)
 
 vmlns = "urn:schemas-microsoft-com:vml"
 officens = "urn:schemas-microsoft-com:office:office"
 excelns = "urn:schemas-microsoft-com:office:excel"
 
 
+VML_ROOT = """
+<xml xmlns:v="urn:schemas-microsoft-com:vml"
+ xmlns:o="urn:schemas-microsoft-com:office:office"
+ xmlns:x="urn:schemas-microsoft-com:office:excel" />
+"""
+
 class ShapeWriter(object):
     """
     Create VML for comments
     """
 
     vml = None
     vml_path = None
@@ -53,25 +62,28 @@
 
         shape.set('id', "_x0000_s%04d" % idx)
         root.append(shape)
 
 
     def write(self, root):
 
+        if root is None:
+            root = VML_ROOT
+
         if not hasattr(root, "findall"):
-            root = Element("xml")
+            root = fromstring(root)
 
         # Remove any existing comment shapes
         comments = root.findall("{%s}shape[@type='#_x0000_t202']" % vmlns)
         for c in comments:
             root.remove(c)
 
         # check whether comments shape type already exists
         shape_types = root.find("{%s}shapetype[@id='_x0000_t202']" % vmlns)
-        if shape_types is None:
+        if not shape_types:
             self.add_comment_shapetype(root)
 
         for idx, (coord, comment) in enumerate(self.comments, 1026):
             self.add_comment_shape(root, idx, coord, comment.height, comment.width)
 
         return tostring(root)
```

### Comparing `openpyxl-3.1.2/openpyxl/compat/__init__.py` & `openpyxl-3.2.0b1/openpyxl/compat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from .numbers import NUMERIC_TYPES
 from .strings import safe_string
 
 import warnings
 from functools import wraps
 import inspect
```

### Comparing `openpyxl-3.1.2/openpyxl/compat/numbers.py` & `openpyxl-3.2.0b1/openpyxl/compat/numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from decimal import Decimal
 
 NUMERIC_TYPES = (int, float, Decimal)
 
 
 try:
```

### Comparing `openpyxl-3.1.2/openpyxl/compat/singleton.py` & `openpyxl-3.2.0b1/openpyxl/compat/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import weakref
 
 
 class Singleton(type):
     """
     Singleton metaclass
```

### Comparing `openpyxl-3.1.2/openpyxl/compat/strings.py` & `openpyxl-3.2.0b1/openpyxl/compat/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from datetime import datetime
 from math import isnan, isinf
 import sys
 
 VER = sys.version_info
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/__init__.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from .base import *
 from .sequence import Sequence
 
 
 class MetaStrict(type):
 
     def __new__(cls, clsname, bases, methods):
         for k, v in methods.items():
             if isinstance(v, Descriptor):
                 v.name = k
         return type.__new__(cls, clsname, bases, methods)
 
 
-class Strict(metaclass=MetaStrict):
-
-    pass
-
-
 class MetaSerialisable(type):
 
     def __new__(cls, clsname, bases, methods):
         attrs = []
         nested = []
         elements = []
         namespaced = []
@@ -34,25 +29,29 @@
                     nested.append(k)
                     elements.append(k)
                 elif isinstance(v, Sequence):
                     elements.append(k)
                 elif isinstance(v, Typed):
                     if hasattr(v.expected_type, 'to_tree'):
                         elements.append(k)
-                    elif isinstance(v.expected_type, tuple):
-                        if any((hasattr(el, "to_tree") for el in v.expected_type)):
-                            # don't bind elements as attrs
-                            continue
                     else:
                         attrs.append(k)
                 else:
                     if not isinstance(v, Alias):
                         attrs.append(k)
 
         if methods.get('__attrs__') is None:
             methods['__attrs__'] = tuple(attrs)
         methods['__namespaced__'] = tuple(namespaced)
         if methods.get('__nested__') is None:
             methods['__nested__'] = tuple(sorted(nested))
         if methods.get('__elements__') is None:
             methods['__elements__'] = tuple(sorted(elements))
         return MetaStrict.__new__(cls, clsname, bases, methods)
+
+
+Strict = MetaStrict('Strict', (object,), {})
+
+_Serialiasable = MetaSerialisable('_Serialisable', (object,), {})
+
+#del MetaStrict
+#del MetaSerialisable
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/base.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 """
 Based on Python Cookbook 3rd Edition, 8.13
 http://chimera.labs.oreilly.com/books/1230000000393/ch08.html#_discussiuncion_130
 """
 
 import datetime
 import re
 
-from openpyxl import DEBUG
 from openpyxl.utils.datetime import from_ISO8601
 
 from .namespace import namespaced
 
 class Descriptor(object):
 
     def __init__(self, name=None, **kw):
@@ -36,18 +35,15 @@
         super(Typed, self).__init__(*args, **kw)
         self.__doc__ = f"Values must be of type {self.expected_type}"
 
     def __set__(self, instance, value):
         if not isinstance(value, self.expected_type):
             if (not self.allow_none
                 or (self.allow_none and value is not None)):
-                msg = f"{instance.__class__}.{self.name} should be {self.expected_type} but value is {type(value)}"
-                if DEBUG:
-                    msg = f"{instance.__class__}.{self.name} should be {self.expected_type} but {value} is {type(value)}"
-                raise TypeError(msg)
+                raise TypeError(f"expected f{self.expected_type} but value is {value} with type {type(value)}")
         super(Typed, self).__set__(instance, value)
 
     def __repr__(self):
         return  self.__doc__
 
 
 def _convert(expected_type, value):
@@ -216,15 +212,15 @@
     def __call__(self):
         return self.expected_type()
 
 
 class Alias(Descriptor):
     """
     Aliases can be used when either the desired attribute name is not allowed
-    or confusing in Python (eg. "type") or a more descriptive name is desired
+    or confusing in Python (eg. "type") or a more descriptve name is desired
     (eg. "underline" for "u")
     """
 
     def __init__(self, alias):
         self.alias = alias
 
     def __set__(self, instance, value):
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/excel.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+#copyright openpyxl 2010-2018
 
 """
 Excel specific descriptors
 """
 
 from openpyxl.xml.constants import REL_NS
 from openpyxl.compat import safe_string
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/nested.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/nested.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+#copyright openpyxl 2010-2015
 
 """
 Generic serialisable classes
 """
 from .base import (
     Convertible,
     Bool,
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/sequence.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/sequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# copyright openpyxl 2010-2015
 
 from openpyxl.compat import safe_string
 from openpyxl.xml.functions import Element
 from openpyxl.utils.indexed_list import IndexedList
 
 from .base import Descriptor, Alias, _convert
 from .namespace import namespaced
@@ -14,25 +14,24 @@
     type
     """
 
     expected_type = type(None)
     seq_types = (list, tuple)
     idx_base = 0
     unique = False
-    container = list
 
 
     def __set__(self, instance, seq):
         if not isinstance(seq, self.seq_types):
-            raise TypeError("Value must be a sequence")
-        seq = self.container(_convert(self.expected_type, value) for value in seq)
+            raise TypeError(f"Value for {self.name} of class {instance.__class__.__name__} must be a sequence")
+        seq = [_convert(self.expected_type, value) for value in seq]
         if self.unique:
             seq = IndexedList(seq)
 
-        super().__set__(instance, seq)
+        super(Sequence, self).__set__(instance, seq)
 
 
     def to_tree(self, tagname, obj, namespace=None):
         """
         Convert the sequence represented by the descriptor to an XML element
         """
         for idx, v in enumerate(obj, self.idx_base):
@@ -41,22 +40,14 @@
             else:
                 tagname = namespaced(obj, tagname, namespace)
                 el = Element(tagname)
                 el.text = safe_string(v)
             yield el
 
 
-class UniqueSequence(Sequence):
-    """
-    Use a set to keep values unique
-    """
-    seq_types = (list, tuple, set)
-    container = set
-
-
 class ValueSequence(Sequence):
     """
     A sequence of primitive types that are stored as a single attribute.
     "val" is the default attribute
     """
 
     attribute = "val"
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/serialisable.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/serialisable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright (c) 2010-2023 openpyxl
+# copyright openpyxl 2010-2015
 
 from copy import copy
 from keyword import kwlist
 KEYWORDS = frozenset(kwlist)
 
 from . import Descriptor
-from . import MetaSerialisable
+from . import _Serialiasable
 from .sequence import (
     Sequence,
     NestedSequence,
     MultiSequencePart,
 )
 from .namespace import namespaced
 
@@ -17,15 +17,15 @@
 from openpyxl.xml.functions import (
     Element,
     localname,
 )
 
 seq_types = (list, tuple)
 
-class Serialisable(metaclass=MetaSerialisable):
+class Serialisable(_Serialiasable):
     """
     Objects can serialise to XML their attributes and child objects.
     The following class attributes are created by the metaclass at runtime:
     __attrs__ = attributes
     __nested__ = single-valued child treated as an attribute
     __elements__ = child elements
     """
```

### Comparing `openpyxl-3.1.2/openpyxl/descriptors/slots.py` & `openpyxl-3.2.0b1/openpyxl/descriptors/slots.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/drawing/colors.py` & `openpyxl-3.2.0b1/openpyxl/drawing/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Typed,
     Integer,
     Set,
     MinMax,
 )
-from openpyxl.descriptors.excel import Percentage
 from openpyxl.descriptors.nested import (
     NestedNoneSet,
     NestedValue,
     NestedInteger,
     EmptyTag,
 )
 
@@ -209,14 +208,15 @@
         self.lum = lum
 
 
 
 class RGBPercent(Serialisable):
 
     tagname = "rgbClr"
+    namespace = DRAWING_NS
 
     r = MinMax(min=0, max=100)
     g = MinMax(min=0, max=100)
     b = MinMax(min=0, max=100)
 
     #TODO add color transform options
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/connector.py` & `openpyxl-3.2.0b1/openpyxl/drawing/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Bool,
     Integer,
     String,
@@ -102,32 +102,38 @@
 class ShapeMeta(Serialisable):
 
     tagname = "nvSpPr"
 
     cNvPr = Typed(expected_type=NonVisualDrawingProps)
     cNvSpPr = Typed(expected_type=NonVisualDrawingShapeProps)
 
+    __elements__ = ("cNvPr", "cNvSpPr")
+
     def __init__(self, cNvPr=None, cNvSpPr=None):
         self.cNvPr = cNvPr
         self.cNvSpPr = cNvSpPr
 
 
 class Shape(Serialisable):
 
+    tagname = "sp"
+
     macro = String(allow_none=True)
     textlink = String(allow_none=True)
     fPublished = Bool(allow_none=True)
     fLocksText = Bool(allow_none=True)
     nvSpPr = Typed(expected_type=ShapeMeta, allow_none=True)
     meta = Alias("nvSpPr")
     spPr = Typed(expected_type=GraphicalProperties)
     graphicalProperties = Alias("spPr")
     style = Typed(expected_type=ShapeStyle, allow_none=True)
     txBody = Typed(expected_type=RichText, allow_none=True)
 
+    __elements__ = ("nvSpPr", "spPr", "style", "txBody")
+
     def __init__(self,
                  macro=None,
                  textlink=None,
                  fPublished=None,
                  fLocksText=None,
                  nvSpPr=None,
                  spPr=None,
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/drawing.py` & `openpyxl-3.2.0b1/openpyxl/drawing/drawing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-
-# Copyright (c) 2010-2023 openpyxl
+from __future__ import division
+# Copyright (c) 2010-2022 openpyxl
 
 import math
 
-from openpyxl.utils.units import pixels_to_EMU
+from openpyxl.compat import deprecated
+
+from openpyxl.styles.colors import Color, BLACK, WHITE
+from openpyxl.utils.units import (
+    pixels_to_EMU,
+    EMU_to_pixels,
+    short_color,
+)
 
 
 class Drawing(object):
     """ a drawing object - eg container for shapes or charts
         we assume user specifies dimensions in pixels; units are
         converted to EMU in the drawing part
     """
@@ -30,49 +37,52 @@
         self.anchorrow = 0 # top row
 
 
     @property
     def width(self):
         return self._width
 
-
     @width.setter
     def width(self, w):
         if self.resize_proportional and w:
             ratio = self._height / self._width
             self._height = round(ratio * w)
         self._width = w
 
-
     @property
     def height(self):
         return self._height
 
-
     @height.setter
     def height(self, h):
         if self.resize_proportional and h:
             ratio = self._width / self._height
             self._width = round(ratio * h)
         self._height = h
 
-
     def set_dimension(self, w=0, h=0):
 
         xratio = w / self._width
         yratio = h / self._height
 
         if self.resize_proportional and w and h:
             if (xratio * self._height) < h:
                 self._height = math.ceil(xratio * self._height)
                 self._width = w
             else:
                 self._width = math.ceil(yratio * self._width)
                 self._height = h
 
+    @deprecated("Private method used when serialising")
+    def get_emu_dimensions(self):
+        """ return (x, y, w, h) in EMU """
+
+        return (pixels_to_EMU(self.left), pixels_to_EMU(self.top),
+            pixels_to_EMU(self._width), pixels_to_EMU(self._height))
+
 
     @property
     def anchor(self):
         from .spreadsheet_drawing import (
             OneCellAnchor,
             TwoCellAnchor,
             AbsoluteAnchor)
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/effect.py` & `openpyxl-3.2.0b1/openpyxl/drawing/effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     String,
     Set,
     Bool,
     Integer,
     Float,
 )
+from openpyxl.xml.constants import DRAWING_NS
 
 from .colors import ColorChoice
 
 
 class TintEffect(Serialisable):
 
     tagname = "tint"
@@ -371,14 +372,16 @@
                  rad=None,
                 ):
         self.rad = rad
 
 
 class EffectList(Serialisable):
 
+    namespace = DRAWING_NS
+
     blur = Typed(expected_type=BlurEffect, allow_none=True)
     fillOverlay = Typed(expected_type=FillOverlayEffect, allow_none=True)
     glow = Typed(expected_type=GlowEffect, allow_none=True)
     innerShdw = Typed(expected_type=InnerShadowEffect, allow_none=True)
     outerShdw = Typed(expected_type=OuterShadow, allow_none=True)
     prstShdw = Typed(expected_type=PresetShadowEffect, allow_none=True)
     reflection = Typed(expected_type=ReflectionEffect, allow_none=True)
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/fill.py` & `openpyxl-3.2.0b1/openpyxl/drawing/fill.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,65 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
+
+from io import BytesIO
+from warnings import warn
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Bool,
     Integer,
     Set,
     NoneSet,
     Typed,
     MinMax,
+    Sequence,
 )
 from openpyxl.descriptors.excel import (
     Relation,
     Percentage,
 )
 from openpyxl.descriptors.nested import NestedNoneSet, NestedValue
 from openpyxl.descriptors.sequence import NestedSequence
-from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
 from openpyxl.xml.constants import DRAWING_NS
 
 from .colors import (
     ColorChoice,
     HSLColor,
     SystemColor,
     SchemeColor,
-    PRESET_COLORS,
     RGBPercent,
+    PRESET_COLORS,
 )
 
-from .effect import (
-    AlphaBiLevelEffect,
-    AlphaCeilingEffect,
-    AlphaFloorEffect,
-    AlphaInverseEffect,
-    AlphaModulateEffect,
-    AlphaModulateFixedEffect,
-    AlphaReplaceEffect,
-    BiLevelEffect,
-    BlurEffect,
-    ColorChangeEffect,
-    ColorReplaceEffect,
-    DuotoneEffect,
-    FillOverlayEffect,
-    GrayscaleEffect,
-    HSLEffect,
-    LuminanceEffect,
-    TintEffect,
-)
+
+from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
+from .effect import *
+
+from openpyxl.drawing.image import Image
+
 
 """
 Fill elements from drawing main schema
 """
 
 class PatternFillProperties(Serialisable):
 
     tagname = "pattFill"
     namespace = DRAWING_NS
 
-    prst = NoneSet(values=(['pct5', 'pct10', 'pct20', 'pct25', 'pct30',
-                            'pct40', 'pct50', 'pct60', 'pct70', 'pct75', 'pct80', 'pct90', 'horz',
-                            'vert', 'ltHorz', 'ltVert', 'dkHorz', 'dkVert', 'narHorz', 'narVert',
-                            'dashHorz', 'dashVert', 'cross', 'dnDiag', 'upDiag', 'ltDnDiag',
-                            'ltUpDiag', 'dkDnDiag', 'dkUpDiag', 'wdDnDiag', 'wdUpDiag', 'dashDnDiag',
-                            'dashUpDiag', 'diagCross', 'smCheck', 'lgCheck', 'smGrid', 'lgGrid',
-                            'dotGrid', 'smConfetti', 'lgConfetti', 'horzBrick', 'diagBrick',
-                            'solidDmnd', 'openDmnd', 'dotDmnd', 'plaid', 'sphere', 'weave', 'divot',
-                            'shingle', 'wave', 'trellis', 'zigZag']))
+    prst = NoneSet(values=(['pct5', 'pct10', 'pct20', 'pct25', 'pct30', 'pct40',
+                        'pct50', 'pct60', 'pct70', 'pct75', 'pct80', 'pct90', 'horz', 'vert',
+                        'ltHorz', 'ltVert', 'dkHorz', 'dkVert', 'narHorz', 'narVert', 'dashHorz',
+                        'dashVert', 'cross', 'dnDiag', 'upDiag', 'ltDnDiag', 'ltUpDiag',
+                        'dkDnDiag', 'dkUpDiag', 'wdDnDiag', 'wdUpDiag', 'dashDnDiag',
+                        'dashUpDiag', 'diagCross', 'smCheck', 'lgCheck', 'smGrid', 'lgGrid',
+                        'dotGrid', 'smConfetti', 'lgConfetti', 'horzBrick', 'diagBrick',
+                        'solidDmnd', 'openDmnd', 'dotDmnd', 'plaid', 'sphere', 'weave', 'divot',
+                        'shingle', 'wave', 'trellis', 'zigZag']))
     preset = Alias("prst")
     fgClr = Typed(expected_type=ColorChoice, allow_none=True)
     foreground = Alias("fgClr")
     bgClr = Typed(expected_type=ColorChoice, allow_none=True)
     background = Alias("bgClr")
 
     __elements__ = ("fgClr", "bgClr")
@@ -261,19 +251,20 @@
         self.prstClr = prstClr
 
 
 class Blip(Serialisable):
 
     tagname = "blip"
     namespace = DRAWING_NS
+    blob = None
 
-    # Using attribute groupAG_Blob
+    #Using attribute groupAG_Blob
     cstate = NoneSet(values=(['email', 'screen', 'print', 'hqprint']))
-    embed = Relation() # rId
-    link = Relation() # hyperlink
+    embed = Relation() #rId
+    link = Relation() #hyperlink
     noGrp = Bool(allow_none=True)
     noSelect = Bool(allow_none=True)
     noRot = Bool(allow_none=True)
     noChangeAspect = Bool(allow_none=True)
     noMove = Bool(allow_none=True)
     noResize = Bool(allow_none=True)
     noEditPoints = Bool(allow_none=True)
@@ -366,14 +357,29 @@
         self.fillOverlay = fillOverlay
         self.grayscl = grayscl
         self.hsl = hsl
         self.lum = lum
         self.tint = tint
 
 
+    def _read(self, rels, archive):
+        """Read image data from archive"""
+        if self.embed is not None:
+            rel = rels[self.embed]
+            src = archive.read(rel.target)
+            data = BytesIO(src)
+            try:
+                img = Image(data)
+            except OSError:
+                msg = "The image {0} will be removed because it cannot be read".format(rel.target)
+                warn(msg)
+                return
+            return img
+
+
 class TileInfoProperties(Serialisable):
 
     tx = Integer(allow_none=True)
     ty = Integer(allow_none=True)
     sx = Integer(allow_none=True)
     sy = Integer(allow_none=True)
     flip = NoneSet(values=(['x', 'y', 'xy']))
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/geometry.py` & `openpyxl-3.2.0b1/openpyxl/drawing/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Float,
     Integer,
     Bool,
     MinMax,
     Set,
     NoneSet,
     String,
     Alias,
 )
+from openpyxl.descriptors.nested import (
+    NestedValue,
+    NestedNoneSet,
+)
 from openpyxl.descriptors.excel import Coordinate, Percentage
+
+
 from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
-from .line import LineProperties
+from .colors import (
+    ColorChoiceDescriptor,
+    RGBPercent,
+    HSLColor,
+    SchemeColor,
+    SystemColor,
+    PRESET_COLORS,
+)
 
 from openpyxl.styles.colors import Color
 from openpyxl.xml.constants import DRAWING_NS
 
 
 class Point2D(Serialisable):
 
@@ -445,14 +458,16 @@
                 ):
         self.name = name
         self.fmla = fmla
 
 
 class GeomGuideList(Serialisable):
 
+    namespace = DRAWING_NS
+
     gd = Typed(expected_type=GeomGuide, allow_none=True)
 
     def __init__(self,
                  gd=None,
                 ):
         self.gd = gd
 
@@ -543,38 +558,88 @@
                 ):
         self.prst = prst
         self.avLst = avLst
 
 
 class FontReference(Serialisable):
 
+    namespace = DRAWING_NS
+
     idx = NoneSet(values=(['major', 'minor']))
+    scrgbClr = Typed(expected_type=RGBPercent, allow_none=True)
+    RGBPercent = Alias('scrgbClr')
+    srgbClr = NestedValue(expected_type=str, allow_none=True) # needs pattern and can have transform
+    RGB = Alias('srgbClr')
+    hslClr = Typed(expected_type=HSLColor, allow_none=True)
+    sysClr = Typed(expected_type=SystemColor, allow_none=True)
+    schemeClr = Typed(expected_type=SchemeColor, allow_none=True)
+    prstClr = NestedNoneSet(values=PRESET_COLORS)
 
     def __init__(self,
                  idx=None,
+                 scrgbClr=None,
+                 srgbClr=None,
+                 hslClr=None,
+                 sysClr=None,
+                 schemeClr=None,
+                 prstClr=None,
                 ):
         self.idx = idx
+        self.scrgbClr = scrgbClr
+        self.srgbClr = srgbClr
+        self.hslClr = hslClr
+        self.sysClr = sysClr
+        self.schemeClr = schemeClr
+        self.prstClr = prstClr
 
 
 class StyleMatrixReference(Serialisable):
 
-    idx = Integer()
+    namespace = DRAWING_NS
 
-    def __init__(self,
-                 idx=None,
+    idx = Integer()
+    scrgbClr = Typed(expected_type=RGBPercent, allow_none=True)
+    RGBPercent = Alias('scrgbClr')
+    srgbClr = NestedValue(expected_type=str, allow_none=True) # needs pattern and can have transform
+    RGB = Alias('srgbClr')
+    hslClr = Typed(expected_type=HSLColor, allow_none=True)
+    sysClr = Typed(expected_type=SystemColor, allow_none=True)
+    schemeClr = Typed(expected_type=SchemeColor, allow_none=True)
+    prstClr = NestedNoneSet(values=PRESET_COLORS)
+
+    __elements__ = ('scrgbClr', 'srgbClr', 'hslClr', 'sysClr', 'schemeClr', 'prstClr')
+
+    def __init__(self,
+                 idx = None,
+                 scrgbClr=None,
+                 srgbClr=None,
+                 hslClr=None,
+                 sysClr=None,
+                 schemeClr=None,
+                 prstClr=None,
                 ):
         self.idx = idx
+        self.scrgbClr = scrgbClr
+        self.srgbClr = srgbClr
+        self.hslClr = hslClr
+        self.sysClr = sysClr
+        self.schemeClr = schemeClr
+        self.prstClr = prstClr
 
 
 class ShapeStyle(Serialisable):
 
-    lnRef = Typed(expected_type=StyleMatrixReference, )
-    fillRef = Typed(expected_type=StyleMatrixReference, )
-    effectRef = Typed(expected_type=StyleMatrixReference, )
-    fontRef = Typed(expected_type=FontReference, )
+    tagname = "style"
+
+    lnRef = Typed(expected_type=StyleMatrixReference)
+    fillRef = Typed(expected_type=StyleMatrixReference)
+    effectRef = Typed(expected_type=StyleMatrixReference)
+    fontRef = Typed(expected_type=FontReference)
+
+    __elements__ = ("lnRef", "fillRef", "effectRef", "fontRef")
 
     def __init__(self,
                  lnRef=None,
                  fillRef=None,
                  effectRef=None,
                  fontRef=None,
                 ):
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/graphic.py` & `openpyxl-3.2.0b1/openpyxl/drawing/graphic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.xml.constants import CHART_NS, DRAWING_NS
+
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Bool,
     String,
     Alias,
+    Sequence,
 )
 from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
 
-from .effect import (
-    EffectList,
-    EffectContainer,
-)
-from .fill import (
-    Blip,
-    GradientFillProperties,
-    BlipFillProperties,
-)
+
+from .effect import *
 from .picture import PictureFrame
 from .properties import (
     NonVisualDrawingProps,
     NonVisualGroupShape,
     GroupShapeProperties,
 )
 from .relation import ChartRelation
@@ -73,14 +68,15 @@
 
 
 class NonVisualGraphicFrame(Serialisable):
 
     tagname = "nvGraphicFramePr"
 
     cNvPr = Typed(expected_type=NonVisualDrawingProps)
+    non_visual_props = Alias("cNvPr")
     cNvGraphicFramePr = Typed(expected_type=NonVisualGraphicFrameProperties)
 
     __elements__ = ('cNvPr', 'cNvGraphicFramePr')
 
     def __init__(self,
                  cNvPr=None,
                  cNvGraphicFramePr=None,
@@ -126,20 +122,21 @@
 
 
 class GraphicFrame(Serialisable):
 
     tagname = "graphicFrame"
 
     nvGraphicFramePr = Typed(expected_type=NonVisualGraphicFrame)
+    props = Alias("nvGraphicFramePr")
     xfrm = Typed(expected_type=XDRTransform2D)
     graphic = Typed(expected_type=GraphicObject)
     macro = String(allow_none=True)
     fPublished = Bool(allow_none=True)
 
-    __elements__ = ('nvGraphicFramePr', 'xfrm', 'graphic', 'macro', 'fPublished')
+    __elements__ = ('nvGraphicFramePr', 'xfrm', 'graphic', 'fPublished')
 
     def __init__(self,
                  nvGraphicFramePr=None,
                  xfrm=None,
                  graphic=None,
                  macro=None,
                  fPublished=None,
@@ -153,25 +150,31 @@
         if graphic is None:
             graphic = GraphicObject()
         self.graphic = graphic
         self.macro = macro
         self.fPublished = fPublished
 
 
+from .connector import Shape
+
+
 class GroupShape(Serialisable):
 
     nvGrpSpPr = Typed(expected_type=NonVisualGroupShape)
     nonVisualProperties = Alias("nvGrpSpPr")
     grpSpPr = Typed(expected_type=GroupShapeProperties)
     visualProperties = Alias("grpSpPr")
-    pic = Typed(expected_type=PictureFrame, allow_none=True)
+    pic = Sequence(expected_type=PictureFrame)
+    sp = Sequence(expected_type=Shape)
 
-    __elements__ = ["nvGrpSpPr", "grpSpPr", "pic"]
+    __elements__ = ("nvGrpSpPr", "grpSpPr", "pic", "sp")
 
     def __init__(self,
                  nvGrpSpPr=None,
                  grpSpPr=None,
-                 pic=None,
+                 pic=(),
+                 sp=(),
                 ):
         self.nvGrpSpPr = nvGrpSpPr
         self.grpSpPr = grpSpPr
         self.pic = pic
+        self.sp = sp
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/image.py` & `openpyxl-3.2.0b1/openpyxl/drawing/image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,27 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from io import BytesIO
 
 try:
     from PIL import Image as PILImage
 except ImportError:
     PILImage = False
 
+from openpyxl.xml.constants import IMAGE_NS
+from openpyxl.descriptors import (
+    Strict,
+    Typed,
+    Integer,
+    String,
+    Sequence,
+)
+
+from openpyxl.packaging.relationship import Relationship
+
 
 def _import_image(img):
     if not PILImage:
         raise ImportError('You must install Pillow to fetch image objects')
 
     if not isinstance(img, PILImage.Image):
         img = PILImage.open(img)
@@ -20,46 +31,87 @@
 
 class Image(object):
     """Image in a spreadsheet"""
 
     _id = 1
     _path = "/xl/media/image{0}.{1}"
     anchor = "A1"
+    format = "PNG"
+    rel_type = IMAGE_NS
 
     def __init__(self, img):
 
         self.ref = img
         mark_to_close = isinstance(img, str)
         image = _import_image(img)
         self.width, self.height = image.size
 
         try:
-            self.format = image.format.lower()
+            self.format = image.format
         except AttributeError:
-            self.format = "png"
+            pass
         if mark_to_close:
             # PIL instances created for metadata should be closed.
             image.close()
 
 
     def _data(self):
         """
         Return image data, convert to supported types if necessary
         """
         img = _import_image(self.ref)
         # don't convert these file formats
-        if self.format in ['gif', 'jpeg', 'png']:
+        if self.format in ['GIF', 'JPEG', 'PNG', "WMF", "EMF"]:
             img.fp.seek(0)
             fp = img.fp
         else:
             fp = BytesIO()
             img.save(fp, format="png")
             fp.seek(0)
 
         data = fp.read()
         fp.close()
         return data
 
 
     @property
     def path(self):
-        return self._path.format(self._id, self.format)
+        return self._path.format(self._id, self.format.lower())
+
+
+    def __eq__(self, other):
+        return self.ref == other.ref
+
+
+    def _write(self, archive):
+        archive.writestr(self.path[1:], self._data())
+
+
+class ImageGroup(Strict):
+
+    """
+    A way of grouping pictures in shapes
+    """
+
+    images = Sequence(expected_type=Image)
+    counter = Integer()
+
+
+    def __init__(self,
+                 images=(),
+                 counter=counter,
+                 archive=None,
+                 anchor=None):
+        self.images = images
+        self.counter = 0
+        self.anchor = anchor
+
+
+    def append(self, img):
+        self.images.append(img)
+        self.images = self.images
+
+
+    @property
+    def name(self):
+        return f"Group {self.counter}"
+
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/line.py` & `openpyxl-3.2.0b1/openpyxl/drawing/line.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
+    Float,
     Integer,
+    Bool,
     MinMax,
+    Set,
     NoneSet,
+    String,
     Alias,
     Sequence
 )
+from openpyxl.descriptors.excel import Coordinate, Percentage
 
 from openpyxl.descriptors.nested import (
     NestedInteger,
+    NestedSet,
     NestedNoneSet,
     EmptyTag,
 )
+from openpyxl.compat import safe_string
 from openpyxl.xml.constants import DRAWING_NS
+from openpyxl.xml.functions import Element
 
 from .colors import ColorChoiceDescriptor
 from .fill import GradientFillProperties, PatternFillProperties
 from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
 
 """
 Line elements from drawing main schema
 """
 
-
 class LineEndProperties(Serialisable):
 
     tagname = "end"
     namespace = DRAWING_NS
 
     type = NoneSet(values=(['none', 'triangle', 'stealth', 'diamond', 'oval', 'arrow']))
     w = NoneSet(values=(['sm', 'med', 'lg']))
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/picture.py` & `openpyxl-3.2.0b1/openpyxl/drawing/picture.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.xml.constants import DRAWING_NS
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Bool,
@@ -19,15 +19,15 @@
 
 
 class PictureLocking(Serialisable):
 
     tagname = "picLocks"
     namespace = DRAWING_NS
 
-    # Using attribute group AG_Locking
+    #Using attribute group AG_Locking
     noCrop = Bool(allow_none=True)
     noGrp = Bool(allow_none=True)
     noSelect = Bool(allow_none=True)
     noRot = Bool(allow_none=True)
     noChangeAspect = Bool(allow_none=True)
     noMove = Bool(allow_none=True)
     noResize = Bool(allow_none=True)
@@ -102,24 +102,22 @@
             cNvPr = NonVisualDrawingProps(id=0, name="Image 1", descr="Name of file")
         self.cNvPr = cNvPr
         if cNvPicPr is None:
             cNvPicPr = NonVisualPictureProperties()
         self.cNvPicPr = cNvPicPr
 
 
-
-
 class PictureFrame(Serialisable):
 
     tagname = "pic"
 
     macro = String(allow_none=True)
     fPublished = Bool(allow_none=True)
-    nvPicPr = Typed(expected_type=PictureNonVisual, )
-    blipFill = Typed(expected_type=BlipFillProperties, )
+    nvPicPr = Typed(expected_type=PictureNonVisual)
+    blipFill = Typed(expected_type=BlipFillProperties)
     spPr = Typed(expected_type=GraphicalProperties, )
     graphicalProperties = Alias('spPr')
     style = Typed(expected_type=ShapeStyle, allow_none=True)
 
     __elements__ = ("nvPicPr", "blipFill", "spPr", "style")
 
     def __init__(self,
@@ -138,7 +136,14 @@
         if blipFill is None:
             blipFill = BlipFillProperties()
         self.blipFill = blipFill
         if spPr is None:
             spPr = GraphicalProperties()
         self.spPr = spPr
         self.style = style
+
+
+    @property
+    def _image(self):
+        blip = self.blipFill.blip
+        if blip is not None and blip.embed:
+            return blip
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/properties.py` & `openpyxl-3.2.0b1/openpyxl/drawing/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.xml.constants import DRAWING_NS
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Bool,
     Integer,
-    Set,
     String,
-    Alias,
     NoneSet,
 )
 from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
 
 from .geometry import GroupTransform2D, Scene3D
 from .text import Hyperlink
 
@@ -52,14 +50,15 @@
     noMove = Bool(allow_none=True)
     noResize = Bool(allow_none=True)
     noChangeArrowheads = Bool(allow_none=True)
     noEditPoints = Bool(allow_none=True)
     noAdjustHandles = Bool(allow_none=True)
     noChangeArrowheads = Bool(allow_none=True)
     noChangeShapeType = Bool(allow_none=True)
+    noTextEdit = Bool(allow_none=True)
     extLst = Typed(expected_type=OfficeArtExtensionList, allow_none=True)
 
     __elements__ = ()
 
     def __init__(self,
                  noGrp=None,
                  noUngrp=None,
@@ -68,27 +67,29 @@
                  noChangeAspect=None,
                  noChangeArrowheads=None,
                  noMove=None,
                  noResize=None,
                  noEditPoints=None,
                  noAdjustHandles=None,
                  noChangeShapeType=None,
+                 noTextEdit=None,
                  extLst=None,
                 ):
         self.noGrp = noGrp
         self.noUngrp = noUngrp
         self.noSelect = noSelect
         self.noRot = noRot
         self.noChangeAspect = noChangeAspect
         self.noChangeArrowheads = noChangeArrowheads
         self.noMove = noMove
         self.noResize = noResize
         self.noEditPoints = noEditPoints
         self.noAdjustHandles = noAdjustHandles
         self.noChangeShapeType = noChangeShapeType
+        self.noTextEdit = noTextEdit
 
 
 class NonVisualGroupDrawingShapeProps(Serialisable):
 
     tagname = "cNvGrpSpPr"
 
     grpSpLocks = Typed(expected_type=GroupLocking, allow_none=True)
@@ -104,18 +105,18 @@
 
 
 class NonVisualDrawingShapeProps(Serialisable):
 
     tagname = "cNvSpPr"
 
     spLocks = Typed(expected_type=GroupLocking, allow_none=True)
-    txBax = Bool(allow_none=True)
+    txBox = Bool(allow_none=True)
     extLst = Typed(expected_type=OfficeArtExtensionList, allow_none=True)
 
-    __elements__ = ("spLocks", "txBax")
+    __elements__ = ("spLocks",)
 
     def __init__(self,
                  spLocks=None,
                  txBox=None,
                  extLst=None,
                 ):
         self.spLocks = spLocks
@@ -131,15 +132,15 @@
     descr = String(allow_none=True)
     hidden = Bool(allow_none=True)
     title = String(allow_none=True)
     hlinkClick = Typed(expected_type=Hyperlink, allow_none=True)
     hlinkHover = Typed(expected_type=Hyperlink, allow_none=True)
     extLst = Typed(expected_type=OfficeArtExtensionList, allow_none=True)
 
-    __elements__ = ["hlinkClick", "hlinkHover"]
+    __elements__ = ("hlinkClick", "hlinkHover")
 
     def __init__(self,
                  id=None,
                  name=None,
                  descr=None,
                  hidden=None,
                  title=None,
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/spreadsheet_drawing.py` & `openpyxl-3.2.0b1/openpyxl/drawing/spreadsheet_drawing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,220 +1,47 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
-    Typed,
-    Bool,
-    NoneSet,
-    Integer,
     Sequence,
-    Alias,
-)
-from openpyxl.descriptors.nested import (
-    NestedText,
-    NestedNoneSet,
+    String,
+    Typed,
 )
-from openpyxl.descriptors.excel import Relation
 
 from openpyxl.packaging.relationship import (
     Relationship,
     RelationshipList,
 )
 from openpyxl.utils import coordinate_to_tuple
 from openpyxl.utils.units import (
     cm_to_EMU,
     pixels_to_EMU,
 )
-from openpyxl.drawing.image import Image
+from openpyxl.drawing.image import (
+    Image,
+    ImageGroup,
+)
 
 from openpyxl.xml.constants import SHEET_DRAWING_NS
 
 from openpyxl.chart._chart import ChartBase
-from .xdr import (
-    XDRPoint2D,
-    XDRPositiveSize2D,
-)
 from .fill import Blip
-from .connector import Shape
 from .graphic import (
-    GroupShape,
-    GraphicFrame,
+     GraphicFrame,
+     GroupShape,
     )
 from .geometry import PresetGeometry2D
 from .picture import PictureFrame
 from .relation import ChartRelation
-
-
-class AnchorClientData(Serialisable):
-
-    fLocksWithSheet = Bool(allow_none=True)
-    fPrintsWithSheet = Bool(allow_none=True)
-
-    def __init__(self,
-                 fLocksWithSheet=None,
-                 fPrintsWithSheet=None,
-                 ):
-        self.fLocksWithSheet = fLocksWithSheet
-        self.fPrintsWithSheet = fPrintsWithSheet
-
-
-class AnchorMarker(Serialisable):
-
-    tagname = "marker"
-
-    col = NestedText(expected_type=int)
-    colOff = NestedText(expected_type=int)
-    row = NestedText(expected_type=int)
-    rowOff = NestedText(expected_type=int)
-
-    def __init__(self,
-                 col=0,
-                 colOff=0,
-                 row=0,
-                 rowOff=0,
-                 ):
-        self.col = col
-        self.colOff = colOff
-        self.row = row
-        self.rowOff = rowOff
-
-
-class _AnchorBase(Serialisable):
-
-    #one of
-    sp = Typed(expected_type=Shape, allow_none=True)
-    shape = Alias("sp")
-    grpSp = Typed(expected_type=GroupShape, allow_none=True)
-    groupShape = Alias("grpSp")
-    graphicFrame = Typed(expected_type=GraphicFrame, allow_none=True)
-    cxnSp = Typed(expected_type=Shape, allow_none=True)
-    connectionShape = Alias("cxnSp")
-    pic = Typed(expected_type=PictureFrame, allow_none=True)
-    contentPart = Relation()
-
-    clientData = Typed(expected_type=AnchorClientData)
-
-    __elements__ = ('sp', 'grpSp', 'graphicFrame',
-                    'cxnSp', 'pic', 'contentPart', 'clientData')
-
-    def __init__(self,
-                 clientData=None,
-                 sp=None,
-                 grpSp=None,
-                 graphicFrame=None,
-                 cxnSp=None,
-                 pic=None,
-                 contentPart=None
-                 ):
-        if clientData is None:
-            clientData = AnchorClientData()
-        self.clientData = clientData
-        self.sp = sp
-        self.grpSp = grpSp
-        self.graphicFrame = graphicFrame
-        self.cxnSp = cxnSp
-        self.pic = pic
-        self.contentPart = contentPart
-
-
-class AbsoluteAnchor(_AnchorBase):
-
-    tagname = "absoluteAnchor"
-
-    pos = Typed(expected_type=XDRPoint2D)
-    ext = Typed(expected_type=XDRPositiveSize2D)
-
-    sp = _AnchorBase.sp
-    grpSp = _AnchorBase.grpSp
-    graphicFrame = _AnchorBase.graphicFrame
-    cxnSp = _AnchorBase.cxnSp
-    pic = _AnchorBase.pic
-    contentPart = _AnchorBase.contentPart
-    clientData = _AnchorBase.clientData
-
-    __elements__ = ('pos', 'ext') + _AnchorBase.__elements__
-
-    def __init__(self,
-                 pos=None,
-                 ext=None,
-                 **kw
-                ):
-        if pos is None:
-            pos = XDRPoint2D(0, 0)
-        self.pos = pos
-        if ext is None:
-            ext = XDRPositiveSize2D(0, 0)
-        self.ext = ext
-        super(AbsoluteAnchor, self).__init__(**kw)
-
-
-class OneCellAnchor(_AnchorBase):
-
-    tagname = "oneCellAnchor"
-
-    _from = Typed(expected_type=AnchorMarker)
-    ext = Typed(expected_type=XDRPositiveSize2D)
-
-    sp = _AnchorBase.sp
-    grpSp = _AnchorBase.grpSp
-    graphicFrame = _AnchorBase.graphicFrame
-    cxnSp = _AnchorBase.cxnSp
-    pic = _AnchorBase.pic
-    contentPart = _AnchorBase.contentPart
-    clientData = _AnchorBase.clientData
-
-    __elements__ = ('_from', 'ext') + _AnchorBase.__elements__
-
-
-    def __init__(self,
-                 _from=None,
-                 ext=None,
-                 **kw
-                ):
-        if _from is None:
-            _from = AnchorMarker()
-        self._from = _from
-        if ext is None:
-            ext = XDRPositiveSize2D(0, 0)
-        self.ext = ext
-        super(OneCellAnchor, self).__init__(**kw)
-
-
-class TwoCellAnchor(_AnchorBase):
-
-    tagname = "twoCellAnchor"
-
-    editAs = NoneSet(values=(['twoCell', 'oneCell', 'absolute']))
-    _from = Typed(expected_type=AnchorMarker)
-    to = Typed(expected_type=AnchorMarker)
-
-    sp = _AnchorBase.sp
-    grpSp = _AnchorBase.grpSp
-    graphicFrame = _AnchorBase.graphicFrame
-    cxnSp = _AnchorBase.cxnSp
-    pic = _AnchorBase.pic
-    contentPart = _AnchorBase.contentPart
-    clientData = _AnchorBase.clientData
-
-    __elements__ = ('_from', 'to') + _AnchorBase.__elements__
-
-    def __init__(self,
-                 editAs=None,
-                 _from=None,
-                 to=None,
-                 **kw
-                 ):
-        self.editAs = editAs
-        if _from is None:
-            _from = AnchorMarker()
-        self._from = _from
-        if to is None:
-            to = AnchorMarker()
-        self.to = to
-        super(TwoCellAnchor, self).__init__(**kw)
+from .anchor import (
+    AbsoluteAnchor,
+    OneCellAnchor,
+    TwoCellAnchor,
+    _AnchorBase,
+)
 
 
 def _check_anchor(obj):
     """
     Check whether an object has an existing Anchor object
     If not create a OneCellAnchor using the provided coordinate
     """
@@ -229,93 +56,163 @@
             anchor.ext.height = cm_to_EMU(obj.height)
         elif isinstance(obj, Image):
             anchor.ext.width = pixels_to_EMU(obj.width)
             anchor.ext.height = pixels_to_EMU(obj.height)
     return anchor
 
 
+
+class Choice(Serialisable):
+    """Markup compatiblity choice"""
+
+    tagname = "choice"
+
+    twoCellAnchor = Typed(expected_type=TwoCellAnchor, allow_none=True)
+    oneCellAnchor = Typed(expected_type=OneCellAnchor, allow_none=True)
+    absoluteAnchor = Typed(expected_type=AbsoluteAnchor, allow_none=True)
+    Requires = String()
+
+
+    def __init__(self,
+                 twoCellAnchor=None,
+                 oneCellAnchor=None,
+                 absoluteAnchor=None,
+                 Requires=None):
+        self.Requires = Requires
+        self.twoCellAnchor = twoCellAnchor
+        self.oneCellAnchor = oneCellAnchor
+        self.absoluteAnchor = absoluteAnchor
+
+
+class AlternateContent(Serialisable):
+    """Markup AlternateContent
+    """
+
+    tagname = "AlternateContent"
+
+    Choice = Typed(expected_type=Choice)
+
+
+    def __init__(self, Choice=None):
+        self.Choice = Choice
+
+
 class SpreadsheetDrawing(Serialisable):
 
     tagname = "wsDr"
     mime_type = "application/vnd.openxmlformats-officedocument.drawing+xml"
     _rel_type = "http://schemas.openxmlformats.org/officeDocument/2006/relationships/drawing"
     _path = PartName="/xl/drawings/drawing{0}.xml"
     _id = None
 
-    twoCellAnchor = Sequence(expected_type=TwoCellAnchor, allow_none=True)
-    oneCellAnchor = Sequence(expected_type=OneCellAnchor, allow_none=True)
-    absoluteAnchor = Sequence(expected_type=AbsoluteAnchor, allow_none=True)
+    twoCellAnchor = Sequence(expected_type=TwoCellAnchor)
+    oneCellAnchor = Sequence(expected_type=OneCellAnchor)
+    absoluteAnchor = Sequence(expected_type=AbsoluteAnchor)
+    AlternateContent = Sequence(expected_type=AlternateContent)
 
-    __elements__ = ("twoCellAnchor", "oneCellAnchor", "absoluteAnchor")
+    __elements__ = ("twoCellAnchor", "oneCellAnchor", "absoluteAnchor",)
 
     def __init__(self,
                  twoCellAnchor=(),
                  oneCellAnchor=(),
                  absoluteAnchor=(),
+                 AlternateContent=(),
                  ):
         self.twoCellAnchor = twoCellAnchor
         self.oneCellAnchor = oneCellAnchor
         self.absoluteAnchor = absoluteAnchor
         self.charts = []
         self.images = []
-        self._rels = []
+        self.shapes = []
+        self._rels = RelationshipList()
+        if AlternateContent:
+            for obj in AlternateContent:
+                if obj.Choice.twoCellAnchor:
+                    self.twoCellAnchor.append(obj.Choice.twoCellAnchor)
+                elif obj.Choice.oneCellAnchor:
+                    self.oneCellAnchor.append(obj.Choice.oneCellAnchor)
+                elif obj.Choice.absoluteAnchor:
+                    self.absoluteAnchor.append(obj.Choice.absoluteAnchor)
 
 
     def __hash__(self):
         """
         Just need to check for identity
         """
         return id(self)
 
 
     def __bool__(self):
-        return bool(self.charts) or bool(self.images)
-
+        return bool(self.charts) or bool(self.images) or bool(self.shapes)
 
 
     def _write(self):
         """
         create required structure and the serialise
         """
         anchors = []
-        for idx, obj in enumerate(self.charts + self.images, 1):
+        for idx, obj in enumerate(self.charts + self.images + self.shapes, 1):
+            rel = None
             anchor = _check_anchor(obj)
             if isinstance(obj, ChartBase):
                 rel = Relationship(type="chart", Target=obj.path)
-                anchor.graphicFrame = self._chart_frame(idx)
+                anchor.graphicFrame = self._chart_frame(idx, anchor.graphicFrame)
+                if obj.hidden:
+                    anchor.graphicFrame.props.non_visual_props.hidden = True
+
             elif isinstance(obj, Image):
                 rel = Relationship(type="image", Target=obj.path)
-                child = anchor.pic or anchor.groupShape and anchor.groupShape.pic
-                if not child:
-                    anchor.pic = self._picture_frame(idx)
+                if anchor.pic:
+                    child = anchor.pic
+                    child.blipFill.blip.embed = f"rId{idx}"
+
                 else:
-                    child.blipFill.blip.embed = "rId{0}".format(idx)
+                    anchor.pic = self._picture_frame(idx)
+
+            elif isinstance(obj, ImageGroup):
+                for img, pic in zip(obj.images, anchor.groupShape.pic):
+                    rel = Relationship(type="image", Target=img.path)
+                    self._rels.append(rel)
+                    pic.blipFill.blip.embed = rel.Id
+                    rel = None # reset to stop it being added twice
+
+            else:
+                link = getattr(obj.nvSpPr.cNvPr, "hlinkClick")
+                if link:
+                    link.id = f"rId{idx}"
+                    rel = Relationship(
+                        type="hyperlink",
+                        Target=link.target,
+                        TargetMode=link.mode,
+                        Id=f"rId{idx}",
+                    )
 
             anchors.append(anchor)
-            self._rels.append(rel)
+            if rel:
+                self._rels.append(rel)
 
         for a in anchors:
             if isinstance(a, OneCellAnchor):
                 self.oneCellAnchor.append(a)
             elif isinstance(a, TwoCellAnchor):
                 self.twoCellAnchor.append(a)
             else:
                 self.absoluteAnchor.append(a)
 
         tree = self.to_tree()
         tree.set('xmlns', SHEET_DRAWING_NS)
         return tree
 
 
-    def _chart_frame(self, idx):
+    def _chart_frame(self, idx, frame=None):
         chart_rel = ChartRelation(f"rId{idx}")
-        frame = GraphicFrame()
-        nv = frame.nvGraphicFramePr.cNvPr
-        nv.id = idx
-        nv.name = "Chart {0}".format(idx)
+        if frame is None:
+            frame = GraphicFrame()
+            frame.props.non_visual_props.name = "Chart {0}".format(idx)
+        frame.props.non_visual_props.id = idx
         frame.graphic.graphicData.chart = chart_rel
         return frame
 
 
     def _picture_frame(self, idx):
         pic = PictureFrame()
         pic.nvPicPr.cNvPr.descr = "Picture"
@@ -328,17 +225,15 @@
 
         pic.spPr.prstGeom = PresetGeometry2D(prst="rect")
         pic.spPr.ln = None
         return pic
 
 
     def _write_rels(self):
-        rels = RelationshipList()
-        rels.Relationship = self._rels
-        return rels.to_tree()
+        return self._rels.to_tree()
 
 
     @property
     def path(self):
         return self._path.format(self._id)
 
 
@@ -351,15 +246,14 @@
         anchors = self.absoluteAnchor + self.oneCellAnchor + self.twoCellAnchor
         for anchor in anchors:
             if anchor.graphicFrame is not None:
                 graphic = anchor.graphicFrame.graphic
                 rel = graphic.graphicData.chart
                 if rel is not None:
                     rel.anchor = anchor
-                    rel.anchor.graphicFrame = None
                     rels.append(rel)
         return rels
 
 
     @property
     def _blip_rels(self):
         """
@@ -367,15 +261,53 @@
 
         Images that are not part of the XLSX package will be ignored.
         """
         rels = []
         anchors = self.absoluteAnchor + self.oneCellAnchor + self.twoCellAnchor
 
         for anchor in anchors:
-            child = anchor.pic or anchor.groupShape and anchor.groupShape.pic
-            if child and child.blipFill:
-                rel = child.blipFill.blip
-                if rel is not None and rel.embed:
-                    rel.anchor = anchor
-                    rels.append(rel)
+            child = anchor._content
+            if isinstance(child, PictureFrame):
+                img = child._image
+                if img:
+                    img.anchor = anchor
+                    img.properties = child.spPr
+                    rels.append(img)
+
+        return rels
+
+
+    @property
+    def _group_rels(self):
+        """
+        Extract groups of images
+        """
+        rels = []
+        anchors = self.absoluteAnchor + self.oneCellAnchor + self.twoCellAnchor
+
+        for anchor in anchors:
+            child = anchor._content
+
+            if isinstance(child, GroupShape):
+                group = [anchor]
+                for pic in child.pic:
+                    img = pic._image
+                    if img is not None:
+                        img.properties = pic.spPr
+                        group.append(img)
+
+                rels.append(group)
 
         return rels
+
+
+    @property
+    def _shapes(self):
+        """Return a list of shapes"""
+        shapes = []
+        anchors = self.absoluteAnchor + self.oneCellAnchor + self.twoCellAnchor
+        for anchor in anchors:
+            if anchor.sp is not None:
+                shape = anchor.sp
+                shape.anchor = anchor
+                shapes.append(shape)
+        return shapes
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/text.py` & `openpyxl-3.2.0b1/openpyxl/drawing/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Typed,
     Set,
@@ -11,39 +11,34 @@
     String,
     Bool,
     MinMax,
     Integer
 )
 from openpyxl.descriptors.excel import (
     HexBinary,
+    TextPoint,
     Coordinate,
+    ExtensionList,
     Relation,
 )
 from openpyxl.descriptors.nested import (
     NestedInteger,
+    NestedString,
     NestedText,
     NestedValue,
     EmptyTag
 )
 from openpyxl.xml.constants import DRAWING_NS
 
 
 from .colors import ColorChoiceDescriptor
-from .effect import (
-    EffectList,
-    EffectContainer,
-)
-from .fill import(
-    GradientFillProperties,
-    BlipFillProperties,
-    PatternFillProperties,
-    Blip
-)
+from .effect import *
+from .fill import *
+from .line import LineProperties
 from .geometry import (
-    LineProperties,
     Color,
     Scene3D
 )
 
 from openpyxl.descriptors.excel import ExtensionList as OfficeArtExtensionList
 from openpyxl.descriptors.nested import NestedBool
 
@@ -70,14 +65,17 @@
     history = Bool(allow_none=True)
     highlightClick = Bool(allow_none=True)
     endSnd = Bool(allow_none=True)
     snd = Typed(expected_type=EmbeddedWAVAudioFile, allow_none=True)
     extLst = Typed(expected_type=OfficeArtExtensionList, allow_none=True)
     id = Relation(allow_none=True)
 
+    target = "" # somewhere to store the URL
+    mode = ""
+
     __elements__ = ('snd',)
 
     def __init__(self,
                  invalidUrl=None,
                  action=None,
                  tgtFrame=None,
                  tooltip=None,
@@ -579,37 +577,41 @@
         self.fmla = fmla
 
 
 class GeomGuideList(Serialisable):
 
     gd = Sequence(expected_type=GeomGuide, allow_none=True)
 
+    __elements__ = ("gd",)
+
     def __init__(self,
-                 gd=None,
+                 gd=(),
                 ):
         self.gd = gd
 
 
 class PresetTextShape(Serialisable):
 
-    prst = Typed(expected_type=Set(values=(
+    prst = Set(values=(
         ['textNoShape', 'textPlain','textStop', 'textTriangle', 'textTriangleInverted', 'textChevron',
          'textChevronInverted', 'textRingInside', 'textRingOutside', 'textArchUp',
          'textArchDown', 'textCircle', 'textButton', 'textArchUpPour',
          'textArchDownPour', 'textCirclePour', 'textButtonPour', 'textCurveUp',
          'textCurveDown', 'textCanUp', 'textCanDown', 'textWave1', 'textWave2',
          'textDoubleWave1', 'textWave4', 'textInflate', 'textDeflate',
          'textInflateBottom', 'textDeflateBottom', 'textInflateTop',
          'textDeflateTop', 'textDeflateInflate', 'textDeflateInflateDeflate',
          'textFadeRight', 'textFadeLeft', 'textFadeUp', 'textFadeDown',
          'textSlantUp', 'textSlantDown', 'textCascadeUp', 'textCascadeDown'
          ]
-    )))
+    ))
     avLst = Typed(expected_type=GeomGuideList, allow_none=True)
 
+    __elements__ = ("avLst",)
+
     def __init__(self,
                  prst=None,
                  avLst=None,
                 ):
         self.prst = prst
         self.avLst = avLst
```

### Comparing `openpyxl-3.1.2/openpyxl/drawing/xdr.py` & `openpyxl-3.2.0b1/openpyxl/drawing/xdr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 Spreadsheet Drawing has some copies of Drawing ML elements
 """
 
 from .geometry import Point2D, PositiveSize2D, Transform2D
```

### Comparing `openpyxl-3.1.2/openpyxl/formatting/formatting.py` & `openpyxl-3.2.0b1/openpyxl/formatting/formatting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from collections import OrderedDict
 
 from openpyxl.descriptors import (
     Bool,
+    String,
     Sequence,
     Alias,
     Convertible,
 )
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 from .rule import Rule
 
 from openpyxl.worksheet.cell_range import MultiCellRange
 
 class ConditionalFormatting(Serialisable):
@@ -34,15 +36,15 @@
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         return self.sqref == other.sqref
 
 
     def __hash__(self):
-        return hash(self.sqref)
+        return hash(str(self.sqref))
 
 
     def __repr__(self):
         return "<{cls} {cells}>".format(cls=self.__class__.__name__, cells=self.sqref)
 
 
     def __contains__(self, coord):
@@ -78,14 +80,16 @@
 
         self._cf_rules.setdefault(cf, []).append(rule)
 
 
     def __bool__(self):
         return bool(self._cf_rules)
 
+    __nonzero = __bool__
+
 
     def __len__(self):
         return len(self._cf_rules)
 
 
     def __iter__(self):
         for cf, rules in self._cf_rules.items():
```

### Comparing `openpyxl-3.1.2/openpyxl/formatting/rule.py` & `openpyxl-3.2.0b1/openpyxl/formatting/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     String,
     Sequence,
     Bool,
@@ -16,15 +16,15 @@
 from openpyxl.styles.differential import DifferentialStyle
 
 from openpyxl.utils.cell import COORD_RE
 
 
 class ValueDescriptor(Float):
     """
-    Expected type depends upon type attribute of parent :-(
+    Expected type depends upon type attribue of parent :-(
 
     Most values should be numeric BUT they can also be cell references
     """
 
     def __set__(self, instance, value):
         ref = None
         if value is not None and isinstance(value, str):
```

### Comparing `openpyxl-3.1.2/openpyxl/formula/tokenizer.py` & `openpyxl-3.2.0b1/openpyxl/formula/tokenizer.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/formula/translate.py` & `openpyxl-3.2.0b1/openpyxl/formula/translate.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/packaging/core.py` & `openpyxl-3.2.0b1/openpyxl/packaging/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import datetime
 
+from openpyxl.compat import safe_string
 from openpyxl.descriptors import (
+    String,
     DateTime,
     Alias,
-)
+    )
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors.nested import NestedText
-from openpyxl.xml.functions import (
-    Element,
-    QName,
-)
+from openpyxl.xml.functions import (Element, QName, tostring)
 from openpyxl.xml.constants import (
     COREPROPS_NS,
     DCORE_NS,
     XSI_NS,
     DCTERMS_NS,
+    DCTERMS_PREFIX
 )
 
-
 class NestedDateTime(DateTime, NestedText):
 
     expected_type = datetime.datetime
 
     def to_tree(self, tagname=None, value=None, namespace=None):
         namespace = getattr(self, "namespace", namespace)
         if namespace is not None:
@@ -70,45 +69,44 @@
     identifier = NestedText(expected_type=str, allow_none=True, namespace=DCORE_NS)
     language = NestedText(expected_type=str, allow_none=True, namespace=DCORE_NS)
     # Dublin Core Terms
     created = QualifiedDateTime(allow_none=True, namespace=DCTERMS_NS)
     modified = QualifiedDateTime(allow_none=True, namespace=DCTERMS_NS)
 
     __elements__ = ("creator", "title", "description", "subject","identifier",
-                    "language", "created", "modified", "lastModifiedBy", "category",
-                    "contentStatus", "version", "revision", "keywords", "lastPrinted",
-                    )
+                  "language", "created", "modified", "lastModifiedBy", "category",
+                  "contentStatus", "version", "revision", "keywords", "lastPrinted",
+                  )
 
 
     def __init__(self,
                  category=None,
                  contentStatus=None,
                  keywords=None,
                  lastModifiedBy=None,
                  lastPrinted=None,
                  revision=None,
                  version=None,
-                 created=None,
+                 created=datetime.datetime.utcnow(),
                  creator="openpyxl",
                  description=None,
                  identifier=None,
                  language=None,
-                 modified=None,
+                 modified=datetime.datetime.utcnow(),
                  subject=None,
                  title=None,
                  ):
-        now = datetime.datetime.utcnow()
         self.contentStatus = contentStatus
         self.lastPrinted = lastPrinted
         self.revision = revision
         self.version = version
         self.creator = creator
         self.lastModifiedBy = lastModifiedBy
-        self.modified = modified or now
-        self.created = created or now
+        self.modified = modified
+        self.created = created
         self.title = title
         self.subject = subject
         self.description = description
         self.identifier = identifier
         self.language = language
         self.keywords = keywords
         self.category = category
```

### Comparing `openpyxl-3.1.2/openpyxl/packaging/custom.py` & `openpyxl-3.2.0b1/openpyxl/packaging/custom.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,286 +1,214 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Implementation of custom properties see § 22.3 in the specification"""
 
-
-from warnings import warn
-
-from openpyxl.descriptors import Strict
+import datetime
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors.sequence import Sequence
 from openpyxl.descriptors import (
     Alias,
     String,
     Integer,
-    Float,
-    DateTime,
-    Bool,
 )
 from openpyxl.descriptors.nested import (
     NestedText,
 )
 
 from openpyxl.xml.constants import (
     CUSTPROPS_NS,
     VTYPES_NS,
     CPROPS_FMTID,
 )
 
 from .core import NestedDateTime
 
+# from Python
+KNOWN_TYPES = {
+    str: "str",
+    int: "i4",
+    float: "r8",
+    datetime.datetime: "filetime",
+    bool: "bool",
+}
 
-class NestedBoolText(Bool, NestedText):
-    """
-    Descriptor for handling nested elements with the value stored in the text part
-    """
-
-    pass
-
+# from XML
+XML_TYPES = {
+    "lwpstr": str,
+    "i4": int,
+    "r8": float,
+    "filetime": datetime.datetime,
+    "bool": bool,
+}
 
-class _CustomDocumentProperty(Serialisable):
+class CustomDocumentProperty(Serialisable):
 
     """
-    Low-level representation of a Custom Document Property.
-    Not used directly
-    Must always contain a child element, even if this is empty
+    to read/write a single Workbook.CustomDocumentProperty saved in 'docProps/custom.xml'
     """
 
     tagname = "property"
-    _typ = None
 
     name = String(allow_none=True)
     lpwstr = NestedText(expected_type=str, allow_none=True, namespace=VTYPES_NS)
     i4 = NestedText(expected_type=int, allow_none=True, namespace=VTYPES_NS)
     r8 = NestedText(expected_type=float, allow_none=True, namespace=VTYPES_NS)
     filetime = NestedDateTime(allow_none=True, namespace=VTYPES_NS)
-    bool = NestedBoolText(expected_type=bool, allow_none=True, namespace=VTYPES_NS)
+    bool = NestedText(expected_type=bool, allow_none=True, namespace=VTYPES_NS)
     linkTarget = String(expected_type=str, allow_none=True)
     fmtid = String()
     pid = Integer()
 
     def __init__(self,
                  name=None,
-                 pid=0,
-                 fmtid=CPROPS_FMTID,
+                 value=None,
+                 typ=None,
+                 lpwstr=None,
+                 i4=None,
+                 r8=None,
+                 filetime=None,
+                 bool=None,
                  linkTarget=None,
-                 **kw):
+                 pid=0,
+                 fmtid=CPROPS_FMTID):
         self.fmtid = fmtid
         self.pid = pid
         self.name = name
-        self._typ = None
+
+        self.lpwstr = lpwstr
+        self.i4 = i4
+        self.r8 = r8
+        self.filetime = filetime
+        self.bool = bool
         self.linkTarget = linkTarget
 
-        for k, v in kw.items():
-            setattr(self, k, v)
-            setattr(self, "_typ", k) # ugh!
-        for e in self.__elements__:
-            if e not in kw:
-                setattr(self, e, None)
+        if linkTarget is not None:
+            self.lpwstr = ""
 
+        if value is not None:
+            t = type(value)
+            prop = KNOWN_TYPES.get(t)
+            if prop is not None:
+                setattr(self, prop, value)
+            elif typ is not None and typ in XML_TYPES:
+                setattr(self, typ, value)
+            else:
+                raise ValueError(f"Unknown type {t}")
+
+
+    @property
+    def value(self):
+        """Return the value from the active property"""
+        for a in self.__elements__:
+            v = getattr(self, a)
+            if v is not None:
+                return v
 
     @property
     def type(self):
-        if self._typ is not None:
-            return self._typ
         for a in self.__elements__:
             if getattr(self, a) is not None:
                 return a
-        if self.linkTarget is not None:
-            return "linkTarget"
-
 
-    def to_tree(self, tagname=None, idx=None, namespace=None):
-        child = getattr(self, self._typ, None)
-        if child is None:
-            setattr(self, self._typ, "")
 
-        return super().to_tree(tagname=None, idx=None, namespace=None)
 
-
-class _CustomDocumentPropertyList(Serialisable):
+class CustomDocumentPropertyList(Serialisable):
 
     """
-    Parses and seriliases property lists but is not used directly
+    to capture the Workbook.CustomDocumentProperties saved in 'docProps/custom.xml'
     """
 
     tagname = "Properties"
 
-    property = Sequence(expected_type=_CustomDocumentProperty, namespace=CUSTPROPS_NS)
+    property = Sequence(expected_type=CustomDocumentProperty, namespace=CUSTPROPS_NS)
     customProps = Alias("property")
 
 
-    def __init__(self, property=()):
+    def __init__(self, property=(), customProps=()):
         self.property = property
+        if customProps:
+            self.customProps = customProps
 
 
-    def __len__(self):
-        return len(self.property)
-
-
-    def to_tree(self, tagname=None, idx=None, namespace=None):
-        for idx, p in enumerate(self.property, 2):
-            p.pid = idx
-        tree = super().to_tree(tagname, idx, namespace)
-        tree.set("xmlns", CUSTPROPS_NS)
-
-        return tree
-
-
-class _TypedProperty(Strict):
-
-    name = String()
-
-    def __init__(self,
-                 name,
-                 value):
-        self.name = name
-        self.value = value
-
-
-    def __eq__(self, other):
-        return self.name == other.name and self.value == other.value
-
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}, name={self.name}, value={self.value}"
-
-
-class IntProperty(_TypedProperty):
-
-    value = Integer()
-
-
-class FloatProperty(_TypedProperty):
-
-    value = Float()
-
-
-class StringProperty(_TypedProperty):
-
-    value = String(allow_none=True)
-
-
-class DateTimeProperty(_TypedProperty):
-
-    value = DateTime()
-
-
-class BoolProperty(_TypedProperty):
-
-    value = Bool()
-
-
-class LinkProperty(_TypedProperty):
-
-    value = String()
-
-
-# from Python
-CLASS_MAPPING = {
-    StringProperty: "lpwstr",
-    IntProperty: "i4",
-    FloatProperty: "r8",
-    DateTimeProperty: "filetime",
-    BoolProperty: "bool",
-    LinkProperty: "linkTarget"
-}
-
-XML_MAPPING = {v:k for k,v in CLASS_MAPPING.items()}
-
+    def _duplicate(self, prop):
+        """
+        Check for whether customProps with the same name already exists
+        """
+        for p in self.customProps:
+            if d.name == prop.name:
+                return True
 
-class CustomPropertyList(Strict):
 
+    def append(self, prop):
+        if not isinstance(prop, CustomDocumentProperty):
+            raise TypeError("""You can only append CustomDocumentProperty objects""")
+        if self._duplicate(prop):
+            raise ValueError("""Document property with the same name already exists""")
+        names = self.customProps[:]
+        names.append(prop)
+        self.customProps = names
 
-    props = Sequence(expected_type=_TypedProperty)
 
-    def __init__(self):
-        self.props = []
+    def __len__(self):
+        return len(self.customProps)
 
 
-    @classmethod
-    def from_tree(cls, tree):
+    def __contains__(self, name):
         """
-        Create list from OOXML element
+        Check for property by name
         """
-        prop_list = _CustomDocumentPropertyList.from_tree(tree)
-        new_props = cls()
-        for prop in prop_list.property:
-            attr = prop.type
-
-            typ = XML_MAPPING.get(attr, None)
-            if not typ:
-                warn(f"Unknown type for {prop.name}")
-                continue
-            value = getattr(prop, attr)
-            link = prop.linkTarget
-            if link is not None:
-                typ = LinkProperty
-                value = prop.linkTarget
+        for prop in self.customProps:
+            if prop.name == name:
+                return True
 
-            new_prop = typ(name=prop.name, value=value)
-            new_props.append(new_prop)
-        return new_props
 
-
-    def append(self, prop):
-        if prop.name in self.names:
-            raise ValueError(f"Property with name {prop.name} already exists")
-        props = self.props
-        props.append(prop)
-        self.props = props
-
-
-    def to_tree(self):
-        props = []
-
-        for p in self.props:
-            attr = CLASS_MAPPING.get(p.__class__, None)
-            if not attr:
-                raise TypeError("Unknown adapter for {p}")
-            np = _CustomDocumentProperty(name=p.name, **{attr:p.value})
-            if isinstance(p, LinkProperty):
-                np._typ = "lpwstr"
-                #np.lpwstr = ""
-            props.append(np)
-
-        prop_list = _CustomDocumentPropertyList(property=props)
-        return prop_list.to_tree()
+    def __getitem__(self, name):
+        """
+        Access document properties by name
+        """
+        defn = self.get(name)
+        if not defn:
+            raise KeyError(f"No docuemnt property called {name}")
+        return defn
 
 
-    def __len__(self):
-        return len(self.props)
+    def get(self, name):
+        """
+        Find a property by name
+        """
+        for defn in self.customProps:
+            if defn.name == name:
+                return defn
 
 
-    @property
-    def names(self):
-        """List of property names"""
-        return [p.name for p in self.props]
+    def __delitem__(self, name):
+        """
+        Delete a property
+        """
+        if not self.delete(name):
+            raise KeyError(f"No defined name {name}")
 
 
-    def __getitem__(self, name):
+    def delete(self, name):
         """
-        Get property by name
+        Delete a property
         """
-        for p in self.props:
-            if p.name == name:
-                return p
-        raise KeyError(f"Property with name {name} not found")
+        for idx, prop in enumerate(self.customProps):
+            if prop.name == name:
+                del self.customProps[idx]
+                return True
 
 
-    def __delitem__(self, name):
+    def namelist(self):
         """
-        Delete a propery by name
+        Provide a list of all custom document property names
         """
-        for idx, p in enumerate(self.props):
-            if p.name == name:
-                self.props.pop(idx)
-                return
-        raise KeyError(f"Property with name {name} not found")
-
+        return [prop.name for prop in self.customProps]
 
-    def __repr__(self):
-        return f"{self.__class__.__name__} containing {self.props}"
 
+    def to_tree(self, tagname=None, idx=None, namespace=None):
+        for idx, p in enumerate(self.property, 2):
+            p.pid = idx
+        tree = super().to_tree(tagname, idx, namespace)
+        tree.set("xmlns", CUSTPROPS_NS)
 
-    def __iter__(self):
-        return iter(self.props)
+        return tree
```

### Comparing `openpyxl-3.1.2/openpyxl/packaging/extended.py` & `openpyxl-3.2.0b1/openpyxl/packaging/extended.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
 )
 from openpyxl.descriptors.nested import (
```

### Comparing `openpyxl-3.1.2/openpyxl/packaging/interface.py` & `openpyxl-3.2.0b1/openpyxl/packaging/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from abc import abstractproperty
 from openpyxl.compat.abc import ABC
 
 
 class ISerialisableFile(ABC):
```

### Comparing `openpyxl-3.1.2/openpyxl/packaging/manifest.py` & `openpyxl-3.2.0b1/openpyxl/packaging/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 File manifest
 """
 from mimetypes import MimeTypes
 import os.path
 
@@ -25,14 +25,15 @@
 # initialise mime-types
 mimetypes = MimeTypes()
 mimetypes.add_type('application/xml', ".xml")
 mimetypes.add_type('application/vnd.openxmlformats-package.relationships+xml', ".rels")
 mimetypes.add_type("application/vnd.ms-office.vbaProject", ".bin")
 mimetypes.add_type("application/vnd.openxmlformats-officedocument.vmlDrawing", ".vml")
 mimetypes.add_type("image/x-emf", ".emf")
+mimetypes.add_type("image/x-wmf", ".wmf")
 
 
 class FileExtension(Serialisable):
 
     tagname = "Default"
 
     Extension = String()
@@ -179,16 +180,33 @@
             self.Default.append(fe)
 
 
     def _write_vba(self, workbook):
         """
         Add content types from cached workbook when keeping VBA
         """
+        if workbook._vba:
+            ct = Override(PartName="/xl/vbaProject.bin", ContentType=VBA)
+            self.Override.append(ct)
         if workbook.vba_archive:
             node = fromstring(workbook.vba_archive.read(ARC_CONTENT_TYPES))
             mf = Manifest.from_tree(node)
             filenames = self.filenames
             for override in mf.Override:
-                if override.PartName not in (ACTIVEX, CTRL, VBA):
+                if override.PartName not in (VBA,):
                     continue
                 if override.PartName not in filenames:
                     self.Override.append(override)
+
+
+class ManifestObject:
+
+    """
+    API for anything that gets added to to the manifest
+    """
+
+    path = None # absolute path within zip archive
+    mime_type = None
+
+    def __init__(self, path, mime_type):
+        self.path = path
+        self.mime_type = mime_type
```

### Comparing `openpyxl-3.1.2/openpyxl/packaging/relationship.py` & `openpyxl-3.2.0b1/openpyxl/packaging/relationship.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
+
 
 import posixpath
-from warnings import warn
 
 from openpyxl.descriptors import (
     String,
     Alias,
     Sequence,
 )
 from openpyxl.descriptors.serialisable import Serialisable
@@ -100,44 +100,62 @@
             if not rel.Id:
                 rel.Id = "rId{0}".format(idx)
             tree.append(rel.to_tree())
 
         return tree
 
 
+    def get_types(self):
+        """Return a set of types contained"""
+        known_types = set()
+        for r in self.Relationship:
+            simple = r.Type.split("/")[-1]
+            if simple not in known_types:
+                known_types.add(simple)
+                collection = []
+                setattr(self, simple, collection)
+            else:
+                collection = getattr(self, simple)
+            collection.append(r)
+
+
 def get_rels_path(path):
     """
     Convert relative path to absolutes that can be loaded from a zip
     archive.
     The path to be passed in is that of containing object (workbook,
     worksheet, etc.)
     """
     folder, obj = posixpath.split(path)
     filename = posixpath.join(folder, '_rels', '{0}.rels'.format(obj))
     return filename
 
 
+from warnings import warn
+
 def get_dependents(archive, filename):
     """
     Normalise dependency file paths to absolute ones
 
     Relative paths are relative to parent object
+
+    Do nothing with hyperlinks
     """
     src = archive.read(filename)
     node = fromstring(src)
     try:
         rels = RelationshipList.from_tree(node)
     except TypeError:
         msg = "{0} contains invalid dependency definitions".format(filename)
         warn(msg)
         rels = RelationshipList()
     folder = posixpath.dirname(filename)
     parent = posixpath.split(folder)[0]
     for r in rels.Relationship:
-        if r.TargetMode == "External":
+        if r.TargetMode == "External" or "hyperlink" in r.Type:
             continue
         elif r.target.startswith("/"):
             r.target = r.target[1:]
         else:
             pth = posixpath.join(parent, r.target)
             r.target = posixpath.normpath(pth)
     return rels
```

### Comparing `openpyxl-3.1.2/openpyxl/packaging/workbook.py` & `openpyxl-3.2.0b1/openpyxl/packaging/workbook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Typed,
     String,
     Integer,
     Bool,
     NoneSet,
+    Set,
+    Sequence,
 )
 from openpyxl.descriptors.excel import ExtensionList, Relation
 from openpyxl.descriptors.sequence import NestedSequence
 from openpyxl.descriptors.nested import NestedString
 
 from openpyxl.xml.constants import SHEET_MAIN_NS
 
-from openpyxl.workbook.defined_name import DefinedNameList
+from openpyxl.workbook.defined_name import DefinedName, DefinedNameList
 from openpyxl.workbook.external_reference import ExternalReference
 from openpyxl.workbook.function_group import FunctionGroupList
 from openpyxl.workbook.properties import WorkbookProperties, CalcProperties, FileVersion
 from openpyxl.workbook.protection import WorkbookProtection, FileSharing
 from openpyxl.workbook.smart_tags import SmartTagList, SmartTagProperties
 from openpyxl.workbook.views import CustomWorkbookView, BookView
 from openpyxl.workbook.web import WebPublishing, WebPublishObjectList
@@ -179,7 +181,24 @@
 
     @property
     def active(self):
         for view in self.bookViews:
             if view.activeTab is not None:
                 return view.activeTab
         return 0
+
+
+    @property
+    def pivot_caches(self):
+        """
+        Get PivotCache objects
+        """
+        d = {}
+        for c in self.caches:
+            cache = get_rel(self.archive, self.rels, id=c.id, cls=CacheDefinition)
+            if cache.deps:
+                records = get_rel(self.archive, cache.deps, cache.id, RecordList)
+            else:
+                records = None
+            cache.records = records
+            d[c.cacheId]  = cache
+        return d
```

### Comparing `openpyxl-3.1.2/openpyxl/pivot/cache.py` & `openpyxl-3.2.0b1/openpyxl/pivot/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Bool,
     Float,
     Set,
```

### Comparing `openpyxl-3.1.2/openpyxl/pivot/fields.py` & `openpyxl-3.2.0b1/openpyxl/pivot/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     DateTime,
     Bool,
     Float,
```

### Comparing `openpyxl-3.1.2/openpyxl/pivot/record.py` & `openpyxl-3.2.0b1/openpyxl/pivot/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Integer,
     Sequence,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/pivot/table.py` & `openpyxl-3.2.0b1/openpyxl/pivot/table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,50 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
-
-from collections import defaultdict
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Integer,
     NoneSet,
     Set,
+    Float,
     Bool,
+    DateTime,
     String,
+    Alias,
     Bool,
     Sequence,
 )
 
 from openpyxl.descriptors.excel import ExtensionList, Relation
+from openpyxl.descriptors.nested import NestedInteger
 from openpyxl.descriptors.sequence import NestedSequence
 from openpyxl.xml.constants import SHEET_MAIN_NS
 from openpyxl.xml.functions import tostring
 from openpyxl.packaging.relationship import (
     RelationshipList,
     Relationship,
     get_rels_path
 )
 from .fields import Index
 
 from openpyxl.worksheet.filters import (
     AutoFilter,
+    CellRange,
+    ColorFilter,
+    CustomFilter,
+    CustomFilters,
+    DateGroupItem,
+    DynamicFilter,
+    FilterColumn,
+    Filters,
+    IconFilter,
+    SortCondition,
+    SortState,
+    Top10,
 )
 
 
 class HierarchyUsage(Serialisable):
 
     tagname = "hierarchyUsage"
 
@@ -314,15 +328,15 @@
     minSubtotal = Bool(allow_none=True)
     productSubtotal = Bool(allow_none=True)
     countSubtotal = Bool(allow_none=True)
     stdDevSubtotal = Bool(allow_none=True)
     stdDevPSubtotal = Bool(allow_none=True)
     varSubtotal = Bool(allow_none=True)
     varPSubtotal = Bool(allow_none=True)
-    x = Sequence(expected_type=Index)
+    x = NestedInteger(allow_none=True, attribute="v")
     extLst = Typed(expected_type=ExtensionList, allow_none=True)
 
     __elements__ = ('x',)
 
     def __init__(self,
                  field=None,
                  count=None,
@@ -337,15 +351,15 @@
                  minSubtotal=None,
                  productSubtotal=None,
                  countSubtotal=None,
                  stdDevSubtotal=None,
                  stdDevPSubtotal=None,
                  varSubtotal=None,
                  varPSubtotal=None,
-                 x=(),
+                 x=None,
                  extLst=None,
                 ):
         self.field = field
         self.selected = selected
         self.byPosition = byPosition
         self.relative = relative
         self.defaultSubtotal = defaultSubtotal
@@ -467,90 +481,14 @@
         self.scope = scope
         self.type = type
         self.priority = priority
         self.pivotAreas = pivotAreas
         self.extLst = extLst
 
 
-class ConditionalFormatList(Serialisable):
-
-    tagname = "conditionalFormats"
-
-    conditionalFormat = Sequence(expected_type=ConditionalFormat)
-
-    __attrs__ = ("count",)
-
-    def __init__(self, conditionalFormat=(), count=None):
-        self.conditionalFormat = conditionalFormat
-
-
-    def by_priority(self):
-        """
-        Return a dictionary of format objects keyed by (field id and format property).
-        This can be used to map the formats to field but also to dedupe to match
-        worksheet definitions which are grouped by cell range
-        """
-
-        fmts = {}
-        for fmt in self.conditionalFormat:
-            for area in fmt.pivotAreas:
-                for ref in area.references:
-                    for field in ref.x:
-                        key = (field.v, fmt.priority)
-                        fmts[key] = fmt
-
-        return fmts
-
-
-    def _dedupe(self):
-        """
-        Group formats by field index and priority.
-        Sorted to match sorting and grouping for corresponding worksheet formats
-
-        The implemtenters notes contain significant deviance from the OOXML
-        specification, in particular how conditional formats in tables relate to
-        those defined in corresponding worksheets and how to determine which
-        format applies to which fields.
-
-        There are some magical interdependencies:
-
-        * Every pivot table fmt must have a worksheet cxf with the same priority.
-
-        * In the reference part the field 4294967294 refers to a data field, the
-        spec says -2
-
-        * Data fields are referenced by the 0-index reference.x.v value
-
-        Things are made more complicated by the fact that field items behave
-        diffently if the parent is a reference or shared item: "In Office if the
-        parent is the reference element, then restrictions of this value are
-        defined by reference@field. If the parent is the tables element, then
-        this value specifies the index into the table tag position in @url."
-        Yeah, right!
-        """
-        fmts = self.by_priority()
-        # sort by priority in order, keeping the highest numerical priority, least when
-        # actually applied
-        # this is not documented but it's what Excel is happy with
-        fmts = {field:fmt for (field, priority), fmt in sorted(fmts.items(), reverse=True)}
-        #fmts = {field:fmt for (field, priority), fmt in fmts.items()}
-        if fmts:
-            self.conditionalFormat = list(fmts.values())
-
-
-    @property
-    def count(self):
-        return len(self.conditionalFormat)
-
-
-    def to_tree(self, tagname=None):
-        self._dedupe()
-        return super().to_tree(tagname)
-
-
 class Format(Serialisable):
 
     tagname = "format"
 
     action = NoneSet(values=(['blank', 'formatting', 'drill', 'formula']))
     dxfId = Integer(allow_none=True)
     pivotArea = Typed(expected_type=PivotArea, )
@@ -1004,15 +942,15 @@
     rowFields = NestedSequence(expected_type=RowColField, count=True)
     rowItems = NestedSequence(expected_type=RowColItem, count=True)
     colFields = NestedSequence(expected_type=RowColField, count=True)
     colItems = NestedSequence(expected_type=RowColItem, count=True)
     pageFields = NestedSequence(expected_type=PageField, count=True)
     dataFields = NestedSequence(expected_type=DataField, count=True)
     formats = NestedSequence(expected_type=Format, count=True)
-    conditionalFormats = Typed(expected_type=ConditionalFormatList, allow_none=True)
+    conditionalFormats = NestedSequence(expected_type=ConditionalFormat, count=True)
     chartFormats = NestedSequence(expected_type=ChartFormat, count=True)
     pivotHierarchies = NestedSequence(expected_type=PivotHierarchy, count=True)
     pivotTableStyleInfo = Typed(expected_type=PivotTableStyle, allow_none=True)
     filters = NestedSequence(expected_type=PivotFilter, count=True)
     rowHierarchiesUsage = Typed(expected_type=RowHierarchiesUsage, allow_none=True)
     colHierarchiesUsage = Typed(expected_type=ColHierarchiesUsage, allow_none=True)
     extLst = Typed(expected_type=ExtensionList, allow_none=True)
@@ -1098,15 +1036,15 @@
                  rowFields=(),
                  rowItems=(),
                  colFields=(),
                  colItems=(),
                  pageFields=(),
                  dataFields=(),
                  formats=(),
-                 conditionalFormats=None,
+                 conditionalFormats=(),
                  chartFormats=(),
                  pivotHierarchies=(),
                  pivotTableStyleInfo=None,
                  filters=(),
                  rowHierarchiesUsage=None,
                  colHierarchiesUsage=None,
                  extLst=None,
@@ -1186,15 +1124,14 @@
         self.rowItems = rowItems
         self.colFields = colFields
         self.colItems = colItems
         self.pageFields = pageFields
         self.dataFields = dataFields
         self.formats = formats
         self.conditionalFormats = conditionalFormats
-        self.conditionalFormats = None
         self.chartFormats = chartFormats
         self.pivotHierarchies = pivotHierarchies
         self.pivotTableStyleInfo = pivotTableStyleInfo
         self.filters = filters
         self.rowHierarchiesUsage = rowHierarchiesUsage
         self.colHierarchiesUsage = colHierarchiesUsage
         self.extLst = extLst
@@ -1235,27 +1172,7 @@
         self.id = r.id
         if self.cache.path[1:] not in archive.namelist():
             self.cache._write(archive, manifest)
 
         path = get_rels_path(self.path)
         xml = tostring(rels.to_tree())
         archive.writestr(path[1:], xml)
-
-
-    def formatted_fields(self):
-        """Map fields to associated conditional formats by priority"""
-        if not self.conditionalFormats:
-            return {}
-        fields = defaultdict(list)
-        for idx, prio in self.conditionalFormats.by_priority():
-            name = self.dataFields[idx].name
-            fields[name].append(prio)
-        return fields
-
-
-    @property
-    def summary(self):
-        """
-        Provide a simplified summary of the table
-        """
-
-        return f"{self.name} {dict(self.location)}"
```

### Comparing `openpyxl-3.1.2/openpyxl/reader/excel.py` & `openpyxl-3.2.0b1/openpyxl/reader/excel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,81 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 """Read an xlsx file into Python"""
 
-# Python stdlib imports
-from zipfile import ZipFile, ZIP_DEFLATED
+# Python stdlib
+from zipfile import (
+    ZipFile,
+
+)
 from io import BytesIO
 import os.path
 import warnings
 
 from openpyxl.pivot.table import TableDefinition
 
 # Allow blanket setting of KEEP_VBA for testing
 try:
     from ..tests import KEEP_VBA
 except ImportError:
     KEEP_VBA = False
 
+
 # package imports
 from openpyxl.utils.exceptions import InvalidFileException
 from openpyxl.xml.constants import (
     ARC_CORE,
     ARC_CUSTOM,
     ARC_CONTENT_TYPES,
     ARC_WORKBOOK,
     ARC_THEME,
-    COMMENTS_NS,
     SHARED_STRINGS,
+    VBA,
     XLTM,
     XLTX,
     XLSM,
     XLSX,
 )
 from openpyxl.cell import MergedCell
 from openpyxl.comments.comment_sheet import CommentSheet
 
 from .strings import read_string_table, read_rich_text
 from .workbook import WorkbookParser
 from openpyxl.styles.stylesheet import apply_stylesheet
 
 from openpyxl.packaging.core import DocumentProperties
-from openpyxl.packaging.custom import CustomPropertyList
+from openpyxl.packaging.custom import CustomDocumentPropertyList
 from openpyxl.packaging.manifest import Manifest, Override
 
 from openpyxl.packaging.relationship import (
     RelationshipList,
     get_dependents,
     get_rels_path,
 )
 
 from openpyxl.worksheet._read_only import ReadOnlyWorksheet
 from openpyxl.worksheet._reader import WorksheetReader
 from openpyxl.chartsheet import Chartsheet
 from openpyxl.worksheet.table import Table
+from openpyxl.worksheet.controls import (
+    FormControl,
+    ActiveXControl
+)
 from openpyxl.drawing.spreadsheet_drawing import SpreadsheetDrawing
+from openpyxl.drawing.legacy import LegacyDrawing
+from openpyxl.drawing.image import Image
 
 from openpyxl.xml.functions import fromstring
 
 from .drawings import find_images
 
 
 SUPPORTED_FORMATS = ('.xlsx', '.xlsm', '.xltx', '.xltm')
 
-
 def _validate_archive(filename):
     """
     Does a first check whether filename is a string or a file-like
     object. If it is a string representing a filename, a check is done
     for supported formats by checking the given file-extension. If the
     file-extension is not in SUPPORTED_FORMATS an InvalidFileException
     will raised. Otherwise the filename (resp. file-like object) will
@@ -114,16 +123,16 @@
 
 class ExcelReader:
 
     """
     Read an Excel package and dispatch the contents to the relevant modules
     """
 
-    def __init__(self, fn, read_only=False, keep_vba=KEEP_VBA,
-                 data_only=False, keep_links=True, rich_text=False):
+    def __init__(self,  fn, read_only=False, keep_vba=KEEP_VBA,
+                  data_only=False, keep_links=True, rich_text=False):
         self.archive = _validate_archive(fn)
         self.valid_files = self.archive.namelist()
         self.read_only = read_only
         self.keep_vba = keep_vba
         self.data_only = data_only
         self.keep_links = keep_links
         self.rich_text = rich_text
@@ -134,57 +143,48 @@
         src = self.archive.read(ARC_CONTENT_TYPES)
         root = fromstring(src)
         self.package = Manifest.from_tree(root)
 
 
     def read_strings(self):
         ct = self.package.find(SHARED_STRINGS)
-        reader = read_string_table
-        if self.rich_text:
-            reader = read_rich_text
         if ct is not None:
             strings_path = ct.PartName[1:]
             with self.archive.open(strings_path,) as src:
-                self.shared_strings = reader(src)
+                self.shared_strings = read_string_table(src)
 
 
     def read_workbook(self):
         wb_part = _find_workbook_part(self.package)
         self.parser = WorkbookParser(self.archive, wb_part.PartName[1:], keep_links=self.keep_links)
         self.parser.parse()
         wb = self.parser.wb
         wb._sheets = []
         wb._data_only = self.data_only
         wb._read_only = self.read_only
         wb.template = wb_part.ContentType in (XLTX, XLTM)
 
-        # If are going to preserve the vba then attach a copy of the archive to the
-        # workbook so that is available for the save.
-        if self.keep_vba:
-            wb.vba_archive = ZipFile(BytesIO(), 'a', ZIP_DEFLATED)
-            for name in self.valid_files:
-                wb.vba_archive.writestr(name, self.archive.read(name))
+        if "xl/vbaProject.bin" in self.archive.namelist():
+            # might also want to search the manifest by content type
+            wb._vba = self.archive.read("xl/vbaProject.bin")
 
         if self.read_only:
             wb._archive = self.archive
 
         self.wb = wb
 
 
     def read_properties(self):
         if ARC_CORE in self.valid_files:
             src = fromstring(self.archive.read(ARC_CORE))
             self.wb.properties = DocumentProperties.from_tree(src)
 
-
-    def read_custom(self):
         if ARC_CUSTOM in self.valid_files:
             src = fromstring(self.archive.read(ARC_CUSTOM))
-            self.wb.custom_doc_props = CustomPropertyList.from_tree(src)
-
+            self.wb.custom_doc_props = CustomDocumentPropertyList.from_tree(src)
 
     def read_theme(self):
         if ARC_THEME in self.valid_files:
             self.wb.loaded_theme = self.archive.read(ARC_THEME)
 
 
     def read_chartsheet(self, sheet, rel):
@@ -200,103 +200,70 @@
         cs = Chartsheet.from_tree(node)
         cs._parent = self.wb
         cs.title = sheet.name
         self.wb._add_sheet(cs)
 
         drawings = rels.find(SpreadsheetDrawing._rel_type)
         for rel in drawings:
-            charts, images = find_images(self.archive, rel.target)
+            charts, images, shapes = find_images(self.archive, rel.target)
             for c in charts:
                 cs.add_chart(c)
 
 
     def read_worksheets(self):
-        comment_warning = """Cell '{0}':{1} is part of a merged range but has a comment which will be removed because merged cells cannot contain any data."""
+
         for sheet, rel in self.parser.find_sheets():
             if rel.target not in self.valid_files:
                 continue
 
             if "chartsheet" in rel.Type:
                 self.read_chartsheet(sheet, rel)
                 continue
 
-            rels_path = get_rels_path(rel.target)
-            rels = RelationshipList()
-            if rels_path in self.valid_files:
-                rels = get_dependents(self.archive, rels_path)
-
             if self.read_only:
                 ws = ReadOnlyWorksheet(self.wb, sheet.name, rel.target, self.shared_strings)
                 ws.sheet_state = sheet.state
                 self.wb._sheets.append(ws)
                 continue
-            else:
-                fh = self.archive.open(rel.target)
-                ws = self.wb.create_sheet(sheet.name)
-                ws._rels = rels
-                ws_parser = WorksheetReader(ws, fh, self.shared_strings, self.data_only, self.rich_text)
-                ws_parser.bind_all()
-
-            # assign any comments to cells
-            for r in rels.find(COMMENTS_NS):
-                src = self.archive.read(r.target)
-                comment_sheet = CommentSheet.from_tree(fromstring(src))
-                for ref, comment in comment_sheet.comments:
-                    try:
-                        ws[ref].comment = comment
-                    except AttributeError:
-                        c = ws[ref]
-                        if isinstance(c, MergedCell):
-                            warnings.warn(comment_warning.format(ws.title, c.coordinate))
-                            continue
-
-            # preserve link to VML file if VBA
-            if self.wb.vba_archive and ws.legacy_drawing:
-                ws.legacy_drawing = rels[ws.legacy_drawing].target
-            else:
-                ws.legacy_drawing = None
+
+            fh = self.archive.open(rel.target)
+            ws = self.wb.create_sheet(sheet.name)
+
+            processor = WorksheetProcessor(ws, self.archive)
+            processor.find_children((rel.target))
+            ws._rels = processor.rels
+
+            ws_parser = WorksheetReader(ws, fh, self.shared_strings, self.data_only, self.rich_text)
+            ws_parser.bind_all()
+            ws.sheet_state = sheet.state
+
+            processor.get_comments()
+            processor.get_pivots(self.parser.pivot_caches)
+            processor.get_drawings()
+            processor.get_activex()
+            processor.get_controls()
+            processor.get_legacy()
 
             for t in ws_parser.tables:
                 src = self.archive.read(t)
                 xml = fromstring(src)
                 table = Table.from_tree(xml)
                 ws.add_table(table)
 
-            drawings = rels.find(SpreadsheetDrawing._rel_type)
-            for rel in drawings:
-                charts, images = find_images(self.archive, rel.target)
-                for c in charts:
-                    ws.add_chart(c, c.anchor)
-                for im in images:
-                    ws.add_image(im, im.anchor)
-
-            pivot_rel = rels.find(TableDefinition.rel_type)
-            for r in pivot_rel:
-                pivot_path = r.Target
-                src = self.archive.read(pivot_path)
-                tree = fromstring(src)
-                pivot = TableDefinition.from_tree(tree)
-                pivot.cache = self.parser.pivot_caches[pivot.cacheId]
-                ws.add_pivot(pivot)
-
-            ws.sheet_state = sheet.state
-
 
     def read(self):
         action = "read manifest"
         try:
             self.read_manifest()
             action = "read strings"
             self.read_strings()
             action = "read workbook"
             self.read_workbook()
             action = "read properties"
             self.read_properties()
-            action = "read custom properties"
-            self.read_custom()
             action = "read theme"
             self.read_theme()
             action = "read stylesheet"
             apply_stylesheet(self.archive, self.wb)
             action = "read worksheets"
             self.read_worksheets()
             action = "assign names"
@@ -307,25 +274,179 @@
             raise ValueError(
                 f"Unable to read workbook: could not {action} from {self.archive.filename}.\n"
                 "This is most probably because the workbook source files contain some invalid XML.\n"
                 "Please see the exception for more details."
                 ) from e
 
 
+class WorksheetProcessor:
+
+    """
+    Collect and assign child objects
+    """
+
+    def __init__(self, ws, archive):
+        self.ws = ws
+        self.archive = archive
+
+
+    def find_children(self, path):
+        """
+        Find relevant and group child objects
+        """
+        rels_path = get_rels_path(path)
+        rels = RelationshipList()
+
+        if rels_path in self.archive.namelist():
+            rels = get_dependents(self.archive, rels_path)
+
+        for attr in ["comments", "pivotTable", "drawing", "ctrlProp", "control", "image"]:
+            setattr(rels, attr, [])
+
+        rels.get_types()
+        self.rels = rels
+
+
+    def get_legacy(self):
+        """
+        Extract VML if it exists and store as object
+        """
+        if self.ws.legacy_drawing is None:
+            return
+
+        rel = self.rels[self.ws.legacy_drawing]
+        vml = self.archive.read(rel.target)
+        vml = vml.replace(b"<br>", b"<br/>")
+        drawing = LegacyDrawing(vml)
+        self.ws.legacy_drawing = drawing
+        rels_path = get_rels_path(rel.target)
+        if rels_path not in self.archive.namelist():
+            return
+
+        rels = get_dependents(self.archive, rels_path)
+
+        for rel in rels.Relationship:
+            rel.blob = self._get_image_for(rel.target)
+
+        drawing.children = rels
+
+
+    def _get_image_for(self, path):
+        """
+        Extract image from the archive and return it as a BytesIO object
+        """
+        img = Image(BytesIO(self.archive.read(path)))
+        if path.endswith(".emf"):
+            img.format = "EMF"
+        return img
+
+
+    def get_comments(self):
+        """Assign comments"""
+
+        comment_warning = """Cell '{0}':{1} is part of a merged range but has a comment which will be removed because merged cells cannot contain any data."""
+
+        for rel in self.rels.comments:
+            src = self.archive.read(rel.target)
+            comment_sheet = CommentSheet.from_tree(fromstring(src))
+            for ref, comment in comment_sheet.comments:
+                try:
+                    self.ws[ref].comment = comment
+                except AttributeError as e:
+                    c = self.ws[ref]
+                    if isinstance(c, MergedCell):
+                        warnings.warn(comment_warning.format(self.ws.title, c.coordinate))
+                        continue
+
+
+    def get_drawings(self):
+        for rel in self.rels.drawing:
+            charts, images, shapes = find_images(self.archive, rel.target)
+            for c in charts:
+                self.ws.add_chart(c, c.anchor)
+            for im in images:
+                self.ws.add_image(im, im.anchor)
+
+            self.ws._shapes = shapes
+
+
+    def get_pivots(self, pivot_caches):
+        for rel in self.rels.pivotTable:
+            pivot_path = rel.Target
+            src = self.archive.read(pivot_path)
+            tree = fromstring(src)
+            pivot = TableDefinition.from_tree(tree)
+            pivot.cache = pivot_caches[pivot.cacheId]
+            self.ws.add_pivot(pivot)
+
+
+    def get_controls(self):
+        """
+        Get related objects for ctrlProps
+        """
+        ctrlProps = {}
+
+        for rel in self.rels.ctrlProp:
+            src = self.archive.read(rel.target)
+            tree = fromstring(src)
+            ctrlProps[rel.id] = FormControl.from_tree(tree)
+
+        for control in self.ws.controls.control:
+            if control.id in ctrlProps:
+                control.shape = ctrlProps[control.id]
+
+            prop = control.controlPr
+            if prop.id:
+                rel = self.rels[prop.id]
+                rel.blob = self._get_image_for(rel.target)
+                prop.image = rel
+
+    def get_activex(self):
+        """
+        Get related objects for ActiveX Controls
+        """
+        active = {}
+
+        for rel in self.rels.control:
+            src = self.archive.read(rel.target)
+            tree = fromstring(src)
+            ctrl = ActiveXControl.from_tree(tree)
+            active[rel.id] = ctrl
+            active_path = get_rels_path(rel.target)
+            rels = get_dependents(self.archive, active_path)
+
+            # get activeX binary
+            bin_rel = rels[ctrl.id]
+            ctrl.bin = self.archive.read(bin_rel.Target)
+
+        images = set()
+        for control in self.ws.controls.control:
+            if control.id in active:
+                control.shape = active[control.id]
+            # embed any graphics, but skip duplicates
+            prop = control.controlPr
+            if prop.id:
+                rel = self.rels[prop.id]
+                if prop.id not in images:
+                    rel.blob = self._get_image_for(rel.target)
+                    images.add(prop.id)
+                prop.image = rel
+
+
 def load_workbook(filename, read_only=False, keep_vba=KEEP_VBA,
                   data_only=False, keep_links=True, rich_text=False):
     """Open the given filename and return the workbook
 
     :param filename: the path to open or a file-like object
     :type filename: string or a file-like object open in binary mode c.f., :class:`zipfile.ZipFile`
 
     :param read_only: optimised for reading, content cannot be edited
     :type read_only: bool
 
-    :param keep_vba: preserve vba content (this does NOT mean you can use it)
+    :param keep_vba: preseve vba content (this does NOT mean you can use it)
     :type keep_vba: bool
 
     :param data_only: controls whether cells with formulae have either the formula (default) or the value stored the last time Excel read the sheet
     :type data_only: bool
 
     :param keep_links: whether links to external workbooks should be preserved. The default is True
     :type keep_links: bool
@@ -338,10 +459,10 @@
     .. note::
 
         When using lazy load, all worksheets will be :class:`openpyxl.worksheet.iter_worksheet.IterableWorksheet`
         and the returned workbook will be read-only.
 
     """
     reader = ExcelReader(filename, read_only, keep_vba,
-                         data_only, keep_links, rich_text)
+                        data_only, keep_links, rich_text)
     reader.read()
     return reader.wb
```

### Comparing `openpyxl-3.1.2/openpyxl/reader/strings.py` & `openpyxl-3.2.0b1/openpyxl/reader/strings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.cell.text import Text
 
 from openpyxl.xml.functions import iterparse
 from openpyxl.xml.constants import SHEET_MAIN_NS
 from openpyxl.cell.rich_text import CellRichText
```

### Comparing `openpyxl-3.1.2/openpyxl/reader/workbook.py` & `openpyxl-3.2.0b1/openpyxl/reader/workbook.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
+import posixpath
 from warnings import warn
 
 from openpyxl.xml.functions import fromstring
 
 from openpyxl.packaging.relationship import (
     get_dependents,
     get_rels_path,
     get_rel,
 )
+from openpyxl.packaging.manifest import Manifest
 from openpyxl.packaging.workbook import WorkbookPackage
 from openpyxl.workbook import Workbook
-from openpyxl.workbook.defined_name import DefinedNameList
+from openpyxl.workbook.defined_name import (
+    _unpack_print_area,
+    _unpack_print_titles,
+)
 from openpyxl.workbook.external_link.external import read_external_link
 from openpyxl.pivot.cache import CacheDefinition
 from openpyxl.pivot.record import RecordList
-from openpyxl.worksheet.print_settings import PrintTitles, PrintArea
 
 from openpyxl.utils.datetime import CALENDAR_MAC_1904
 
 
 class WorkbookParser:
 
     _rels = None
 
     def __init__(self, archive, workbook_part_name, keep_links=True):
         self.archive = archive
         self.workbook_part_name = workbook_part_name
-        self.defined_names = DefinedNameList()
         self.wb = Workbook()
         self.keep_links = keep_links
         self.sheets = []
 
 
     @property
     def rels(self):
@@ -50,84 +53,74 @@
         self.wb.code_name = package.properties.codeName
         self.wb.active = package.active
         self.wb.views = package.bookViews
         self.sheets = package.sheets
         self.wb.calculation = package.calcPr
         self.caches = package.pivotCaches
 
-        # external links contain cached worksheets and can be very big
+        #external links contain cached worksheets and can be very big
         if not self.keep_links:
             package.externalReferences = []
 
         for ext_ref in package.externalReferences:
             rel = self.rels[ext_ref.id]
             self.wb._external_links.append(
                 read_external_link(self.archive, rel.Target)
             )
 
         if package.definedNames:
-            self.defined_names = package.definedNames
+            package.definedNames._cleanup()
+            self.wb.defined_names = package.definedNames
 
         self.wb.security = package.workbookProtection
 
 
     def find_sheets(self):
         """
         Find all sheets in the workbook and return the link to the source file.
 
         Older XLSM files sometimes contain invalid sheet elements.
         Warn user when these are removed.
         """
 
         for sheet in self.sheets:
             if not sheet.id:
-                msg = f"File contains an invalid specification for {0}. This will be removed".format(sheet.name)
+                msg = "File contains an invalid specification for {0}. This will be removed".format(sheet.name)
                 warn(msg)
                 continue
             yield sheet, self.rels[sheet.id]
 
 
     def assign_names(self):
         """
-        Bind defined names and other definitions to worksheets or the workbook
+        Bind reserved names to parsed worksheets
         """
+        defns = []
 
-        for idx, names in self.defined_names.by_sheet().items():
-            if idx == "global":
-                self.wb.defined_names = names
-                continue
-
-            try:
-                sheet = self.wb._sheets[idx]
-            except IndexError:
-                warn(f"Defined names for sheet index {idx} cannot be located")
-                continue
-
-            for name, defn in names.items():
-                reserved = defn.is_reserved
-                if reserved is None:
-                    sheet.defined_names[name] = defn
-
-                elif reserved == "Print_Titles":
-                    titles = PrintTitles.from_string(defn.value)
-                    sheet._print_rows = titles.rows
-                    sheet._print_cols = titles.cols
+        for defn in self.wb.defined_names.definedName:
+            reserved = defn.is_reserved
+            if reserved in ("Print_Titles", "Print_Area"):
+                sheet = self.wb._sheets[defn.localSheetId]
+                if reserved == "Print_Titles":
+                    rows, cols = _unpack_print_titles(defn)
+                    sheet.print_title_rows = rows
+                    sheet.print_title_cols = cols
                 elif reserved == "Print_Area":
-                    try:
-                        sheet._print_area = PrintArea.from_string(defn.value)
-                    except TypeError:
-                        warn(f"Print area cannot be set to Defined name: {defn.value}.")
-                        continue
+                    sheet.print_area = _unpack_print_area(defn)
+            else:
+                defns.append(defn)
+        self.wb.defined_names.definedName = defns
+
 
     @property
     def pivot_caches(self):
         """
         Get PivotCache objects
         """
         d = {}
         for c in self.caches:
             cache = get_rel(self.archive, self.rels, id=c.id, cls=CacheDefinition)
             if cache.deps:
                 records = get_rel(self.archive, cache.deps, cache.id, RecordList)
                 cache.records = records
-            d[c.cacheId] = cache
+            d[c.cacheId]  = cache
         return d
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/alignment.py` & `openpyxl-3.2.0b1/openpyxl/styles/alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.compat import safe_string
 
 from openpyxl.descriptors import Bool, MinMax, Min, Alias, NoneSet
 from openpyxl.descriptors.serialisable import Serialisable
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/borders.py` & `openpyxl-3.2.0b1/openpyxl/styles/borders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.compat import safe_string
 from openpyxl.descriptors import (
     NoneSet,
     Typed,
     Bool,
     Alias,
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/builtins.py` & `openpyxl-3.2.0b1/openpyxl/styles/builtins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 # Builtins styles as defined in Part 4 Annex G.2
 
 from .named_styles import NamedStyle
 from openpyxl.xml.functions import fromstring
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/cell_style.py` & `openpyxl-3.2.0b1/openpyxl/styles/cell_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from array import array
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Float,
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/colors.py` & `openpyxl-3.2.0b1/openpyxl/styles/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import re
 from openpyxl.compat import safe_string
 from openpyxl.descriptors import (
     String,
     Bool,
     MinMax,
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/differential.py` & `openpyxl-3.2.0b1/openpyxl/styles/differential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Typed,
     Sequence,
     Alias,
 )
 from openpyxl.descriptors.serialisable import Serialisable
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/fills.py` & `openpyxl-3.2.0b1/openpyxl/styles/fills.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-
-# Copyright (c) 2010-2023 openpyxl
+from __future__ import division
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Float,
     Set,
     Alias,
     NoneSet,
     Sequence,
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/fonts.py` & `openpyxl-3.2.0b1/openpyxl/styles/fonts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 from openpyxl.descriptors import (
     Alias,
     Sequence,
     Integer
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/named_styles.py` & `openpyxl-3.2.0b1/openpyxl/styles/named_styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.compat import safe_string
 
 from openpyxl.descriptors import (
     Typed,
     Integer,
     Bool,
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/numbers.py` & `openpyxl-3.2.0b1/openpyxl/styles/numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import re
 
 from openpyxl.descriptors import (
     String,
     Sequence,
     Integer,
@@ -102,15 +102,15 @@
 # +ve;-ve;zero;text
 
 def is_date_format(fmt):
     if fmt is None:
         return False
     fmt = fmt.split(";")[0] # only look at the first format
     fmt = STRIP_RE.sub("", fmt) # ignore some formats
-    return re.search(r"(?<!\\)[dmhysDMHYS]", fmt) is not None
+    return re.search(r"[^\\][dmhysDMHYS]", fmt) is not None
 
 
 def is_timedelta_format(fmt):
     if fmt is None:
         return False
     fmt = fmt.split(";")[0] # only look at the first format
     return TIMEDELTA_RE.search(fmt) is not None
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/proxy.py` & `openpyxl-3.2.0b1/openpyxl/styles/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from copy import copy
 
 from openpyxl.compat import deprecated
 
 
 class StyleProxy(object):
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/styleable.py` & `openpyxl-3.2.0b1/openpyxl/styles/styleable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from copy import copy
 from warnings import warn
 
 from .numbers import (
     BUILTIN_FORMATS,
     BUILTIN_FORMATS_MAX_SIZE,
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/stylesheet.py` & `openpyxl-3.2.0b1/openpyxl/styles/stylesheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from warnings import warn
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/styles/table.py` & `openpyxl-3.2.0b1/openpyxl/styles/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Float,
     Bool,
     Set,
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/cell.py` & `openpyxl-3.2.0b1/openpyxl/utils/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 Collection of utilities used within the package and also available for client code
 """
 import re
 from string import digits
 
@@ -188,15 +188,15 @@
     cols = (get_column_letter(col) for col in range(min_col, max_col+1))
     for col in cols:
         yield tuple('{0}{1}'.format(col, row) for row in rows)
 
 
 def coordinate_to_tuple(coordinate):
     """
-    Convert an Excel style coordinate to (row, column) tuple
+    Convert an Excel style coordinate to (row, colum) tuple
     """
     for idx, c in enumerate(coordinate):
         if c in digits:
             break
     col = coordinate[:idx].upper()
     row = coordinate[idx:]
     return int(row), _COL_STRING_CACHE[col]
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/datetime.py` & `openpyxl-3.2.0b1/openpyxl/utils/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Manage Excel date weirdness."""
 
 # Python stdlib imports
 import datetime
 from math import isnan
 import re
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/escape.py` & `openpyxl-3.2.0b1/openpyxl/utils/escape.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 OOXML has non-standard escaping for characters < \031
 """
 
 import re
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/exceptions.py` & `openpyxl-3.2.0b1/openpyxl/utils/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 """Definitions for openpyxl shared exception classes."""
 
 
 class CellCoordinatesException(Exception):
     """Error for converting between numeric and A1-style cell references."""
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/formulas.py` & `openpyxl-3.2.0b1/openpyxl/utils/formulas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,9 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 List of builtin formulae
 """
 
 FORMULAE = ("CUBEKPIMEMBER", "CUBEMEMBER", "CUBEMEMBERPROPERTY", "CUBERANKEDMEMBER", "CUBESET", "CUBESETCOUNT", "CUBEVALUE", "DAVERAGE", "DCOUNT", "DCOUNTA", "DGET", "DMAX", "DMIN", "DPRODUCT", "DSTDEV", "DSTDEVP", "DSUM", "DVAR", "DVARP", "DATE", "DATEDIF", "DATEVALUE", "DAY", "DAYS360", "EDATE", "EOMONTH", "HOUR", "MINUTE", "MONTH", "NETWORKDAYS", "NETWORKDAYS.INTL", "NOW", "SECOND", "TIME", "TIMEVALUE", "TODAY", "WEEKDAY", "WEEKNUM", "WORKDAY ", "WORKDAY.INTL", "YEAR", "YEARFRAC", "BESSELI", "BESSELJ", "BESSELK", "BESSELY", "BIN2DEC", "BIN2HEX", "BIN2OCT", "COMPLEX", "CONVERT", "DEC2BIN", "DEC2HEX", "DEC2OCT", "DELTA", "ERF", "ERFC", "GESTEP", "HEX2BIN", "HEX2DEC", "HEX2OCT", "IMABS", "IMAGINARY", "IMARGUMENT", "IMCONJUGATE", "IMCOS", "IMDIV", "IMEXP", "IMLN", "IMLOG10", "IMLOG2", "IMPOWER", "IMPRODUCT", "IMREAL", "IMSIN", "IMSQRT", "IMSUB", "IMSUM", "OCT2BIN", "OCT2DEC", "OCT2HEX", "ACCRINT", "ACCRINTM", "AMORDEGRC", "AMORLINC", "COUPDAYBS", "COUPDAYS", "COUPDAYSNC", "COUPNCD", "COUPNUM", "COUPPCD", "CUMIPMT", "CUMPRINC", "DB", "DDB", "DISC", "DOLLARDE", "DOLLARFR", "DURATION", "EFFECT", "FV", "FVSCHEDULE", "INTRATE", "IPMT", "IRR", "ISPMT", "MDURATION", "MIRR", "NOMINAL", "NPER", "NPV", "ODDFPRICE", "ODDFYIELD", "ODDLPRICE", "ODDLYIELD", "PMT", "PPMT", "PRICE", "PRICEDISC", "PRICEMAT", "PV", "RATE", "RECEIVED", "SLN", "SYD", "TBILLEQ", "TBILLPRICE", "TBILLYIELD", "VDB", "XIRR", "XNPV", "YIELD", "YIELDDISC", "YIELDMAT", "CELL", "ERROR.TYPE", "INFO", "ISBLANK", "ISERR", "ISERROR", "ISEVEN", "ISLOGICAL", "ISNA", "ISNONTEXT", "ISNUMBER", "ISODD", "ISREF", "ISTEXT", "N", "NA", "TYPE", "AND", "FALSE", "IF", "IFERROR", "NOT", "OR", "TRUE ADDRESS", "AREAS", "CHOOSE", "COLUMN", "COLUMNS", "GETPIVOTDATA", "HLOOKUP", "HYPERLINK", "INDEX", "INDIRECT", "LOOKUP", "MATCH", "OFFSET", "ROW", "ROWS", "RTD", "TRANSPOSE", "VLOOKUP", "ABS", "ACOS", "ACOSH", "ASIN", "ASINH", "ATAN", "ATAN2", "ATANH", "CEILING", "COMBIN", "COS", "COSH", "DEGREES", "ECMA.CEILING", "EVEN", "EXP", "FACT", "FACTDOUBLE", "FLOOR", "GCD", "INT", "ISO.CEILING", "LCM", "LN", "LOG", "LOG10", "MDETERM", "MINVERSE", "MMULT", "MOD", "MROUND", "MULTINOMIAL", "ODD", "PI", "POWER", "PRODUCT", "QUOTIENT", "RADIANS", "RAND", "RANDBETWEEN", "ROMAN", "ROUND", "ROUNDDOWN", "ROUNDUP", "SERIESSUM", "SIGN", "SIN", "SINH", "SQRT", "SQRTPI", "SUBTOTAL", "SUM", "SUMIF", "SUMIFS", "SUMPRODUCT", "SUMSQ", "SUMX2MY2", "SUMX2PY2", "SUMXMY2", "TAN", "TANH", "TRUNC", "AVEDEV", "AVERAGE", "AVERAGEA", "AVERAGEIF", "AVERAGEIFS", "BETADIST", "BETAINV", "BINOMDIST", "CHIDIST", "CHIINV", "CHITEST", "CONFIDENCE", "CORREL", "COUNT", "COUNTA", "COUNTBLANK", "COUNTIF", "COUNTIFS", "COVAR", "CRITBINOM", "DEVSQ", "EXPONDIST", "FDIST", "FINV", "FISHER", "FISHERINV", "FORECAST", "FREQUENCY", "FTEST", "GAMMADIST", "GAMMAINV", "GAMMALN", "GEOMEAN", "GROWTH", "HARMEAN", "HYPGEOMDIST", "INTERCEPT", "KURT", "LARGE", "LINEST", "LOGEST", "LOGINV", "LOGNORMDIST", "MAX", "MAXA", "MEDIAN", "MIN", "MINA", "MODE", "NEGBINOMDIST", "NORMDIST", "NORMINV", "NORMSDIST", "NORMSINV", "PEARSON", "PERCENTILE", "PERCENTRANK", "PERMUT", "POISSON", "PROB", "QUARTILE", "RANK", "RSQ", "SKEW", "SLOPE", "SMALL", "STANDARDIZE", "STDEV STDEVA", "STDEVP", "STDEVPA STEYX", "TDIST", "TINV", "TREND", "TRIMMEAN", "TTEST", "VAR", "VARA", "VARP", "VARPA", "WEIBULL", "ZTEST", "ASC", "BAHTTEXT", "CHAR", "CLEAN", "CODE", "CONCATENATE", "DOLLAR", "EXACT", "FIND", "FINDB", "FIXED", "JIS", "LEFT", "LEFTB", "LEN", "LENB", "LOWER", "MID", "MIDB", "PHONETIC", "PROPER", "REPLACE", "REPLACEB", "REPT", "RIGHT", "RIGHTB", "SEARCH", "SEARCHB", "SUBSTITUTE", "T", "TEXT", "TRIM", "UPPER", "VALUE")
 
 FORMULAE = frozenset(FORMULAE)
-
-
-from openpyxl.formula import Tokenizer
-
-
-def validate(formula):
-    """
-    Utility function for checking whether a formula is syntactically correct
-    """
-    assert formula.startswith("=")
-    formula = Tokenizer(formula)
-    for t in formula.items:
-        if t.type == "FUNC" and t.subtype == "OPEN":
-            if not t.value.startswith("_xlfn.") and t.value[:-1] not in FORMULAE:
-                raise ValueError(f"Unknown function {t.value} in {formula.formula}. The function may need a prefix")
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/indexed_list.py` & `openpyxl-3.2.0b1/openpyxl/utils/indexed_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 class IndexedList(list):
     """
     List with optimised access by value
     Based on Alex Martelli's recipe
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/inference.py` & `openpyxl-3.2.0b1/openpyxl/utils/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
 Type inference functions
 """
 import datetime
 import re
 
@@ -20,15 +20,15 @@
 ([0-5][0-9])?\.
 (?P<microsecond>\d{1,6}))
 """, re.VERBOSE)
 NUMBER_REGEX = re.compile(r'^-?([\d]|[\d]+\.[\d]*|\.[\d]+|[1-9][\d]+\.?[\d]*)((E|e)[-+]?[\d]+)?$')
 
 
 def cast_numeric(value):
-    """Explicitly convert a string to a numeric value"""
+    """Explicity convert a string to a numeric value"""
     if NUMBER_REGEX.match(value):
         try:
             return int(value)
         except ValueError:
             return float(value)
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/protection.py` & `openpyxl-3.2.0b1/openpyxl/utils/protection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 def hash_password(plaintext_password=''):
     """
     Create a password hash from a given string for protecting a worksheet
     only. This will not work for encrypting a workbook.
```

### Comparing `openpyxl-3.1.2/openpyxl/utils/units.py` & `openpyxl-3.2.0b1/openpyxl/utils/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-
-# Copyright (c) 2010-2023 openpyxl
+from __future__ import division
+# Copyright (c) 2010-2022 openpyxl
 
 import math
 
 
 #constants
 
 DEFAULT_ROW_HEIGHT = 15.  # Default row height measured in point size.
@@ -33,15 +33,15 @@
 pct: Half-points are used to specify font sizes. A font-size of 12pt equals 24 half points
 
 EMU: English Metric Unit, EMUs are used for coordinates in vector-based
 drawings and embedded pictures. One inch equates to 914400 EMUs and a
 centimeter is 360000. For bitmaps the default resolution is 96 dpi (known as
 PixelsPerInch in Excel). Spec p. 1122
 
-For radial geometry Excel uses integer units of 1/60000th of a degree.
+For radial geometry Excel uses integert units of 1/60000th of a degree.
 """
 
 
 
 def inch_to_dxa(value):
     """1 inch = 72 * 20 dxa"""
     return int(value * 20 * 72)
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/_writer.py` & `openpyxl-3.2.0b1/openpyxl/workbook/_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Write the workbook global settings to the archive."""
 
-from openpyxl.utils import quote_sheetname
+from copy import copy
+
+from openpyxl.utils import absolute_coordinate, quote_sheetname
 from openpyxl.xml.constants import (
     ARC_APP,
     ARC_CORE,
     ARC_CUSTOM,
     ARC_WORKBOOK,
     PKG_REL_NS,
     CUSTOMUI_NS,
     ARC_ROOT_RELS,
 )
 from openpyxl.xml.functions import tostring, fromstring
 
 from openpyxl.packaging.relationship import Relationship, RelationshipList
-from openpyxl.workbook.defined_name import (
-    DefinedName,
-    DefinedNameList,
-)
+from openpyxl.workbook.defined_name import DefinedName
 from openpyxl.workbook.external_reference import ExternalReference
 from openpyxl.packaging.workbook import ChildSheet, WorkbookPackage, PivotCache
 from openpyxl.workbook.properties import WorkbookProperties
 from openpyxl.utils.datetime import CALENDAR_MAC_1904
 
 
 def get_active_sheet(wb):
@@ -86,42 +85,42 @@
             rel = Relationship(type=link._rel_type, Target=link.path)
             self.rels.append(rel)
             ext = ExternalReference(id=rel.id)
             self.package.externalReferences.append(ext)
 
 
     def write_names(self):
-        defined_names = list(self.wb.defined_names.values())
+        defined_names = copy(self.wb.defined_names)
 
+        # Defined names -> autoFilter
         for idx, sheet in enumerate(self.wb.worksheets):
-            quoted = quote_sheetname(sheet.title)
-
-            # local names
-            if sheet.defined_names:
-                names = sheet.defined_names.values()
-                for n in names:
-                    n.localSheetId = idx
-                defined_names.extend(names)
+            auto_filter = sheet.auto_filter.ref
 
-            if sheet.auto_filter:
+            if auto_filter:
                 name = DefinedName(name='_FilterDatabase', localSheetId=idx, hidden=True)
-                name.value = f"{quoted}!{sheet.auto_filter}"
+                name.value = u"{0}!{1}".format(quote_sheetname(sheet.title),
+                                              absolute_coordinate(auto_filter)
+                                              )
                 defined_names.append(name)
 
+            # print titles
             if sheet.print_titles:
                 name = DefinedName(name="Print_Titles", localSheetId=idx)
-                name.value = sheet.print_titles
+                name.value = ",".join([u"{0}!{1}".format(quote_sheetname(sheet.title), r)
+                                      for r in sheet.print_titles.split(",")])
                 defined_names.append(name)
 
+            # print areas
             if sheet.print_area:
                 name = DefinedName(name="Print_Area", localSheetId=idx)
-                name.value = sheet.print_area
+                name.value = ",".join([u"{0}!{1}".format(quote_sheetname(sheet.title), r)
+                                      for r in sheet.print_area])
                 defined_names.append(name)
 
-        self.package.definedNames = DefinedNameList(definedName=defined_names)
+        self.package.definedNames = defined_names
 
 
     def write_pivots(self):
         pivot_caches = set()
         for pivot in self.wb._pivots:
             if pivot.cache not in pivot_caches:
                 pivot_caches.add(pivot.cache)
@@ -158,15 +157,15 @@
 
         styles =  Relationship(type='styles', Target='styles.xml')
         self.rels.append(styles)
 
         theme =  Relationship(type='theme', Target='theme/theme1.xml')
         self.rels.append(theme)
 
-        if self.wb.vba_archive:
+        if self.wb._vba:
             vba =  Relationship(type='', Target='vbaProject.bin')
             vba.Type ='http://schemas.microsoft.com/office/2006/relationships/vbaProject'
             self.rels.append(vba)
 
         return tostring(self.rels.to_tree())
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/child.py` & `openpyxl-3.2.0b1/openpyxl/workbook/child.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import re
 import warnings
 
 from openpyxl.worksheet.header_footer import HeaderFooter
 
 """
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/defined_name.py` & `openpyxl-3.2.0b1/openpyxl/workbook/defined_name.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,69 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
-from collections import defaultdict
 import re
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
+    Typed,
     String,
+    Float,
     Integer,
     Bool,
+    NoneSet,
+    Set,
     Sequence,
     Descriptor,
 )
 from openpyxl.compat import safe_string
 from openpyxl.formula import Tokenizer
-from openpyxl.utils.cell import SHEETRANGE_RE
+from openpyxl.utils.cell import (
+    SHEETRANGE_RE,
+    SHEET_TITLE,
+)
 
 RESERVED = frozenset(["Print_Area", "Print_Titles", "Criteria",
                       "_FilterDatabase", "Extract", "Consolidate_Area",
                       "Sheet_Title"])
 
 _names = "|".join(RESERVED)
 RESERVED_REGEX = re.compile(r"^_xlnm\.(?P<name>{0})".format(_names))
+COL_RANGE = r"""(?P<cols>[$]?[a-zA-Z]{1,3}:[$]?[a-zA-Z]{1,3})"""
+COL_RANGE_RE = re.compile(COL_RANGE)
+ROW_RANGE = r"""(?P<rows>[$]?\d+:[$]?\d+)"""
+ROW_RANGE_RE = re.compile(ROW_RANGE)
+TITLES_REGEX = re.compile("""{0}{1}?,?{2}?""".format(SHEET_TITLE, ROW_RANGE, COL_RANGE),
+                          re.VERBOSE)
+
+
+### utilities
+
+def _unpack_print_titles(defn):
+    """
+    Extract rows and or columns from print titles so that they can be
+    assigned to a worksheet
+    """
+    scanner = TITLES_REGEX.finditer(defn.value)
+    kw = dict((k, v) for match in scanner
+              for k, v in match.groupdict().items() if v)
+
+    return kw.get('rows'), kw.get('cols')
+
+
+def _unpack_print_area(defn):
+    """
+    Extract print area
+    """
+    new = []
+    for m in SHEETRANGE_RE.finditer(defn.value): # can be multiple
+        coord = m.group("cells")
+        if coord:
+            new.append(coord)
+    return new
 
 
 class DefinedName(Serialisable):
 
     tagname = "definedName"
 
     name = String() # unique per workbook/worksheet
@@ -122,68 +160,107 @@
             v = getattr(self, key)
             if v is not None:
                 if v in RESERVED:
                     v = "_xlnm." + v
                 yield key, safe_string(v)
 
 
-class DefinedNameDict(dict):
-
-    """
-    Utility class for storing defined names.
-    Allows access by name and separation of global and scoped names
-    """
-
-    def __setitem__(self, key, value):
-        if not isinstance(value, DefinedName):
-            raise TypeError("Value must be a an instance of DefinedName")
-        elif value.name != key:
-            raise ValueError("Key must be the same as the name")
-        super().__setitem__(key, value)
-
-
-    def add(self, value):
-        """
-        Add names without worrying about key and name matching.
-        """
-        self[value.name] = value
-
-
 class DefinedNameList(Serialisable):
 
     tagname = "definedNames"
 
     definedName = Sequence(expected_type=DefinedName)
 
 
     def __init__(self, definedName=()):
         self.definedName = definedName
 
 
-    def by_sheet(self):
+    def _cleanup(self):
         """
-        Break names down into sheet locals and globals
+        Strip invalid definitions and remove special hidden ones
         """
-        names = defaultdict(DefinedNameDict)
-        for defn in self.definedName:
-            if defn.localSheetId is None:
-                if defn.name in ("_xlnm.Print_Titles", "_xlnm.Print_Area", "_xlnm._FilterDatabase"):
-                    continue
-                names["global"][defn.name] = defn
-            else:
-                sheet = int(defn.localSheetId)
-                names[sheet][defn.name] = defn
-        return names
+        valid_names = []
+        for n in self.definedName:
+            if n.name in ("_xlnm.Print_Titles", "_xlnm.Print_Area") and n.localSheetId is None:
+                continue
+            elif n.name == "_xlnm._FilterDatabase":
+                continue
+            valid_names.append(n)
+        self.definedName = valid_names
 
 
     def _duplicate(self, defn):
         """
         Check for whether DefinedName with the same name and scope already
         exists
         """
         for d in self.definedName:
             if d.name == defn.name and d.localSheetId == defn.localSheetId:
                 return True
 
 
+    def append(self, defn):
+        if not isinstance(defn, DefinedName):
+            raise TypeError("""You can only append DefinedNames""")
+        if self._duplicate(defn):
+            raise ValueError("""DefinedName with the same name and scope already exists""")
+        names = self.definedName[:]
+        names.append(defn)
+        self.definedName = names
+
+
     def __len__(self):
         return len(self.definedName)
+
+
+    def __contains__(self, name):
+        """
+        See if a globaly defined name exists
+        """
+        for defn in self.definedName:
+            if defn.name == name and defn.localSheetId is None:
+                return True
+
+
+    def __getitem__(self, name):
+        """
+        Get globally defined name
+        """
+        defn = self.get(name)
+        if not defn:
+            raise KeyError("No definition called {0}".format(name))
+        return defn
+
+
+    def get(self, name, scope=None):
+        """
+        Get the name assigned to a specicic sheet or global
+        """
+        for defn in self.definedName:
+            if defn.name == name and defn.localSheetId == scope:
+                return defn
+
+
+    def __delitem__(self, name):
+        """
+        Delete a globally defined name
+        """
+        if not self.delete(name):
+            raise KeyError("No globally defined name {0}".format(name))
+
+
+    def delete(self, name, scope=None):
+        """
+        Delete a name assigned to a specific or global
+        """
+        for idx, defn in enumerate(self.definedName):
+            if defn.name == name and defn.localSheetId == scope:
+                del self.definedName[idx]
+                return True
+
+
+    def localnames(self, scope):
+        """
+        Provide a list of all names for a particular worksheet
+        """
+        return [defn.name for defn in self.definedName if defn.localSheetId == scope]
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/external_link/external.py` & `openpyxl-3.2.0b1/openpyxl/workbook/external_link/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     String,
     Bool,
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/function_group.py` & `openpyxl-3.2.0b1/openpyxl/workbook/function_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Sequence,
     String,
     Integer,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/properties.py` & `openpyxl-3.2.0b1/openpyxl/workbook/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     String,
     Float,
     Integer,
     Bool,
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/protection.py` & `openpyxl-3.2.0b1/openpyxl/workbook/protection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Typed,
     String,
     Float,
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/smart_tags.py` & `openpyxl-3.2.0b1/openpyxl/workbook/smart_tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Sequence,
     String,
     Bool,
     NoneSet,
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/views.py` & `openpyxl-3.2.0b1/openpyxl/workbook/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Sequence,
     String,
     Float,
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/web.py` & `openpyxl-3.2.0b1/openpyxl/workbook/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Sequence,
     String,
     Float,
```

### Comparing `openpyxl-3.1.2/openpyxl/workbook/workbook.py` & `openpyxl-3.2.0b1/openpyxl/workbook/workbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Workbook is the top-level container for all document information."""
 from copy import copy
 
 from openpyxl.compat import deprecated
 from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.worksheet._read_only import ReadOnlyWorksheet
@@ -25,17 +25,17 @@
 from openpyxl.styles.fonts import DEFAULT_FONT
 from openpyxl.styles.protection import Protection
 from openpyxl.styles.colors import COLOR_INDEX
 from openpyxl.styles.named_styles import NamedStyleList
 from openpyxl.styles.table import TableStyleList
 
 from openpyxl.chartsheet import Chartsheet
-from .defined_name import DefinedName, DefinedNameDict
+from .defined_name import DefinedName, DefinedNameList
 from openpyxl.packaging.core import DocumentProperties
-from openpyxl.packaging.custom import CustomPropertyList
+from openpyxl.packaging.custom import CustomDocumentPropertyList
 from openpyxl.packaging.relationship import RelationshipList
 from .child import _WorkbookChild
 from .protection import DocumentSecurity
 from .properties import CalcProperties
 from .views import BookView
 
 
@@ -59,26 +59,27 @@
     def __init__(self,
                  write_only=False,
                  iso_dates=False,
                  ):
         self._sheets = []
         self._pivots = []
         self._active_sheet_index = 0
-        self.defined_names = DefinedNameDict()
+        self.defined_names = DefinedNameList()
         self._external_links = []
         self.properties = DocumentProperties()
-        self.custom_doc_props = CustomPropertyList()
+        self.custom_doc_props = CustomDocumentPropertyList()
         self.security = DocumentSecurity()
         self.__write_only = write_only
         self.shared_strings = IndexedList()
 
         self._setup_styles()
 
         self.loaded_theme = None
         self.vba_archive = None
+        self._vba = None
         self.is_template = False
         self.code_name = None
         self.epoch = WINDOWS_EPOCH
         self.encoding = "utf-8"
         self.iso_dates = iso_dates
 
         if not self.write_only:
@@ -228,14 +229,17 @@
         new_pos = idx + offset
         self._sheets.insert(new_pos, sheet)
 
 
     def remove(self, worksheet):
         """Remove `worksheet` from this workbook."""
         idx = self._sheets.index(worksheet)
+        localnames = self.defined_names.localnames(scope=idx)
+        for name in localnames:
+            self.defined_names.delete(name, scope=idx)
         self._sheets.remove(worksheet)
 
 
     @deprecated("Use wb.remove(worksheet) or del wb[sheetname]")
     def remove_sheet(self, worksheet):
         """Remove `worksheet` from this workbook."""
         self.remove(worksheet)
@@ -321,27 +325,23 @@
         Names are returned in the worksheets order.
 
         :type: list of strings
 
         """
         return [s.title for s in self._sheets]
 
-
-    @deprecated("Assign scoped named ranges directly to worksheets or global ones to the workbook. Deprecated in 3.1")
     def create_named_range(self, name, worksheet=None, value=None, scope=None):
-        """Create a new named_range on a worksheet
-
-        """
-        defn = DefinedName(name=name)
+        """Create a new named_range on a worksheet"""
+        defn = DefinedName(name=name, localSheetId=scope)
         if worksheet is not None:
             defn.value = "{0}!{1}".format(quote_sheetname(worksheet.title), value)
         else:
             defn.value = value
 
-        self.defined_names[name] = defn
+        self.defined_names.append(defn)
 
 
     def add_named_style(self, style):
         """
         Add a named style
         """
         self._named_styles.append(style)
@@ -352,35 +352,58 @@
     def named_styles(self):
         """
         List available named styles
         """
         return self._named_styles.names
 
 
+    @deprecated("Use workbook.defined_names.definedName")
+    def get_named_ranges(self):
+        """Return all named ranges"""
+        return self.defined_names.definedName
+
+
+    @deprecated("Use workbook.defined_names.append")
+    def add_named_range(self, named_range):
+        """Add an existing named_range to the list of named_ranges."""
+        self.defined_names.append(named_range)
+
+
+    @deprecated("Use workbook.defined_names[name]")
+    def get_named_range(self, name):
+        """Return the range specified by name."""
+        return self.defined_names[name]
+
+
+    @deprecated("Use del workbook.defined_names[name]")
+    def remove_named_range(self, named_range):
+        """Remove a named_range from this workbook."""
+        del self.defined_names[named_range]
+
+
     @property
     def mime_type(self):
         """
         The mime type is determined by whether a workbook is a template or
         not and whether it contains macros or not. Excel requires the file
         extension to match but openpyxl does not enforce this.
-
         """
         ct = self.template and XLTX or XLSX
-        if self.vba_archive:
+        if self._vba:
             ct = self.template and XLTM or XLSM
         return ct
 
 
     def save(self, filename):
         """Save the current workbook under the given `filename`.
         Use this function instead of using an `ExcelWriter`.
 
         .. warning::
             When creating your workbook using `write_only` set to True,
-            you will only be able to call this function once. Subsequent attempts to
+            you will only be able to call this function once. Subsequents attempts to
             modify or save the file will raise an :class:`openpyxl.shared.exc.WorkbookAlreadySaved` exception.
         """
         if self.read_only:
             raise TypeError("""Workbook is read-only""")
         if self.write_only and not self.worksheets:
             self.create_sheet()
         save_workbook(self, filename)
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/_read_only.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/_read_only.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """ Read worksheets on-demand
 """
 
 from .worksheet import Worksheet
 from openpyxl.cell.read_only import ReadOnlyCell, EMPTY_CELL
 from openpyxl.utils import get_column_letter
 
 from ._reader import WorkSheetParser
-from openpyxl.workbook.defined_name import DefinedNameDict
 
 
 def read_dimension(source):
     parser = WorkSheetParser(source, [])
     return parser.parse_dimensions()
 
 
@@ -36,15 +35,14 @@
         self.parent = parent_workbook
         self.title = title
         self.sheet_state = 'visible'
         self._current_row = None
         self._worksheet_path = worksheet_path
         self._shared_strings = shared_strings
         self._get_size()
-        self.defined_names = DefinedNameDict()
 
 
     def _get_size(self):
         src = self._get_source()
         parser = WorkSheetParser(src, [])
         dimensions = parser.parse_dimensions()
         src.close()
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/_reader.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Reader for a single worksheet."""
 from copy import copy
 from warnings import warn
 
 # compatibility imports
 from openpyxl.xml.functions import iterparse
@@ -26,14 +26,15 @@
     get_column_letter,
     coordinate_to_tuple,
     )
 from openpyxl.utils.datetime import from_excel, from_ISO8601, WINDOWS_EPOCH
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.cell.rich_text import CellRichText
 
+from .controls import ControlList
 from .formula import DataTableFormula, ArrayFormula
 from .filters import AutoFilter
 from .header_footer import HeaderFooter
 from .hyperlink import HyperlinkList
 from .merge import MergeCells
 from .page import PageMargins, PrintOptions, PrintPageSetup
 from .pagebreak import RowBreak, ColBreak
@@ -71,14 +72,15 @@
 FORMAT_TAG = '{%s}sheetFormatPr' % SHEET_MAIN_NS
 ROW_BREAK_TAG = '{%s}rowBreaks' % SHEET_MAIN_NS
 COL_BREAK_TAG = '{%s}colBreaks' % SHEET_MAIN_NS
 SCENARIOS_TAG = '{%s}scenarios' % SHEET_MAIN_NS
 DATA_TAG = '{%s}sheetData' % SHEET_MAIN_NS
 DIMENSION_TAG = '{%s}dimension' % SHEET_MAIN_NS
 CUSTOM_VIEWS_TAG = '{%s}customSheetViews' % SHEET_MAIN_NS
+CONTROLS_TAG = "{%s}controls" % SHEET_MAIN_NS
 
 
 def _cast_number(value):
     "Convert numbers as string to an int or float"
     if "." in value or "E" in value or "e" in value:
         return float(value)
     return int(value)
@@ -115,14 +117,15 @@
         self.keep_vba = False
         self.hyperlinks = HyperlinkList()
         self.formatting = []
         self.legacy_drawing = None
         self.merged_cells = None
         self.row_breaks = RowBreak()
         self.col_breaks = ColBreak()
+        self.controls = None
         self.rich_text = rich_text
 
 
     def parse(self):
         dispatcher = {
             COL_TAG: self.parse_column_dimensions,
             PROT_TAG: self.parse_sheet_protection,
@@ -144,15 +147,15 @@
             PROPERTIES_TAG: ('sheet_properties', WorksheetProperties),
             VIEWS_TAG: ('views', SheetViewList),
             FORMAT_TAG: ('sheet_format', SheetFormatProperties),
             SCENARIOS_TAG: ('scenarios', ScenarioList),
             TABLE_TAG: ('tables', TablePartList),
             HYPERLINK_TAG: ('hyperlinks', HyperlinkList),
             MERGE_TAG: ('merged_cells', MergeCells),
-
+            CONTROLS_TAG: ("controls", ControlList),
         }
 
         it = iterparse(self.source) # add a finaliser to close the source when this becomes possible
 
         for _, element in it:
             tag_name = element.tag
             if tag_name in dispatcher:
@@ -450,15 +453,15 @@
 
 
     def bind_properties(self):
         for k in ('print_options', 'page_margins', 'page_setup',
                   'HeaderFooter', 'auto_filter', 'data_validations',
                   'sheet_properties', 'views', 'sheet_format',
                   'row_breaks', 'col_breaks', 'scenarios', 'legacy_drawing',
-                  'protection',
+                  'protection', "controls"
                   ):
             v = getattr(self.parser, k, None)
             if v is not None:
                 setattr(self.ws, k, v)
 
 
     def bind_all(self):
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/_write_only.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/_write_only.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 """Write worksheets to xml representations in an optimized way"""
 
 from inspect import isgenerator
 
 from openpyxl.cell import Cell, WriteOnlyCell
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/_writer.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import atexit
 from collections import defaultdict
 from io import BytesIO
 import os
 from tempfile import NamedTemporaryFile
 from warnings import warn
 
 from openpyxl.xml.functions import xmlfile
 from openpyxl.xml.constants import SHEET_MAIN_NS
 
 from openpyxl.comments.comment_sheet import CommentRecord
+from openpyxl.drawing.legacy import LegacyDrawing
 from openpyxl.packaging.relationship import Relationship, RelationshipList
 from openpyxl.styles.differential import DifferentialStyle
 
 from .dimensions import SheetDimension
 from .hyperlink import HyperlinkList
 from .merge import MergeCell, MergeCells
 from .related import Related
@@ -44,14 +45,16 @@
 class WorksheetWriter:
 
 
     def __init__(self, ws, out=None):
         self.ws = ws
         self.ws._hyperlinks = []
         self.ws._comments = []
+        self.controls = []
+        self.control_images = []
         if out is None:
             out = create_temporary_file()
         self.out = out
         self._rels = RelationshipList()
         self.xf = self.get_stream()
         next(self.xf) # start generator
 
@@ -238,30 +241,63 @@
         brks = (self.ws.row_breaks, self.ws.col_breaks)
         for brk in brks:
             if brk:
                 self.xf.send(brk.to_tree())
 
 
     def write_drawings(self):
-        if self.ws._charts or self.ws._images:
+        if self.ws._charts or self.ws._images or self.ws._shapes:
             rel = Relationship(type="drawing", Target="")
             self._rels.append(rel)
             drawing = Related()
             drawing.id = rel.id
             self.xf.send(drawing.to_tree("drawing"))
 
 
     def write_legacy(self):
         """
         Comments & VBA controls use VML and require an additional element
         that is no longer in the specification.
         """
-        if (self.ws.legacy_drawing is not None or self.ws._comments):
-            legacy = Related(id="anysvml")
-            self.xf.send(legacy.to_tree("legacyDrawing"))
+        if not self.ws.legacy_drawing and not self.ws._comments:
+            return
+        if not self.ws.legacy_drawing:
+            self.ws.legacy_drawing = LegacyDrawing(vml=None)
+
+        rel = Relationship(type="vmlDrawing", Target="")
+        self._rels.append(rel)
+        legacy = Related(id=rel.id)
+        self.ws.legacy_drawing._rel_id = rel.id
+        self.xf.send(legacy.to_tree("legacyDrawing"))
+
+
+    def write_controls(self):
+        controls = self.ws.controls
+        if not controls:
+            return
+
+        targets = []
+        for ctrl in controls.control:
+            shape = ctrl.shape # ActiveX or CtrlProp
+            self.controls.append(shape)
+            rel = Relationship(Type=shape.rel_type, Target="")
+            self._rels.append(rel)
+            ctrl.id = rel.id
+            shape._rel_id = rel.id
+            embedded = getattr(ctrl.controlPr, "image", None)
+
+            if embedded:
+                embedded.id = None
+                if embedded.Target not in targets:
+                    self.control_images.append(embedded)
+                    self._rels.append(embedded)
+                    targets.append(embedded.Target)
+                ctrl.controlPr.id = embedded.id
+
+        self.xf.send(controls.to_tree())
 
 
     def write_tables(self):
         tables = TablePartList()
 
         for table in self.ws.tables.values():
             if not table.tableColumns:
@@ -344,14 +380,15 @@
         self.write_print()
         self.write_margins()
         self.write_page()
         self.write_header()
         self.write_breaks()
         self.write_drawings()
         self.write_legacy()
+        self.write_controls()
         self.write_tables()
 
 
     def write(self):
         """
         High level
         """
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/cell_range.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/cell_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from copy import copy
-from operator import attrgetter
 
 from openpyxl.descriptors import Strict
-from openpyxl.descriptors import MinMax
-from openpyxl.descriptors.sequence import UniqueSequence
+from openpyxl.descriptors import MinMax, Sequence
 from openpyxl.descriptors.serialisable import Serialisable
 
 from openpyxl.utils import (
     range_boundaries,
     range_to_tuple,
     get_column_letter,
     quote_sheetname,
 )
 
+
 class CellRange(Serialisable):
     """
     Represents a range in a sheet: title and coordinates.
 
     This object is used to perform operations on ranges, like:
 
     - shift, expand or shrink
@@ -132,18 +131,14 @@
     def __repr__(self):
         fmt = u"<{cls} {coord}>"
         if self.title:
             fmt = u"<{cls} {title!r}!{coord}>"
         return fmt.format(cls=self.__class__.__name__, title=self.title, coord=self.coord)
 
 
-    def __hash__(self):
-        return hash((self.min_row, self.min_col, self.max_row, self.max_col))
-
-
     def __str__(self):
         fmt = "{coord}"
         title = self.title
         if title:
             fmt = u"{title}!{coord}"
             title = quote_sheetname(title)
         return fmt.format(title=title, coord=self.coord)
@@ -378,15 +373,15 @@
         :type right: int
         :param right: shrink range from the right by this number of cells
         :type down: int
         :param down: shrink range from the top by this number of cells
         :type left: int
         :param left: shrink range from the left by this number of cells
         :type up: int
-        :param up: shrink range from the bottom by this number of cells
+        :param up: shrink range from the bottown by this number of cells
         """
         self.min_col += left
         self.min_row += top
         self.max_col -= right
         self.max_row -= bottom
 
 
@@ -421,64 +416,55 @@
         """A list of cell coordinates that comprise the right-side of the range"""
         return [(row, self.max_col) for row in range(self.min_row, self.max_row+1)]
 
 
 class MultiCellRange(Strict):
 
 
-    ranges = UniqueSequence(expected_type=CellRange)
+    ranges = Sequence(expected_type=CellRange)
 
 
-    def __init__(self, ranges=set()):
+    def __init__(self, ranges=()):
         if isinstance(ranges, str):
             ranges = [CellRange(r) for r in ranges.split()]
-        self.ranges = set(ranges)
+        self.ranges = ranges
 
 
     def __contains__(self, coord):
         if isinstance(coord, str):
             coord = CellRange(coord)
         for r in self.ranges:
             if coord <= r:
                 return True
         return False
 
 
     def __repr__(self):
-        ranges = " ".join([str(r) for r in self.sorted()])
-        return f"<{self.__class__.__name__} [{ranges}]>"
+        ranges = " ".join([str(r) for r in self.ranges])
+        return "<{0} [{1}]>".format(self.__class__.__name__, ranges)
 
 
     def __str__(self):
-        ranges = u" ".join([str(r) for r in self.sorted()])
+        ranges = u" ".join([str(r) for r in self.ranges])
         return ranges
 
-
-    def __hash__(self):
-        return hash(str(self))
-
-
-    def sorted(self):
-        """
-        Return a sorted list of items
-        """
-        return sorted(self.ranges, key=attrgetter('min_col', 'min_row', 'max_col', 'max_row'))
+    __str__ = __str__
 
 
     def add(self, coord):
         """
         Add a cell coordinate or CellRange
         """
         cr = coord
         if isinstance(coord, str):
             cr = CellRange(coord)
         elif not isinstance(coord, CellRange):
             raise ValueError("You can only add CellRanges")
         if cr not in self:
-            self.ranges.add(cr)
+            self.ranges.append(cr)
 
 
     def __iadd__(self, coord):
         self.add(coord)
         return self
 
 
@@ -504,9 +490,12 @@
 
     def __iter__(self):
         for cr in self.ranges:
             yield cr
 
 
     def __copy__(self):
-        ranges = {copy(r) for r in self.ranges}
-        return MultiCellRange(ranges)
+        n = MultiCellRange()
+
+        for r in self.ranges:
+            n.ranges.append(copy(r))
+        return n
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/cell_watch.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/cell_watch.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/controls.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/scenario.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,105 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
-    Typed,
-    Bool,
-    Integer,
     String,
+    Integer,
+    Bool,
     Sequence,
+    Convertible,
 )
-
-from openpyxl.descriptors.excel import Relation
-from .ole import ObjectAnchor
+from .cell_range import MultiCellRange
 
 
-class ControlProperty(Serialisable):
+class InputCells(Serialisable):
 
-    tagname = "controlPr"
+    tagname = "inputCells"
 
-    anchor = Typed(expected_type=ObjectAnchor, )
-    locked = Bool(allow_none=True)
-    defaultSize = Bool(allow_none=True)
-    _print = Bool(allow_none=True)
-    disabled = Bool(allow_none=True)
-    recalcAlways = Bool(allow_none=True)
-    uiObject = Bool(allow_none=True)
-    autoFill = Bool(allow_none=True)
-    autoLine = Bool(allow_none=True)
-    autoPict = Bool(allow_none=True)
-    macro = String(allow_none=True)
-    altText = String(allow_none=True)
-    linkedCell = String(allow_none=True)
-    listFillRange = String(allow_none=True)
-    cf = String(allow_none=True)
-    id = Relation(allow_none=True)
-
-    __elements__ = ('anchor',)
+    r = String()
+    deleted = Bool(allow_none=True)
+    undone = Bool(allow_none=True)
+    val = String()
+    numFmtId = Integer(allow_none=True)
 
     def __init__(self,
-                 anchor=None,
-                 locked=True,
-                 defaultSize=True,
-                 _print=True,
-                 disabled=False,
-                 recalcAlways=False,
-                 uiObject=False,
-                 autoFill=True,
-                 autoLine=True,
-                 autoPict=True,
-                 macro=None,
-                 altText=None,
-                 linkedCell=None,
-                 listFillRange=None,
-                 cf='pict',
-                 id=None,
+                 r=None,
+                 deleted=False,
+                 undone=False,
+                 val=None,
+                 numFmtId=None,
                 ):
-        self.anchor = anchor
-        self.locked = locked
-        self.defaultSize = defaultSize
-        self._print = _print
-        self.disabled = disabled
-        self.recalcAlways = recalcAlways
-        self.uiObject = uiObject
-        self.autoFill = autoFill
-        self.autoLine = autoLine
-        self.autoPict = autoPict
-        self.macro = macro
-        self.altText = altText
-        self.linkedCell = linkedCell
-        self.listFillRange = listFillRange
-        self.cf = cf
-        self.id = id
-
-
-class Control(Serialisable):
-
-    tagname = "control"
-
-    controlPr = Typed(expected_type=ControlProperty, allow_none=True)
-    shapeId = Integer()
-    name = String(allow_none=True)
+        self.r = r
+        self.deleted = deleted
+        self.undone = undone
+        self.val = val
+        self.numFmtId = numFmtId
+
+
+class Scenario(Serialisable):
 
-    __elements__ = ('controlPr',)
+    tagname = "scenario"
+
+    inputCells = Sequence(expected_type=InputCells)
+    name = String()
+    locked = Bool(allow_none=True)
+    hidden = Bool(allow_none=True)
+    user = String(allow_none=True)
+    comment = String(allow_none=True)
+
+    __elements__ = ('inputCells',)
+    __attrs__ = ('name', 'locked', 'hidden', 'user', 'comment', 'count')
 
     def __init__(self,
-                 controlPr=None,
-                 shapeId=None,
+                 inputCells=(),
                  name=None,
+                 locked=False,
+                 hidden=False,
+                 count=None,
+                 user=None,
+                 comment=None,
                 ):
-        self.controlPr = controlPr
-        self.shapeId = shapeId
+        self.inputCells = inputCells
         self.name = name
+        self.locked = locked
+        self.hidden = hidden
+        self.user = user
+        self.comment = comment
+
 
+    @property
+    def count(self):
+        return len(self.inputCells)
 
-class Controls(Serialisable):
 
-    tagname = "controls"
+class ScenarioList(Serialisable):
 
-    control = Sequence(expected_type=Control)
+    tagname = "scenarios"
 
-    __elements__ = ('control',)
+    scenario = Sequence(expected_type=Scenario)
+    current = Integer(allow_none=True)
+    show = Integer(allow_none=True)
+    sqref = Convertible(expected_type=MultiCellRange, allow_none=True)
+
+    __elements__ = ('scenario',)
 
     def __init__(self,
-                 control=(),
+                 scenario=(),
+                 current=None,
+                 show=None,
+                 sqref=None,
                 ):
-        self.control = control
+        self.scenario = scenario
+        self.current = current
+        self.show = show
+        self.sqref = sqref
+
+
+    def append(self, scenario):
+        s = self.scenario
+        s.append(scenario)
+        self.scenario = s
+
+
+    def __bool__(self):
+        return bool(self.scenario)
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/copier.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/copier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 #standard lib imports
 from copy import copy
 
 from .worksheet import Worksheet
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/custom.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/custom.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/datavalidation.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/datavalidation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from collections import defaultdict
 from itertools import chain
 from operator import itemgetter
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
@@ -75,19 +75,20 @@
 
     tagname = "dataValidation"
 
     sqref = Convertible(expected_type=MultiCellRange)
     cells = Alias("sqref")
     ranges = Alias("sqref")
 
+    showErrorMessage = Bool()
     showDropDown = Bool(allow_none=True)
     hide_drop_down = Alias('showDropDown')
-    showInputMessage = Bool(allow_none=True)
-    showErrorMessage = Bool(allow_none=True)
-    allowBlank = Bool(allow_none=True)
+    showInputMessage = Bool()
+    showErrorMessage = Bool()
+    allowBlank = Bool()
     allow_blank = Alias('allowBlank')
 
     errorTitle = String(allow_none = True)
     error = String(allow_none = True)
     promptTitle = String(allow_none = True)
     prompt = String(allow_none = True)
     formula1 = NestedText(allow_none=True, expected_type=str)
@@ -103,27 +104,27 @@
                                "lessThan", "lessThanOrEqual", "greaterThan", "greaterThanOrEqual"))
     validation_type = Alias('type')
 
     def __init__(self,
                  type=None,
                  formula1=None,
                  formula2=None,
-                 showErrorMessage=False,
-                 showInputMessage=False,
-                 showDropDown=False,
-                 allowBlank=False,
+                 showErrorMessage=True,
+                 showInputMessage=True,
+                 showDropDown=None,
+                 allowBlank=None,
                  sqref=(),
                  promptTitle=None,
                  errorStyle=None,
                  error=None,
                  prompt=None,
                  errorTitle=None,
                  imeMode=None,
                  operator=None,
-                 allow_blank=False,
+                 allow_blank=None,
                  ):
         self.sqref = sqref
         self.showDropDown = showDropDown
         self.imeMode = imeMode
         self.operator = operator
         self.formula1 = formula1
         self.formula2 = formula2
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/dimensions.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/dimensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from copy import copy
 
 from openpyxl.compat import safe_string
 from openpyxl.utils import (
     get_column_interval,
     column_index_from_string,
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/errors.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/errors.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/filters.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import re
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Alias,
     Typed,
@@ -15,15 +15,14 @@
     String,
     Sequence,
     MinMax,
     Convertible,
 )
 from openpyxl.descriptors.excel import ExtensionList, CellRange
 from openpyxl.descriptors.sequence import ValueSequence
-from openpyxl.utils import absolute_coordinate
 
 
 class SortCondition(Serialisable):
 
     tagname = "sortCondition"
 
     descending = Bool(allow_none=True)
@@ -297,16 +296,16 @@
     extLst = Typed(expected_type=ExtensionList, allow_none=True)
 
     __elements__ = ('filters', 'top10', 'customFilters', 'dynamicFilter',
                     'colorFilter', 'iconFilter')
 
     def __init__(self,
                  colId=None,
-                 hiddenButton=False,
-                 showButton=True,
+                 hiddenButton=None,
+                 showButton=None,
                  filters=None,
                  top10=None,
                  customFilters=None,
                  dynamicFilter=None,
                  colorFilter=None,
                  iconFilter=None,
                  extLst=None,
@@ -350,17 +349,14 @@
         self.sortState = sortState
 
 
     def __bool__(self):
         return self.ref is not None
 
 
-    def __str__(self):
-        return absolute_coordinate(self.ref)
-
 
     def add_filter_column(self, col_id, vals, blank=False):
         """
         Add row filter for specified column.
 
         :param col_id: Zero-origin column id. 0 means first column.
         :type  col_id: int
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/formula.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.compat import safe_string
 
 class DataTableFormula:
 
 
     t = "dataTable"
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/header_footer.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/header_footer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 # Simplified implementation of headers and footers: let worksheets have separate items
 
 import re
 from warnings import warn
 
 from openpyxl.descriptors import (
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/hyperlink.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/hyperlink.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/merge.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 import copy
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Integer,
     Sequence,
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/ole.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/ole.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Typed,
     Integer,
     String,
     Set,
     Bool,
     Sequence,
 )
+from openpyxl.descriptors.nested import NestedText
 
-from openpyxl.drawing.spreadsheet_drawing import AnchorMarker
+from openpyxl.drawing.anchor import AnchorMarker
 from openpyxl.xml.constants import SHEET_DRAWING_NS
 
 
+class AnchorMarker(AnchorMarker):
+
+    ## XDR namespace for child elements only
+
+    col = NestedText(expected_type=int, namespace=SHEET_DRAWING_NS)
+    colOff = NestedText(expected_type=int, namespace=SHEET_DRAWING_NS)
+    row = NestedText(expected_type=int, namespace=SHEET_DRAWING_NS)
+    rowOff = NestedText(expected_type=int, namespace=SHEET_DRAWING_NS)
+
+
 class ObjectAnchor(Serialisable):
 
     tagname = "anchor"
 
-    _from = Typed(expected_type=AnchorMarker, namespace=SHEET_DRAWING_NS)
-    to = Typed(expected_type=AnchorMarker, namespace=SHEET_DRAWING_NS)
+    _from = Typed(expected_type=AnchorMarker)
+    to = Typed(expected_type=AnchorMarker)
     moveWithCells = Bool(allow_none=True)
     sizeWithCells = Bool(allow_none=True)
     z_order = Integer(allow_none=True, hyphenated=True)
 
 
     def __init__(self,
                  _from=None,
@@ -39,15 +50,15 @@
         self.z_order = z_order
 
 
 class ObjectPr(Serialisable):
 
     tagname = "objectPr"
 
-    anchor = Typed(expected_type=ObjectAnchor, )
+    anchor = Typed(expected_type=ObjectAnchor)
     locked = Bool(allow_none=True)
     defaultSize = Bool(allow_none=True)
     _print = Bool(allow_none=True)
     disabled = Bool(allow_none=True)
     uiObject = Bool(allow_none=True)
     autoFill = Bool(allow_none=True)
     autoLine = Bool(allow_none=True)
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/page.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Float,
     Bool,
     Integer,
     NoneSet,
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/pagebreak.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/pagebreak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Integer,
     Bool,
     Sequence,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/properties.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Worksheet Properties"""
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import String, Bool, Typed
 from openpyxl.styles.colors import ColorDescriptor
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/protection.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/protection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Bool,
     String,
     Alias,
     Integer,
 )
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/smart_tag.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/smart_tag.py`

 * *Files identical despite different names*

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/table.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.descriptors import (
     Descriptor,
     Alias,
     Typed,
     Bool,
@@ -321,15 +321,15 @@
         Column headings must be strings and must match cells in the worksheet.
         """
 
         min_col, min_row, max_col, max_row = range_boundaries(self.ref)
         for idx in range(min_col, max_col+1):
             col = TableColumn(id=idx, name="Column{0}".format(idx))
             self.tableColumns.append(col)
-        if self.headerRowCount and not self.autoFilter:
+        if self.headerRowCount:
             self.autoFilter = AutoFilter(ref=self.ref)
 
 
     @property
     def column_names(self):
         return [column.name for column in self.tableColumns]
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/views.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 from openpyxl.descriptors import (
     Bool,
     Integer,
     String,
     Set,
     Float,
```

### Comparing `openpyxl-3.1.2/openpyxl/worksheet/worksheet.py` & `openpyxl-3.2.0b1/openpyxl/worksheet/worksheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Worksheet is the 2nd-level container in Excel."""
 
 
 # Python stdlib imports
 from itertools import chain
 from operator import itemgetter
@@ -22,18 +22,15 @@
     coordinate_to_tuple,
     absolute_coordinate,
 )
 from openpyxl.cell import Cell, MergedCell
 from openpyxl.formatting.formatting import ConditionalFormattingList
 from openpyxl.packaging.relationship import RelationshipList
 from openpyxl.workbook.child import _WorkbookChild
-from openpyxl.workbook.defined_name import (
-    DefinedNameDict,
-)
-
+from openpyxl.workbook.defined_name import COL_RANGE_RE, ROW_RANGE_RE
 from openpyxl.formula.translate import Translator
 
 from .datavalidation import DataValidationList
 from .page import (
     PrintPageSetup,
     PageMargins,
     PrintOptions,
@@ -47,27 +44,22 @@
 from .protection import SheetProtection
 from .filters import AutoFilter
 from .views import (
     Pane,
     Selection,
     SheetViewList,
 )
+from .controls import ControlList
 from .cell_range import MultiCellRange, CellRange
 from .merge import MergedCellRange
 from .properties import WorksheetProperties
 from .pagebreak import RowBreak, ColBreak
 from .scenario import ScenarioList
 from .table import TableList
 from .formula import ArrayFormula
-from .print_settings import (
-    PrintTitles,
-    ColRange,
-    RowRange,
-    PrintArea,
-)
 
 
 class Worksheet(_WorkbookChild):
     """Represents a worksheet.
 
     Do not create worksheets yourself,
     use :func:`openpyxl.workbook.Workbook.create_sheet` instead
@@ -113,40 +105,43 @@
         self.column_dimensions = DimensionHolder(worksheet=self,
                                                  default_factory=self._add_column)
         self.row_breaks = RowBreak()
         self.col_breaks = ColBreak()
         self._cells = {}
         self._charts = []
         self._images = []
+        self._shapes = []
         self._rels = RelationshipList()
         self._drawing = None
         self._comments = []
         self.merged_cells = MultiCellRange()
         self._tables = TableList()
         self._pivots = []
         self.data_validations = DataValidationList()
         self._hyperlinks = []
         self.sheet_state = 'visible'
         self.page_setup = PrintPageSetup(worksheet=self)
         self.print_options = PrintOptions()
         self._print_rows = None
         self._print_cols = None
-        self._print_area = PrintArea()
+        self._print_area = None
         self.page_margins = PageMargins()
         self.views = SheetViewList()
         self.protection = SheetProtection()
-        self.defined_names = DefinedNameDict()
 
         self._current_row = 0
         self.auto_filter = AutoFilter()
+        self.paper_size = None
+        self.orientation = None
         self.conditional_formatting = ConditionalFormattingList()
         self.legacy_drawing = None
         self.sheet_properties = WorksheetProperties()
         self.sheet_format = SheetFormatProperties()
         self.scenarios = ScenarioList()
+        self.controls = ControlList()
 
 
     @property
     def sheet_view(self):
         return self.views.sheetView[0]
 
 
@@ -251,15 +246,15 @@
 
     def _get_cell(self, row, column):
         """
         Internal method for getting a cell from a worksheet.
         Will create a new cell if one doesn't already exist.
         """
         if not 0 < row < 1048577:
-            raise ValueError(f"Row numbers must be between 1 and 1048576. Row number supplied was {row}")
+            raise ValueError("Row numbers must be between 1 and 1048576")
         coordinate = (row, column)
         if not coordinate in self._cells:
             cell = Cell(self, row=row, column=column)
             self._add_cell(cell)
         return self._cells[coordinate]
 
 
@@ -326,15 +321,15 @@
         row, column = coordinate_to_tuple(key)
         if (row, column) in self._cells:
             del self._cells[(row, column)]
 
 
     @property
     def min_row(self):
-        """The minimum row index containing data (1-based)
+        """The minimium row index containing data (1-based)
 
         :type: int
         """
         min_row = 1
         if self._cells:
             rows = set(c[0] for c in self._cells)
             min_row = min(rows)
@@ -830,72 +825,74 @@
         return RowDimension(self)
 
 
     @property
     def print_title_rows(self):
         """Rows to be printed at the top of every page (ex: '1:3')"""
         if self._print_rows:
-            return str(self._print_rows)
+            return self._print_rows
 
 
     @print_title_rows.setter
     def print_title_rows(self, rows):
         """
         Set rows to be printed on the top of every page
         format `1:3`
         """
         if rows is not None:
-            self._print_rows = RowRange(rows)
+            if not ROW_RANGE_RE.match(rows):
+                raise ValueError("Print title rows must be the form 1:3")
+        self._print_rows = rows
 
 
     @property
     def print_title_cols(self):
         """Columns to be printed at the left side of every page (ex: 'A:C')"""
         if self._print_cols:
-            return str(self._print_cols)
+            return self._print_cols
 
 
     @print_title_cols.setter
     def print_title_cols(self, cols):
         """
         Set cols to be printed on the left of every page
         format ``A:C`
         """
         if cols is not None:
-            self._print_cols = ColRange(cols)
+            if not COL_RANGE_RE.match(cols):
+                raise ValueError("Print title cols must be the form C:D")
+        self._print_cols = cols
 
 
     @property
     def print_titles(self):
-        titles = PrintTitles(cols=self._print_cols, rows=self._print_rows, title=self.title)
-        return str(titles)
+        if self.print_title_cols and self.print_title_rows:
+            return ",".join([self.print_title_rows, self.print_title_cols])
+        else:
+            return self.print_title_rows or self.print_title_cols
 
 
     @property
     def print_area(self):
         """
         The print area for the worksheet, or None if not set. To set, supply a range
         like 'A1:D4' or a list of ranges.
         """
-        self._print_area.title = self.title
-        return str(self._print_area)
+        return self._print_area
 
 
     @print_area.setter
     def print_area(self, value):
         """
-        Range of cells in the form A1:D4 or list of ranges. Print area can be cleared
-        by passing `None` or an empty list
+        Range of cells in the form A1:D4 or list of ranges
         """
-        if not value:
-            self._print_area = PrintArea()
-        elif isinstance(value, str):
-            self._print_area = PrintArea.from_string(value)
-        elif hasattr(value, "__iter__"):
-            self._print_area = PrintArea.from_string(",".join(value))
+        if isinstance(value, str):
+            value = [value]
+
+        self._print_area = [absolute_coordinate(v) for v in value]
 
 
 def _gutter(idx, offset, max_val):
     """
     When deleting rows and columns are deleted we rely on overwriting.
     This may not be the case for a large offset on small set of cells:
     range(cells_to_delete) > range(cell_to_be_moved)
```

### Comparing `openpyxl-3.1.2/openpyxl/writer/excel.py` & `openpyxl-3.2.0b1/openpyxl/writer/excel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
+"""Write a .xlsx file."""
 
 # Python stdlib imports
-import datetime
 import re
+from tempfile import TemporaryFile
 from zipfile import ZipFile, ZIP_DEFLATED
 
 # package imports
+from openpyxl.compat import deprecated
 from openpyxl.utils.exceptions import InvalidFileException
 from openpyxl.xml.constants import (
     ARC_ROOT_RELS,
     ARC_WORKBOOK_RELS,
-    ARC_APP,
-    ARC_CORE,
-    ARC_CUSTOM,
-    CPROPS_TYPE,
+    ARC_APP, ARC_CORE,
+    ARC_CUSTOM, CPROPS_TYPE,
     ARC_THEME,
     ARC_STYLE,
     ARC_WORKBOOK,
-    )
+    IMAGE_NS,
+)
 from openpyxl.drawing.spreadsheet_drawing import SpreadsheetDrawing
-from openpyxl.xml.functions import tostring, fromstring
+from openpyxl.drawing.legacy import LegacyDrawing
+from openpyxl.drawing.image import ImageGroup
+from openpyxl.xml.functions import tostring
 from openpyxl.packaging.manifest import Manifest
 from openpyxl.packaging.relationship import (
     get_rels_path,
     RelationshipList,
     Relationship,
 )
 from openpyxl.comments.comment_sheet import CommentSheet
@@ -34,31 +37,35 @@
 from openpyxl.workbook._writer import WorkbookWriter
 from .theme import theme_xml
 
 
 class ExcelWriter(object):
     """Write a workbook object to an Excel file."""
 
+
     def __init__(self, workbook, archive):
-        self._archive = archive
+        self.archive = archive
         self.workbook = workbook
         self.manifest = Manifest()
         self.vba_modified = set()
         self._tables = []
         self._charts = []
         self._images = []
         self._drawings = []
         self._comments = []
         self._pivots = []
+        self.activex = []
+        self.legacy = []
+        self.form_controls = []
 
 
     def write_data(self):
         """Write the various xml files into the zip archive."""
         # cleanup all worksheets
-        archive = self._archive
+        archive = self.archive
 
         props = ExtendedProperties()
         archive.writestr(ARC_APP, tostring(props.to_tree()))
 
         archive.writestr(ARC_CORE, tostring(self.workbook.properties.to_tree()))
         if self.workbook.loaded_theme:
             archive.writestr(ARC_THEME, self.workbook.loaded_theme)
@@ -68,228 +75,319 @@
         if len(self.workbook.custom_doc_props) >= 1:
             archive.writestr(ARC_CUSTOM, tostring(self.workbook.custom_doc_props.to_tree()))
             class CustomOverride():
                 path = "/" + ARC_CUSTOM #PartName
                 mime_type = CPROPS_TYPE #ContentType
 
             custom_override = CustomOverride()
+            # custom_override = Override(PartName="/docProps/custom.xml", ContentType="application/vnd.openxmlformats-officedocument.custom-properties+xml")
             self.manifest.append(custom_override)
 
-        self._write_worksheets()
-        self._write_chartsheets()
-        self._write_images()
-        self._write_charts()
+        self.write_worksheets()
+        self.write_chartsheets()
+        #self.write_images()
+        self.write_charts()
 
-        self._write_external_links()
+        self.write_external_links()
 
         stylesheet = write_stylesheet(self.workbook)
         archive.writestr(ARC_STYLE, tostring(stylesheet))
 
         writer = WorkbookWriter(self.workbook)
         archive.writestr(ARC_ROOT_RELS, writer.write_root_rels())
         archive.writestr(ARC_WORKBOOK, writer.write())
         archive.writestr(ARC_WORKBOOK_RELS, writer.write_rels())
 
         self._merge_vba()
 
         self.manifest._write(archive, self.workbook)
 
+
+    @property
+    def images(self):
+        return self._images
+
+
+    def add_image(self, img):
+        """
+        Images must have unique names with a workbook. This is done by a simple counter.
+        Adding an image will check whether the image has already been included.
+        The index is set directly on the image but also returned
+        """
+        if img in self._images:
+            idx = self._images.index(img) + 1
+            return idx
+        else:
+            self._images.append(img)
+            idx = len(self._images)
+        img._id = idx
+        img._write(self.archive)
+        return idx
+
+
     def _merge_vba(self):
         """
         If workbook contains macros then extract associated files from cache
         of old file and add to archive
         """
-        ARC_VBA = re.compile("|".join(
-            ('xl/vba', r'xl/drawings/.*vmlDrawing\d\.vml',
-             'xl/ctrlProps', 'customUI', 'xl/activeX', r'xl/media/.*\.emf')
-        )
-                             )
-
-        if self.workbook.vba_archive:
-            for name in set(self.workbook.vba_archive.namelist()) - self.vba_modified:
-                if ARC_VBA.match(name):
-                    self._archive.writestr(name, self.workbook.vba_archive.read(name))
+        if self.workbook._vba:
+            self.archive.writestr("xl/vbaProject.bin", self.workbook._vba)
+        #ARC_VBA = re.compile("|".join(
+            #('xl/vba','customUI', ))
+                             #)
+
+        #if self.workbook.vba_archive:
+            #for name in set(self.workbook.vba_archive.namelist()) - self.vba_modified:
+                #if ARC_VBA.match(name):
+                    #self.archive.writestr(name, self.workbook.vba_archive.read(name))
 
 
-    def _write_images(self):
-        # delegate to object
-        for img in self._images:
-            self._archive.writestr(img.path[1:], img._data())
-
-
-    def _write_charts(self):
+    def write_charts(self):
         # delegate to object
         if len(self._charts) != len(set(self._charts)):
             raise InvalidFileException("The same chart cannot be used in more than one worksheet")
         for chart in self._charts:
-            self._archive.writestr(chart.path[1:], tostring(chart._write()))
+            self.archive.writestr(chart.path[1:], tostring(chart._write()))
             self.manifest.append(chart)
 
 
-    def _write_drawing(self, drawing):
+    def write_drawing(self, drawing):
         """
         Write a drawing
         """
         self._drawings.append(drawing)
         drawing._id = len(self._drawings)
         for chart in drawing.charts:
             self._charts.append(chart)
             chart._id = len(self._charts)
+        #idx = len(self._images)
         for img in drawing.images:
-            self._images.append(img)
-            img._id = len(self._images)
+            if isinstance(img, ImageGroup):
+                for im in img.images:
+                    self.add_image(im)
+            else:
+                self.add_image(img)
+            #idx = img._write(self.archive, idx)
         rels_path = get_rels_path(drawing.path)[1:]
-        self._archive.writestr(drawing.path[1:], tostring(drawing._write()))
-        self._archive.writestr(rels_path, tostring(drawing._write_rels()))
+        self.archive.writestr(drawing.path[1:], tostring(drawing._write()))
+        self.archive.writestr(rels_path, tostring(drawing._write_rels()))
         self.manifest.append(drawing)
 
 
-    def _write_chartsheets(self):
+    def write_chartsheets(self):
         for idx, sheet in enumerate(self.workbook.chartsheets, 1):
 
             sheet._id = idx
             xml = tostring(sheet.to_tree())
 
-            self._archive.writestr(sheet.path[1:], xml)
+            self.archive.writestr(sheet.path[1:], xml)
             self.manifest.append(sheet)
 
             if sheet._drawing:
-                self._write_drawing(sheet._drawing)
+                self.write_drawing(sheet._drawing)
 
                 rel = Relationship(type="drawing", Target=sheet._drawing.path)
                 rels = RelationshipList()
                 rels.append(rel)
                 tree = rels.to_tree()
 
                 rels_path = get_rels_path(sheet.path[1:])
-                self._archive.writestr(rels_path, tostring(tree))
+                self.archive.writestr(rels_path, tostring(tree))
 
 
-    def _write_comment(self, ws):
+    def write_comment(self, ws):
 
         cs = CommentSheet.from_comments(ws._comments)
         self._comments.append(cs)
         cs._id = len(self._comments)
-        self._archive.writestr(cs.path[1:], tostring(cs.to_tree()))
+        self.archive.writestr(cs.path[1:], tostring(cs.to_tree()))
         self.manifest.append(cs)
 
-        if ws.legacy_drawing is None or self.workbook.vba_archive is None:
-            ws.legacy_drawing = 'xl/drawings/commentsDrawing{0}.vml'.format(cs._id)
-            vml = None
+        vml = None
+        if ws.legacy_drawing is not None:
+            vml = ws.legacy_drawing.vml
         else:
-            vml = fromstring(self.workbook.vba_archive.read(ws.legacy_drawing))
+            ws.legacy_drawing = LegacyDrawing(vml)
 
         vml = cs.write_shapes(vml)
-
-        self._archive.writestr(ws.legacy_drawing, vml)
-        self.vba_modified.add(ws.legacy_drawing)
+        ws.legacy_drawing.vml = vml
 
         comment_rel = Relationship(Id="comments", type=cs._rel_type, Target=cs.path)
         ws._rels.append(comment_rel)
 
 
+    def write_legacy(self, ws):
+        """
+        Write VML
+        """
+        drawing = ws.legacy_drawing
+        if ws.legacy_drawing is None:
+            return
+
+        self.legacy.append(drawing)
+        drawing._counter = len(self.legacy)
+        drawing._write(self.archive)
+
+        for rel in drawing.children.Relationship:
+            img = rel.blob
+            self.add_image(img)
+            rel.Target = img.path
+
+        if drawing.children:
+            xml = drawing.children.to_tree()
+            path = get_rels_path(ws.legacy_drawing.path)
+            self.archive.writestr(path[1:], tostring(xml))
+
+
     def write_worksheet(self, ws):
         ws._drawing = SpreadsheetDrawing()
         ws._drawing.charts = ws._charts
         ws._drawing.images = ws._images
+        ws._drawing.shapes = ws._shapes
+
         if self.workbook.write_only:
             if not ws.closed:
                 ws.close()
             writer = ws._writer
         else:
             writer = WorksheetWriter(ws)
             writer.write()
 
         ws._rels = writer._rels
-        self._archive.write(writer.out, ws.path[1:])
+
+        if ws._comments:
+            self.write_comment(ws)
+        self.write_controls(ws, writer.controls)
+        self.write_embedded(ws, writer.control_images)
+
+        if ws.legacy_drawing:
+            drawing = ws.legacy_drawing
+            self.write_legacy(ws)
+            rel = ws._rels[drawing._rel_id]
+            rel.Target = drawing.path
+
+        if ws._drawing:
+            self.write_drawing(ws._drawing)
+            for r in ws._rels.Relationship:
+                if "drawing" in r.Type:
+                    r.Target = ws._drawing.path
+
+        for t in ws._tables.values():
+            self._tables.append(t)
+            t.id = len(self._tables)
+            t._write(self.archive)
+            self.manifest.append(t)
+            ws._rels[t._rel_id].Target = t.path
+
+        self.archive.write(writer.out, ws.path[1:])
         self.manifest.append(ws)
+
         writer.cleanup()
 
 
-    def _write_worksheets(self):
+    def write_controls(self, ws, controls):
+        """Serialise form controls for a specific worksheet"""
+
+        for ctrl in controls:
+            if hasattr(ctrl, "bin"): # ugh!
+                store = self.activex
+            else:
+                store = self.form_controls
+            store.append(ctrl)
+            ctrl.counter = len(store) # ugh!
+            ctrl._write(self.archive, self.manifest)
+
+            ws._rels[ctrl._rel_id].Target = ctrl.path
+
+
+    def write_embedded(self, ws, control_images):
+        """
+        Update path for embedded images for controls
+        """
+        for obj in control_images:
+            img = obj.blob
+            self.add_image(img)
+            obj.Target = img.path
+
+
+    def write_worksheets(self):
 
         pivot_caches = set()
 
         for idx, ws in enumerate(self.workbook.worksheets, 1):
-
             ws._id = idx
             self.write_worksheet(ws)
 
-            if ws._drawing:
-                self._write_drawing(ws._drawing)
-
-                for r in ws._rels.Relationship:
-                    if "drawing" in r.Type:
-                        r.Target = ws._drawing.path
-
-            if ws._comments:
-                self._write_comment(ws)
-
-            if ws.legacy_drawing is not None:
-                shape_rel = Relationship(type="vmlDrawing", Id="anysvml",
-                                         Target="/" + ws.legacy_drawing)
-                ws._rels.append(shape_rel)
-
-            for t in ws._tables.values():
-                self._tables.append(t)
-                t.id = len(self._tables)
-                t._write(self._archive)
-                self.manifest.append(t)
-                ws._rels[t._rel_id].Target = t.path
-
             for p in ws._pivots:
                 if p.cache not in pivot_caches:
                     pivot_caches.add(p.cache)
                     p.cache._id = len(pivot_caches)
 
                 self._pivots.append(p)
                 p._id = len(self._pivots)
-                p._write(self._archive, self.manifest)
+                p._write(self.archive, self.manifest)
                 self.workbook._pivots.append(p)
                 r = Relationship(Type=p.rel_type, Target=p.path)
                 ws._rels.append(r)
 
             if ws._rels:
                 tree = ws._rels.to_tree()
                 rels_path = get_rels_path(ws.path)[1:]
-                self._archive.writestr(rels_path, tostring(tree))
+                self.archive.writestr(rels_path, tostring(tree))
 
 
-    def _write_external_links(self):
+    def write_external_links(self):
         # delegate to object
         """Write links to external workbooks"""
         wb = self.workbook
         for idx, link in enumerate(wb._external_links, 1):
             link._id = idx
             rels_path = get_rels_path(link.path[1:])
 
             xml = link.to_tree()
-            self._archive.writestr(link.path[1:], tostring(xml))
+            self.archive.writestr(link.path[1:], tostring(xml))
             rels = RelationshipList()
             rels.append(link.file_link)
-            self._archive.writestr(rels_path, tostring(rels.to_tree()))
+            self.archive.writestr(rels_path, tostring(rels.to_tree()))
             self.manifest.append(link)
 
 
     def save(self):
         """Write data into the archive."""
         self.write_data()
-        self._archive.close()
+        self.archive.close()
 
 
 def save_workbook(workbook, filename):
     """Save the given workbook on the filesystem under the name filename.
 
     :param workbook: the workbook to save
     :type workbook: :class:`openpyxl.workbook.Workbook`
 
     :param filename: the path to which save the workbook
     :type filename: string
 
     :rtype: bool
 
     """
+    #if wb._vba and not filename.endswith(".xlsm"):
+        #warn()
     archive = ZipFile(filename, 'w', ZIP_DEFLATED, allowZip64=True)
-    workbook.properties.modified = datetime.datetime.utcnow()
     writer = ExcelWriter(workbook, archive)
     writer.save()
     return True
+
+
+@deprecated("Use a NamedTemporaryFile")
+def save_virtual_workbook(workbook):
+    """Return an in-memory workbook, suitable for a Django response."""
+    tmp = TemporaryFile()
+    archive = ZipFile(tmp, 'w', ZIP_DEFLATED, allowZip64=True)
+
+    writer = ExcelWriter(workbook, archive)
+    writer.save()
+
+    tmp.seek(0)
+    virtual_workbook = tmp.read()
+    tmp.close()
+
+    return virtual_workbook
```

### Comparing `openpyxl-3.1.2/openpyxl/writer/theme.py` & `openpyxl-3.2.0b1/openpyxl/writer/theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """Write the theme xml based on a fixed string."""
 
 
 theme_xml = """<?xml version="1.0"?>
 <a:theme xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main" name="Office Theme">
   <a:themeElements>
```

### Comparing `openpyxl-3.1.2/openpyxl/xml/__init__.py` & `openpyxl-3.2.0b1/openpyxl/xml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 """Collection of XML resources compatible across different Python versions"""
 import os
 
 
 def lxml_available():
```

### Comparing `openpyxl-3.1.2/openpyxl/xml/constants.py` & `openpyxl-3.2.0b1/openpyxl/xml/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 
 """Constants for fixed paths in a file and xml namespace urls."""
 
 MIN_ROW = 0
 MIN_COLUMN = 0
 MAX_COLUMN = 16384
@@ -42,15 +42,15 @@
 DCORE_NS = 'http://purl.org/dc/elements/1.1/'
 DCTERMS_NS = 'http://purl.org/dc/terms/'
 DCTERMS_PREFIX = 'dcterms'
 
 # Document
 DOC_NS = "http://schemas.openxmlformats.org/officeDocument/2006/"
 REL_NS = DOC_NS + "relationships"
-COMMENTS_NS = REL_NS + "/comments"
+COMMENTS_REL = REL_NS + "/comments"
 IMAGE_NS = REL_NS + "/image"
 VML_NS =  REL_NS + "/vmlDrawing"
 VTYPES_NS = DOC_NS + 'docPropsVTypes'
 XPROPS_NS = DOC_NS + 'extended-properties'
 CUSTPROPS_NS = DOC_NS + 'custom-properties'
 EXTERNAL_LINK_NS = REL_NS + "/externalLink"
 
@@ -70,26 +70,31 @@
 # Drawing
 CHART_NS = "http://schemas.openxmlformats.org/drawingml/2006/chart"
 DRAWING_NS = "http://schemas.openxmlformats.org/drawingml/2006/main"
 SHEET_DRAWING_NS = "http://schemas.openxmlformats.org/drawingml/2006/spreadsheetDrawing"
 CHART_DRAWING_NS = "http://schemas.openxmlformats.org/drawingml/2006/chartDrawing"
 
 CUSTOMUI_NS = 'http://schemas.microsoft.com/office/2006/relationships/ui/extensibility'
+MARKUP_NS = "http://schemas.openxmlformats.org/markup-compatibility/2006"
+ACTIVEX_NS = "http://schemas.microsoft.com/office/2006/activeX"
 
+XL_2009 = "http://schemas.microsoft.com/office/spreadsheetml/2009/9/main"
 
 NAMESPACES = {
     'cp': COREPROPS_NS,
     'dc': DCORE_NS,
     DCTERMS_PREFIX: DCTERMS_NS,
     'dcmitype': 'http://purl.org/dc/dcmitype/',
     'xsi': XSI_NS,
     'vt': VTYPES_NS,
     'xml': XML_NS,
     'main': SHEET_MAIN_NS,
     'cust': CUSTPROPS_NS,
+    "mc": MARKUP_NS,
+    "ax": ACTIVEX_NS
 }
 
 ## Mime types
 WORKBOOK_MACRO = "application/vnd.ms-excel.%s.macroEnabled.main+xml"
 WORKBOOK = "application/vnd.openxmlformats-officedocument.spreadsheetml.%s.main+xml"
 SPREADSHEET = "application/vnd.openxmlformats-officedocument.spreadsheetml.%s+xml"
 SHARED_STRINGS = SPREADSHEET % "sharedStrings"
```

### Comparing `openpyxl-3.1.2/openpyxl/xml/functions.py` & `openpyxl-3.2.0b1/openpyxl/xml/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Copyright (c) 2010-2023 openpyxl
+# Copyright (c) 2010-2022 openpyxl
 
 """
-XML compatibility functions
+XML compatability functions
 """
 
 # Python stdlib imports
 import re
 from functools import partial
 
 from openpyxl import DEFUSEDXML, LXML
@@ -49,39 +49,40 @@
     SHEET_MAIN_NS,
     REL_NS,
     VTYPES_NS,
     COREPROPS_NS,
     CUSTPROPS_NS,
     DCTERMS_NS,
     DCTERMS_PREFIX,
-    XML_NS
+    XML_NS,
+    ACTIVEX_NS,
 )
 
 register_namespace(DCTERMS_PREFIX, DCTERMS_NS)
 register_namespace('dcmitype', 'http://purl.org/dc/dcmitype/')
 register_namespace('cp', COREPROPS_NS)
 register_namespace('c', CHART_NS)
 register_namespace('a', DRAWING_NS)
 register_namespace('s', SHEET_MAIN_NS)
 register_namespace('r', REL_NS)
 register_namespace('vt', VTYPES_NS)
 register_namespace('xdr', SHEET_DRAWING_NS)
 register_namespace('cdr', CHART_DRAWING_NS)
 register_namespace('xml', XML_NS)
 register_namespace('cust', CUSTPROPS_NS)
+register_namespace("ax", ACTIVEX_NS)
 
 
 tostring = partial(tostring, encoding="utf-8")
 
 NS_REGEX = re.compile("({(?P<namespace>.*)})?(?P<localname>.*)")
 
 def localname(node):
     if callable(node.tag):
         return "comment"
     m = NS_REGEX.match(node.tag)
     return m.group('localname')
 
 
 def whitespace(node):
-    stripped = node.text.strip()
-    if stripped and node.text != stripped:
+    if node.text != node.text.strip():
         node.set("{%s}space" % XML_NS, "preserve")
```

### Comparing `openpyxl-3.1.2/openpyxl.egg-info/PKG-INFO` & `openpyxl-3.2.0b1/openpyxl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: openpyxl
-Version: 3.1.2
+Version: 3.2.0b1
 Summary: A Python library to read/write Excel 2010 xlsx/xlsm files
 Home-page: https://openpyxl.readthedocs.io
 Author: See AUTHORS
 Author-email: charlie.clark@clark-consulting.eu
 License: MIT
 Project-URL: Documentation, https://openpyxl.readthedocs.io/en/stable/
 Project-URL: Source, https://foss.heptapod.net/openpyxl/openpyxl
 Project-URL: Tracker, https://foss.heptapod.net/openpyxl/openpyxl/-/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENCE.rst
 
 .. image:: https://coveralls.io/repos/bitbucket/openpyxl/openpyxl/badge.svg?branch=default
     :target: https://coveralls.io/bitbucket/openpyxl/openpyxl?branch=default
     :alt: coverage status
 
 Introduction
@@ -79,7 +78,9 @@
 The documentation is at: https://openpyxl.readthedocs.io
 
 * installation methods
 * code examples
 * instructions for contributing
 
 Release notes: https://openpyxl.readthedocs.io/en/stable/changes.html
+
+
```

### Comparing `openpyxl-3.1.2/openpyxl.egg-info/SOURCES.txt` & `openpyxl-3.2.0b1/openpyxl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,22 +75,24 @@
 openpyxl/descriptors/excel.py
 openpyxl/descriptors/namespace.py
 openpyxl/descriptors/nested.py
 openpyxl/descriptors/sequence.py
 openpyxl/descriptors/serialisable.py
 openpyxl/descriptors/slots.py
 openpyxl/drawing/__init__.py
+openpyxl/drawing/anchor.py
 openpyxl/drawing/colors.py
 openpyxl/drawing/connector.py
 openpyxl/drawing/drawing.py
 openpyxl/drawing/effect.py
 openpyxl/drawing/fill.py
 openpyxl/drawing/geometry.py
 openpyxl/drawing/graphic.py
 openpyxl/drawing/image.py
+openpyxl/drawing/legacy.py
 openpyxl/drawing/line.py
 openpyxl/drawing/picture.py
 openpyxl/drawing/properties.py
 openpyxl/drawing/relation.py
 openpyxl/drawing/spreadsheet_drawing.py
 openpyxl/drawing/text.py
 openpyxl/drawing/xdr.py
@@ -179,15 +181,14 @@
 openpyxl/worksheet/header_footer.py
 openpyxl/worksheet/hyperlink.py
 openpyxl/worksheet/merge.py
 openpyxl/worksheet/ole.py
 openpyxl/worksheet/page.py
 openpyxl/worksheet/pagebreak.py
 openpyxl/worksheet/picture.py
-openpyxl/worksheet/print_settings.py
 openpyxl/worksheet/properties.py
 openpyxl/worksheet/protection.py
 openpyxl/worksheet/related.py
 openpyxl/worksheet/scenario.py
 openpyxl/worksheet/smart_tag.py
 openpyxl/worksheet/table.py
 openpyxl/worksheet/views.py
```

### Comparing `openpyxl-3.1.2/setup.py` & `openpyxl-3.2.0b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,11 +90,9 @@
                  'Operating System :: POSIX',
                  'License :: OSI Approved :: MIT License',
                  'Programming Language :: Python',
                  'Programming Language :: Python :: 3.6',
                  'Programming Language :: Python :: 3.7',
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: 3.10',
-                 'Programming Language :: Python :: 3.11',
                  ],
     )
```

