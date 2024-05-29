# Comparing `tmp/pixano-0.5.2.tar.gz` & `tmp/pixano-0.5.3.tar.gz`

## Comparing `pixano-0.5.2.tar` & `pixano-0.5.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/__version__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/analytics/__init__.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/analytics/feature_statistics.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/analytics/image_statistics.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/__init__.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/display.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/main.py
--rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/serve.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/api/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/api/datasets.py
--rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/api/items.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/api/models.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/favicon.ico
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/index.html
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/robots.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/env.js
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/version.json
--rw-r--r--   0        0        0    34589 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/0.B5OR-Toy.css
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/4.BrLiNAg8.css
--rw-r--r--   0        0        0    34417 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/5.ZhT30vvc.css
--rw-r--r--   0        0        0    34567 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/_layout.BNzN0mkq.css
--rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/_page.BJ18IbJM.css
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/_page.BrLiNAg8.css
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/favicon.OuiISzV3.ico
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/pixano.NAI_8qFW.png
--rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/assets/pixano_white.BVKPSmmP.png
--rw-r--r--   0        0        0   179210 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/Histogram.USYLred5.js
--rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/PrimaryButton.2luo0sZd.js
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/TooltipIconButton.h3qFl-sW.js
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/api.BxNj-TAm.js
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/checkbox.OiMtEzVH.js
--rw-r--r--   0        0        0   158114 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/command.YXxPKXvy.js
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/datasetStores.BZ9GDOPp.js
--rw-r--r--   0        0        0    27459 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/entry.BdqlkNrw.js
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/icons.Dxr1AG5A.js
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/index.D__UofN6.js
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/loader-2.Cz-VINyt.js
--rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/scheduler.Cq5UBZ1T.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/stores.titGXIKi.js
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/entry/app.B1yXTTAH.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/entry/start.eFYr5dE2.js
--rw-r--r--   0        0        0    20011 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/0.DW46KZ9m.js
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/1.C5NidKnH.js
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/2.CZmQkO2Y.js
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/3.JUP818GM.js
--rw-r--r--   0        0        0    58218 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/4.DGnIT7o0.js
--rw-r--r--   0        0        0  1197721 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/5.Bo-LObf-.js
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/__init__.py
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/bbox.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/camera.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/compressed_rle.py
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/depth_image.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/gt_info.py
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/image.py
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/pixano_type.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/pose.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/core/utils.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/__init__.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/fields.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/settings.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/dataset/__init__.py
--rw-r--r--   0        0        0    31236 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/dataset/dataset.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/dataset/dataset_info.py
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/dataset/dataset_item.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/dataset/dataset_stat.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/dataset/dataset_table.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/exporters/__init__.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/exporters/coco_exporter.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/exporters/exporter.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/importers/__init__.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/importers/coco_importer.py
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/importers/dota_importer.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/importers/image_importer.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/importers/importer.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/item/__init__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/item/item_embedding.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/item/item_feature.py
--rw-r--r--   0        0        0     7802 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/item/item_object.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/data/item/item_view.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/models/__init__.py
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/models/inference_model.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/utils/__init__.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/utils/boxes.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/utils/image.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/utils/labels.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pixano-0.5.2/pixano/utils/python.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pixano-0.5.2/.gitignore
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 pixano-0.5.2/LICENSE
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pixano-0.5.2/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pixano-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 pixano-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/__version__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/analytics/__init__.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/analytics/feature_statistics.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/analytics/image_statistics.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/__init__.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/display.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/main.py
+-rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/serve.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/api/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/api/datasets.py
+-rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/api/items.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/api/models.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/favicon.ico
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/index.html
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/robots.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/env.js
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/version.json
+-rw-r--r--   0        0        0    34589 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/0.B5OR-Toy.css
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/4.BrLiNAg8.css
+-rw-r--r--   0        0        0    34417 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/5.ZhT30vvc.css
+-rw-r--r--   0        0        0    34567 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/_layout.BNzN0mkq.css
+-rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/_page.BJ18IbJM.css
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/_page.BrLiNAg8.css
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/favicon.OuiISzV3.ico
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/pixano.NAI_8qFW.png
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/assets/pixano_white.BVKPSmmP.png
+-rw-r--r--   0        0        0   179210 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/Histogram.YSM0wxsW.js
+-rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/PrimaryButton.CjwzDHMn.js
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/TooltipIconButton.DmW3ppx8.js
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/api.BxNj-TAm.js
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/checkbox.DTaWBrBv.js
+-rw-r--r--   0        0        0   158114 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/command.CjKwrCHU.js
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/datasetStores.Davxg0aA.js
+-rw-r--r--   0        0        0    27459 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/entry.BGJCdFkn.js
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/icons.Dxr1AG5A.js
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/index.D__UofN6.js
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/loader-2.yiAD6ux3.js
+-rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/scheduler.Cq5UBZ1T.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/stores.baCeY990.js
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/entry/app.y5DFN3Js.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/entry/start.u9UDkqYj.js
+-rw-r--r--   0        0        0    20011 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/0.ChfaHG46.js
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/1.DCJl0UMA.js
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/2.C5hi1hQI.js
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/3.CQlFeuu8.js
+-rw-r--r--   0        0        0    58883 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/4.BYwXogVv.js
+-rw-r--r--   0        0        0  1197698 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/5.BngP3_K5.js
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/__init__.py
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/bbox.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/camera.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/compressed_rle.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/depth_image.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/gt_info.py
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/image.py
+-rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/pixano_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/pose.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/core/utils.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/__init__.py
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/fields.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/settings.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/dataset/__init__.py
+-rw-r--r--   0        0        0    31236 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/dataset/dataset.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/dataset/dataset_info.py
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/dataset/dataset_item.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/dataset/dataset_stat.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/dataset/dataset_table.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/exporters/__init__.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/exporters/coco_exporter.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/exporters/exporter.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/importers/__init__.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/importers/coco_importer.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/importers/dota_importer.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/importers/image_importer.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/importers/importer.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/item/__init__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/item/item_embedding.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/item/item_feature.py
+-rw-r--r--   0        0        0     7802 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/item/item_object.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/data/item/item_view.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/models/__init__.py
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/models/inference_model.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/utils/__init__.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/utils/boxes.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/utils/image.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/utils/labels.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pixano-0.5.3/pixano/utils/python.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pixano-0.5.3/.gitignore
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 pixano-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pixano-0.5.3/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pixano-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 pixano-0.5.3/PKG-INFO
```

### Comparing `pixano-0.5.2/pixano/__init__.py` & `pixano-0.5.3/pixano/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/__version__.py` & `pixano-0.5.3/pixano/app/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,9 +6,7 @@
 # generate and explore labeled data for computer vision applications.
 # This software is governed by the CeCILL-C license under French law and
 # abiding by the rules of distribution of free software. You can use,
 # modify and/ or redistribute the software under the terms of the CeCILL-C
 # license as circulated by CEA, CNRS and INRIA at the following URL
 #
 # http://www.cecill.info
-
-__version__ = "0.5.2"
```

### Comparing `pixano-0.5.2/pixano/analytics/__init__.py` & `pixano-0.5.3/pixano/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/analytics/feature_statistics.py` & `pixano-0.5.3/pixano/analytics/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/analytics/image_statistics.py` & `pixano-0.5.3/pixano/analytics/image_statistics.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/README.md` & `pixano-0.5.3/pixano/app/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 ```python
 app.display()
 ```
 
 ## Using the Pixano app
 
-Please refer to our [user guide](https://pixano.github.io/user/app/) on our documentation website for more information on how to use it.
+Please refer to our [user guide](https://pixano.github.io) on our documentation website for more information on how to use it.
```

### Comparing `pixano-0.5.2/pixano/app/__init__.py` & `pixano-0.5.3/pixano/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/display.py` & `pixano-0.5.3/pixano/app/display.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/main.py` & `pixano-0.5.3/pixano/app/main.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/serve.py` & `pixano-0.5.3/pixano/app/serve.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/api/__init__.py` & `pixano-0.5.3/pixano/data/exporters/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,7 +6,15 @@
 # generate and explore labeled data for computer vision applications.
 # This software is governed by the CeCILL-C license under French law and
 # abiding by the rules of distribution of free software. You can use,
 # modify and/ or redistribute the software under the terms of the CeCILL-C
 # license as circulated by CEA, CNRS and INRIA at the following URL
 #
 # http://www.cecill.info
+
+from pixano.data.exporters.coco_exporter import COCOExporter
+from pixano.data.exporters.exporter import Exporter
+
+__all__ = [
+    "Exporter",
+    "COCOExporter",
+]
```

### Comparing `pixano-0.5.2/pixano/app/api/datasets.py` & `pixano-0.5.3/pixano/app/api/datasets.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/api/items.py` & `pixano-0.5.3/pixano/app/api/items.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/api/models.py` & `pixano-0.5.3/pixano/app/api/models.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/favicon.ico` & `pixano-0.5.3/pixano/app/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/index.html` & `pixano-0.5.3/pixano/app/dist/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 <!doctype html>
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <link rel="icon" href="data:," />
     
-		<link rel="modulepreload" href="/_app/immutable/entry/start.eFYr5dE2.js">
-		<link rel="modulepreload" href="/_app/immutable/chunks/entry.BdqlkNrw.js">
+		<link rel="modulepreload" href="/_app/immutable/entry/start.u9UDkqYj.js">
+		<link rel="modulepreload" href="/_app/immutable/chunks/entry.BGJCdFkn.js">
 		<link rel="modulepreload" href="/_app/immutable/chunks/scheduler.Cq5UBZ1T.js">
-		<link rel="modulepreload" href="/_app/immutable/entry/app.B1yXTTAH.js">
+		<link rel="modulepreload" href="/_app/immutable/entry/app.y5DFN3Js.js">
 		<link rel="modulepreload" href="/_app/immutable/chunks/index.D__UofN6.js">
   </head>
   <body data-sveltekit-preload-data="hover">
     <div style="display: contents">
 			<script>
 				{
-					__sveltekit_oqq3xw = {
+					__sveltekit_3o1b6a = {
 						base: ""
 					};
 
 					const element = document.currentScript.parentElement;
 
 					Promise.all([
-						import("/_app/immutable/entry/start.eFYr5dE2.js"),
-						import("/_app/immutable/entry/app.B1yXTTAH.js")
+						import("/_app/immutable/entry/start.u9UDkqYj.js"),
+						import("/_app/immutable/entry/app.y5DFN3Js.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element);
 					});
 				}
 			</script>
 		</div>
   </body>
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/0.B5OR-Toy.css` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/0.B5OR-Toy.css`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/5.ZhT30vvc.css` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/5.ZhT30vvc.css`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/_layout.BNzN0mkq.css` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/_layout.BNzN0mkq.css`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/_page.BJ18IbJM.css` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/_page.BJ18IbJM.css`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/favicon.OuiISzV3.ico` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/favicon.OuiISzV3.ico`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/pixano.NAI_8qFW.png` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/pixano.NAI_8qFW.png`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/assets/pixano_white.BVKPSmmP.png` & `pixano-0.5.3/pixano/app/dist/_app/immutable/assets/pixano_white.BVKPSmmP.png`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/Histogram.USYLred5.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/Histogram.YSM0wxsW.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -33,19 +33,19 @@
     a as ys,
     t as ks,
     e as ws
 } from "./index.D__UofN6.js";
 import {
     u as Ms,
     H as te
-} from "./command.YXxPKXvy.js";
+} from "./command.CjKwrCHU.js";
 import {
     g as To,
     a as Ao
-} from "./datasetStores.BZ9GDOPp.js";
+} from "./datasetStores.Davxg0aA.js";
 /*!
  * @kurkle/color v0.3.2
  * https://github.com/kurkle/color#readme
  * (c) 2023 Jukka Kurkela
  * Released under the MIT License
  */
 function ue(i) {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/PrimaryButton.2luo0sZd.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/PrimaryButton.CjwzDHMn.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -32,19 +32,19 @@
     d as K,
     m as L,
     e as R
 } from "./index.D__UofN6.js";
 import {
     c as C,
     b as M
-} from "./command.YXxPKXvy.js";
+} from "./command.CjKwrCHU.js";
 import {
     g as U,
     a as ie
-} from "./datasetStores.BZ9GDOPp.js";
+} from "./datasetStores.Davxg0aA.js";
 
 function Be() {
     const l = le();
     return e => {
         const {
             originalEvent: r
         } = e.detail, {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/TooltipIconButton.h3qFl-sW.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/TooltipIconButton.DmW3ppx8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -48,26 +48,26 @@
 } from "./index.D__UofN6.js";
 import {
     d as Be,
     e as Pe,
     f as Ie,
     c as le,
     h as Se
-} from "./command.YXxPKXvy.js";
+} from "./command.CjKwrCHU.js";
 import {
     d as He
-} from "./entry.BdqlkNrw.js";
+} from "./entry.BGJCdFkn.js";
 import {
     g as L,
     a as je
-} from "./datasetStores.BZ9GDOPp.js";
+} from "./datasetStores.Davxg0aA.js";
 import {
     c as ze,
     B as Ue
-} from "./PrimaryButton.2luo0sZd.js";
+} from "./PrimaryButton.CjwzDHMn.js";
 
 function me(t) {
     let e, n;
     return {
         c() {
             e = V("p"), n = Z(t[1]), this.h()
         },
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/api.BxNj-TAm.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/api.BxNj-TAm.js`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/checkbox.OiMtEzVH.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/checkbox.DTaWBrBv.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -43,27 +43,27 @@
     m as U,
     e as W,
     f as ve
 } from "./index.D__UofN6.js";
 import {
     g as G,
     a as se
-} from "./datasetStores.BZ9GDOPp.js";
+} from "./datasetStores.Davxg0aA.js";
 import {
     s as pe,
     g as de,
     a as Ce,
     c as x
-} from "./command.YXxPKXvy.js";
+} from "./command.CjKwrCHU.js";
 import {
     c as ye
-} from "./PrimaryButton.2luo0sZd.js";
+} from "./PrimaryButton.CjwzDHMn.js";
 import {
     I as me
-} from "./loader-2.Cz-VINyt.js";
+} from "./loader-2.yiAD6ux3.js";
 
 function ie(i) {
     let e, l;
     return {
         c() {
             e = D("p"), l = $(i[1]), this.h()
         },
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/command.YXxPKXvy.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/command.CjKwrCHU.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
 } from "./scheduler.Cq5UBZ1T.js";
 import "./index.D__UofN6.js";
 import {
     d as bt,
     w as oe,
     r as Vo,
     a as uo
-} from "./entry.BdqlkNrw.js";
+} from "./entry.BGJCdFkn.js";
 
 function mr(e, t, r) {
     this.k = e, this.x = t, this.y = r
 }
 mr.prototype = {
     constructor: mr,
     scale: function(e) {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/datasetStores.BZ9GDOPp.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/datasetStores.Davxg0aA.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
     a as v
 } from "./index.D__UofN6.js";
 import {
     M as I
 } from "./scheduler.Cq5UBZ1T.js";
 import {
     w as _
-} from "./entry.BdqlkNrw.js";
+} from "./entry.BGJCdFkn.js";
 
 function z(e) {
     return (e == null ? void 0 : e.length) !== void 0 ? e : Array.from(e)
 }
 
 function j(e, f) {
     M(e, 1, 1, () => {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/entry.BdqlkNrw.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/entry.BGJCdFkn.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 import {
-    n as V,
+    n as F,
     ai as st,
     M as it,
     s as ct,
     Q as lt,
     K as ft
 } from "./scheduler.Cq5UBZ1T.js";
 new URL("sveltekit-internal://");
@@ -75,42 +75,42 @@
 function bt(e) {
     const n = atob(e),
         t = new Uint8Array(n.length);
     for (let r = 0; r < n.length; r++) t[r] = n.charCodeAt(r);
     return t.buffer
 }
 const $e = window.fetch;
-window.fetch = (e, n) => ((e instanceof Request ? e.method : (n == null ? void 0 : n.method) || "GET") !== "GET" && F.delete(ge(e)), $e(e, n));
-const F = new Map;
+window.fetch = (e, n) => ((e instanceof Request ? e.method : (n == null ? void 0 : n.method) || "GET") !== "GET" && q.delete(ge(e)), $e(e, n));
+const q = new Map;
 
 function vt(e, n) {
     const t = ge(e, n),
         r = document.querySelector(t);
     if (r != null && r.textContent) {
         let {
             body: a,
             ...o
         } = JSON.parse(r.textContent);
         const i = r.getAttribute("data-ttl");
-        return i && F.set(t, {
+        return i && q.set(t, {
             body: a,
             init: o,
             ttl: 1e3 * Number(i)
         }), r.getAttribute("data-b64") !== null && (a = bt(a)), Promise.resolve(new Response(a, o))
     }
     return window.fetch(e, n)
 }
 
 function Et(e, n, t) {
-    if (F.size > 0) {
+    if (q.size > 0) {
         const r = ge(e, t),
-            a = F.get(r);
+            a = q.get(r);
         if (a) {
             if (performance.now() < a.ttl && ["default", "force-cache", "only-if-cached", void 0].includes(t == null ? void 0 : t.cache)) return new Response(a.body, a.init);
-            F.delete(r)
+            q.delete(r)
         }
     }
     return window.fetch(n, t)
 }
 
 function ge(e, n) {
     let r = `script[data-sveltekit-fetched][data-url=${JSON.stringify(e instanceof Request?e.url:e)}]`;
@@ -220,15 +220,15 @@
 
 function Pt(e, n) {
     return {
         subscribe: ne(e, n).subscribe
     }
 }
 
-function ne(e, n = V) {
+function ne(e, n = F) {
     let t;
     const r = new Set;
 
     function a(s) {
         if (ct(e, s) && (e = s, t)) {
             const c = !N.length;
             for (const l of r) l[1](), N.push(l, e);
@@ -239,17 +239,17 @@
         }
     }
 
     function o(s) {
         a(s(e))
     }
 
-    function i(s, c = V) {
+    function i(s, c = F) {
         const l = [s, c];
-        return r.add(l), r.size === 1 && (t = n(a, o) || V), s(e), () => {
+        return r.add(l), r.size === 1 && (t = n(a, o) || F), s(e), () => {
             r.delete(l), r.size === 0 && t && (t(), t = null)
         }
     }
     return {
         set: a,
         update: o,
         subscribe: i
@@ -261,20 +261,20 @@
         a = r ? [e] : e;
     if (!a.every(Boolean)) throw new Error("derived() expects stores as input, got a falsy value");
     const o = n.length < 2;
     return Pt(t, (i, s) => {
         let c = !1;
         const l = [];
         let u = 0,
-            h = V;
+            h = F;
         const g = () => {
                 if (u) return;
                 h();
                 const m = n(r ? l[0] : l, i, s);
-                o ? i(m) : h = lt(m) ? m : V
+                o ? i(m) : h = lt(m) ? m : F
             },
             d = a.map((m, f) => st(m, _ => {
                 l[f] = _, u &= ~(1 << f), c && g()
             }, () => {
                 u |= 1 << f
             }));
         return c = !0, g(),
@@ -286,35 +286,35 @@
 
 function rn(e) {
     return {
         subscribe: e.subscribe.bind(e)
     }
 }
 var Oe;
-const I = ((Oe = globalThis.__sveltekit_oqq3xw) == null ? void 0 : Oe.base) ?? "";
+const I = ((Oe = globalThis.__sveltekit_3o1b6a) == null ? void 0 : Oe.base) ?? "";
 var je;
-const xt = ((je = globalThis.__sveltekit_oqq3xw) == null ? void 0 : je.assets) ?? I,
-    Tt = "1716815462815",
+const xt = ((je = globalThis.__sveltekit_3o1b6a) == null ? void 0 : je.assets) ?? I,
+    Tt = "1716995202829",
     Ce = "sveltekit:snapshot",
-    qe = "sveltekit:scroll",
-    Ve = "sveltekit:states",
+    Ve = "sveltekit:scroll",
+    Fe = "sveltekit:states",
     Ut = "sveltekit:pageurl",
     $ = "sveltekit:history",
     M = "sveltekit:navigation",
     Y = {
         tap: 1,
         hover: 2,
         viewport: 3,
         eager: 4,
         off: -1,
         false: -1
     },
     K = location.origin;
 
-function Fe(e) {
+function qe(e) {
     if (e instanceof URL) return e;
     let n = document.baseURI;
     if (!n) {
         const t = document.getElementsByTagName("base");
         n = t.length ? t[0].href : document.URL
     }
     return new URL(e, n)
@@ -452,28 +452,28 @@
     return e.origin !== K || !e.pathname.startsWith(n)
 }
 const Ot = -1,
     jt = -2,
     $t = -3,
     Dt = -4,
     Ct = -5,
-    qt = -6;
+    Vt = -6;
 
-function Vt(e, n) {
+function Ft(e, n) {
     if (typeof e == "number") return a(e, !0);
     if (!Array.isArray(e) || e.length === 0) throw new Error("Invalid input");
     const t = e,
         r = Array(t.length);
 
     function a(o, i = !1) {
         if (o === Ot) return;
         if (o === $t) return NaN;
         if (o === Dt) return 1 / 0;
         if (o === Ct) return -1 / 0;
-        if (o === qt) return -0;
+        if (o === Vt) return -0;
         if (i) throw new Error("Invalid input");
         if (o in r) return r[o];
         const s = t[o];
         if (!s || typeof s != "object") r[o] = s;
         else if (Array.isArray(s))
             if (typeof s[0] == "string") {
                 const c = s[0],
@@ -528,16 +528,16 @@
         }
         return r[o]
     }
     return a(0)
 }
 const Be = new Set(["load", "prerender", "csr", "ssr", "trailingSlash", "config"]);
 [...Be];
-const Ft = new Set([...Be]);
-[...Ft];
+const qt = new Set([...Be]);
+[...qt];
 
 function Mt(e) {
     return e.filter(n => n != null)
 }
 class re {
     constructor(n, t) {
         this.status = n, typeof t == "string" ? this.body = {
@@ -566,15 +566,15 @@
 function W(e) {
     return e instanceof re || e instanceof _e ? e.status : 500
 }
 
 function Ht(e) {
     return e instanceof _e ? e.text : "Internal Error"
 }
-const U = De(qe) ?? {},
+const U = De(Ve) ?? {},
     G = De(Ce) ?? {},
     x = {
         url: Pe({}),
         page: Pe({}),
         navigating: ne(null),
         updated: Nt()
     };
@@ -606,15 +606,15 @@
         error: null,
         url: null
     },
     we = !1,
     Z = !1,
     Te = !0,
     B = !1,
-    q = !1,
+    V = !1,
     Ye = !1,
     be = !1,
     ve, k, A, R, ee;
 async function on(e, n, t) {
     var a, o;
     document.URL !== location.href && (location.href = location.href), C = e, oe = Lt(e), L = document.documentElement, pe = n, he = e.nodes[0], X = e.nodes[1], he(), X(), k = (a = history.state) == null ? void 0 : a[$], A = (o = history.state) == null ? void 0 : o[M], k || (k = A = Date.now(), history.replaceState({
         ...history.state,
@@ -639,20 +639,20 @@
     (n = G[e]) == null || n.forEach((t, r) => {
         var a, o;
         (o = (a = Q[r]) == null ? void 0 : a.snapshot) == null || o.restore(t)
     })
 }
 
 function Ue() {
-    ye(k), Ie(qe, U), Je(A), Ie(Ce, G)
+    ye(k), Ie(Ve, U), Je(A), Ie(Ce, G)
 }
 async function Xe(e, n, t, r) {
     return z({
         type: "goto",
-        url: Fe(e),
+        url: qe(e),
         keepfocus: n.keepFocus,
         noscroll: n.noScroll,
         replace_state: n.replaceState,
         state: n.state,
         redirect_count: t,
         nav_token: r,
         accept: () => {
@@ -1150,15 +1150,15 @@
         else return Xe(new URL(f.location, n).href, {}, s + 1, c), !1;
     else f.props.page.status >= 400 && await x.updated.check() && await D(n);
     if (Ke.length = 0, be = !1, ye(d), Je(m), f.props.page.url.pathname !== n.pathname && (n.pathname = f.props.page.url.pathname), i = t ? t.state : i, !t) {
         const p = o ? 0 : 1,
             y = {
                 [$]: k += p,
                 [M]: A += p,
-                [Ve]: i
+                [Fe]: i
             };
         (o ? history.replaceState : history.pushState).call(history, y, "", n), o || Kt(k, A)
     }
     if (P = null, f.props.page.state = i, Z) {
         w = f.state, f.props.page && (f.props.page.url = n);
         const p = (await Promise.all(zt.map(y => y(g.navigation)))).filter(y => typeof y == "function");
         if (p.length > 0) {
@@ -1255,15 +1255,15 @@
         message: r
     }) ?? {
         message: r
     }
 }
 
 function Qt(e, n = {}) {
-    return e = Fe(e), e.origin !== K ? Promise.reject(new Error("goto: invalid URL")) : Xe(e, n, 0)
+    return e = qe(e), e.origin !== K ? Promise.reject(new Error("goto: invalid URL")) : Xe(e, n, 0)
 }
 
 function Zt() {
     var n;
     history.scrollRestoration = "manual", addEventListener("beforeunload", t => {
         let r = !1;
         if (Ue(), !B) {
@@ -1308,16 +1308,16 @@
             const [, d] = w.url.href.split("#");
             if (d === h) {
                 t.preventDefault(), h === "" || h === "top" && r.ownerDocument.getElementById("top") === null ? window.scrollTo({
                     top: 0
                 }) : (g = r.ownerDocument.getElementById(h)) == null || g.scrollIntoView();
                 return
             }
-            if (q = !0, ye(k), e(a), !c.replace_state) return;
-            q = !1
+            if (V = !0, ye(k), e(a), !c.replace_state) return;
+            V = !1
         }
         t.preventDefault(), z({
             type: "link",
             url: a,
             keepfocus: c.keepfocus,
             noscroll: c.noscroll,
             replace_state: c.replace_state ?? a.href === location.href
@@ -1344,15 +1344,15 @@
         })
     }), addEventListener("popstate", async t => {
         var r;
         if ((r = t.state) != null && r[$]) {
             const a = t.state[$];
             if (ee = {}, a === k) return;
             const o = U[a],
-                i = t.state[Ve] ?? {},
+                i = t.state[Fe] ?? {},
                 s = new URL(t.state[Ut] ?? location.href),
                 c = t.state[M],
                 l = le(location) === le(w.url);
             if (c === A && (Ye || l)) {
                 e(s), U[k] = me(), o && scrollTo(o.x, o.y), i !== R.state && (R = {
                     ...R,
                     state: i
@@ -1374,20 +1374,20 @@
                     k = a, A = c
                 },
                 block: () => {
                     history.go(-h)
                 },
                 nav_token: ee
             })
-        } else if (!q) {
+        } else if (!V) {
             const a = new URL(location.href);
             e(a)
         }
     }), addEventListener("hashchange", () => {
-        q && (q = !1, history.replaceState({
+        V && (V = !1, history.replaceState({
             ...history.state,
             [$]: ++k,
             [M]: A
         }, "", location.href))
     });
     for (const t of document.querySelectorAll("link")) t.rel === "icon" && (t.href = t.href);
     addEventListener("pageshow", t => {
@@ -1482,15 +1482,15 @@
     return new Promise(async o => {
         var h;
         const i = new Map,
             s = r.body.getReader(),
             c = new TextDecoder;
 
         function l(g) {
-            return Vt(g, {
+            return Ft(g, {
                 Promise: d => new Promise((m, f) => {
                     i.set(d, {
                         fulfil: m,
                         reject: f
                     })
                 })
             })
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/icons.Dxr1AG5A.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/icons.Dxr1AG5A.js`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/index.D__UofN6.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/index.D__UofN6.js`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/loader-2.Cz-VINyt.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/loader-2.yiAD6ux3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
     m as U,
     e as V
 } from "./index.D__UofN6.js";
 import {
     e as B,
     g as E,
     a as X
-} from "./datasetStores.BZ9GDOPp.js";
+} from "./datasetStores.Davxg0aA.js";
 const I = {
     xmlns: "http://www.w3.org/2000/svg",
     width: 24,
     height: 24,
     viewBox: "0 0 24 24",
     fill: "none",
     stroke: "currentColor",
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/chunks/scheduler.Cq5UBZ1T.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/chunks/scheduler.Cq5UBZ1T.js`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/entry/app.B1yXTTAH.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/entry/app.y5DFN3Js.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -371,15 +371,15 @@
             components: 0,
             form: 2,
             data_0: 3,
             data_1: 4
         })
     }
 }
-const ae = [() => k(() => import("../nodes/0.DW46KZ9m.js"), __vite__mapDeps([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]), import.meta.url), () => k(() => import("../nodes/1.C5NidKnH.js"), __vite__mapDeps([13, 1, 2, 3, 4]), import.meta.url), () => k(() => import("../nodes/2.CZmQkO2Y.js"), __vite__mapDeps([14, 1, 2, 8, 4, 7, 11]), import.meta.url), () => k(() => import("../nodes/3.JUP818GM.js"), __vite__mapDeps([15, 1, 2, 3, 4, 5, 6, 8, 16]), import.meta.url), () => k(() => import("../nodes/4.DGnIT7o0.js"), __vite__mapDeps([17, 1, 2, 3, 4, 8, 7, 6, 18, 10, 11, 16, 19]), import.meta.url), () => k(() => import("../nodes/5.Bo-LObf-.js"), __vite__mapDeps([20, 1, 2, 3, 4, 5, 6, 10, 8, 9, 11, 18, 21]), import.meta.url)],
+const ae = [() => k(() => import("../nodes/0.ChfaHG46.js"), __vite__mapDeps([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]), import.meta.url), () => k(() => import("../nodes/1.DCJl0UMA.js"), __vite__mapDeps([13, 1, 2, 3, 4]), import.meta.url), () => k(() => import("../nodes/2.C5hi1hQI.js"), __vite__mapDeps([14, 1, 2, 8, 4, 7, 11]), import.meta.url), () => k(() => import("../nodes/3.CQlFeuu8.js"), __vite__mapDeps([15, 1, 2, 3, 4, 5, 6, 8, 16]), import.meta.url), () => k(() => import("../nodes/4.BYwXogVv.js"), __vite__mapDeps([17, 1, 2, 3, 4, 8, 7, 6, 18, 10, 11, 16, 19]), import.meta.url), () => k(() => import("../nodes/5.BngP3_K5.js"), __vite__mapDeps([20, 1, 2, 3, 4, 5, 6, 10, 8, 9, 11, 18, 21]), import.meta.url)],
     le = [],
     fe = {
         "/": [2],
         "/[dataset]/dashboard": [3],
         "/[dataset]/dataset": [4],
         "/[dataset]/dataset/[itemId]": [5]
     },
@@ -393,11 +393,11 @@
     };
 export {
     fe as dictionary, ce as hooks, re as matchers, ae as nodes, oe as root, le as server_loads
 };
 
 function __vite__mapDeps(indexes) {
     if (!__vite__mapDeps.viteFileDeps) {
-        __vite__mapDeps.viteFileDeps = ["../nodes/0.DW46KZ9m.js", "../chunks/scheduler.Cq5UBZ1T.js", "../chunks/index.D__UofN6.js", "../chunks/stores.titGXIKi.js", "../chunks/entry.BdqlkNrw.js", "../chunks/api.BxNj-TAm.js", "../chunks/command.YXxPKXvy.js", "../chunks/icons.Dxr1AG5A.js", "../chunks/datasetStores.BZ9GDOPp.js", "../chunks/TooltipIconButton.h3qFl-sW.js", "../chunks/PrimaryButton.2luo0sZd.js", "../chunks/loader-2.Cz-VINyt.js", "../assets/0.B5OR-Toy.css", "../nodes/1.C5NidKnH.js", "../nodes/2.CZmQkO2Y.js", "../nodes/3.JUP818GM.js", "../chunks/Histogram.USYLred5.js", "../nodes/4.DGnIT7o0.js", "../chunks/checkbox.OiMtEzVH.js", "../assets/4.BrLiNAg8.css", "../nodes/5.Bo-LObf-.js", "../assets/5.ZhT30vvc.css"]
+        __vite__mapDeps.viteFileDeps = ["../nodes/0.ChfaHG46.js", "../chunks/scheduler.Cq5UBZ1T.js", "../chunks/index.D__UofN6.js", "../chunks/stores.baCeY990.js", "../chunks/entry.BGJCdFkn.js", "../chunks/api.BxNj-TAm.js", "../chunks/command.CjKwrCHU.js", "../chunks/icons.Dxr1AG5A.js", "../chunks/datasetStores.Davxg0aA.js", "../chunks/TooltipIconButton.DmW3ppx8.js", "../chunks/PrimaryButton.CjwzDHMn.js", "../chunks/loader-2.yiAD6ux3.js", "../assets/0.B5OR-Toy.css", "../nodes/1.DCJl0UMA.js", "../nodes/2.C5hi1hQI.js", "../nodes/3.CQlFeuu8.js", "../chunks/Histogram.YSM0wxsW.js", "../nodes/4.BYwXogVv.js", "../chunks/checkbox.DTaWBrBv.js", "../assets/4.BrLiNAg8.css", "../nodes/5.BngP3_K5.js", "../assets/5.ZhT30vvc.css"]
     }
     return indexes.map((i) => __vite__mapDeps.viteFileDeps[i])
 }
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/0.DW46KZ9m.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/0.ChfaHG46.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -39,51 +39,51 @@
     t as k,
     e as U,
     g as te,
     c as ne
 } from "../chunks/index.D__UofN6.js";
 import {
     p as Pe
-} from "../chunks/stores.titGXIKi.js";
+} from "../chunks/stores.baCeY990.js";
 import {
     a as ye,
     b as ze,
     s as Ue,
     c as Re,
     g as Oe
 } from "../chunks/api.BxNj-TAm.js";
-import "../chunks/command.YXxPKXvy.js";
+import "../chunks/command.CjKwrCHU.js";
 import {
     a as Fe
 } from "../chunks/icons.Dxr1AG5A.js";
 import {
     g as re,
     a as oe,
     d as de,
     e as Ne,
     s as _e,
     i as We,
     b as De,
     m as Ge,
     c as Ke
-} from "../chunks/datasetStores.BZ9GDOPp.js";
+} from "../chunks/datasetStores.Davxg0aA.js";
 import {
     g as pe
-} from "../chunks/entry.BdqlkNrw.js";
+} from "../chunks/entry.BGJCdFkn.js";
 import {
     T as $e,
     C as Ye
-} from "../chunks/TooltipIconButton.h3qFl-sW.js";
+} from "../chunks/TooltipIconButton.DmW3ppx8.js";
 import {
     P as Je
-} from "../chunks/PrimaryButton.2luo0sZd.js";
+} from "../chunks/PrimaryButton.CjwzDHMn.js";
 import {
     I as ie,
     L as Qe
-} from "../chunks/loader-2.Cz-VINyt.js";
+} from "../chunks/loader-2.yiAD6ux3.js";
 const Xe = !1,
     Ze = !1,
     Zt = Object.freeze(Object.defineProperty({
         __proto__: null,
         prerender: Xe,
         ssr: Ze
     }, Symbol.toStringTag, {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/1.C5NidKnH.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/1.DCJl0UMA.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
 } from "../chunks/scheduler.Cq5UBZ1T.js";
 import {
     S as q,
     i as y
 } from "../chunks/index.D__UofN6.js";
 import {
     p as C
-} from "../chunks/stores.titGXIKi.js";
+} from "../chunks/stores.baCeY990.js";
 
 function H(i) {
     var f;
     let a, s = i[0].status + "",
         r, o, n, p = ((f = i[0].error) == null ? void 0 : f.message) + "",
         c;
     return {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/2.CZmQkO2Y.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/2.C5hi1hQI.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -33,24 +33,24 @@
     d as ie,
     m as oe,
     e as ce
 } from "../chunks/index.D__UofN6.js";
 import {
     d as _e,
     e as Y
-} from "../chunks/datasetStores.BZ9GDOPp.js";
+} from "../chunks/datasetStores.Davxg0aA.js";
 import {
     g as he
-} from "../chunks/entry.BdqlkNrw.js";
+} from "../chunks/entry.BGJCdFkn.js";
 import {
     s as pe
 } from "../chunks/icons.Dxr1AG5A.js";
 import {
     L as ve
-} from "../chunks/loader-2.Cz-VINyt.js";
+} from "../chunks/loader-2.yiAD6ux3.js";
 const ge = !1,
     be = !1,
     Be = Object.freeze(Object.defineProperty({
         __proto__: null,
         prerender: ge,
         ssr: be
     }, Symbol.toStringTag, {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/3.JUP818GM.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/3.CQlFeuu8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -29,28 +29,28 @@
     b as ue,
     d as _e,
     m as de,
     e as he
 } from "../chunks/index.D__UofN6.js";
 import {
     p as ve
-} from "../chunks/stores.titGXIKi.js";
+} from "../chunks/stores.baCeY990.js";
 import {
     g as be
 } from "../chunks/api.BxNj-TAm.js";
 import {
     c as ee
-} from "../chunks/command.YXxPKXvy.js";
+} from "../chunks/command.CjKwrCHU.js";
 import {
     e as G,
     d as ge
-} from "../chunks/datasetStores.BZ9GDOPp.js";
+} from "../chunks/datasetStores.Davxg0aA.js";
 import {
     H as ke
-} from "../chunks/Histogram.USYLred5.js";
+} from "../chunks/Histogram.YSM0wxsW.js";
 const xe = !1,
     De = !1,
     He = Object.freeze(Object.defineProperty({
         __proto__: null,
         prerender: xe,
         ssr: De
     }, Symbol.toStringTag, {
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/4.DGnIT7o0.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/4.BYwXogVv.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1578 +1,1295 @@
-var xt = Object.defineProperty;
-var es = (n, e, t) => e in n ? xt(n, e, {
+var ss = Object.defineProperty;
+var rs = (n, e, t) => e in n ? ss(n, e, {
     enumerable: !0,
     configurable: !0,
     writable: !0,
     value: t
 }) : n[e] = t;
-var D = (n, e, t) => (es(n, typeof e != "symbol" ? e + "" : e, t), t);
+var I = (n, e, t) => (rs(n, typeof e != "symbol" ? e + "" : e, t), t);
 import {
-    n as q,
-    X as ts,
-    y as ue,
-    Q as Mt,
-    s as se,
+    n as J,
+    X as ls,
+    y as fe,
+    Q as Ot,
+    s as ee,
     e as j,
     c as A,
-    b as M,
-    f as g,
-    o as $,
-    i as F,
-    r as Oe,
-    h as C,
-    p as ae,
-    M as Ne,
+    b as R,
+    f as _,
+    o as v,
+    i as T,
+    r as He,
+    h as y,
+    p as ne,
+    M as ze,
     I as je,
-    t as ne,
-    d as oe,
-    j as be,
+    t as re,
+    d as le,
+    j as me,
     J as Ae,
-    v as N,
-    q as Ue,
-    x as Rt,
-    a as P,
-    g as L,
-    a8 as lt,
-    A as Bt,
-    B as Ht,
-    C as Ot,
-    T as ss,
-    D as nt,
-    k as ye,
-    E as rs,
-    w as Pt,
-    G as ls,
-    S as Je,
-    L as ve,
+    v as z,
+    x as Ht,
+    A as Nt,
+    B as Pt,
+    C as Lt,
+    D as ot,
+    k as Ee,
+    E as ns,
+    w as Vt,
+    G as os,
+    S as We,
+    q as Qe,
+    a as L,
+    g as V,
+    a8 as it,
+    T as is,
+    L as be,
     R as ce,
-    a9 as qe,
+    a9 as Je,
     l as Te,
     m as De,
-    aa as ot
+    aa as at
 } from "../chunks/scheduler.Cq5UBZ1T.js";
 import {
-    n as ns,
-    l as os,
-    o as as,
-    p as is,
-    S as re,
-    i as le,
-    b as z,
-    d as J,
-    m as G,
-    a as I,
-    t as S,
-    e as K,
+    n as as,
+    l as cs,
+    o as fs,
+    p as us,
+    S as te,
+    i as se,
+    b as K,
+    d as W,
+    m as q,
+    a as E,
+    t as F,
+    e as U,
     g as Z,
     c as x,
-    j as cs,
-    h as us,
-    f as We
+    f as Xe,
+    j as ds,
+    h as hs
 } from "../chunks/index.D__UofN6.js";
 import {
-    p as fs
-} from "../chunks/stores.titGXIKi.js";
+    p as ps
+} from "../chunks/stores.baCeY990.js";
 import {
     d as Y,
     r as Ie,
-    w as me,
-    g as ds
-} from "../chunks/entry.BdqlkNrw.js";
+    w as ge,
+    g as _s
+} from "../chunks/entry.BGJCdFkn.js";
 import {
-    e as ie,
+    g as de,
+    a as Ne,
+    e as oe,
     u as Me,
-    f as hs,
-    g as _e,
-    a as Pe,
-    o as Le,
-    b as Se,
-    D as ps,
-    h as _s,
-    d as gs
-} from "../chunks/datasetStores.BZ9GDOPp.js";
+    f as gs,
+    o as Pe,
+    b as Fe,
+    D as ms,
+    h as bs,
+    d as vs
+} from "../chunks/datasetStores.Davxg0aA.js";
 import {
-    b as ms,
-    c as bs,
-    s as vs,
-    a as $s,
-    d as ws,
-    e as ks,
-    f as ys,
-    g as Es,
-    h as Cs
+    b as $s,
+    c as ws,
+    s as ks,
+    a as ys,
+    d as Es,
+    e as Cs,
+    f as Is,
+    g as Ts,
+    h as Ds
 } from "../chunks/icons.Dxr1AG5A.js";
 import {
-    i as Lt,
-    q as Is
-} from "../chunks/command.YXxPKXvy.js";
+    i as zt,
+    q as Ss
+} from "../chunks/command.CjKwrCHU.js";
 import {
-    C as Ts,
-    W as Ds
-} from "../chunks/checkbox.OiMtEzVH.js";
+    C as Fs,
+    W as js
+} from "../chunks/checkbox.DTaWBrBv.js";
 import {
-    B as Nt,
-    P as Fs
-} from "../chunks/PrimaryButton.2luo0sZd.js";
+    B as Gt,
+    P as As
+} from "../chunks/PrimaryButton.CjwzDHMn.js";
 import {
-    H as Ss
-} from "../chunks/Histogram.USYLred5.js";
+    H as Ms
+} from "../chunks/Histogram.YSM0wxsW.js";
 import {
-    L as js
-} from "../chunks/loader-2.Cz-VINyt.js";
+    L as Rs
+} from "../chunks/loader-2.yiAD6ux3.js";
 
-function As(n, e, t, s) {
-    if (!e) return q;
+function Bs(n, e, t, s) {
+    if (!e) return J;
     const r = n.getBoundingClientRect();
-    if (e.left === r.left && e.right === r.right && e.top === r.top && e.bottom === r.bottom) return q;
+    if (e.left === r.left && e.right === r.right && e.top === r.top && e.bottom === r.bottom) return J;
     const {
         delay: l = 0,
         duration: o = 300,
-        easing: a = ts,
-        start: i = ns() + l,
-        end: c = i + o,
-        tick: d = q,
-        css: w
+        easing: i = ls,
+        start: a = as() + l,
+        end: c = a + o,
+        tick: d = J,
+        css: $
     } = t(n, {
         from: e,
         to: r
     }, s);
-    let y = !0,
-        m = !1,
-        b;
+    let k = !0,
+        g = !1,
+        m;
 
-    function f() {
-        w && (b = as(n, 0, 1, o, l, a, w)), l || (m = !0)
+    function u() {
+        $ && (m = fs(n, 0, 1, o, l, i, $)), l || (g = !0)
     }
 
-    function u() {
-        w && is(n, b), y = !1
+    function f() {
+        $ && us(n, m), k = !1
     }
-    return os(h => {
-        if (!m && h >= i && (m = !0), m && h >= c && (d(1, 0), u()), !y) return !1;
-        if (m) {
-            const p = h - i,
-                v = 0 + 1 * a(p / o);
-            d(v, 1 - v)
+    return cs(h => {
+        if (!g && h >= a && (g = !0), g && h >= c && (d(1, 0), f()), !k) return !1;
+        if (g) {
+            const p = h - a,
+                b = 0 + 1 * i(p / o);
+            d(b, 1 - b)
         }
         return !0
-    }), f(), d(0, 1), u
+    }), u(), d(0, 1), f
 }
 
-function Ms(n) {
+function Os(n) {
     const e = getComputedStyle(n);
     if (e.position !== "absolute" && e.position !== "fixed") {
         const {
             width: t,
             height: s
         } = e, r = n.getBoundingClientRect();
-        n.style.position = "absolute", n.style.width = t, n.style.height = s, Vt(n, r)
+        n.style.position = "absolute", n.style.width = t, n.style.height = s, Kt(n, r)
     }
 }
 
-function Vt(n, e) {
+function Kt(n, e) {
     const t = n.getBoundingClientRect();
     if (e.left !== t.left || e.top !== t.top) {
         const s = getComputedStyle(n),
             r = s.transform === "none" ? "" : s.transform;
         n.style.transform = `${r} translate(${e.left-t.left}px, ${e.top-t.top}px)`
     }
 }
 
-function Rs({
+function Hs({
     fallback: n,
     ...e
 }) {
     const t = new Map,
         s = new Map;
 
-    function r(o, a, i) {
+    function r(o, i, a) {
         const {
             delay: c = 0,
-            duration: d = V => Math.sqrt(V) * 30,
-            easing: w = Lt
-        } = ue(ue({}, e), i), y = o.getBoundingClientRect(), m = a.getBoundingClientRect(), b = y.left - m.left, f = y.top - m.top, u = y.width / m.width, h = y.height / m.height, p = Math.sqrt(b * b + f * f), v = getComputedStyle(a), R = v.transform === "none" ? "" : v.transform, ee = +v.opacity;
+            duration: d = O => Math.sqrt(O) * 30,
+            easing: $ = zt
+        } = fe(fe({}, e), a), k = o.getBoundingClientRect(), g = i.getBoundingClientRect(), m = k.left - g.left, u = k.top - g.top, f = k.width / g.width, h = k.height / g.height, p = Math.sqrt(m * m + u * u), b = getComputedStyle(i), B = b.transform === "none" ? "" : b.transform, S = +b.opacity;
         return {
             delay: c,
-            duration: Mt(d) ? d(p) : d,
-            easing: w,
-            css: (V, k) => `
-				opacity: ${V*ee};
+            duration: Ot(d) ? d(p) : d,
+            easing: $,
+            css: (O, G) => `
+				opacity: ${O*S};
 				transform-origin: top left;
-				transform: ${R} translate(${k*b}px,${k*f}px) scale(${V+(1-V)*u}, ${V+(1-V)*h});
+				transform: ${B} translate(${G*m}px,${G*u}px) scale(${O+(1-O)*f}, ${O+(1-O)*h});
 			`
         }
     }
 
-    function l(o, a, i) {
+    function l(o, i, a) {
         return (c, d) => (o.set(d.key, c), () => {
-            if (a.has(d.key)) {
-                const w = a.get(d.key);
-                return a.delete(d.key), r(w, c, d)
+            if (i.has(d.key)) {
+                const $ = i.get(d.key);
+                return i.delete(d.key), r($, c, d)
             }
-            return o.delete(d.key), n && n(c, d, i)
+            return o.delete(d.key), n && n(c, d, a)
         })
     }
     return [l(s, t, !1), l(t, s, !0)]
 }
-const Bs = !1,
-    Hs = !1,
-    Ml = Object.freeze(Object.defineProperty({
+const Ns = !1,
+    Ps = !1,
+    Ol = Object.freeze(Object.defineProperty({
         __proto__: null,
-        prerender: Bs,
-        ssr: Hs
+        prerender: Ns,
+        ssr: Ps
     }, Symbol.toStringTag, {
         value: "Module"
     }));
 
-function Os(n) {
+function Ls(n) {
     let e, t, s;
-    return t = new Ss({
+    return t = new Ms({
         props: {
             hist: n[0],
             minimal: !0
         }
     }), {
         c() {
-            e = j("div"), z(t.$$.fragment), this.h()
+            e = j("div"), K(t.$$.fragment), this.h()
         },
         l(r) {
             e = A(r, "DIV", {
                 class: !0
             });
-            var l = M(e);
-            J(t.$$.fragment, l), l.forEach(g), this.h()
+            var l = R(e);
+            W(t.$$.fragment, l), l.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "mx-8 h-24")
+            v(e, "class", "mx-8 h-24")
         },
         m(r, l) {
-            F(r, e, l), G(t, e, null), s = !0
+            T(r, e, l), q(t, e, null), s = !0
         },
         p(r, [l]) {
             const o = {};
             l & 1 && (o.hist = r[0]), t.$set(o)
         },
         i(r) {
-            s || (I(t.$$.fragment, r), s = !0)
+            s || (E(t.$$.fragment, r), s = !0)
         },
         o(r) {
-            S(t.$$.fragment, r), s = !1
+            F(t.$$.fragment, r), s = !1
         },
         d(r) {
-            r && g(e), K(t)
+            r && _(e), U(t)
         }
     }
 }
 
-function Ps(n, e, t) {
+function Vs(n, e, t) {
     let {
         value: s
     } = e;
     return n.$$set = r => {
         "value" in r && t(0, s = r.value)
     }, [s]
 }
-class Ls extends re {
+class zs extends te {
     constructor(e) {
-        super(), le(this, e, Ps, Os, se, {
+        super(), se(this, e, Vs, Ls, ee, {
             value: 0
         })
     }
 }
 
-function Ns(n) {
+function Gs(n) {
     let e, t, s;
     return {
         c() {
             e = j("div"), t = j("img"), this.h()
         },
         l(r) {
             e = A(r, "DIV", {
                 class: !0
             });
-            var l = M(e);
+            var l = R(e);
             t = A(l, "IMG", {
                 class: !0,
                 src: !0,
                 alt: !0
-            }), l.forEach(g), this.h()
+            }), l.forEach(_), this.h()
         },
         h() {
-            $(t, "class", "h-full w-full object-cover rounded"), Oe(t.src, s = n[0]) || $(t, "src", s), $(t, "alt", n[0]), $(e, "class", "mx-8 h-20 aspect-square")
+            v(t, "class", "h-full w-full object-cover rounded"), He(t.src, s = n[0]) || v(t, "src", s), v(t, "alt", n[0]), v(e, "class", "mx-8 h-20 aspect-square")
         },
         m(r, l) {
-            F(r, e, l), C(e, t)
+            T(r, e, l), y(e, t)
         },
         p(r, [l]) {
-            l & 1 && !Oe(t.src, s = r[0]) && $(t, "src", s), l & 1 && $(t, "alt", r[0])
+            l & 1 && !He(t.src, s = r[0]) && v(t, "src", s), l & 1 && v(t, "alt", r[0])
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(r) {
-            r && g(e)
+            r && _(e)
         }
     }
 }
 
-function Vs(n, e, t) {
+function Ks(n, e, t) {
     let {
         value: s
     } = e;
     return n.$$set = r => {
         "value" in r && t(0, s = r.value)
     }, [s]
 }
-class zs extends re {
+class qs extends te {
     constructor(e) {
-        super(), le(this, e, Vs, Ns, se, {
+        super(), se(this, e, Ks, Gs, ee, {
             value: 0
         })
     }
 }
 
-function Gs(n) {
+function Us(n) {
     let e, t, s, r, l;
     return {
         c() {
             e = j("div"), t = j("video"), this.h()
         },
         l(o) {
             e = A(o, "DIV", {
                 class: !0
             });
-            var a = M(e);
-            t = A(a, "VIDEO", {
+            var i = R(e);
+            t = A(i, "VIDEO", {
                 src: !0,
                 class: !0
-            }), M(t).forEach(g), a.forEach(g), this.h()
+            }), R(t).forEach(_), i.forEach(_), this.h()
         },
         h() {
-            Oe(t.src, s = n[0]) || $(t, "src", s), t.loop = !0, t.muted = !0, $(t, "class", "h-full w-full object-cover rounded"), $(e, "class", "mx-8 h-20 aspect-square")
+            He(t.src, s = n[0]) || v(t, "src", s), t.loop = !0, t.muted = !0, v(t, "class", "h-full w-full object-cover rounded"), v(e, "class", "mx-8 h-20 aspect-square")
         },
-        m(o, a) {
-            F(o, e, a), C(e, t), n[3](t), r || (l = [ae(t, "mouseenter", n[2]), ae(t, "mouseleave", n[2])], r = !0)
+        m(o, i) {
+            T(o, e, i), y(e, t), n[3](t), r || (l = [ne(t, "mouseenter", n[2]), ne(t, "mouseleave", n[2])], r = !0)
         },
-        p(o, [a]) {
-            a & 1 && !Oe(t.src, s = o[0]) && $(t, "src", s)
+        p(o, [i]) {
+            i & 1 && !He(t.src, s = o[0]) && v(t, "src", s)
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(o) {
-            o && g(e), n[3](null), r = !1, Ne(l)
+            o && _(e), n[3](null), r = !1, ze(l)
         }
     }
 }
 
-function Ks(n, e, t) {
+function Js(n, e, t) {
     let {
         value: s
     } = e, r, l = !1;
 
     function o() {
         l = !l, l ? (t(1, r.playbackRate = 4, r), r.play().catch(() => console.error("video playback error"))) : r.pause()
     }
 
-    function a(i) {
-        je[i ? "unshift" : "push"](() => {
-            r = i, t(1, r)
+    function i(a) {
+        je[a ? "unshift" : "push"](() => {
+            r = a, t(1, r)
         })
     }
-    return n.$$set = i => {
-        "value" in i && t(0, s = i.value)
-    }, [s, r, o, a]
+    return n.$$set = a => {
+        "value" in a && t(0, s = a.value)
+    }, [s, r, o, i]
 }
-class qs extends re {
+class Ws extends te {
     constructor(e) {
-        super(), le(this, e, Ks, Gs, se, {
+        super(), se(this, e, Js, Us, ee, {
             value: 0
         })
     }
 }
 
-function Us(n) {
+function Qs(n) {
     let e, t;
     return {
         c() {
-            e = j("div"), t = ne(n[0]), this.h()
+            e = j("div"), t = re(n[0]), this.h()
         },
         l(s) {
             e = A(s, "DIV", {
                 class: !0
             });
-            var r = M(e);
-            t = oe(r, n[0]), r.forEach(g), this.h()
+            var r = R(e);
+            t = le(r, n[0]), r.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "min-w-16 px-2")
+            v(e, "class", "min-w-16 px-2")
         },
         m(s, r) {
-            F(s, e, r), C(e, t)
+            T(s, e, r), y(e, t)
         },
         p(s, [r]) {
-            r & 1 && be(t, s[0])
+            r & 1 && me(t, s[0])
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(s) {
-            s && g(e)
+            s && _(e)
         }
     }
 }
 
-function Js(n, e, t) {
+function Xs(n, e, t) {
     let {
         value: s
     } = e;
     return n.$$set = r => {
         "value" in r && t(0, s = r.value)
     }, [s]
 }
-class at extends re {
+class ct extends te {
     constructor(e) {
-        super(), le(this, e, Js, Us, se, {
+        super(), se(this, e, Xs, Qs, ee, {
             value: 0
         })
     }
 }
 
-function Ws(n) {
+function Ys(n) {
     let e, t, s;
     return {
         c() {
             e = j("input"), this.h()
         },
         l(r) {
             e = A(r, "INPUT", {
                 type: !0,
                 class: !0
             }), this.h()
         },
         h() {
-            $(e, "type", "checkbox"), e.disabled = !0, $(e, "class", "px-4 pointer-events: none;")
+            v(e, "type", "checkbox"), e.disabled = !0, v(e, "class", "px-4 pointer-events: none;")
         },
         m(r, l) {
-            F(r, e, l), e.checked = n[0], t || (s = ae(e, "change", n[1]), t = !0)
+            T(r, e, l), e.checked = n[0], t || (s = ne(e, "change", n[1]), t = !0)
         },
         p(r, [l]) {
             l & 1 && (e.checked = r[0])
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(r) {
-            r && g(e), t = !1, s()
+            r && _(e), t = !1, s()
         }
     }
 }
 
-function Qs(n, e, t) {
+function Zs(n, e, t) {
     let {
         value: s
     } = e;
 
     function r() {
         s = this.checked, t(0, s)
     }
     return n.$$set = l => {
         "value" in l && t(0, s = l.value)
     }, [s, r]
 }
-class Xs extends re {
+class xs extends te {
     constructor(e) {
-        super(), le(this, e, Qs, Ws, se, {
+        super(), se(this, e, Zs, Ys, ee, {
             value: 0
         })
     }
 }
 
-function Ys(n) {
+function er(n) {
     let e, t;
     return {
         c() {
-            e = j("div"), t = ne(n[0]), this.h()
+            e = j("div"), t = re(n[0]), this.h()
         },
         l(s) {
             e = A(s, "DIV", {
                 class: !0
             });
-            var r = M(e);
-            t = oe(r, n[0]), r.forEach(g), this.h()
+            var r = R(e);
+            t = le(r, n[0]), r.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "min-w-24 px-2")
+            v(e, "class", "min-w-24 px-2")
         },
         m(s, r) {
-            F(s, e, r), C(e, t)
+            T(s, e, r), y(e, t)
         },
         p(s, [r]) {
-            r & 1 && be(t, s[0])
+            r & 1 && me(t, s[0])
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(s) {
-            s && g(e)
+            s && _(e)
         }
     }
 }
 
-function Zs(n, e, t) {
+function tr(n, e, t) {
     let {
         value: s
     } = e;
     return n.$$set = r => {
         "value" in r && t(0, s = r.value)
     }, [s]
 }
-class xs extends re {
+class sr extends te {
     constructor(e) {
-        super(), le(this, e, Zs, Ys, se, {
+        super(), se(this, e, tr, er, ee, {
             value: 0
         })
     }
 }
 
-function er(n) {
+function rr(n) {
     let e, t, s;
     var r = n[1][n[0].dtype];
 
-    function l(o, a) {
+    function l(o, i) {
         return {
             props: {
                 value: o[0].value
             }
         }
     }
     return r && (e = Ae(r, l(n))), {
         c() {
-            e && z(e.$$.fragment), t = N()
+            e && K(e.$$.fragment), t = z()
         },
         l(o) {
-            e && J(e.$$.fragment, o), t = N()
+            e && W(e.$$.fragment, o), t = z()
         },
-        m(o, a) {
-            e && G(e, o, a), F(o, t, a), s = !0
+        m(o, i) {
+            e && q(e, o, i), T(o, t, i), s = !0
         },
-        p(o, [a]) {
-            if (a & 1 && r !== (r = o[1][o[0].dtype])) {
+        p(o, [i]) {
+            if (i & 1 && r !== (r = o[1][o[0].dtype])) {
                 if (e) {
                     Z();
-                    const i = e;
-                    S(i.$$.fragment, 1, 0, () => {
-                        K(i, 1)
+                    const a = e;
+                    F(a.$$.fragment, 1, 0, () => {
+                        U(a, 1)
                     }), x()
                 }
-                r ? (e = Ae(r, l(o)), z(e.$$.fragment), I(e.$$.fragment, 1), G(e, t.parentNode, t)) : e = null
+                r ? (e = Ae(r, l(o)), K(e.$$.fragment), E(e.$$.fragment, 1), q(e, t.parentNode, t)) : e = null
             } else if (r) {
-                const i = {};
-                a & 1 && (i.value = o[0].value), e.$set(i)
+                const a = {};
+                i & 1 && (a.value = o[0].value), e.$set(a)
             }
         },
         i(o) {
-            s || (e && I(e.$$.fragment, o), s = !0)
+            s || (e && E(e.$$.fragment, o), s = !0)
         },
         o(o) {
-            e && S(e.$$.fragment, o), s = !1
+            e && F(e.$$.fragment, o), s = !1
         },
         d(o) {
-            o && g(t), e && K(e, o)
+            o && _(t), e && U(e, o)
         }
     }
 }
 
-function tr(n, e, t) {
+function lr(n, e, t) {
     let {
         itemFeature: s
     } = e;
     const r = {
-        int: at,
-        float: at,
-        bool: Xs,
-        str: xs,
-        image: zs,
-        video: qs,
-        histogram: Ls
+        int: ct,
+        float: ct,
+        bool: xs,
+        str: sr,
+        image: qs,
+        video: Ws,
+        histogram: zs
     };
     return n.$$set = l => {
         "itemFeature" in l && t(0, s = l.itemFeature)
     }, [s, r]
 }
-class sr extends re {
+class Le extends te {
     constructor(e) {
-        super(), le(this, e, tr, er, se, {
+        super(), se(this, e, lr, rr, ee, {
             itemFeature: 0
         })
     }
 }
-
-function rr(n, {
-    from: e,
-    to: t
-}, s = {}) {
-    const r = getComputedStyle(n),
-        l = r.transform === "none" ? "" : r.transform,
-        [o, a] = r.transformOrigin.split(" ").map(parseFloat),
-        i = e.left + e.width * o / t.width - (t.left + o),
-        c = e.top + e.height * a / t.height - (t.top + a),
-        {
-            delay: d = 0,
-            duration: w = m => Math.sqrt(m) * 120,
-            easing: y = Lt
-        } = s;
-    return {
-        delay: d,
-        duration: Mt(w) ? w(Math.sqrt(i * i + c * c)) : w,
-        easing: y,
-        css: (m, b) => {
-            const f = b * i,
-                u = b * c,
-                h = m + b * e.width / t.width,
-                p = m + b * e.height / t.height;
-            return `transform: ${l} translate(${f}px, ${u}px) scale(${h}, ${p});`
-        }
-    }
-}
-
-function it(n, e, t) {
-    const s = n.slice();
-    return s[15] = e[t], s[17] = t, s
-}
-const lr = n => ({
-        item: n & 1,
-        index: n & 1
-    }),
-    ct = n => ({
-        item: n[15],
-        index: n[17]
-    });
-
-function ut(n) {
-    let e, t = [],
-        s = new Map,
-        r, l = ie(n[0]);
-    const o = a => a[8](a[15]);
-    for (let a = 0; a < l.length; a += 1) {
-        let i = it(n, l, a),
-            c = o(i);
-        s.set(c, t[a] = ft(c, i))
-    }
-    return {
-        c() {
-            e = j("ul");
-            for (let a = 0; a < t.length; a += 1) t[a].c();
-            this.h()
-        },
-        l(a) {
-            e = A(a, "UL", {
-                class: !0
-            });
-            var i = M(e);
-            for (let c = 0; c < t.length; c += 1) t[c].l(i);
-            i.forEach(g), this.h()
-        },
-        h() {
-            $(e, "class", "svelte-s1iyrp")
-        },
-        m(a, i) {
-            F(a, e, i);
-            for (let c = 0; c < t.length; c += 1) t[c] && t[c].m(e, null);
-            r = !0
-        },
-        p(a, i) {
-            if (i & 1523) {
-                l = ie(a[0]), Z();
-                for (let c = 0; c < t.length; c += 1) t[c].r();
-                t = Me(t, i, o, 1, a, l, s, e, hs, ft, null, it);
-                for (let c = 0; c < t.length; c += 1) t[c].a();
-                x()
-            }
-        },
-        i(a) {
-            if (!r) {
-                for (let i = 0; i < l.length; i += 1) I(t[i]);
-                r = !0
-            }
-        },
-        o(a) {
-            for (let i = 0; i < t.length; i += 1) S(t[i]);
-            r = !1
-        },
-        d(a) {
-            a && g(e);
-            for (let i = 0; i < t.length; i += 1) t[i].d()
-        }
-    }
-}
-
-function nr(n) {
-    let e, t = n[8](n[15]) + "",
-        s;
-    return {
-        c() {
-            e = j("p"), s = ne(t)
-        },
-        l(r) {
-            e = A(r, "P", {});
-            var l = M(e);
-            s = oe(l, t), l.forEach(g)
-        },
-        m(r, l) {
-            F(r, e, l), C(e, s)
-        },
-        p(r, l) {
-            l & 1 && t !== (t = r[8](r[15]) + "") && be(s, t)
-        },
-        d(r) {
-            r && g(e)
-        }
-    }
-}
-
-function ft(n, e) {
-    let t, s, r, l, o, a, i, c = q,
-        d, w, y;
-    const m = e[11].default,
-        b = Rt(m, e, e[10], ct),
-        f = b || nr(e);
-    return {
-        key: n,
-        first: null,
-        c() {
-            t = j("li"), f && f.c(), s = P(), this.h()
-        },
-        l(u) {
-            t = A(u, "LI", {
-                "data-index": !0,
-                "data-id": !0,
-                draggable: !0,
-                class: !0
-            });
-            var h = M(t);
-            f && f.l(h), s = L(h), h.forEach(g), this.h()
-        },
-        h() {
-            $(t, "data-index", r = e[17]), $(t, "data-id", l = JSON.stringify(e[8](e[15]))), $(t, "draggable", "true"), $(t, "class", "svelte-s1iyrp"), lt(t, "over", e[8](e[15]) === e[1]), this.first = t
-        },
-        m(u, h) {
-            F(u, t, h), f && f.m(t, null), C(t, s), d = !0, w || (y = [ae(t, "dragstart", e[4]), ae(t, "dragover", e[5]), ae(t, "dragleave", e[6]), ae(t, "drop", e[7])], w = !0)
-        },
-        p(u, h) {
-            e = u, b ? b.p && (!d || h & 1025) && Bt(b, m, e, e[10], d ? Ot(m, e[10], h, lr) : Ht(e[10]), ct) : f && f.p && (!d || h & 1) && f.p(e, d ? h : -1), (!d || h & 1 && r !== (r = e[17])) && $(t, "data-index", r), (!d || h & 1 && l !== (l = JSON.stringify(e[8](e[15])))) && $(t, "data-id", l), (!d || h & 259) && lt(t, "over", e[8](e[15]) === e[1])
-        },
-        r() {
-            i = t.getBoundingClientRect()
-        },
-        f() {
-            Ms(t), c(), Vt(t, i)
-        },
-        a() {
-            c(), c = As(t, i, rr, {
-                duration: 300
-            })
-        },
-        i(u) {
-            d || (I(f, u), u && ss(() => {
-                d && (a && a.end(1), o = cs(t, e[3], {
-                    key: e[8](e[15])
-                }), o.start())
-            }), d = !0)
-        },
-        o(u) {
-            S(f, u), o && o.invalidate(), u && (a = us(t, e[2], {
-                key: e[8](e[15])
-            })), d = !1
-        },
-        d(u) {
-            u && g(t), f && f.d(u), u && a && a.end(), w = !1, Ne(y)
-        }
-    }
-}
-
-function or(n) {
-    let e, t, s = n[0] && n[0].length && ut(n);
-    return {
-        c() {
-            s && s.c(), e = N()
-        },
-        l(r) {
-            s && s.l(r), e = N()
-        },
-        m(r, l) {
-            s && s.m(r, l), F(r, e, l), t = !0
-        },
-        p(r, [l]) {
-            r[0] && r[0].length ? s ? (s.p(r, l), l & 1 && I(s, 1)) : (s = ut(r), s.c(), I(s, 1), s.m(e.parentNode, e)) : s && (Z(), S(s, 1, 1, () => {
-                s = null
-            }), x())
-        },
-        i(r) {
-            t || (I(s), t = !0)
-        },
-        o(r) {
-            S(s), t = !1
-        },
-        d(r) {
-            r && g(e), s && s.d(r)
-        }
-    }
-}
-
-function ar(n, e, t) {
-    let {
-        $$slots: s = {},
-        $$scope: r
-    } = e;
-    const [l, o] = Rs({
-        duration: p => Math.sqrt(p * 200),
-        fallback(p, v) {
-            const R = getComputedStyle(p),
-                ee = R.transform === "none" ? "" : R.transform;
-            return {
-                duration: 600,
-                easing: Is,
-                css: V => `
-					transform: ${ee} scale(${V});
-					opacity: ${V}
-				`
-            }
-        }
-    });
-    let a = !1;
-    const i = p => p.dataset.index && p.dataset || i(p.parentNode),
-        c = p => {
-            p.dataTransfer.setData("source", p.target.dataset.index)
-        },
-        d = p => {
-            p.preventDefault();
-            let v = i(p.target);
-            a !== v.id && t(1, a = JSON.parse(v.id))
-        },
-        w = p => {
-            let v = i(p.target);
-            a === v.id && t(1, a = !1)
-        },
-        y = p => {
-            t(1, a = !1), p.preventDefault();
-            let v = i(p.target),
-                R = p.dataTransfer.getData("source"),
-                ee = v.index;
-            b({
-                from: R,
-                to: ee
-            })
-        },
-        m = Ue(),
-        b = ({
-            from: p,
-            to: v
-        }) => {
-            let R = [...u];
-            R[p] = [R[v], R[v] = R[p]][0], m("sort", R)
-        },
-        f = p => h ? p[h] : p;
-    let {
-        list: u
-    } = e, {
-        key: h
-    } = e;
-    return n.$$set = p => {
-        "list" in p && t(0, u = p.list), "key" in p && t(9, h = p.key), "$$scope" in p && t(10, r = p.$$scope)
-    }, [u, a, l, o, c, d, w, y, f, h, r, s]
-}
-class ir extends re {
-    constructor(e) {
-        super(), le(this, e, ar, or, se, {
-            list: 0,
-            key: 9
-        })
-    }
-}
-const zt = n => {
+const qt = n => {
         const e = Object.entries(n),
             t = e.map(([s]) => s);
         return Y(e.map(([, s]) => s), s => Object.fromEntries(s.map((r, l) => [t[l], r])))
     },
-    cr = n => n & 1,
-    ur = n => ({}),
-    dt = n => ({
+    nr = n => n & 1,
+    or = n => ({}),
+    ft = n => ({
         ...n[0]
     });
 
-function fr(n) {
+function ir(n) {
     let e;
     const t = n[3].default,
-        s = Rt(t, n, n[2], dt);
+        s = Ht(t, n, n[2], ft);
     return {
         c() {
             s && s.c()
         },
         l(r) {
             s && s.l(r)
         },
         m(r, l) {
             s && s.m(r, l), e = !0
         },
         p(r, [l]) {
-            s && s.p && (!e || l & 5) && Bt(s, t, r, r[2], cr(l) || !e ? Ht(r[2]) : Ot(t, r[2], l, ur), dt)
+            s && s.p && (!e || l & 5) && Nt(s, t, r, r[2], nr(l) || !e ? Pt(r[2]) : Lt(t, r[2], l, or), ft)
         },
         i(r) {
-            e || (I(s, r), e = !0)
+            e || (E(s, r), e = !0)
         },
         o(r) {
-            S(s, r), e = !1
+            F(s, r), e = !1
         },
         d(r) {
             s && s.d(r)
         }
     }
 }
 
-function dr(n, e, t) {
+function ar(n, e, t) {
     const s = [];
-    let r = nt(e, s),
+    let r = ot(e, s),
         l, {
             $$slots: o = {},
-            $$scope: a
+            $$scope: i
         } = e;
-    const i = zt(r);
-    return ye(n, i, c => t(0, l = c)), n.$$set = c => {
-        e = ue(ue({}, e), rs(c)), t(4, r = nt(e, s)), "$$scope" in c && t(2, a = c.$$scope)
-    }, [l, i, a, o]
+    const a = qt(r);
+    return Ee(n, a, c => t(0, l = c)), n.$$set = c => {
+        e = fe(fe({}, e), ns(c)), t(4, r = ot(e, s)), "$$scope" in c && t(2, i = c.$$scope)
+    }, [l, a, i, o]
 }
-class Re extends re {
+class Re extends te {
     constructor(e) {
-        super(), le(this, e, dr, fr, se, {})
+        super(), se(this, e, ar, ir, ee, {})
     }
 }
 
-function ht(n, e, t) {
+function ut(n, e, t) {
     const s = n.slice();
     return s[5] = e[t], s
 }
 
-function hr(n) {
+function cr(n) {
     let e, t, s;
     const r = [n[2] ?? {}];
     var l = n[1].component;
 
-    function o(a, i) {
+    function o(i, a) {
         let c = {
             $$slots: {
-                default: [_r]
+                default: [ur]
             },
             $$scope: {
-                ctx: a
+                ctx: i
             }
         };
-        if (i !== void 0 && i & 4) c = _e(r, [Pe(a[2] ?? {})]);
+        if (a !== void 0 && a & 4) c = de(r, [Ne(i[2] ?? {})]);
         else
-            for (let d = 0; d < r.length; d += 1) c = ue(c, r[d]);
+            for (let d = 0; d < r.length; d += 1) c = fe(c, r[d]);
         return {
             props: c
         }
     }
     return l && (e = Ae(l, o(n)), n[4](e)), {
         c() {
-            e && z(e.$$.fragment), t = N()
+            e && K(e.$$.fragment), t = z()
         },
-        l(a) {
-            e && J(e.$$.fragment, a), t = N()
+        l(i) {
+            e && W(e.$$.fragment, i), t = z()
         },
-        m(a, i) {
-            e && G(e, a, i), F(a, t, i), s = !0
+        m(i, a) {
+            e && q(e, i, a), T(i, t, a), s = !0
         },
-        p(a, i) {
-            if (i & 2 && l !== (l = a[1].component)) {
+        p(i, a) {
+            if (a & 2 && l !== (l = i[1].component)) {
                 if (e) {
                     Z();
                     const c = e;
-                    S(c.$$.fragment, 1, 0, () => {
-                        K(c, 1)
+                    F(c.$$.fragment, 1, 0, () => {
+                        U(c, 1)
                     }), x()
                 }
-                l ? (e = Ae(l, o(a, i)), a[4](e), z(e.$$.fragment), I(e.$$.fragment, 1), G(e, t.parentNode, t)) : e = null
+                l ? (e = Ae(l, o(i, a)), i[4](e), K(e.$$.fragment), E(e.$$.fragment, 1), q(e, t.parentNode, t)) : e = null
             } else if (l) {
-                const c = i & 4 ? _e(r, [Pe(a[2] ?? {})]) : {};
-                i & 258 && (c.$$scope = {
-                    dirty: i,
-                    ctx: a
+                const c = a & 4 ? de(r, [Ne(i[2] ?? {})]) : {};
+                a & 258 && (c.$$scope = {
+                    dirty: a,
+                    ctx: i
                 }), e.$set(c)
             }
         },
-        i(a) {
-            s || (e && I(e.$$.fragment, a), s = !0)
+        i(i) {
+            s || (e && E(e.$$.fragment, i), s = !0)
         },
-        o(a) {
-            e && S(e.$$.fragment, a), s = !1
+        o(i) {
+            e && F(e.$$.fragment, i), s = !1
         },
-        d(a) {
-            a && g(t), n[4](null), e && K(e, a)
+        d(i) {
+            i && _(t), n[4](null), e && U(e, i)
         }
     }
 }
 
-function pr(n) {
+function fr(n) {
     let e, t, s;
     const r = [n[2] ?? {}];
     var l = n[1].component;
 
-    function o(a, i) {
+    function o(i, a) {
         let c = {};
-        if (i !== void 0 && i & 4) c = _e(r, [Pe(a[2] ?? {})]);
+        if (a !== void 0 && a & 4) c = de(r, [Ne(i[2] ?? {})]);
         else
-            for (let d = 0; d < r.length; d += 1) c = ue(c, r[d]);
+            for (let d = 0; d < r.length; d += 1) c = fe(c, r[d]);
         return {
             props: c
         }
     }
     return l && (e = Ae(l, o(n)), n[3](e)), {
         c() {
-            e && z(e.$$.fragment), t = N()
+            e && K(e.$$.fragment), t = z()
         },
-        l(a) {
-            e && J(e.$$.fragment, a), t = N()
+        l(i) {
+            e && W(e.$$.fragment, i), t = z()
         },
-        m(a, i) {
-            e && G(e, a, i), F(a, t, i), s = !0
+        m(i, a) {
+            e && q(e, i, a), T(i, t, a), s = !0
         },
-        p(a, i) {
-            if (i & 2 && l !== (l = a[1].component)) {
+        p(i, a) {
+            if (a & 2 && l !== (l = i[1].component)) {
                 if (e) {
                     Z();
                     const c = e;
-                    S(c.$$.fragment, 1, 0, () => {
-                        K(c, 1)
+                    F(c.$$.fragment, 1, 0, () => {
+                        U(c, 1)
                     }), x()
                 }
-                l ? (e = Ae(l, o(a, i)), a[3](e), z(e.$$.fragment), I(e.$$.fragment, 1), G(e, t.parentNode, t)) : e = null
+                l ? (e = Ae(l, o(i, a)), i[3](e), K(e.$$.fragment), E(e.$$.fragment, 1), q(e, t.parentNode, t)) : e = null
             } else if (l) {
-                const c = i & 4 ? _e(r, [Pe(a[2] ?? {})]) : {};
+                const c = a & 4 ? de(r, [Ne(i[2] ?? {})]) : {};
                 e.$set(c)
             }
         },
-        i(a) {
-            s || (e && I(e.$$.fragment, a), s = !0)
+        i(i) {
+            s || (e && E(e.$$.fragment, i), s = !0)
         },
-        o(a) {
-            e && S(e.$$.fragment, a), s = !1
+        o(i) {
+            e && F(e.$$.fragment, i), s = !1
         },
-        d(a) {
-            a && g(t), n[3](null), e && K(e, a)
+        d(i) {
+            i && _(t), n[3](null), e && U(e, i)
         }
     }
 }
 
-function pt(n) {
+function dt(n) {
     let e, t;
-    return e = new Xe({
+    return e = new Ze({
         props: {
             of: n[5]
         }
     }), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(s) {
-            J(e.$$.fragment, s)
+            W(e.$$.fragment, s)
         },
         m(s, r) {
-            G(e, s, r), t = !0
+            q(e, s, r), t = !0
         },
         p(s, r) {
             const l = {};
             r & 2 && (l.of = s[5]), e.$set(l)
         },
         i(s) {
-            t || (I(e.$$.fragment, s), t = !0)
+            t || (E(e.$$.fragment, s), t = !0)
         },
         o(s) {
-            S(e.$$.fragment, s), t = !1
+            F(e.$$.fragment, s), t = !1
         },
         d(s) {
-            K(e, s)
+            U(e, s)
         }
     }
 }
 
-function _r(n) {
-    let e, t, s = ie(n[1].children),
+function ur(n) {
+    let e, t, s = oe(n[1].children),
         r = [];
-    for (let o = 0; o < s.length; o += 1) r[o] = pt(ht(n, s, o));
-    const l = o => S(r[o], 1, 1, () => {
+    for (let o = 0; o < s.length; o += 1) r[o] = dt(ut(n, s, o));
+    const l = o => F(r[o], 1, 1, () => {
         r[o] = null
     });
     return {
         c() {
             for (let o = 0; o < r.length; o += 1) r[o].c();
-            e = N()
+            e = z()
         },
         l(o) {
-            for (let a = 0; a < r.length; a += 1) r[a].l(o);
-            e = N()
+            for (let i = 0; i < r.length; i += 1) r[i].l(o);
+            e = z()
         },
-        m(o, a) {
-            for (let i = 0; i < r.length; i += 1) r[i] && r[i].m(o, a);
-            F(o, e, a), t = !0
-        },
-        p(o, a) {
-            if (a & 2) {
-                s = ie(o[1].children);
-                let i;
-                for (i = 0; i < s.length; i += 1) {
-                    const c = ht(o, s, i);
-                    r[i] ? (r[i].p(c, a), I(r[i], 1)) : (r[i] = pt(c), r[i].c(), I(r[i], 1), r[i].m(e.parentNode, e))
+        m(o, i) {
+            for (let a = 0; a < r.length; a += 1) r[a] && r[a].m(o, i);
+            T(o, e, i), t = !0
+        },
+        p(o, i) {
+            if (i & 2) {
+                s = oe(o[1].children);
+                let a;
+                for (a = 0; a < s.length; a += 1) {
+                    const c = ut(o, s, a);
+                    r[a] ? (r[a].p(c, i), E(r[a], 1)) : (r[a] = dt(c), r[a].c(), E(r[a], 1), r[a].m(e.parentNode, e))
                 }
-                for (Z(), i = s.length; i < r.length; i += 1) l(i);
+                for (Z(), a = s.length; a < r.length; a += 1) l(a);
                 x()
             }
         },
         i(o) {
             if (!t) {
-                for (let a = 0; a < s.length; a += 1) I(r[a]);
+                for (let i = 0; i < s.length; i += 1) E(r[i]);
                 t = !0
             }
         },
         o(o) {
             r = r.filter(Boolean);
-            for (let a = 0; a < r.length; a += 1) S(r[a]);
+            for (let i = 0; i < r.length; i += 1) F(r[i]);
             t = !1
         },
         d(o) {
-            o && g(e), Pt(r, o)
+            o && _(e), Vt(r, o)
         }
     }
 }
 
-function gr(n) {
+function dr(n) {
     let e, t, s, r;
-    const l = [pr, hr],
+    const l = [fr, cr],
         o = [];
 
-    function a(i, c) {
-        return i[1].children.length === 0 ? 0 : 1
+    function i(a, c) {
+        return a[1].children.length === 0 ? 0 : 1
     }
-    return e = a(n), t = o[e] = l[e](n), {
+    return e = i(n), t = o[e] = l[e](n), {
         c() {
-            t.c(), s = N()
+            t.c(), s = z()
         },
-        l(i) {
-            t.l(i), s = N()
+        l(a) {
+            t.l(a), s = z()
         },
-        m(i, c) {
-            o[e].m(i, c), F(i, s, c), r = !0
+        m(a, c) {
+            o[e].m(a, c), T(a, s, c), r = !0
         },
-        p(i, [c]) {
+        p(a, [c]) {
             let d = e;
-            e = a(i), e === d ? o[e].p(i, c) : (Z(), S(o[d], 1, 1, () => {
+            e = i(a), e === d ? o[e].p(a, c) : (Z(), F(o[d], 1, 1, () => {
                 o[d] = null
-            }), x(), t = o[e], t ? t.p(i, c) : (t = o[e] = l[e](i), t.c()), I(t, 1), t.m(s.parentNode, s))
+            }), x(), t = o[e], t ? t.p(a, c) : (t = o[e] = l[e](a), t.c()), E(t, 1), t.m(s.parentNode, s))
         },
-        i(i) {
-            r || (I(t), r = !0)
+        i(a) {
+            r || (E(t), r = !0)
         },
-        o(i) {
-            S(t), r = !1
+        o(a) {
+            F(t), r = !1
         },
-        d(i) {
-            i && g(s), o[e].d(i)
+        d(a) {
+            a && _(s), o[e].d(a)
         }
     }
 }
 
-function mr(n, e, t) {
+function hr(n, e, t) {
     let {
         instance: s = void 0
     } = e, {
         config: r
     } = e, {
         props: l = void 0
     } = e;
 
-    function o(i) {
-        je[i ? "unshift" : "push"](() => {
-            s = i, t(0, s)
+    function o(a) {
+        je[a ? "unshift" : "push"](() => {
+            s = a, t(0, s)
         })
     }
 
-    function a(i) {
-        je[i ? "unshift" : "push"](() => {
-            s = i, t(0, s)
+    function i(a) {
+        je[a ? "unshift" : "push"](() => {
+            s = a, t(0, s)
         })
     }
-    return n.$$set = i => {
-        "instance" in i && t(0, s = i.instance), "config" in i && t(1, r = i.config), "props" in i && t(2, l = i.props)
-    }, [s, r, l, o, a]
+    return n.$$set = a => {
+        "instance" in a && t(0, s = a.instance), "config" in a && t(1, r = a.config), "props" in a && t(2, l = a.props)
+    }, [s, r, l, o, i]
 }
-class Gt extends re {
+class Ut extends te {
     constructor(e) {
-        super(), le(this, e, mr, gr, se, {
+        super(), se(this, e, hr, dr, ee, {
             instance: 0,
             config: 1,
             props: 2
         })
     }
 }
-const Qe = n => (n == null ? void 0 : n.subscribe) instanceof Function,
-    br = Ie(void 0);
+const Ye = n => (n == null ? void 0 : n.subscribe) instanceof Function,
+    pr = Ie(void 0);
 
-function vr(n) {
+function _r(n) {
     let e, t, s;
 
     function r(o) {
         n[3](o)
     }
     let l = {
         config: n[0],
         props: n[0].props
     };
-    return n[1] !== void 0 && (l.instance = n[1]), e = new Gt({
+    return n[1] !== void 0 && (l.instance = n[1]), e = new Ut({
         props: l
-    }), je.push(() => We(e, "instance", r)), {
+    }), je.push(() => Xe(e, "instance", r)), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(o) {
-            J(e.$$.fragment, o)
+            W(e.$$.fragment, o)
         },
-        m(o, a) {
-            G(e, o, a), s = !0
+        m(o, i) {
+            q(e, o, i), s = !0
         },
-        p(o, a) {
-            const i = {};
-            a & 1 && (i.config = o[0]), a & 1 && (i.props = o[0].props), !t && a & 2 && (t = !0, i.instance = o[1], Je(() => t = !1)), e.$set(i)
+        p(o, i) {
+            const a = {};
+            i & 1 && (a.config = o[0]), i & 1 && (a.props = o[0].props), !t && i & 2 && (t = !0, a.instance = o[1], We(() => t = !1)), e.$set(a)
         },
         i(o) {
-            s || (I(e.$$.fragment, o), s = !0)
+            s || (E(e.$$.fragment, o), s = !0)
         },
         o(o) {
-            S(e.$$.fragment, o), s = !1
+            F(e.$$.fragment, o), s = !1
         },
         d(o) {
-            K(e, o)
+            U(e, o)
         }
     }
 }
 
-function $r(n) {
+function gr(n) {
     let e, t;
     return e = new Re({
         props: {
             props: n[0].props,
             $$slots: {
-                default: [wr, ({
+                default: [mr, ({
                     props: s
                 }) => ({
                     4: s
                 }), ({
                     props: s
                 }) => s ? 16 : 0]
             },
             $$scope: {
                 ctx: n
             }
         }
     }), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(s) {
-            J(e.$$.fragment, s)
+            W(e.$$.fragment, s)
         },
         m(s, r) {
-            G(e, s, r), t = !0
+            q(e, s, r), t = !0
         },
         p(s, r) {
             const l = {};
             r & 1 && (l.props = s[0].props), r & 51 && (l.$$scope = {
                 dirty: r,
                 ctx: s
             }), e.$set(l)
         },
         i(s) {
-            t || (I(e.$$.fragment, s), t = !0)
+            t || (E(e.$$.fragment, s), t = !0)
         },
         o(s) {
-            S(e.$$.fragment, s), t = !1
+            F(e.$$.fragment, s), t = !1
         },
         d(s) {
-            K(e, s)
+            U(e, s)
         }
     }
 }
 
-function wr(n) {
+function mr(n) {
     let e, t, s;
 
     function r(o) {
         n[2](o)
     }
     let l = {
         config: n[0],
         props: n[4]
     };
-    return n[1] !== void 0 && (l.instance = n[1]), e = new Gt({
+    return n[1] !== void 0 && (l.instance = n[1]), e = new Ut({
         props: l
-    }), je.push(() => We(e, "instance", r)), {
+    }), je.push(() => Xe(e, "instance", r)), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(o) {
-            J(e.$$.fragment, o)
+            W(e.$$.fragment, o)
         },
-        m(o, a) {
-            G(e, o, a), s = !0
+        m(o, i) {
+            q(e, o, i), s = !0
         },
-        p(o, a) {
-            const i = {};
-            a & 1 && (i.config = o[0]), a & 16 && (i.props = o[4]), !t && a & 2 && (t = !0, i.instance = o[1], Je(() => t = !1)), e.$set(i)
+        p(o, i) {
+            const a = {};
+            i & 1 && (a.config = o[0]), i & 16 && (a.props = o[4]), !t && i & 2 && (t = !0, a.instance = o[1], We(() => t = !1)), e.$set(a)
         },
         i(o) {
-            s || (I(e.$$.fragment, o), s = !0)
+            s || (E(e.$$.fragment, o), s = !0)
         },
         o(o) {
-            S(e.$$.fragment, o), s = !1
+            F(e.$$.fragment, o), s = !1
         },
         d(o) {
-            K(e, o)
+            U(e, o)
         }
     }
 }
 
-function kr(n) {
+function br(n) {
     let e, t, s, r, l;
-    const o = [$r, vr],
-        a = [];
+    const o = [gr, _r],
+        i = [];
 
-    function i(c, d) {
-        return d & 1 && (e = null), e == null && (e = !!Qe(c[0].props)), e ? 0 : 1
+    function a(c, d) {
+        return d & 1 && (e = null), e == null && (e = !!Ye(c[0].props)), e ? 0 : 1
     }
-    return t = i(n, -1), s = a[t] = o[t](n), {
+    return t = a(n, -1), s = i[t] = o[t](n), {
         c() {
-            s.c(), r = N()
+            s.c(), r = z()
         },
         l(c) {
-            s.l(c), r = N()
+            s.l(c), r = z()
         },
         m(c, d) {
-            a[t].m(c, d), F(c, r, d), l = !0
+            i[t].m(c, d), T(c, r, d), l = !0
         },
         p(c, [d]) {
-            let w = t;
-            t = i(c, d), t === w ? a[t].p(c, d) : (Z(), S(a[w], 1, 1, () => {
-                a[w] = null
-            }), x(), s = a[t], s ? s.p(c, d) : (s = a[t] = o[t](c), s.c()), I(s, 1), s.m(r.parentNode, r))
+            let $ = t;
+            t = a(c, d), t === $ ? i[t].p(c, d) : (Z(), F(i[$], 1, 1, () => {
+                i[$] = null
+            }), x(), s = i[t], s ? s.p(c, d) : (s = i[t] = o[t](c), s.c()), E(s, 1), s.m(r.parentNode, r))
         },
         i(c) {
-            l || (I(s), l = !0)
+            l || (E(s), l = !0)
         },
         o(c) {
-            S(s), l = !1
+            F(s), l = !1
         },
         d(c) {
-            c && g(r), a[t].d(c)
+            c && _(r), i[t].d(c)
         }
     }
 }
 
-function yr(n, e, t) {
+function vr(n, e, t) {
     let {
         config: s
     } = e, r;
-    ls(function() {
-        return s.eventHandlers.forEach(([i, c]) => {
-                const d = r.$$.callbacks[i] ?? [];
-                d.push(c), t(1, r.$$.callbacks[i] = d, r)
+    os(function() {
+        return s.eventHandlers.forEach(([a, c]) => {
+                const d = r.$$.callbacks[a] ?? [];
+                d.push(c), t(1, r.$$.callbacks[a] = d, r)
             }),
             function() {
                 s.eventHandlers.forEach(([c, d]) => {
-                    const w = r.$$.callbacks[c],
-                        y = w.findIndex(m => m === d);
-                    w.splice(y, 1)
+                    const $ = r.$$.callbacks[c],
+                        k = $.findIndex(g => g === d);
+                    $.splice(k, 1)
                 })
             }
     });
 
-    function l(a) {
-        r = a, t(1, r)
+    function l(i) {
+        r = i, t(1, r)
     }
 
-    function o(a) {
-        r = a, t(1, r)
+    function o(i) {
+        r = i, t(1, r)
     }
-    return n.$$set = a => {
-        "config" in a && t(0, s = a.config)
+    return n.$$set = i => {
+        "config" in i && t(0, s = i.config)
     }, [s, r, l, o]
 }
-class Er extends re {
+class $r extends te {
     constructor(e) {
-        super(), le(this, e, yr, kr, se, {
+        super(), se(this, e, vr, br, ee, {
             config: 0
         })
     }
 }
 
-function Cr(n) {
+function wr(n) {
     let e, t;
-    return e = new Er({
+    return e = new $r({
         props: {
             config: n[0]
         }
     }), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(s) {
-            J(e.$$.fragment, s)
+            W(e.$$.fragment, s)
         },
         m(s, r) {
-            G(e, s, r), t = !0
+            q(e, s, r), t = !0
         },
         p(s, r) {
             const l = {};
             r & 1 && (l.config = s[0]), e.$set(l)
         },
         i(s) {
-            t || (I(e.$$.fragment, s), t = !0)
+            t || (E(e.$$.fragment, s), t = !0)
         },
         o(s) {
-            S(e.$$.fragment, s), t = !1
+            F(e.$$.fragment, s), t = !1
         },
         d(s) {
-            K(e, s)
+            U(e, s)
         }
     }
 }
 
-function Ir(n) {
+function kr(n) {
     let e;
     return {
         c() {
-            e = ne(n[0])
+            e = re(n[0])
         },
         l(t) {
-            e = oe(t, n[0])
+            e = le(t, n[0])
         },
         m(t, s) {
-            F(t, e, s)
+            T(t, e, s)
         },
         p(t, s) {
-            s & 1 && be(e, t[0])
+            s & 1 && me(e, t[0])
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(t) {
-            t && g(e)
+            t && _(e)
         }
     }
 }
 
-function Tr(n) {
+function yr(n) {
     let e;
     return {
         c() {
-            e = ne(n[1])
+            e = re(n[1])
         },
         l(t) {
-            e = oe(t, n[1])
+            e = le(t, n[1])
         },
         m(t, s) {
-            F(t, e, s)
+            T(t, e, s)
         },
         p(t, s) {
-            s & 2 && be(e, t[1])
+            s & 2 && me(e, t[1])
         },
-        i: q,
-        o: q,
+        i: J,
+        o: J,
         d(t) {
-            t && g(e)
+            t && _(e)
         }
     }
 }
 
-function Dr(n) {
+function Er(n) {
     let e, t, s, r, l;
-    const o = [Tr, Ir, Cr],
-        a = [];
+    const o = [yr, kr, wr],
+        i = [];
 
-    function i(c, d) {
-        return d & 1 && (e = null), e == null && (e = !!Qe(c[0])), e ? 0 : typeof c[0] != "object" ? 1 : 2
+    function a(c, d) {
+        return d & 1 && (e = null), e == null && (e = !!Ye(c[0])), e ? 0 : typeof c[0] != "object" ? 1 : 2
     }
-    return t = i(n, -1), s = a[t] = o[t](n), {
+    return t = a(n, -1), s = i[t] = o[t](n), {
         c() {
-            s.c(), r = N()
+            s.c(), r = z()
         },
         l(c) {
-            s.l(c), r = N()
+            s.l(c), r = z()
         },
         m(c, d) {
-            a[t].m(c, d), F(c, r, d), l = !0
+            i[t].m(c, d), T(c, r, d), l = !0
         },
         p(c, [d]) {
-            let w = t;
-            t = i(c, d), t === w ? a[t].p(c, d) : (Z(), S(a[w], 1, 1, () => {
-                a[w] = null
-            }), x(), s = a[t], s ? s.p(c, d) : (s = a[t] = o[t](c), s.c()), I(s, 1), s.m(r.parentNode, r))
+            let $ = t;
+            t = a(c, d), t === $ ? i[t].p(c, d) : (Z(), F(i[$], 1, 1, () => {
+                i[$] = null
+            }), x(), s = i[t], s ? s.p(c, d) : (s = i[t] = o[t](c), s.c()), E(s, 1), s.m(r.parentNode, r))
         },
         i(c) {
-            l || (I(s), l = !0)
+            l || (E(s), l = !0)
         },
         o(c) {
-            S(s), l = !1
+            F(s), l = !1
         },
         d(c) {
-            c && g(r), a[t].d(c)
+            c && _(r), i[t].d(c)
         }
     }
 }
 
-function Fr(n, e, t) {
+function Cr(n, e, t) {
     let s, {
         of: r
     } = e;
-    const l = Qe(r) ? r : br;
-    return ye(n, l, o => t(1, s = o)), n.$$set = o => {
+    const l = Ye(r) ? r : pr;
+    return Ee(n, l, o => t(1, s = o)), n.$$set = o => {
         "of" in o && t(0, r = o.of)
     }, [r, s, l]
 }
-class Xe extends re {
+class Ze extends te {
     constructor(e) {
-        super(), le(this, e, Fr, Dr, se, {
+        super(), se(this, e, Cr, Er, ee, {
             of: 0
         })
     }
 }
-class Sr {
+class Ir {
     constructor(e, t) {
-        D(this, "component");
-        D(this, "props");
-        D(this, "eventHandlers", []);
-        D(this, "children", []);
+        I(this, "component");
+        I(this, "props");
+        I(this, "eventHandlers", []);
+        I(this, "children", []);
         this.component = e, this.props = t
     }
     on(e, t) {
         return this.eventHandlers.push([e, t]), this
     }
     slot(...e) {
         return this.children = e, this
     }
 }
 
-function jr(n, e) {
-    return new Sr(n, e)
+function Ve(n, e) {
+    return new Ir(n, e)
 }
-class Kt {
+class Jt {
     constructor({
         header: e,
         footer: t,
         height: s,
         plugins: r
     }) {
-        D(this, "header");
-        D(this, "footer");
-        D(this, "height");
-        D(this, "plugins");
+        I(this, "header");
+        I(this, "footer");
+        I(this, "height");
+        I(this, "plugins");
         this.header = e, this.footer = t, this.height = s, this.plugins = r
     }
     isFlat() {
         return "__flat" in this
     }
     isData() {
         return "__data" in this
@@ -1580,163 +1297,163 @@
     isDisplay() {
         return "__display" in this
     }
     isGroup() {
         return "__group" in this
     }
 }
-class qt extends Kt {
+class Wt extends Jt {
     constructor({
         header: t,
         footer: s,
         plugins: r,
         id: l
     }) {
         super({
             header: t,
             footer: s,
             plugins: r,
             height: 1
         });
-        D(this, "__flat", !0);
-        D(this, "id");
+        I(this, "__flat", !0);
+        I(this, "id");
         this.id = l ?? String(t)
     }
 }
-class Ar extends qt {
+class Tr extends Wt {
     constructor({
         header: t,
         footer: s,
         plugins: r,
         cell: l,
         accessor: o,
-        id: a
+        id: i
     }) {
         super({
             header: t,
             footer: s,
             plugins: r,
             id: "Initialization not complete"
         });
-        D(this, "__data", !0);
-        D(this, "cell");
-        D(this, "accessorKey");
-        D(this, "accessorFn");
-        if (this.cell = l, o instanceof Function ? this.accessorFn = o : this.accessorKey = o, a === void 0 && this.accessorKey === void 0 && t === void 0) throw new Error("A column id, string accessor, or header is required");
-        const i = typeof this.accessorKey == "string" ? this.accessorKey : null;
-        this.id = a ?? i ?? String(t)
+        I(this, "__data", !0);
+        I(this, "cell");
+        I(this, "accessorKey");
+        I(this, "accessorFn");
+        if (this.cell = l, o instanceof Function ? this.accessorFn = o : this.accessorKey = o, i === void 0 && this.accessorKey === void 0 && t === void 0) throw new Error("A column id, string accessor, or header is required");
+        const a = typeof this.accessorKey == "string" ? this.accessorKey : null;
+        this.id = i ?? a ?? String(t)
     }
     getValue(t) {
         if (this.accessorFn !== void 0) return this.accessorFn(t);
         if (this.accessorKey !== void 0) return t[this.accessorKey]
     }
 }
-class Mr extends qt {
+class Dr extends Wt {
     constructor({
         header: t,
         footer: s,
         plugins: r,
         id: l,
         cell: o,
-        data: a
+        data: i
     }) {
         super({
             header: t,
             footer: s,
             plugins: r,
             id: l
         });
-        D(this, "__display", !0);
-        D(this, "cell");
-        D(this, "data");
-        this.cell = o, this.data = a
+        I(this, "__display", !0);
+        I(this, "cell");
+        I(this, "data");
+        this.cell = o, this.data = i
     }
 }
-class Rr extends Kt {
+class Sr extends Jt {
     constructor({
         header: t,
         footer: s,
         columns: r,
         plugins: l
     }) {
-        const o = Math.max(...r.map(a => a.height)) + 1;
+        const o = Math.max(...r.map(i => i.height)) + 1;
         super({
             header: t,
             footer: s,
             height: o,
             plugins: l
         });
-        D(this, "__group", !0);
-        D(this, "columns");
-        D(this, "ids");
-        this.columns = r, this.ids = Ut(r)
+        I(this, "__group", !0);
+        I(this, "columns");
+        I(this, "ids");
+        this.columns = r, this.ids = Qt(r)
     }
 }
-const Ut = n => n.flatMap(e => e.isFlat() ? [e.id] : e.isGroup() ? e.ids : []),
-    Jt = n => n.flatMap(e => e.isFlat() ? [e] : e.isGroup() ? Jt(e.columns) : []),
-    Br = n => {
+const Qt = n => n.flatMap(e => e.isFlat() ? [e.id] : e.isGroup() ? e.ids : []),
+    Xt = n => n.flatMap(e => e.isFlat() ? [e] : e.isGroup() ? Xt(e.columns) : []),
+    Fr = n => {
         const e = new Map;
         return n.forEach(t => {
             e.set(t, (e.get(t) ?? 0) + 1)
         }), e
     },
-    Hr = n => Array.from(Br(n).entries()).filter(([, e]) => e !== 1).map(([e]) => e),
-    Or = n => Object.entries(n).map(([e, t]) => `${e}:${t}`).join(";"),
-    Pr = (n, e) => n.style === void 0 && e.style === void 0 ? {
+    jr = n => Array.from(Fr(n).entries()).filter(([, e]) => e !== 1).map(([e]) => e),
+    Ar = n => Object.entries(n).map(([e, t]) => `${e}:${t}`).join(";"),
+    Mr = (n, e) => n.style === void 0 && e.style === void 0 ? {
         ...n,
         ...e
     } : {
         ...n,
         ...e,
         style: {
             ...typeof n.style == "object" ? n.style : {},
             ...typeof e.style == "object" ? e.style : {}
         }
     },
-    He = n => n.style === void 0 || typeof n.style != "object" ? n : {
+    Oe = n => n.style === void 0 || typeof n.style != "object" ? n : {
         ...n,
-        style: Or(n.style)
+        style: Ar(n.style)
     };
-class Ve {
+class Ge {
     constructor({
         id: e
     }) {
-        D(this, "id");
-        D(this, "attrsForName", {});
-        D(this, "propsForName", {});
-        D(this, "state");
+        I(this, "id");
+        I(this, "attrsForName", {});
+        I(this, "propsForName", {});
+        I(this, "state");
         this.id = e
     }
     attrs() {
         return Y(Object.values(this.attrsForName), e => {
             let t = {};
             return e.forEach(s => {
-                t = Pr(t, s)
-            }), He(t)
+                t = Mr(t, s)
+            }), Oe(t)
         })
     }
     props() {
-        return zt(this.propsForName)
+        return qt(this.propsForName)
     }
     injectState(e) {
         this.state = e
     }
     applyHook(e, t) {
         t.props !== void 0 && (this.propsForName[e] = t.props), t.attrs !== void 0 && (this.attrsForName[e] = t.attrs)
     }
 }
-class Wt extends Ve {
+class Yt extends Ge {
     constructor({
         id: t,
         row: s
     }) {
         super({
             id: t
         });
-        D(this, "row");
+        I(this, "row");
         this.row = s
     }
     attrs() {
         return Y(super.attrs(), t => ({
             ...t,
             role: "cell"
         }))
@@ -1750,89 +1467,89 @@
     isData() {
         return "__data" in this
     }
     isDisplay() {
         return "__display" in this
     }
 }
-class Ye extends Wt {
+class xe extends Yt {
     constructor({
         row: t,
         column: s,
         label: r,
         value: l
     }) {
         super({
             id: s.id,
             row: t
         });
-        D(this, "__data", !0);
-        D(this, "column");
-        D(this, "label");
-        D(this, "value");
+        I(this, "__data", !0);
+        I(this, "column");
+        I(this, "label");
+        I(this, "value");
         this.column = s, this.label = r, this.value = l
     }
     render() {
         if (this.label === void 0) return `${this.value}`;
         if (this.state === void 0) throw new Error("Missing `state` reference");
         return this.label(this, this.state)
     }
     clone() {
-        return new Ye({
+        return new xe({
             row: this.row,
             column: this.column,
             label: this.label,
             value: this.value
         })
     }
 }
-class Ze extends Wt {
+class et extends Yt {
     constructor({
         row: t,
         column: s,
         label: r
     }) {
         super({
             id: s.id,
             row: t
         });
-        D(this, "__display", !0);
-        D(this, "column");
-        D(this, "label");
+        I(this, "__display", !0);
+        I(this, "column");
+        I(this, "label");
         this.column = s, this.label = r
     }
     render() {
         if (this.state === void 0) throw new Error("Missing `state` reference");
         return this.label(this, this.state)
     }
     clone() {
-        return new Ze({
+        return new et({
             row: this.row,
             column: this.column,
             label: this.label
         })
     }
 }
-const ke = n => n !== void 0;
-class Lr extends Ve {
+const ye = n => n !== void 0;
+class Rr extends Ge {
     constructor({
         id: t,
         cells: s,
         cellForId: r,
         depth: l = 0,
         parentRow: o
     }) {
         super({
             id: t
         });
-        D(this, "cells");
-        D(this, "cellForId");
-        D(this, "depth");
-        D(this, "parentRow");
-        D(this, "subRows");
+        I(this, "cells");
+        I(this, "cellForId");
+        I(this, "depth");
+        I(this, "parentRow");
+        I(this, "subRows");
         this.cells = s, this.cellForId = r, this.depth = l, this.parentRow = o
     }
     attrs() {
         return Y(super.attrs(), t => ({
             ...t,
             role: "row"
         }))
@@ -1840,139 +1557,139 @@
     isData() {
         return "__data" in this
     }
     isDisplay() {
         return "__display" in this
     }
 }
-class xe extends Lr {
+class tt extends Rr {
     constructor({
         id: t,
         dataId: s,
         original: r,
         cells: l,
         cellForId: o,
-        depth: a = 0,
-        parentRow: i
+        depth: i = 0,
+        parentRow: a
     }) {
         super({
             id: t,
             cells: l,
             cellForId: o,
-            depth: a,
-            parentRow: i
+            depth: i,
+            parentRow: a
         });
-        D(this, "__data", !0);
-        D(this, "dataId");
-        D(this, "original");
+        I(this, "__data", !0);
+        I(this, "dataId");
+        I(this, "original");
         this.dataId = s, this.original = r
     }
     clone({
         includeCells: t = !1,
         includeSubRows: s = !1
     } = {}) {
         var l;
-        const r = new xe({
+        const r = new tt({
             id: this.id,
             dataId: this.dataId,
             cellForId: this.cellForId,
             cells: this.cells,
             original: this.original,
             depth: this.depth
         });
         if (t) {
-            const o = Object.fromEntries(Object.entries(r.cellForId).map(([i, c]) => {
+            const o = Object.fromEntries(Object.entries(r.cellForId).map(([a, c]) => {
                     const d = c.clone();
-                    return d.row = r, [i, d]
+                    return d.row = r, [a, d]
                 })),
-                a = r.cells.map(({
-                    id: i
-                }) => o[i]);
-            r.cellForId = o, r.cells = a
+                i = r.cells.map(({
+                    id: a
+                }) => o[a]);
+            r.cellForId = o, r.cells = i
         }
         if (s) {
-            const o = (l = this.subRows) == null ? void 0 : l.map(a => a.clone({
+            const o = (l = this.subRows) == null ? void 0 : l.map(i => i.clone({
                 includeCells: t,
                 includeSubRows: s
             }));
             r.subRows = o
         } else r.subRows = this.subRows;
         return r
     }
 }
-const Nr = (n, e, {
+const Br = (n, e, {
         rowDataId: t
     } = {}) => {
         const s = n.map((r, l) => {
             const o = l.toString();
-            return new xe({
+            return new tt({
                 id: o,
                 dataId: t !== void 0 ? t(r, l) : o,
                 original: r,
                 cells: [],
                 cellForId: {}
             })
         });
         return n.forEach((r, l) => {
-            const o = e.map(a => {
-                if (a.isData()) {
-                    const i = a,
-                        c = i.getValue(r);
-                    return new Ye({
+            const o = e.map(i => {
+                if (i.isData()) {
+                    const a = i,
+                        c = a.getValue(r);
+                    return new xe({
                         row: s[l],
-                        column: i,
-                        label: a.cell,
+                        column: a,
+                        label: i.cell,
                         value: c
                     })
                 }
-                if (a.isDisplay()) {
-                    const i = a;
-                    return new Ze({
+                if (i.isDisplay()) {
+                    const a = i;
+                    return new et({
                         row: s[l],
-                        column: i,
-                        label: a.cell
+                        column: a,
+                        label: i.cell
                     })
                 }
                 throw new Error("Unrecognized `FlatColumn` implementation")
             });
-            s[l].cells = o, e.forEach((a, i) => {
-                s[l].cellForId[a.id] = o[i]
+            s[l].cells = o, e.forEach((i, a) => {
+                s[l].cellForId[i.id] = o[a]
             })
         }), s
     },
-    Vr = (n, e) => {
+    Or = (n, e) => {
         const t = n.map(s => {
             const r = s.clone();
             return r.cells = [], r.cellForId = {}, r
         });
         return n.length === 0 || e.length === 0 ? n : (n.forEach((s, r) => {
-            const l = s.cells.map(a => {
-                    const i = a.clone();
-                    return i.row = t[r], i
+            const l = s.cells.map(i => {
+                    const a = i.clone();
+                    return a.row = t[r], a
                 }),
-                o = e.map(a => l.find(i => i.id === a)).filter(ke);
-            t[r].cells = o, l.forEach(a => {
-                t[r].cellForId[a.id] = a
+                o = e.map(i => l.find(a => a.id === i)).filter(ye);
+            t[r].cells = o, l.forEach(i => {
+                t[r].cellForId[i.id] = i
             })
         }), t)
     },
-    Qt = " ";
-class Xt extends Ve {
+    Zt = " ";
+class xt extends Ge {
     constructor({
         id: t,
         label: s,
         colspan: r,
         colstart: l
     }) {
         super({
             id: t
         });
-        D(this, "label");
-        D(this, "colspan");
-        D(this, "colstart");
+        I(this, "label");
+        I(this, "colspan");
+        I(this, "colstart");
         this.label = s, this.colspan = r, this.colstart = l
     }
     render() {
         if (this.label instanceof Function) {
             if (this.state === void 0) throw new Error("Missing `state` reference");
             return this.label(this, this.state)
         }
@@ -1997,278 +1714,278 @@
     isGroup() {
         return "__group" in this
     }
     isGroupDisplay() {
         return "__group" in this && "__display" in this
     }
 }
-class ze extends Xt {
+class Ke extends xt {
     constructor({
         id: t,
         label: s,
         colstart: r
     }) {
         super({
             id: t,
             label: s,
             colspan: 1,
             colstart: r
         });
-        D(this, "__flat", !0)
+        I(this, "__flat", !0)
     }
     clone() {
-        return new ze({
+        return new Ke({
             id: this.id,
             label: this.label,
             colstart: this.colstart
         })
     }
 }
-class et extends ze {
+class st extends Ke {
     constructor({
         id: t,
         label: s,
         accessorKey: r,
         accessorFn: l,
         colstart: o
     }) {
         super({
             id: t,
             label: s,
             colstart: o
         });
-        D(this, "__data", !0);
-        D(this, "accessorKey");
-        D(this, "accessorFn");
+        I(this, "__data", !0);
+        I(this, "accessorKey");
+        I(this, "accessorFn");
         this.accessorKey = r, this.accessorFn = l
     }
     clone() {
-        return new et({
+        return new st({
             id: this.id,
             label: this.label,
             accessorFn: this.accessorFn,
             accessorKey: this.accessorKey,
             colstart: this.colstart
         })
     }
 }
-class Ge extends ze {
+class qe extends Ke {
     constructor({
         id: t,
-        label: s = Qt,
+        label: s = Zt,
         colstart: r
     }) {
         super({
             id: t,
             label: s,
             colstart: r
         });
-        D(this, "__display", !0)
+        I(this, "__display", !0)
     }
     clone() {
-        return new Ge({
+        return new qe({
             id: this.id,
             label: this.label,
             colstart: this.colstart
         })
     }
 }
-class Ke extends Xt {
+class Ue extends xt {
     constructor({
         label: t,
         ids: s,
         allIds: r,
         colspan: l,
         colstart: o
     }) {
         super({
             id: `[${s.join(",")}]`,
             label: t,
             colspan: l,
             colstart: o
         });
-        D(this, "__group", !0);
-        D(this, "ids");
-        D(this, "allId");
-        D(this, "allIds");
+        I(this, "__group", !0);
+        I(this, "ids");
+        I(this, "allId");
+        I(this, "allIds");
         this.ids = s, this.allId = `[${r.join(",")}]`, this.allIds = r
     }
     setIds(t) {
         this.ids = t, this.id = `[${this.ids.join(",")}]`
     }
     pushId(t) {
         this.ids = [...this.ids, t], this.id = `[${this.ids.join(",")}]`
     }
     clone() {
-        return new Ke({
+        return new Ue({
             label: this.label,
             ids: this.ids,
             allIds: this.allIds,
             colspan: this.colspan,
             colstart: this.colstart
         })
     }
 }
-class tt extends Ke {
+class rt extends Ue {
     constructor({
-        label: t = Qt,
+        label: t = Zt,
         ids: s,
         allIds: r,
         colspan: l = 1,
         colstart: o
     }) {
         super({
             label: t,
             ids: s,
             allIds: r,
             colspan: l,
             colstart: o
         });
-        D(this, "__display", !0)
+        I(this, "__display", !0)
     }
     clone() {
-        return new tt({
+        return new rt({
             label: this.label,
             ids: this.ids,
             allIds: this.allIds,
             colspan: this.colspan,
             colstart: this.colstart
         })
     }
 }
-const zr = n => n.reduce((e, t) => e + t, 0),
-    Yt = (n, e) => {
+const Hr = n => n.reduce((e, t) => e + t, 0),
+    es = (n, e) => {
         const t = [];
         for (let s = 0; s < e; s++) t.push(Array(n).fill(null));
         return t
     },
-    _t = n => {
+    ht = n => {
         const e = n.length;
         if (e === 0) return n;
         const t = n[0].length,
-            s = Yt(e, t);
+            s = es(e, t);
         for (let r = 0; r < t; r++)
             for (let l = 0; l < e; l++) s[r][l] = n[l][r];
         return s
     };
-class st extends Ve {
+class lt extends Ge {
     constructor({
         id: t,
         cells: s
     }) {
         super({
             id: t
         });
-        D(this, "cells");
+        I(this, "cells");
         this.cells = s
     }
     attrs() {
         return Y(super.attrs(), t => ({
             ...t,
             role: "row"
         }))
     }
     clone() {
-        return new st({
+        return new lt({
             id: this.id,
             cells: this.cells
         })
     }
 }
-const Gr = (n, e = []) => {
-        const t = Kr(n);
-        let s = _t(t);
-        return s = qr(s, e), Ur(s), Jr(_t(s))
+const Nr = (n, e = []) => {
+        const t = Pr(n);
+        let s = ht(t);
+        return s = Lr(s, e), Vr(s), zr(ht(s))
     },
-    Kr = n => {
-        const e = zr(n.map(l => l.isGroup() ? l.ids.length : 1)),
+    Pr = n => {
+        const e = Hr(n.map(l => l.isGroup() ? l.ids.length : 1)),
             t = Math.max(...n.map(l => l.height)),
-            s = Yt(e, t);
+            s = es(e, t);
         let r = 0;
         return n.forEach(l => {
             const o = t - l.height;
-            Zt(s, l, o, r), r += l.isGroup() ? l.ids.length : 1
-        }), s.map((l, o) => l.map((a, i) => {
+            ts(s, l, o, r), r += l.isGroup() ? l.ids.length : 1
+        }), s.map((l, o) => l.map((i, a) => {
             var d;
-            if (a !== null) return a;
-            if (o === t - 1) return new Ge({
-                id: i.toString(),
-                colstart: i
+            if (i !== null) return i;
+            if (o === t - 1) return new qe({
+                id: a.toString(),
+                colstart: a
             });
-            const c = ((d = s[t - 1][i]) == null ? void 0 : d.id) ?? i.toString();
-            return new tt({
+            const c = ((d = s[t - 1][a]) == null ? void 0 : d.id) ?? a.toString();
+            return new rt({
                 ids: [],
                 allIds: [c],
-                colstart: i
+                colstart: a
             })
         }))
     },
-    Zt = (n, e, t, s) => {
+    ts = (n, e, t, s) => {
         if (e.isData()) {
-            n[n.length - 1][s] = new et({
+            n[n.length - 1][s] = new st({
                 label: e.header,
                 accessorFn: e.accessorFn,
                 accessorKey: e.accessorKey,
                 id: e.id,
                 colstart: s
             });
             return
         }
         if (e.isDisplay()) {
-            n[n.length - 1][s] = new Ge({
+            n[n.length - 1][s] = new qe({
                 id: e.id,
                 label: e.header,
                 colstart: s
             });
             return
         }
         if (e.isGroup()) {
-            for (let l = 0; l < e.ids.length; l++) n[t][s + l] = new Ke({
+            for (let l = 0; l < e.ids.length; l++) n[t][s + l] = new Ue({
                 label: e.header,
                 colspan: 1,
                 allIds: e.ids,
                 ids: [],
                 colstart: s
             });
             let r = 0;
             e.columns.forEach(l => {
-                Zt(n, l, t + 1, s + r), r += l.isGroup() ? l.ids.length : 1
+                ts(n, l, t + 1, s + r), r += l.isGroup() ? l.ids.length : 1
             });
             return
         }
     },
-    qr = (n, e) => {
+    Lr = (n, e) => {
         if (e.length === 0) return n;
         const t = [];
         return e.forEach((s, r) => {
             const l = n.find(o => {
-                const a = o[o.length - 1];
-                if (!a.isFlat()) throw new Error("The last element of each column must be a `FlatHeaderCell`");
-                return a.id === s
+                const i = o[o.length - 1];
+                if (!i.isFlat()) throw new Error("The last element of each column must be a `FlatHeaderCell`");
+                return i.id === s
             });
             l !== void 0 && t.push(l.map(o => {
-                const a = o.clone();
-                return a.colstart = r, a
+                const i = o.clone();
+                return i.colstart = r, i
             }))
         }), t
     },
-    Ur = n => {
+    Vr = n => {
         n.forEach(e => {
             const t = e[e.length - 1];
             if (!t.isFlat()) throw new Error("The last element of each column must be a `FlatHeaderCell`");
             e.forEach(s => {
                 s.isGroup() && s.pushId(t.id)
             })
         })
     },
-    Jr = n => n.map((e, t) => new st({
+    zr = n => n.map((e, t) => new lt({
         id: t.toString(),
-        cells: Wr(e)
+        cells: Gr(e)
     })),
-    Wr = n => {
+    Gr = n => {
         if (n.length === 0) return n;
         const e = [];
         let t = 0,
             s = 1;
         for (; t < n.length;) {
             const r = n[t].clone();
             if (!r.isGroup()) {
@@ -2282,1721 +1999,2030 @@
                 if (!o.isGroup() || r.allId !== o.allId) break;
                 l.push(...o.ids), s++
             }
             r.setIds(l), r.colspan = s - t, e.push(r), t = s
         }
         return e
     },
-    Qr = (n, e, {
+    Kr = (n, e, {
         rowDataId: t
     } = {}) => {
         const {
             data: s,
             plugins: r
-        } = n, l = Jt(e), o = Ie(l), a = Y([s, o], ([T, B]) => Nr(T, B, {
+        } = n, l = Xt(e), o = Ie(l), i = Y([s, o], ([C, H]) => Br(C, H, {
             rowDataId: t
-        })), i = me([]), c = me(), d = me([]), w = me([]), y = me({
+        })), a = ge([]), c = ge(), d = ge([]), $ = ge([]), k = ge({
             role: "table"
-        }), m = me({}), b = me({
+        }), g = ge({}), m = ge({
             role: "rowgroup"
-        }), f = {
+        }), u = {
             data: s,
             columns: e,
             flatColumns: l,
-            tableAttrs: y,
-            tableHeadAttrs: m,
-            tableBodyAttrs: b,
-            visibleColumns: i,
+            tableAttrs: k,
+            tableHeadAttrs: g,
+            tableBodyAttrs: m,
+            visibleColumns: a,
             headerRows: c,
-            originalRows: a,
+            originalRows: i,
             rows: d,
-            pageRows: w
-        }, u = Object.fromEntries(Object.entries(r).map(([T, B]) => {
-            const O = Object.fromEntries(l.map(Q => {
-                var fe;
-                const X = (fe = Q.plugins) == null ? void 0 : fe[T];
+            pageRows: $
+        }, f = Object.fromEntries(Object.entries(r).map(([C, H]) => {
+            const P = Object.fromEntries(l.map(Q => {
+                var ue;
+                const X = (ue = Q.plugins) == null ? void 0 : ue[C];
                 if (X !== void 0) return [Q.id, X]
-            }).filter(ke));
-            return [T, B({
-                pluginName: T,
-                tableState: f,
-                columnOptions: O
+            }).filter(ye));
+            return [C, H({
+                pluginName: C,
+                tableState: u,
+                columnOptions: P
             })]
-        })), h = Object.fromEntries(Object.entries(u).map(([T, B]) => [T, B.pluginState])), p = {
+        })), h = Object.fromEntries(Object.entries(f).map(([C, H]) => [C, H.pluginState])), p = {
             data: s,
             columns: e,
             flatColumns: l,
-            tableAttrs: y,
-            tableHeadAttrs: m,
-            tableBodyAttrs: b,
-            visibleColumns: i,
+            tableAttrs: k,
+            tableHeadAttrs: g,
+            tableBodyAttrs: m,
+            visibleColumns: a,
             headerRows: c,
-            originalRows: a,
+            originalRows: i,
             rows: d,
-            pageRows: w,
+            pageRows: $,
             pluginStates: h
-        }, v = Object.values(u).map(T => T.deriveTableAttrs).filter(ke);
-        let R = Ie({
+        }, b = Object.values(f).map(C => C.deriveTableAttrs).filter(ye);
+        let B = Ie({
             role: "table"
         });
-        v.forEach(T => {
-            R = T(R)
+        b.forEach(C => {
+            B = C(B)
         });
-        const ee = Y(R, T => {
-                const B = He(T);
-                return y.set(B), B
+        const S = Y(B, C => {
+                const H = Oe(C);
+                return k.set(H), H
             }),
-            V = Object.values(u).map(T => T.deriveTableBodyAttrs).filter(ke);
-        let k = Ie({});
-        V.forEach(T => {
-            k = T(k)
-        });
-        const U = Y(k, T => {
-                const B = He(T);
-                return m.set(B), B
+            O = Object.values(f).map(C => C.deriveTableBodyAttrs).filter(ye);
+        let G = Ie({});
+        O.forEach(C => {
+            G = C(G)
+        });
+        const ve = Y(G, C => {
+                const H = Oe(C);
+                return g.set(H), H
             }),
-            W = Object.values(u).map(T => T.deriveTableBodyAttrs).filter(ke);
-        let te = Ie({
+            ie = Object.values(f).map(C => C.deriveTableBodyAttrs).filter(ye);
+        let ae = Ie({
             role: "rowgroup"
         });
-        W.forEach(T => {
-            te = T(te)
+        ie.forEach(C => {
+            ae = C(ae)
         });
-        const Fe = Y(te, T => {
-                const B = He(T);
-                return b.set(B), B
+        const Se = Y(ae, C => {
+                const H = Oe(C);
+                return m.set(H), H
             }),
-            de = Object.values(u).map(T => T.deriveFlatColumns).filter(ke);
-        let he = o;
-        de.forEach(T => {
-            he = T(he)
-        });
-        const ge = Y(he, T => (i.set(T), T)),
-            $e = Y([a, ge], ([T, B]) => Vr(T, B.map(O => O.id))),
-            Ee = Object.values(u).map(T => T.deriveRows).filter(ke);
-        let pe = $e;
-        Ee.forEach(T => {
-            pe = T(pe)
-        });
-        const _ = Y(pe, T => (T.forEach(B => {
-                B.injectState(p), B.cells.forEach(O => {
-                    O.injectState(p)
+            he = Object.values(f).map(C => C.deriveFlatColumns).filter(ye);
+        let $e = o;
+        he.forEach(C => {
+            $e = C($e)
+        });
+        const pe = Y($e, C => (a.set(C), C)),
+            _e = Y([i, pe], ([C, H]) => Or(C, H.map(P => P.id))),
+            we = Object.values(f).map(C => C.deriveRows).filter(ye);
+        let M = _e;
+        we.forEach(C => {
+            M = C(M)
+        });
+        const w = Y(M, C => (C.forEach(H => {
+                H.injectState(p), H.cells.forEach(P => {
+                    P.injectState(p)
                 })
-            }), Object.entries(u).forEach(([B, O]) => {
-                T.forEach(Q => {
+            }), Object.entries(f).forEach(([H, P]) => {
+                C.forEach(Q => {
                     var X;
-                    ((X = O.hooks) == null ? void 0 : X["tbody.tr"]) !== void 0 && Q.applyHook(B, O.hooks["tbody.tr"](Q)), Q.cells.forEach(fe => {
-                        var we;
-                        ((we = O.hooks) == null ? void 0 : we["tbody.tr.td"]) !== void 0 && fe.applyHook(B, O.hooks["tbody.tr.td"](fe))
+                    ((X = P.hooks) == null ? void 0 : X["tbody.tr"]) !== void 0 && Q.applyHook(H, P.hooks["tbody.tr"](Q)), Q.cells.forEach(ue => {
+                        var ke;
+                        ((ke = P.hooks) == null ? void 0 : ke["tbody.tr.td"]) !== void 0 && ue.applyHook(H, P.hooks["tbody.tr.td"](ue))
                     })
                 })
-            }), d.set(T), T)),
-            E = Object.values(u).map(T => T.derivePageRows).filter(ke);
-        let H = _;
-        E.forEach(T => {
-            H = T(H)
-        });
-        const Ce = Y(H, T => (T.forEach(B => {
-                B.injectState(p), B.cells.forEach(O => {
-                    O.injectState(p)
+            }), d.set(C), C)),
+            D = Object.values(f).map(C => C.derivePageRows).filter(ye);
+        let N = w;
+        D.forEach(C => {
+            N = C(N)
+        });
+        const Ce = Y(N, C => (C.forEach(H => {
+                H.injectState(p), H.cells.forEach(P => {
+                    P.injectState(p)
                 })
-            }), Object.entries(u).forEach(([B, O]) => {
-                T.forEach(Q => {
+            }), Object.entries(f).forEach(([H, P]) => {
+                C.forEach(Q => {
                     var X;
-                    ((X = O.hooks) == null ? void 0 : X["tbody.tr"]) !== void 0 && Q.applyHook(B, O.hooks["tbody.tr"](Q)), Q.cells.forEach(fe => {
-                        var we;
-                        ((we = O.hooks) == null ? void 0 : we["tbody.tr.td"]) !== void 0 && fe.applyHook(B, O.hooks["tbody.tr.td"](fe))
+                    ((X = P.hooks) == null ? void 0 : X["tbody.tr"]) !== void 0 && Q.applyHook(H, P.hooks["tbody.tr"](Q)), Q.cells.forEach(ue => {
+                        var ke;
+                        ((ke = P.hooks) == null ? void 0 : ke["tbody.tr.td"]) !== void 0 && ue.applyHook(H, P.hooks["tbody.tr.td"](ue))
                     })
                 })
-            }), w.set(T), T)),
-            Be = Y(ge, T => {
-                const B = Gr(e, T.map(O => O.id));
-                return B.forEach(O => {
-                    O.injectState(p), O.cells.forEach(Q => {
+            }), $.set(C), C)),
+            Be = Y(pe, C => {
+                const H = Nr(e, C.map(P => P.id));
+                return H.forEach(P => {
+                    P.injectState(p), P.cells.forEach(Q => {
                         Q.injectState(p)
                     })
-                }), Object.entries(u).forEach(([O, Q]) => {
-                    B.forEach(X => {
-                        var fe;
-                        ((fe = Q.hooks) == null ? void 0 : fe["thead.tr"]) !== void 0 && X.applyHook(O, Q.hooks["thead.tr"](X)), X.cells.forEach(we => {
-                            var rt;
-                            ((rt = Q.hooks) == null ? void 0 : rt["thead.tr.th"]) !== void 0 && we.applyHook(O, Q.hooks["thead.tr.th"](we))
+                }), Object.entries(f).forEach(([P, Q]) => {
+                    H.forEach(X => {
+                        var ue;
+                        ((ue = Q.hooks) == null ? void 0 : ue["thead.tr"]) !== void 0 && X.applyHook(P, Q.hooks["thead.tr"](X)), X.cells.forEach(ke => {
+                            var nt;
+                            ((nt = Q.hooks) == null ? void 0 : nt["thead.tr.th"]) !== void 0 && ke.applyHook(P, Q.hooks["thead.tr.th"](ke))
                         })
                     })
-                }), c.set(B), B
+                }), c.set(H), H
             });
         return {
-            tableAttrs: ee,
-            tableHeadAttrs: U,
-            tableBodyAttrs: Fe,
-            visibleColumns: ge,
+            tableAttrs: S,
+            tableHeadAttrs: ve,
+            tableBodyAttrs: Se,
+            visibleColumns: pe,
             flatColumns: l,
             headerRows: Be,
-            originalRows: a,
-            rows: _,
+            originalRows: i,
+            rows: w,
             pageRows: Ce,
             pluginStates: h
         }
     };
-let Xr = class {
+let qr = class {
     constructor(e, t) {
-        D(this, "data");
-        D(this, "plugins");
+        I(this, "data");
+        I(this, "plugins");
         this.data = e, this.plugins = t
     }
     createColumns(e) {
-        const t = Ut(e),
-            s = Hr(t);
+        const t = Qt(e),
+            s = jr(t);
         if (s.length !== 0) throw new Error(`Duplicate column ids not allowed: "${s.join('", "')}"`);
         return e
     }
     column(e) {
-        return new Ar(e)
+        return new Tr(e)
     }
     group(e) {
-        return new Rr(e)
+        return new Sr(e)
     }
     display(e) {
-        return new Mr(e)
+        return new Dr(e)
     }
     createViewModel(e, t) {
-        return Qr(this, e, t)
+        return Kr(this, e, t)
     }
 };
-const Yr = (n, e = {}) => new Xr(n, e),
-    Zr = ({
-        initialColumnIdOrder: n = [],
-        hideUnspecifiedColumns: e = !1
-    } = {}) => () => {
-        const t = me(n);
-        return {
-            pluginState: {
-                columnIdOrder: t
-            },
-            deriveFlatColumns: l => Y([l, t], ([o, a]) => {
-                const i = [...o],
-                    c = [];
-                return a.forEach(d => {
-                    const w = i.findIndex(y => y.id === d);
-                    c.push(...i.splice(w, 1))
-                }), e || c.push(...i), c
+const Ur = (n, e = {}) => new qr(n, e);
+/**
+ * @copyright CEA
+ * @author CEA
+ * @license CECILL
+ *
+ * This software is a collaborative computer program whose purpose is to
+ * generate and explore labeled data for computer vision applications.
+ * This software is governed by the CeCILL-C license under French law and
+ * abiding by the rules of distribution of free software. You can use,
+ * modify and/ or redistribute the software under the terms of the CeCILL-C
+ * license as circulated by CEA, CNRS and INRIA at the following URL
+ *
+ * http://www.cecill.info
+ */
+const pt = n => {
+        if (n.id === "id") return Ve(Le, {
+            itemFeature: {
+                name: n.id,
+                dtype: "int",
+                value: n.value
+            }
+        });
+        if (n.id === "split") return Ve(Le, {
+            itemFeature: {
+                name: n.id,
+                dtype: "str",
+                value: n.value
+            }
+        })
+    },
+    Jr = n => Ve(Le, {
+        itemFeature: JSON.parse(n.value)
+    }),
+    Wr = n => {
+        const e = JSON.parse(n.value);
+        return Ve(Le, {
+            itemFeature: {
+                name: e.id,
+                dtype: e.type,
+                value: e.thumbnail
+            }
+        })
+    };
+
+function Qr(n, {
+    from: e,
+    to: t
+}, s = {}) {
+    const r = getComputedStyle(n),
+        l = r.transform === "none" ? "" : r.transform,
+        [o, i] = r.transformOrigin.split(" ").map(parseFloat),
+        a = e.left + e.width * o / t.width - (t.left + o),
+        c = e.top + e.height * i / t.height - (t.top + i),
+        {
+            delay: d = 0,
+            duration: $ = g => Math.sqrt(g) * 120,
+            easing: k = zt
+        } = s;
+    return {
+        delay: d,
+        duration: Ot($) ? $(Math.sqrt(a * a + c * c)) : $,
+        easing: k,
+        css: (g, m) => {
+            const u = m * a,
+                f = m * c,
+                h = g + m * e.width / t.width,
+                p = g + m * e.height / t.height;
+            return `transform: ${l} translate(${u}px, ${f}px) scale(${h}, ${p});`
+        }
+    }
+}
+
+function _t(n, e, t) {
+    const s = n.slice();
+    return s[15] = e[t], s[17] = t, s
+}
+const Xr = n => ({
+        item: n & 1,
+        index: n & 1
+    }),
+    gt = n => ({
+        item: n[15],
+        index: n[17]
+    });
+
+function mt(n) {
+    let e, t = [],
+        s = new Map,
+        r, l = oe(n[0]);
+    const o = i => i[8](i[15]);
+    for (let i = 0; i < l.length; i += 1) {
+        let a = _t(n, l, i),
+            c = o(a);
+        s.set(c, t[i] = bt(c, a))
+    }
+    return {
+        c() {
+            e = j("ul");
+            for (let i = 0; i < t.length; i += 1) t[i].c();
+            this.h()
+        },
+        l(i) {
+            e = A(i, "UL", {
+                class: !0
+            });
+            var a = R(e);
+            for (let c = 0; c < t.length; c += 1) t[c].l(a);
+            a.forEach(_), this.h()
+        },
+        h() {
+            v(e, "class", "svelte-s1iyrp")
+        },
+        m(i, a) {
+            T(i, e, a);
+            for (let c = 0; c < t.length; c += 1) t[c] && t[c].m(e, null);
+            r = !0
+        },
+        p(i, a) {
+            if (a & 1523) {
+                l = oe(i[0]), Z();
+                for (let c = 0; c < t.length; c += 1) t[c].r();
+                t = Me(t, a, o, 1, i, l, s, e, gs, bt, null, _t);
+                for (let c = 0; c < t.length; c += 1) t[c].a();
+                x()
+            }
+        },
+        i(i) {
+            if (!r) {
+                for (let a = 0; a < l.length; a += 1) E(t[a]);
+                r = !0
+            }
+        },
+        o(i) {
+            for (let a = 0; a < t.length; a += 1) F(t[a]);
+            r = !1
+        },
+        d(i) {
+            i && _(e);
+            for (let a = 0; a < t.length; a += 1) t[a].d()
+        }
+    }
+}
+
+function Yr(n) {
+    let e, t = n[8](n[15]) + "",
+        s;
+    return {
+        c() {
+            e = j("p"), s = re(t)
+        },
+        l(r) {
+            e = A(r, "P", {});
+            var l = R(e);
+            s = le(l, t), l.forEach(_)
+        },
+        m(r, l) {
+            T(r, e, l), y(e, s)
+        },
+        p(r, l) {
+            l & 1 && t !== (t = r[8](r[15]) + "") && me(s, t)
+        },
+        d(r) {
+            r && _(e)
+        }
+    }
+}
+
+function bt(n, e) {
+    let t, s, r, l, o, i, a, c = J,
+        d, $, k;
+    const g = e[11].default,
+        m = Ht(g, e, e[10], gt),
+        u = m || Yr(e);
+    return {
+        key: n,
+        first: null,
+        c() {
+            t = j("li"), u && u.c(), s = L(), this.h()
+        },
+        l(f) {
+            t = A(f, "LI", {
+                "data-index": !0,
+                "data-id": !0,
+                draggable: !0,
+                class: !0
+            });
+            var h = R(t);
+            u && u.l(h), s = V(h), h.forEach(_), this.h()
+        },
+        h() {
+            v(t, "data-index", r = e[17]), v(t, "data-id", l = JSON.stringify(e[8](e[15]))), v(t, "draggable", "true"), v(t, "class", "svelte-s1iyrp"), it(t, "over", e[8](e[15]) === e[1]), this.first = t
+        },
+        m(f, h) {
+            T(f, t, h), u && u.m(t, null), y(t, s), d = !0, $ || (k = [ne(t, "dragstart", e[4]), ne(t, "dragover", e[5]), ne(t, "dragleave", e[6]), ne(t, "drop", e[7])], $ = !0)
+        },
+        p(f, h) {
+            e = f, m ? m.p && (!d || h & 1025) && Nt(m, g, e, e[10], d ? Lt(g, e[10], h, Xr) : Pt(e[10]), gt) : u && u.p && (!d || h & 1) && u.p(e, d ? h : -1), (!d || h & 1 && r !== (r = e[17])) && v(t, "data-index", r), (!d || h & 1 && l !== (l = JSON.stringify(e[8](e[15])))) && v(t, "data-id", l), (!d || h & 259) && it(t, "over", e[8](e[15]) === e[1])
+        },
+        r() {
+            a = t.getBoundingClientRect()
+        },
+        f() {
+            Os(t), c(), Kt(t, a)
+        },
+        a() {
+            c(), c = Bs(t, a, Qr, {
+                duration: 300
             })
+        },
+        i(f) {
+            d || (E(u, f), f && is(() => {
+                d && (i && i.end(1), o = ds(t, e[3], {
+                    key: e[8](e[15])
+                }), o.start())
+            }), d = !0)
+        },
+        o(f) {
+            F(u, f), o && o.invalidate(), f && (i = hs(t, e[2], {
+                key: e[8](e[15])
+            })), d = !1
+        },
+        d(f) {
+            f && _(t), u && u.d(f), f && i && i.end(), $ = !1, ze(k)
         }
-    };
+    }
+}
+
+function Zr(n) {
+    let e, t, s = n[0] && n[0].length && mt(n);
+    return {
+        c() {
+            s && s.c(), e = z()
+        },
+        l(r) {
+            s && s.l(r), e = z()
+        },
+        m(r, l) {
+            s && s.m(r, l), T(r, e, l), t = !0
+        },
+        p(r, [l]) {
+            r[0] && r[0].length ? s ? (s.p(r, l), l & 1 && E(s, 1)) : (s = mt(r), s.c(), E(s, 1), s.m(e.parentNode, e)) : s && (Z(), F(s, 1, 1, () => {
+                s = null
+            }), x())
+        },
+        i(r) {
+            t || (E(s), t = !0)
+        },
+        o(r) {
+            F(s), t = !1
+        },
+        d(r) {
+            r && _(e), s && s.d(r)
+        }
+    }
+}
+
+function xr(n, e, t) {
+    let {
+        $$slots: s = {},
+        $$scope: r
+    } = e;
+    const [l, o] = Hs({
+        duration: p => Math.sqrt(p * 200),
+        fallback(p, b) {
+            const B = getComputedStyle(p),
+                S = B.transform === "none" ? "" : B.transform;
+            return {
+                duration: 600,
+                easing: Ss,
+                css: O => `
+					transform: ${S} scale(${O});
+					opacity: ${O}
+				`
+            }
+        }
+    });
+    let i = !1;
+    const a = p => p.dataset.index && p.dataset || a(p.parentNode),
+        c = p => {
+            p.dataTransfer.setData("source", p.target.dataset.index)
+        },
+        d = p => {
+            p.preventDefault();
+            let b = a(p.target);
+            i !== b.id && t(1, i = JSON.parse(b.id))
+        },
+        $ = p => {
+            let b = a(p.target);
+            i === b.id && t(1, i = !1)
+        },
+        k = p => {
+            t(1, i = !1), p.preventDefault();
+            let b = a(p.target),
+                B = p.dataTransfer.getData("source"),
+                S = b.index;
+            m({
+                from: B,
+                to: S
+            })
+        },
+        g = Qe(),
+        m = ({
+            from: p,
+            to: b
+        }) => {
+            let B = [...f];
+            B[p] = [B[b], B[b] = B[p]][0], g("sort", B)
+        },
+        u = p => h ? p[h] : p;
+    let {
+        list: f
+    } = e, {
+        key: h
+    } = e;
+    return n.$$set = p => {
+        "list" in p && t(0, f = p.list), "key" in p && t(9, h = p.key), "$$scope" in p && t(10, r = p.$$scope)
+    }, [f, i, l, o, c, d, $, k, u, h, r, s]
+}
+class el extends te {
+    constructor(e) {
+        super(), se(this, e, xr, Zr, ee, {
+            list: 0,
+            key: 9
+        })
+    }
+}
+const tl = ({
+    initialColumnIdOrder: n = [],
+    hideUnspecifiedColumns: e = !1
+} = {}) => () => {
+    const t = ge(n);
+    return {
+        pluginState: {
+            columnIdOrder: t
+        },
+        deriveFlatColumns: l => Y([l, t], ([o, i]) => {
+            const a = [...o],
+                c = [];
+            return i.forEach(d => {
+                const $ = a.findIndex(k => k.id === d);
+                c.push(...a.splice($, 1))
+            }), e || c.push(...a), c
+        })
+    }
+};
 Ie(void 0);
-const xr = ({
+const sl = ({
     initialHiddenColumnIds: n = []
 } = {}) => () => {
-    const e = me(n);
+    const e = ge(n);
     return {
         pluginState: {
             hiddenColumnIds: e
         },
-        deriveFlatColumns: r => Y([r, e], ([l, o]) => o.length === 0 ? l : l.filter(a => !o.includes(a.id)))
+        deriveFlatColumns: r => Y([r, e], ([l, o]) => o.length === 0 ? l : l.filter(i => !o.includes(i.id)))
     }
 };
 
-function gt(n, e, t) {
+function vt(n, e, t) {
     const s = n.slice();
-    return s[31] = e[t], s
+    return s[28] = e[t], s
 }
 
-function mt(n, e, t) {
+function $t(n, e, t) {
     const s = n.slice();
-    return s[35] = e[t], s
+    return s[32] = e[t], s
 }
 
-function bt(n, e, t) {
+function wt(n, e, t) {
     const s = n.slice();
-    return s[39] = e[t], s
+    return s[36] = e[t], s
 }
 
-function vt(n, e, t) {
+function kt(n, e, t) {
     const s = n.slice();
-    return s[35] = e[t], s
+    return s[32] = e[t], s
 }
 
-function el(n) {
-    let e, t, s, r, l, o = n[44] + "",
-        a, i, c, d, w, y;
+function rl(n) {
+    let e, t, s, r, l, o = n[41] + "",
+        i, a, c, d, $, k;
 
-    function m(f) {
-        n[17](f, n[44])
+    function g(u) {
+        n[16](u, n[41])
     }
-    let b = {
-        id: n[44]
+    let m = {
+        id: n[41]
     };
-    return n[1][n[44]] !== void 0 && (b.checked = n[1][n[44]]), t = new Ts({
-        props: b
-    }), je.push(() => We(t, "checked", m)), {
+    return n[0][n[41]] !== void 0 && (m.checked = n[0][n[41]]), t = new Fs({
+        props: m
+    }), je.push(() => Xe(t, "checked", g)), {
         c() {
-            e = j("div"), z(t.$$.fragment), r = P(), l = j("label"), a = ne(o), c = P(), d = Te("svg"), w = Te("path"), this.h()
+            e = j("div"), K(t.$$.fragment), r = L(), l = j("label"), i = re(o), c = L(), d = Te("svg"), $ = Te("path"), this.h()
         },
-        l(f) {
-            e = A(f, "DIV", {
+        l(u) {
+            e = A(u, "DIV", {
                 class: !0
             });
-            var u = M(e);
-            J(t.$$.fragment, u), r = L(u), l = A(u, "LABEL", {
+            var f = R(e);
+            W(t.$$.fragment, f), r = V(f), l = A(f, "LABEL", {
                 for: !0,
                 class: !0
             });
-            var h = M(l);
-            a = oe(h, o), h.forEach(g), c = L(u), d = De(u, "svg", {
+            var h = R(l);
+            i = le(h, o), h.forEach(_), c = V(f), d = De(f, "svg", {
                 xmlns: !0,
                 height: !0,
                 viewBox: !0,
                 width: !0,
                 class: !0
             });
-            var p = M(d);
-            w = De(p, "path", {
+            var p = R(d);
+            $ = De(p, "path", {
                 d: !0,
                 fill: !0
-            }), M(w).forEach(g), p.forEach(g), u.forEach(g), this.h()
+            }), R($).forEach(_), p.forEach(_), f.forEach(_), this.h()
         },
         h() {
-            $(l, "for", i = n[44]), $(l, "class", "text-sm select-none grow cursor-pointer"), $(w, "d", ms), $(w, "fill", "grey"), $(d, "xmlns", "http://www.w3.org/2000/svg"), $(d, "height", "48"), $(d, "viewBox", "0 -960 960 960"), $(d, "width", "48"), $(d, "class", "h-6 w-6 cursor-move"), $(e, "class", "py-1 px-2 flex items-center space-x-2 border rounded-sm")
+            v(l, "for", a = n[41]), v(l, "class", "text-sm select-none grow cursor-pointer"), v($, "d", $s), v($, "fill", "grey"), v(d, "xmlns", "http://www.w3.org/2000/svg"), v(d, "height", "48"), v(d, "viewBox", "0 -960 960 960"), v(d, "width", "48"), v(d, "class", "h-6 w-6 cursor-move"), v(e, "class", "py-1 px-2 flex items-center space-x-2 border rounded-sm")
         },
-        m(f, u) {
-            F(f, e, u), G(t, e, null), C(e, r), C(e, l), C(l, a), C(e, c), C(e, d), C(d, w), y = !0
+        m(u, f) {
+            T(u, e, f), q(t, e, null), y(e, r), y(e, l), y(l, i), y(e, c), y(e, d), y(d, $), k = !0
         },
-        p(f, u) {
-            n = f;
+        p(u, f) {
+            n = u;
             const h = {};
-            u[1] & 8192 && (h.id = n[44]), !s && u[0] & 2 | u[1] & 8192 && (s = !0, h.checked = n[1][n[44]], Je(() => s = !1)), t.$set(h), (!y || u[1] & 8192) && o !== (o = n[44] + "") && be(a, o), (!y || u[1] & 8192 && i !== (i = n[44])) && $(l, "for", i)
+            f[1] & 1024 && (h.id = n[41]), !s && f[0] & 1 | f[1] & 1024 && (s = !0, h.checked = n[0][n[41]], We(() => s = !1)), t.$set(h), (!k || f[1] & 1024) && o !== (o = n[41] + "") && me(i, o), (!k || f[1] & 1024 && a !== (a = n[41])) && v(l, "for", a)
         },
-        i(f) {
-            y || (I(t.$$.fragment, f), y = !0)
+        i(u) {
+            k || (E(t.$$.fragment, u), k = !0)
         },
-        o(f) {
-            S(t.$$.fragment, f), y = !1
+        o(u) {
+            F(t.$$.fragment, u), k = !1
         },
-        d(f) {
-            f && g(e), K(t)
+        d(u) {
+            u && _(e), U(t)
         }
     }
 }
 
-function tl(n) {
+function ll(n) {
     let e;
     return {
         c() {
-            e = ne("Done")
+            e = re("Done")
         },
         l(t) {
-            e = oe(t, "Done")
+            e = le(t, "Done")
         },
         m(t, s) {
-            F(t, e, s)
+            T(t, e, s)
         },
         d(t) {
-            t && g(e)
+            t && _(e)
         }
     }
 }
 
-function sl(n) {
+function nl(n) {
     let e, t, s;
-    t = new Xe({
+    t = new Ze({
         props: {
-            of: n[35].render()
+            of: n[32].render()
         }
     });
-    let r = [n[38], {
+    let r = [n[35], {
             class: "relative py-4 font-semibold"
         }],
         l = {};
-    for (let o = 0; o < r.length; o += 1) l = ue(l, r[o]);
+    for (let o = 0; o < r.length; o += 1) l = fe(l, r[o]);
     return {
         c() {
-            e = j("th"), z(t.$$.fragment), this.h()
+            e = j("th"), K(t.$$.fragment), this.h()
         },
         l(o) {
             e = A(o, "TH", {
                 class: !0
             });
-            var a = M(e);
-            J(t.$$.fragment, a), a.forEach(g), this.h()
+            var i = R(e);
+            W(t.$$.fragment, i), i.forEach(_), this.h()
         },
         h() {
             ce(e, l)
         },
-        m(o, a) {
-            F(o, e, a), G(t, e, null), s = !0
+        m(o, i) {
+            T(o, e, i), q(t, e, null), s = !0
         },
-        p(o, a) {
-            const i = {};
-            a[0] & 32 && (i.of = o[35].render()), t.$set(i), ce(e, l = _e(r, [a[1] & 128 && o[38], {
+        p(o, i) {
+            const a = {};
+            i[0] & 16 && (a.of = o[32].render()), t.$set(a), ce(e, l = de(r, [i[1] & 16 && o[35], {
                 class: "relative py-4 font-semibold"
             }]))
         },
         i(o) {
-            s || (I(t.$$.fragment, o), s = !0)
+            s || (E(t.$$.fragment, o), s = !0)
         },
         o(o) {
-            S(t.$$.fragment, o), s = !1
+            F(t.$$.fragment, o), s = !1
         },
         d(o) {
-            o && g(e), K(t)
+            o && _(e), U(t)
         }
     }
 }
 
-function $t(n, e) {
+function yt(n, e) {
     let t, s, r;
     return s = new Re({
         props: {
-            attrs: e[35].attrs(),
+            attrs: e[32].attrs(),
             $$slots: {
-                default: [sl, ({
+                default: [nl, ({
                     attrs: l
                 }) => ({
-                    38: l
+                    35: l
                 }), ({
                     attrs: l
-                }) => [0, l ? 128 : 0]]
+                }) => [0, l ? 16 : 0]]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         key: n,
         first: null,
         c() {
-            t = N(), z(s.$$.fragment), this.h()
+            t = z(), K(s.$$.fragment), this.h()
         },
         l(l) {
-            t = N(), J(s.$$.fragment, l), this.h()
+            t = z(), W(s.$$.fragment, l), this.h()
         },
         h() {
             this.first = t
         },
         m(l, o) {
-            F(l, t, o), G(s, l, o), r = !0
+            T(l, t, o), q(s, l, o), r = !0
         },
         p(l, o) {
             e = l;
-            const a = {};
-            o[0] & 32 && (a.attrs = e[35].attrs()), o[0] & 32 | o[1] & 16512 && (a.$$scope = {
+            const i = {};
+            o[0] & 16 && (i.attrs = e[32].attrs()), o[0] & 16 | o[1] & 2064 && (i.$$scope = {
                 dirty: o,
                 ctx: e
-            }), s.$set(a)
+            }), s.$set(i)
         },
         i(l) {
-            r || (I(s.$$.fragment, l), r = !0)
+            r || (E(s.$$.fragment, l), r = !0)
         },
         o(l) {
-            S(s.$$.fragment, l), r = !1
+            F(s.$$.fragment, l), r = !1
         },
         d(l) {
-            l && g(t), K(s, l)
+            l && _(t), U(s, l)
         }
     }
 }
 
-function rl(n) {
+function ol(n) {
     let e, t, s;
     return {
         c() {
             e = Te("svg"), t = Te("title"), s = Te("path"), this.h()
         },
         l(r) {
             e = De(r, "svg", {
                 xmlns: !0,
                 height: !0,
                 viewBox: !0,
                 width: !0,
                 class: !0
             });
-            var l = M(e);
-            t = De(l, "title", {}), M(t).forEach(g), s = De(l, "path", {
+            var l = R(e);
+            t = De(l, "title", {}), R(t).forEach(_), s = De(l, "path", {
                 d: !0,
                 fill: !0
-            }), M(s).forEach(g), l.forEach(g), this.h()
+            }), R(s).forEach(_), l.forEach(_), this.h()
         },
         h() {
-            $(s, "d", bs), $(s, "fill", "#111"), $(e, "xmlns", "http://www.w3.org/2000/svg"), $(e, "height", "48"), $(e, "viewBox", "0 -960 960 960"), $(e, "width", "48"), $(e, "class", "h-6 w-6")
+            v(s, "d", ws), v(s, "fill", "#111"), v(e, "xmlns", "http://www.w3.org/2000/svg"), v(e, "height", "48"), v(e, "viewBox", "0 -960 960 960"), v(e, "width", "48"), v(e, "class", "h-6 w-6")
         },
         m(r, l) {
-            F(r, e, l), C(e, t), C(e, s)
+            T(r, e, l), y(e, t), y(e, s)
         },
-        p: q,
+        p: J,
         d(r) {
-            r && g(e)
+            r && _(e)
         }
     }
 }
 
-function ll(n) {
+function il(n) {
     let e, t = [],
         s = new Map,
-        r, l, o, a, i, c, d, w = ie(n[39].cells);
-    const y = f => f[35].id;
-    for (let f = 0; f < w.length; f += 1) {
-        let u = vt(n, w, f),
-            h = y(u);
-        s.set(h, t[f] = $t(h, u))
+        r, l, o, i, a, c, d, $ = oe(n[36].cells);
+    const k = u => u[32].id;
+    for (let u = 0; u < $.length; u += 1) {
+        let f = kt(n, $, u),
+            h = k(f);
+        s.set(h, t[u] = yt(h, f))
     }
-    i = new Nt({
+    a = new Gt({
         props: {
             variant: "ghost",
             $$slots: {
-                default: [rl]
+                default: [ol]
             },
             $$scope: {
                 ctx: n
             }
         }
-    }), i.$on("click", n[19]);
-    let m = [n[34], {
+    }), a.$on("click", n[18]);
+    let g = [n[31], {
             class: "sticky top-0 z-10 bg-white shadow-sm shadow-slate-300 border-b border-b-slate-400"
         }],
-        b = {};
-    for (let f = 0; f < m.length; f += 1) b = ue(b, m[f]);
+        m = {};
+    for (let u = 0; u < g.length; u += 1) m = fe(m, g[u]);
     return {
         c() {
             e = j("tr");
-            for (let f = 0; f < t.length; f += 1) t[f].c();
-            r = P(), l = j("th"), o = P(), a = j("th"), z(i.$$.fragment), c = P(), this.h()
+            for (let u = 0; u < t.length; u += 1) t[u].c();
+            r = L(), l = j("th"), o = L(), i = j("th"), K(a.$$.fragment), c = L(), this.h()
         },
-        l(f) {
-            e = A(f, "TR", {
+        l(u) {
+            e = A(u, "TR", {
                 class: !0
             });
-            var u = M(e);
-            for (let p = 0; p < t.length; p += 1) t[p].l(u);
-            r = L(u), l = A(u, "TH", {
+            var f = R(e);
+            for (let p = 0; p < t.length; p += 1) t[p].l(f);
+            r = V(f), l = A(f, "TH", {
                 class: !0
-            }), M(l).forEach(g), o = L(u), a = A(u, "TH", {
+            }), R(l).forEach(_), o = V(f), i = A(f, "TH", {
                 class: !0
             });
-            var h = M(a);
-            J(i.$$.fragment, h), h.forEach(g), u.forEach(g), c = L(f), this.h()
+            var h = R(i);
+            W(a.$$.fragment, h), h.forEach(_), f.forEach(_), c = V(u), this.h()
         },
         h() {
-            $(l, "class", "w-full"), $(a, "class", "pr-4"), ce(e, b)
+            v(l, "class", "w-full"), v(i, "class", "pr-4"), ce(e, m)
         },
-        m(f, u) {
-            F(f, e, u);
+        m(u, f) {
+            T(u, e, f);
             for (let h = 0; h < t.length; h += 1) t[h] && t[h].m(e, null);
-            C(e, r), C(e, l), C(e, o), C(e, a), G(i, a, null), F(f, c, u), d = !0
+            y(e, r), y(e, l), y(e, o), y(e, i), q(a, i, null), T(u, c, f), d = !0
         },
-        p(f, u) {
-            u[0] & 32 | u[1] & 128 && (w = ie(f[39].cells), Z(), t = Me(t, u, y, 1, f, w, s, e, Le, $t, r, vt), x());
+        p(u, f) {
+            f[0] & 16 | f[1] & 16 && ($ = oe(u[36].cells), Z(), t = Me(t, f, k, 1, u, $, s, e, Pe, yt, r, kt), x());
             const h = {};
-            u[1] & 16384 && (h.$$scope = {
-                dirty: u,
-                ctx: f
-            }), i.$set(h), ce(e, b = _e(m, [u[1] & 8 && f[34], {
+            f[1] & 2048 && (h.$$scope = {
+                dirty: f,
+                ctx: u
+            }), a.$set(h), ce(e, m = de(g, [f[1] & 1 && u[31], {
                 class: "sticky top-0 z-10 bg-white shadow-sm shadow-slate-300 border-b border-b-slate-400"
             }]))
         },
-        i(f) {
+        i(u) {
             if (!d) {
-                for (let u = 0; u < w.length; u += 1) I(t[u]);
-                I(i.$$.fragment, f), d = !0
+                for (let f = 0; f < $.length; f += 1) E(t[f]);
+                E(a.$$.fragment, u), d = !0
             }
         },
-        o(f) {
-            for (let u = 0; u < t.length; u += 1) S(t[u]);
-            S(i.$$.fragment, f), d = !1
+        o(u) {
+            for (let f = 0; f < t.length; f += 1) F(t[f]);
+            F(a.$$.fragment, u), d = !1
         },
-        d(f) {
-            f && (g(e), g(c));
-            for (let u = 0; u < t.length; u += 1) t[u].d();
-            K(i)
+        d(u) {
+            u && (_(e), _(c));
+            for (let f = 0; f < t.length; f += 1) t[f].d();
+            U(a)
         }
     }
 }
 
-function wt(n, e) {
+function Et(n, e) {
     let t, s, r;
     return s = new Re({
         props: {
-            rowAttrs: e[39].attrs(),
+            rowAttrs: e[36].attrs(),
             $$slots: {
-                default: [ll, ({
+                default: [il, ({
                     rowAttrs: l
                 }) => ({
-                    34: l
+                    31: l
                 }), ({
                     rowAttrs: l
-                }) => [0, l ? 8 : 0]]
+                }) => [0, l ? 1 : 0]]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         key: n,
         first: null,
         c() {
-            t = N(), z(s.$$.fragment), this.h()
+            t = z(), K(s.$$.fragment), this.h()
         },
         l(l) {
-            t = N(), J(s.$$.fragment, l), this.h()
+            t = z(), W(s.$$.fragment, l), this.h()
         },
         h() {
             this.first = t
         },
         m(l, o) {
-            F(l, t, o), G(s, l, o), r = !0
+            T(l, t, o), q(s, l, o), r = !0
         },
         p(l, o) {
             e = l;
-            const a = {};
-            o[0] & 32 && (a.rowAttrs = e[39].attrs()), o[0] & 36 | o[1] & 16392 && (a.$$scope = {
+            const i = {};
+            o[0] & 16 && (i.rowAttrs = e[36].attrs()), o[0] & 18 | o[1] & 2049 && (i.$$scope = {
                 dirty: o,
                 ctx: e
-            }), s.$set(a)
+            }), s.$set(i)
         },
         i(l) {
-            r || (I(s.$$.fragment, l), r = !0)
+            r || (E(s.$$.fragment, l), r = !0)
         },
         o(l) {
-            S(s.$$.fragment, l), r = !1
+            F(s.$$.fragment, l), r = !1
         },
         d(l) {
-            l && g(t), K(s, l)
+            l && _(t), U(s, l)
         }
     }
 }
 
-function nl(n) {
+function al(n) {
     let e, t, s;
-    t = new Xe({
+    t = new Ze({
         props: {
-            of: n[35].render()
+            of: n[32].render()
         }
     });
-    let r = [n[38], {
+    let r = [n[35], {
             class: "border-b border-slate-300"
         }],
         l = {};
-    for (let o = 0; o < r.length; o += 1) l = ue(l, r[o]);
+    for (let o = 0; o < r.length; o += 1) l = fe(l, r[o]);
     return {
         c() {
-            e = j("td"), z(t.$$.fragment), this.h()
+            e = j("td"), K(t.$$.fragment), this.h()
         },
         l(o) {
             e = A(o, "TD", {
                 class: !0
             });
-            var a = M(e);
-            J(t.$$.fragment, a), a.forEach(g), this.h()
+            var i = R(e);
+            W(t.$$.fragment, i), i.forEach(_), this.h()
         },
         h() {
             ce(e, l)
         },
-        m(o, a) {
-            F(o, e, a), G(t, e, null), s = !0
+        m(o, i) {
+            T(o, e, i), q(t, e, null), s = !0
         },
-        p(o, a) {
-            const i = {};
-            a[0] & 128 && (i.of = o[35].render()), t.$set(i), ce(e, l = _e(r, [a[1] & 128 && o[38], {
+        p(o, i) {
+            const a = {};
+            i[0] & 64 && (a.of = o[32].render()), t.$set(a), ce(e, l = de(r, [i[1] & 16 && o[35], {
                 class: "border-b border-slate-300"
             }]))
         },
         i(o) {
-            s || (I(t.$$.fragment, o), s = !0)
+            s || (E(t.$$.fragment, o), s = !0)
         },
         o(o) {
-            S(t.$$.fragment, o), s = !1
+            F(t.$$.fragment, o), s = !1
         },
         d(o) {
-            o && g(e), K(t)
+            o && _(e), U(t)
         }
     }
 }
 
-function kt(n, e) {
+function Ct(n, e) {
     let t, s, r;
     return s = new Re({
         props: {
-            attrs: e[35].attrs(),
+            attrs: e[32].attrs(),
             $$slots: {
-                default: [nl, ({
+                default: [al, ({
                     attrs: l
                 }) => ({
-                    38: l
+                    35: l
                 }), ({
                     attrs: l
-                }) => [0, l ? 128 : 0]]
+                }) => [0, l ? 16 : 0]]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         key: n,
         first: null,
         c() {
-            t = N(), z(s.$$.fragment), this.h()
+            t = z(), K(s.$$.fragment), this.h()
         },
         l(l) {
-            t = N(), J(s.$$.fragment, l), this.h()
+            t = z(), W(s.$$.fragment, l), this.h()
         },
         h() {
             this.first = t
         },
         m(l, o) {
-            F(l, t, o), G(s, l, o), r = !0
+            T(l, t, o), q(s, l, o), r = !0
         },
         p(l, o) {
             e = l;
-            const a = {};
-            o[0] & 128 && (a.attrs = e[35].attrs()), o[0] & 128 | o[1] & 16512 && (a.$$scope = {
+            const i = {};
+            o[0] & 64 && (i.attrs = e[32].attrs()), o[0] & 64 | o[1] & 2064 && (i.$$scope = {
                 dirty: o,
                 ctx: e
-            }), s.$set(a)
+            }), s.$set(i)
         },
         i(l) {
-            r || (I(s.$$.fragment, l), r = !0)
+            r || (E(s.$$.fragment, l), r = !0)
         },
         o(l) {
-            S(s.$$.fragment, l), r = !1
+            F(s.$$.fragment, l), r = !1
         },
         d(l) {
-            l && g(t), K(s, l)
+            l && _(t), U(s, l)
         }
     }
 }
 
-function ol(n) {
+function cl(n) {
     let e, t = [],
         s = new Map,
-        r, l, o, a, i = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 mx-auto p-1 ml-3 border rounded-full border-slate-300 transition-colors hover:bg-slate-200"><title>Open</title><path d="${vs}" fill="currentcolor"></path></svg>`,
-        c, d, w, y, m = ie(n[31].cells);
-    const b = p => p[35].id;
-    for (let p = 0; p < m.length; p += 1) {
-        let v = mt(n, m, p),
-            R = b(v);
-        s.set(R, t[p] = kt(R, v))
+        r, l, o, i, a = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 mx-auto p-1 ml-3 border rounded-full border-slate-300 transition-colors hover:bg-slate-200"><title>Open</title><path d="${ks}" fill="currentcolor"></path></svg>`,
+        c, d, $, k, g = oe(n[28].cells);
+    const m = p => p[32].id;
+    for (let p = 0; p < g.length; p += 1) {
+        let b = $t(n, g, p),
+            B = m(b);
+        s.set(B, t[p] = Ct(B, b))
     }
-    let f = [n[34], {
+    let u = [n[31], {
             class: "h-24 cursor-pointer hover:bg-slate-100"
         }],
-        u = {};
-    for (let p = 0; p < f.length; p += 1) u = ue(u, f[p]);
+        f = {};
+    for (let p = 0; p < u.length; p += 1) f = fe(f, u[p]);
 
     function h() {
-        return n[20](n[31])
+        return n[19](n[28])
     }
     return {
         c() {
             e = j("tr");
             for (let p = 0; p < t.length; p += 1) t[p].c();
-            r = P(), l = j("td"), o = P(), a = j("td"), a.innerHTML = i, c = P(), this.h()
+            r = L(), l = j("td"), o = L(), i = j("td"), i.innerHTML = a, c = L(), this.h()
         },
         l(p) {
             e = A(p, "TR", {
                 class: !0
             });
-            var v = M(e);
-            for (let R = 0; R < t.length; R += 1) t[R].l(v);
-            r = L(v), l = A(v, "TD", {
+            var b = R(e);
+            for (let B = 0; B < t.length; B += 1) t[B].l(b);
+            r = V(b), l = A(b, "TD", {
                 class: !0
-            }), M(l).forEach(g), o = L(v), a = A(v, "TD", {
+            }), R(l).forEach(_), o = V(b), i = A(b, "TD", {
                 class: !0,
                 "data-svelte-h": !0
-            }), ve(a) !== "svelte-nb66sx" && (a.innerHTML = i), v.forEach(g), c = L(p), this.h()
+            }), be(i) !== "svelte-nb66sx" && (i.innerHTML = a), b.forEach(_), c = V(p), this.h()
         },
         h() {
-            $(l, "class", "w-full border-b border-slate-300"), $(a, "class", "border-b border-slate-300"), ce(e, u)
+            v(l, "class", "w-full border-b border-slate-300"), v(i, "class", "border-b border-slate-300"), ce(e, f)
         },
-        m(p, v) {
-            F(p, e, v);
-            for (let R = 0; R < t.length; R += 1) t[R] && t[R].m(e, null);
-            C(e, r), C(e, l), C(e, o), C(e, a), F(p, c, v), d = !0, w || (y = ae(e, "click", h), w = !0)
+        m(p, b) {
+            T(p, e, b);
+            for (let B = 0; B < t.length; B += 1) t[B] && t[B].m(e, null);
+            y(e, r), y(e, l), y(e, o), y(e, i), T(p, c, b), d = !0, $ || (k = ne(e, "click", h), $ = !0)
         },
-        p(p, v) {
-            n = p, v[0] & 128 | v[1] & 128 && (m = ie(n[31].cells), Z(), t = Me(t, v, b, 1, n, m, s, e, Le, kt, r, mt), x()), ce(e, u = _e(f, [v[1] & 8 && n[34], {
+        p(p, b) {
+            n = p, b[0] & 64 | b[1] & 16 && (g = oe(n[28].cells), Z(), t = Me(t, b, m, 1, n, g, s, e, Pe, Ct, r, $t), x()), ce(e, f = de(u, [b[1] & 1 && n[31], {
                 class: "h-24 cursor-pointer hover:bg-slate-100"
             }]))
         },
         i(p) {
             if (!d) {
-                for (let v = 0; v < m.length; v += 1) I(t[v]);
+                for (let b = 0; b < g.length; b += 1) E(t[b]);
                 d = !0
             }
         },
         o(p) {
-            for (let v = 0; v < t.length; v += 1) S(t[v]);
+            for (let b = 0; b < t.length; b += 1) F(t[b]);
             d = !1
         },
         d(p) {
-            p && (g(e), g(c));
-            for (let v = 0; v < t.length; v += 1) t[v].d();
-            w = !1, y()
+            p && (_(e), _(c));
+            for (let b = 0; b < t.length; b += 1) t[b].d();
+            $ = !1, k()
         }
     }
 }
 
-function yt(n, e) {
+function It(n, e) {
     let t, s, r;
     return s = new Re({
         props: {
-            rowAttrs: e[31].attrs(),
+            rowAttrs: e[28].attrs(),
             $$slots: {
-                default: [ol, ({
+                default: [cl, ({
                     rowAttrs: l
                 }) => ({
-                    34: l
+                    31: l
                 }), ({
                     rowAttrs: l
-                }) => [0, l ? 8 : 0]]
+                }) => [0, l ? 1 : 0]]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         key: n,
         first: null,
         c() {
-            t = N(), z(s.$$.fragment), this.h()
+            t = z(), K(s.$$.fragment), this.h()
         },
         l(l) {
-            t = N(), J(s.$$.fragment, l), this.h()
+            t = z(), W(s.$$.fragment, l), this.h()
         },
         h() {
             this.first = t
         },
         m(l, o) {
-            F(l, t, o), G(s, l, o), r = !0
+            T(l, t, o), q(s, l, o), r = !0
         },
         p(l, o) {
             e = l;
-            const a = {};
-            o[0] & 128 && (a.rowAttrs = e[31].attrs()), o[0] & 129 | o[1] & 16392 && (a.$$scope = {
+            const i = {};
+            o[0] & 64 && (i.rowAttrs = e[28].attrs()), o[0] & 64 | o[1] & 2049 && (i.$$scope = {
                 dirty: o,
                 ctx: e
-            }), s.$set(a)
+            }), s.$set(i)
         },
         i(l) {
-            r || (I(s.$$.fragment, l), r = !0)
+            r || (E(s.$$.fragment, l), r = !0)
         },
         o(l) {
-            S(s.$$.fragment, l), r = !1
+            F(s.$$.fragment, l), r = !1
         },
         d(l) {
-            l && g(t), K(s, l)
+            l && _(t), U(s, l)
         }
     }
 }
 
-function al(n) {
+function fl(n) {
     let e, t, s, r = "Column settings",
-        l, o, a = "Drag and drop to re-order, toggle box for visibility.",
-        i, c, d, w, y, m, b, f, u, h, p, v = [],
-        R = new Map,
-        ee, V, k = [],
-        U = new Map,
-        W;
-    d = new ir({
+        l, o, i = "Drag and drop to re-order, toggle box for visibility.",
+        a, c, d, $, k, g, m, u, f, h, p, b = [],
+        B = new Map,
+        S, O, G = [],
+        ve = new Map,
+        ie;
+    d = new el({
         props: {
-            list: n[3],
+            list: n[2],
             $$slots: {
-                default: [el, ({
-                    item: _
+                default: [rl, ({
+                    item: w
                 }) => ({
-                    44: _
+                    41: w
                 }), ({
-                    item: _
-                }) => [0, _ ? 8192 : 0]]
+                    item: w
+                }) => [0, w ? 1024 : 0]]
             },
             $$scope: {
                 ctx: n
             }
         }
-    }), d.$on("sort", n[13]), m = new Nt({
+    }), d.$on("sort", n[13]), g = new Gt({
         props: {
             class: "text-white",
             $$slots: {
-                default: [tl]
+                default: [ll]
             },
             $$scope: {
                 ctx: n
             }
         }
-    }), m.$on("click", n[18]);
-    let te = ie(n[5]);
-    const Fe = _ => _[39].id;
-    for (let _ = 0; _ < te.length; _ += 1) {
-        let E = bt(n, te, _),
-            H = Fe(E);
-        R.set(H, v[_] = wt(H, E))
-    }
-    let de = ie(n[7]);
-    const he = _ => _[31].id;
-    for (let _ = 0; _ < de.length; _ += 1) {
-        let E = gt(n, de, _),
-            H = he(E);
-        U.set(H, k[_] = yt(H, E))
-    }
-    let ge = [n[6]],
-        $e = {};
-    for (let _ = 0; _ < ge.length; _ += 1) $e = ue($e, ge[_]);
-    let Ee = [n[4], {
+    }), g.$on("click", n[17]);
+    let ae = oe(n[4]);
+    const Se = w => w[36].id;
+    for (let w = 0; w < ae.length; w += 1) {
+        let D = wt(n, ae, w),
+            N = Se(D);
+        B.set(N, b[w] = Et(N, D))
+    }
+    let he = oe(n[6]);
+    const $e = w => w[28].id;
+    for (let w = 0; w < he.length; w += 1) {
+        let D = vt(n, he, w),
+            N = $e(D);
+        ve.set(N, G[w] = It(N, D))
+    }
+    let pe = [n[5]],
+        _e = {};
+    for (let w = 0; w < pe.length; w += 1) _e = fe(_e, pe[w]);
+    let we = [n[3], {
             class: "table-auto z-0 w-full text-center text-base text-slate-800"
         }],
-        pe = {};
-    for (let _ = 0; _ < Ee.length; _ += 1) pe = ue(pe, Ee[_]);
+        M = {};
+    for (let w = 0; w < we.length; w += 1) M = fe(M, we[w]);
     return {
         c() {
-            e = j("div"), t = j("div"), s = j("span"), s.textContent = r, l = P(), o = j("span"), o.textContent = a, i = P(), c = j("div"), z(d.$$.fragment), w = P(), y = j("div"), z(m.$$.fragment), f = P(), u = j("div"), h = j("table"), p = j("thead");
-            for (let _ = 0; _ < v.length; _ += 1) v[_].c();
-            ee = P(), V = j("tbody");
-            for (let _ = 0; _ < k.length; _ += 1) k[_].c();
+            e = j("div"), t = j("div"), s = j("span"), s.textContent = r, l = L(), o = j("span"), o.textContent = i, a = L(), c = j("div"), K(d.$$.fragment), $ = L(), k = j("div"), K(g.$$.fragment), u = L(), f = j("div"), h = j("table"), p = j("thead");
+            for (let w = 0; w < b.length; w += 1) b[w].c();
+            S = L(), O = j("tbody");
+            for (let w = 0; w < G.length; w += 1) G[w].c();
             this.h()
         },
-        l(_) {
-            e = A(_, "DIV", {
+        l(w) {
+            e = A(w, "DIV", {
                 class: !0
             });
-            var E = M(e);
-            t = A(E, "DIV", {
+            var D = R(e);
+            t = A(D, "DIV", {
                 class: !0
             });
-            var H = M(t);
-            s = A(H, "SPAN", {
+            var N = R(t);
+            s = A(N, "SPAN", {
                 class: !0,
                 "data-svelte-h": !0
-            }), ve(s) !== "svelte-1k4dd0o" && (s.textContent = r), l = L(H), o = A(H, "SPAN", {
+            }), be(s) !== "svelte-1k4dd0o" && (s.textContent = r), l = V(N), o = A(N, "SPAN", {
                 class: !0,
                 "data-svelte-h": !0
-            }), ve(o) !== "svelte-du859n" && (o.textContent = a), i = L(H), c = A(H, "DIV", {
+            }), be(o) !== "svelte-du859n" && (o.textContent = i), a = V(N), c = A(N, "DIV", {
                 class: !0
             });
-            var Ce = M(c);
-            J(d.$$.fragment, Ce), Ce.forEach(g), w = L(H), y = A(H, "DIV", {
+            var Ce = R(c);
+            W(d.$$.fragment, Ce), Ce.forEach(_), $ = V(N), k = A(N, "DIV", {
                 class: !0
             });
-            var Be = M(y);
-            J(m.$$.fragment, Be), Be.forEach(g), H.forEach(g), E.forEach(g), f = L(_), u = A(_, "DIV", {
+            var Be = R(k);
+            W(g.$$.fragment, Be), Be.forEach(_), N.forEach(_), D.forEach(_), u = V(w), f = A(w, "DIV", {
                 class: !0
             });
-            var T = M(u);
-            h = A(T, "TABLE", {
+            var C = R(f);
+            h = A(C, "TABLE", {
                 class: !0
             });
-            var B = M(h);
-            p = A(B, "THEAD", {});
-            var O = M(p);
-            for (let X = 0; X < v.length; X += 1) v[X].l(O);
-            O.forEach(g), ee = L(B), V = A(B, "TBODY", {});
-            var Q = M(V);
-            for (let X = 0; X < k.length; X += 1) k[X].l(Q);
-            Q.forEach(g), B.forEach(g), T.forEach(g), this.h()
+            var H = R(h);
+            p = A(H, "THEAD", {});
+            var P = R(p);
+            for (let X = 0; X < b.length; X += 1) b[X].l(P);
+            P.forEach(_), S = V(H), O = A(H, "TBODY", {});
+            var Q = R(O);
+            for (let X = 0; X < G.length; X += 1) G[X].l(Q);
+            Q.forEach(_), H.forEach(_), C.forEach(_), this.h()
         },
         h() {
-            $(s, "class", "text-3xl font-bold mb-4"), $(o, "class", "text-sm italic text-gray-500 font-medium mb-3"), $(c, "class", "flex flex-col space-y-2"), $(y, "class", "my-6 flex justify-end items-end"), $(t, "class", "px-12 pt-10 flex flex-col bg-white border border-slate-300 shadow-sm shadow-slate-300 rounded-lg"), $(e, "class", b = "fixed w-full h-full z-20 top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-gray-500/30 backdrop:blur-lg flex items-center justify-center font-Montserrat " + (n[2] ? "block" : "hidden")), ce(V, $e), ce(h, pe), $(u, "class", "h-full w-full overflow-y-auto overflow-x-auto rounded-sm bg-white border border-slate-300 shadow-sm shadow-slate-300 font-Montserrat")
+            v(s, "class", "text-3xl font-bold mb-4"), v(o, "class", "text-sm italic text-gray-500 font-medium mb-3"), v(c, "class", "flex flex-col space-y-2"), v(k, "class", "my-6 flex justify-end items-end"), v(t, "class", "px-12 pt-10 flex flex-col bg-white border border-slate-300 shadow-sm shadow-slate-300 rounded-lg"), v(e, "class", m = "fixed w-full h-full z-20 top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-gray-500/30 backdrop:blur-lg flex items-center justify-center font-Montserrat " + (n[1] ? "block" : "hidden")), ce(O, _e), ce(h, M), v(f, "class", "h-full w-full overflow-y-auto overflow-x-auto rounded-sm bg-white border border-slate-300 shadow-sm shadow-slate-300 font-Montserrat")
         },
-        m(_, E) {
-            F(_, e, E), C(e, t), C(t, s), C(t, l), C(t, o), C(t, i), C(t, c), G(d, c, null), C(t, w), C(t, y), G(m, y, null), F(_, f, E), F(_, u, E), C(u, h), C(h, p);
-            for (let H = 0; H < v.length; H += 1) v[H] && v[H].m(p, null);
-            C(h, ee), C(h, V);
-            for (let H = 0; H < k.length; H += 1) k[H] && k[H].m(V, null);
-            W = !0
+        m(w, D) {
+            T(w, e, D), y(e, t), y(t, s), y(t, l), y(t, o), y(t, a), y(t, c), q(d, c, null), y(t, $), y(t, k), q(g, k, null), T(w, u, D), T(w, f, D), y(f, h), y(h, p);
+            for (let N = 0; N < b.length; N += 1) b[N] && b[N].m(p, null);
+            y(h, S), y(h, O);
+            for (let N = 0; N < G.length; N += 1) G[N] && G[N].m(O, null);
+            ie = !0
         },
-        p(_, E) {
-            const H = {};
-            E[0] & 8 && (H.list = _[3]), E[0] & 2 | E[1] & 24576 && (H.$$scope = {
-                dirty: E,
-                ctx: _
-            }), d.$set(H);
+        p(w, D) {
+            const N = {};
+            D[0] & 4 && (N.list = w[2]), D[0] & 1 | D[1] & 3072 && (N.$$scope = {
+                dirty: D,
+                ctx: w
+            }), d.$set(N);
             const Ce = {};
-            E[1] & 16384 && (Ce.$$scope = {
-                dirty: E,
-                ctx: _
-            }), m.$set(Ce), (!W || E[0] & 4 && b !== (b = "fixed w-full h-full z-20 top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-gray-500/30 backdrop:blur-lg flex items-center justify-center font-Montserrat " + (_[2] ? "block" : "hidden"))) && $(e, "class", b), E[0] & 36 | E[1] & 136 && (te = ie(_[5]), Z(), v = Me(v, E, Fe, 1, _, te, R, p, Le, wt, null, bt), x()), E[0] & 32897 | E[1] & 136 && (de = ie(_[7]), Z(), k = Me(k, E, he, 1, _, de, U, V, Le, yt, null, gt), x()), ce(V, $e = _e(ge, [E[0] & 64 && _[6]])), ce(h, pe = _e(Ee, [E[0] & 16 && _[4], {
+            D[1] & 2048 && (Ce.$$scope = {
+                dirty: D,
+                ctx: w
+            }), g.$set(Ce), (!ie || D[0] & 2 && m !== (m = "fixed w-full h-full z-20 top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-gray-500/30 backdrop:blur-lg flex items-center justify-center font-Montserrat " + (w[1] ? "block" : "hidden"))) && v(e, "class", m), D[0] & 18 | D[1] & 17 && (ae = oe(w[4]), Z(), b = Me(b, D, Se, 1, w, ae, B, p, Pe, Et, null, wt), x()), D[0] & 192 | D[1] & 17 && (he = oe(w[6]), Z(), G = Me(G, D, $e, 1, w, he, ve, O, Pe, It, null, vt), x()), ce(O, _e = de(pe, [D[0] & 32 && w[5]])), ce(h, M = de(we, [D[0] & 8 && w[3], {
                 class: "table-auto z-0 w-full text-center text-base text-slate-800"
             }]))
         },
-        i(_) {
-            if (!W) {
-                I(d.$$.fragment, _), I(m.$$.fragment, _);
-                for (let E = 0; E < te.length; E += 1) I(v[E]);
-                for (let E = 0; E < de.length; E += 1) I(k[E]);
-                W = !0
+        i(w) {
+            if (!ie) {
+                E(d.$$.fragment, w), E(g.$$.fragment, w);
+                for (let D = 0; D < ae.length; D += 1) E(b[D]);
+                for (let D = 0; D < he.length; D += 1) E(G[D]);
+                ie = !0
             }
         },
-        o(_) {
-            S(d.$$.fragment, _), S(m.$$.fragment, _);
-            for (let E = 0; E < v.length; E += 1) S(v[E]);
-            for (let E = 0; E < k.length; E += 1) S(k[E]);
-            W = !1
+        o(w) {
+            F(d.$$.fragment, w), F(g.$$.fragment, w);
+            for (let D = 0; D < b.length; D += 1) F(b[D]);
+            for (let D = 0; D < G.length; D += 1) F(G[D]);
+            ie = !1
         },
-        d(_) {
-            _ && (g(e), g(f), g(u)), K(d), K(m);
-            for (let E = 0; E < v.length; E += 1) v[E].d();
-            for (let E = 0; E < k.length; E += 1) k[E].d()
+        d(w) {
+            w && (_(e), _(u), _(f)), U(d), U(g);
+            for (let D = 0; D < b.length; D += 1) b[D].d();
+            for (let D = 0; D < G.length; D += 1) G[D].d()
         }
     }
 }
 
-function il(n, e, t) {
-    let s, r, l, o, a, i, {
+function ul(n, e, t) {
+    var _e, we;
+    let s, r, l, o, i, a, {
         items: c
     } = e;
-    const d = Ie(c),
-        w = Yr(d, {
-            colOrder: Zr(),
-            hideCols: xr()
-        });
-    let y = [],
-        m = [],
-        b = [];
-    const f = _ => jr(sr, {
-        itemFeature: _.value
-    });
-    Object.values(c[0]).forEach(_ => {
-        y.push(w.column({
-            header: _.name,
-            cell: f,
-            accessor: E => E.find(H => H.name === _.name)
-        })), _.dtype === "image" || _.dtype === "video" ? m.push(_.name) : b.push(_.name)
+    const d = Qe();
+
+    function $(M) {
+        d("selectItem", M)
+    }
+    const k = Ie(c),
+        g = Ur(k, {
+            colOrder: tl(),
+            hideCols: sl()
+        });
+    let m = [g.column({
+            header: "ID",
+            cell: pt,
+            accessor: "id"
+        }), g.column({
+            header: "Split",
+            cell: pt,
+            accessor: "split"
+        })],
+        u = [];
+    (_e = c[0]) != null && _e.views && Object.values(c[0].views).forEach(({
+        id: M
+    }) => {
+        m.push(g.column({
+            header: M,
+            cell: Wr,
+            accessor: w => JSON.stringify(w.views[M])
+        })), u.push(M)
+    }), u.push("id"), u.push("split"), (we = c[0]) != null && we.features && Object.values(c[0].features).forEach(({
+        name: M
+    }) => {
+        m.push(g.column({
+            header: M,
+            cell: Jr,
+            accessor: w => JSON.stringify(w.features[M])
+        })), u.push(M)
     });
-    let u = [...m, ...b];
-    const h = w.createColumns(y),
+    const f = g.createColumns(m),
         {
-            headerRows: p,
-            rows: v,
-            tableAttrs: R,
-            tableBodyAttrs: ee,
-            pluginStates: V
-        } = w.createViewModel(h);
-    ye(n, p, _ => t(5, o = _)), ye(n, v, _ => t(7, i = _)), ye(n, R, _ => t(4, l = _)), ye(n, ee, _ => t(6, a = _));
+            headerRows: h,
+            rows: p,
+            tableAttrs: b,
+            tableBodyAttrs: B,
+            pluginStates: S
+        } = g.createViewModel(f);
+    Ee(n, h, M => t(4, o = M)), Ee(n, p, M => t(6, a = M)), Ee(n, b, M => t(3, l = M)), Ee(n, B, M => t(5, i = M));
     const {
-        columnIdOrder: k
-    } = V.colOrder;
-    ye(n, k, _ => t(3, r = _)), qe(k, r = [...u], r);
-    const U = _ => {
-            qe(k, r = _.detail, r)
+        columnIdOrder: O
+    } = S.colOrder;
+    Ee(n, O, M => t(2, r = M)), Je(O, r = [...u], r);
+    const G = M => {
+            Je(O, r = M.detail, r)
         },
         {
-            hiddenColumnIds: W
-        } = V.hideCols;
-    ye(n, W, _ => t(21, s = _));
-    let te = Object.fromEntries(r.map(_ => [_, !0]));
-    const Fe = Ue();
-
-    function de(_) {
-        Fe("selectItem", _)
-    }
-    let he = !1;
-
-    function ge(_, E) {
-        n.$$.not_equal(te[E], _) && (te[E] = _, t(1, te))
-    }
-    const $e = () => {
-            t(2, he = !1)
-        },
-        Ee = () => {
-            t(2, he = !0)
-        },
-        pe = _ => {
-            for (const E of c[_.id])
-                if (E.name === "id") {
-                    de(E.value);
-                    return
-                }
+            hiddenColumnIds: ve
+        } = S.hideCols;
+    Ee(n, ve, M => t(20, s = M));
+    let ie = Object.fromEntries(r.map(M => [M, !0])),
+        ae = !1;
+
+    function Se(M, w) {
+        n.$$.not_equal(ie[w], M) && (ie[w] = M, t(0, ie))
+    }
+    const he = () => {
+            t(1, ae = !1)
+        },
+        $e = () => {
+            t(1, ae = !0)
+        },
+        pe = M => {
+            $(M.original.id)
         };
-    return n.$$set = _ => {
-        "items" in _ && t(0, c = _.items)
+    return n.$$set = M => {
+        "items" in M && t(15, c = M.items)
     }, n.$$.update = () => {
-        n.$$.dirty[0] & 2 && qe(W, s = Object.entries(te).filter(([, _]) => !_).map(([_]) => _), s)
-    }, [c, te, he, r, l, o, a, i, p, v, R, ee, k, U, W, de, f, ge, $e, Ee, pe]
+        n.$$.dirty[0] & 1 && Je(ve, s = Object.entries(ie).filter(([, M]) => !M).map(([M]) => M), s)
+    }, [ie, ae, r, l, o, i, a, $, h, p, b, B, O, G, ve, c, Se, he, $e, pe]
 }
-class cl extends re {
+class dl extends te {
     constructor(e) {
-        super(), le(this, e, il, al, se, {
-            items: 0,
-            FeatureCell: 16
+        super(), se(this, e, ul, fl, ee, {
+            items: 15
         }, null, [-1, -1])
     }
-    get FeatureCell() {
-        return this.$$.ctx[16]
-    }
 }
 
-function Et(n, e, t) {
+function Tt(n, e, t) {
     const s = n.slice();
-    return s[19] = e[t], s
+    return s[18] = e[t], s
 }
 
-function Ct(n) {
-    let e, t, s, r, l, o, a, i, c, d, w, y = n[7].length > 0 && ul(n);
-    const m = [hl, dl, fl],
-        b = [];
+function Dt(n) {
+    let e, t, s, r, l, o, i, a, c, d, $, k = n[7].length > 0 && hl(n);
+    const g = [gl, _l, pl],
+        m = [];
 
-    function f(h, p) {
+    function u(h, p) {
         return h[1] ? 0 : h[0].isErrored ? 2 : 1
     }
-    a = f(n), i = b[a] = m[a](n);
-    let u = !n[0].isErrored && Dt(n);
+    i = u(n), a = m[i] = g[i](n);
+    let f = !n[0].isErrored && jt(n);
     return {
         c() {
-            e = j("div"), t = j("div"), s = j("div"), r = P(), l = j("div"), y && y.c(), o = P(), i.c(), c = P(), u && u.c(), d = N(), this.h()
+            e = j("div"), t = j("div"), s = j("div"), r = L(), l = j("div"), k && k.c(), o = L(), a.c(), c = L(), f && f.c(), d = z(), this.h()
         },
         l(h) {
             e = A(h, "DIV", {
                 class: !0
             });
-            var p = M(e);
+            var p = R(e);
             t = A(p, "DIV", {
                 class: !0
             });
-            var v = M(t);
-            s = A(v, "DIV", {
+            var b = R(t);
+            s = A(b, "DIV", {
                 class: !0
-            }), M(s).forEach(g), r = L(v), l = A(v, "DIV", {
+            }), R(s).forEach(_), r = V(b), l = A(b, "DIV", {
                 class: !0
             });
-            var R = M(l);
-            y && y.l(R), R.forEach(g), v.forEach(g), o = L(p), i.l(p), p.forEach(g), c = L(h), u && u.l(h), d = N(), this.h()
+            var B = R(l);
+            k && k.l(B), B.forEach(_), b.forEach(_), o = V(p), a.l(p), p.forEach(_), c = V(h), f && f.l(h), d = z(), this.h()
         },
         h() {
-            $(s, "class", "flex-grow"), $(l, "class", "relative flex items-center"), $(t, "class", "py-5 h-20 flex space-x-2 items-center"), $(e, "class", "w-full h-full flex flex-col")
+            v(s, "class", "flex-grow"), v(l, "class", "relative flex items-center"), v(t, "class", "py-5 h-20 flex space-x-2 items-center"), v(e, "class", "w-full h-full flex flex-col")
         },
         m(h, p) {
-            F(h, e, p), C(e, t), C(t, s), C(t, r), C(t, l), y && y.m(l, null), C(e, o), b[a].m(e, null), F(h, c, p), u && u.m(h, p), F(h, d, p), w = !0
+            T(h, e, p), y(e, t), y(t, s), y(t, r), y(t, l), k && k.m(l, null), y(e, o), m[i].m(e, null), T(h, c, p), f && f.m(h, p), T(h, d, p), $ = !0
         },
         p(h, p) {
-            h[7].length > 0 && y.p(h, p);
-            let v = a;
-            a = f(h), a === v ? b[a].p(h, p) : (Z(), S(b[v], 1, 1, () => {
-                b[v] = null
-            }), x(), i = b[a], i ? i.p(h, p) : (i = b[a] = m[a](h), i.c()), I(i, 1), i.m(e, null)), h[0].isErrored ? u && (u.d(1), u = null) : u ? u.p(h, p) : (u = Dt(h), u.c(), u.m(d.parentNode, d))
+            h[7].length > 0 && k.p(h, p);
+            let b = i;
+            i = u(h), i === b ? m[i].p(h, p) : (Z(), F(m[b], 1, 1, () => {
+                m[b] = null
+            }), x(), a = m[i], a ? a.p(h, p) : (a = m[i] = g[i](h), a.c()), E(a, 1), a.m(e, null)), h[0].isErrored ? f && (f.d(1), f = null) : f ? f.p(h, p) : (f = jt(h), f.c(), f.m(d.parentNode, d))
         },
         i(h) {
-            w || (I(i), w = !0)
+            $ || (E(a), $ = !0)
         },
         o(h) {
-            S(i), w = !1
+            F(a), $ = !1
         },
         d(h) {
-            h && (g(e), g(c), g(d)), y && y.d(), b[a].d(), u && u.d(h)
+            h && (_(e), _(c), _(d)), k && k.d(), m[i].d(), f && f.d(h)
         }
     }
 }
 
-function ul(n) {
-    let e, t, s, r, l, o, a, i, c, d, w, y = ie(n[7]),
-        m = [];
-    for (let f = 0; f < y.length; f += 1) m[f] = It(Et(n, y, f));
-    let b = n[5] !== "" && Tt(n);
+function hl(n) {
+    let e, t, s, r, l, o, i, a, c, d, $, k = oe(n[7]),
+        g = [];
+    for (let u = 0; u < k.length; u += 1) g[u] = St(Tt(n, k, u));
+    let m = n[5] !== "" && Ft(n);
     return {
         c() {
             e = j("select");
-            for (let f = 0; f < m.length; f += 1) m[f].c();
-            t = P(), s = j("div"), r = j("input"), o = P(), a = Te("svg"), i = Te("path"), c = P(), b && b.c(), this.h()
+            for (let u = 0; u < g.length; u += 1) g[u].c();
+            t = L(), s = j("div"), r = j("input"), o = L(), i = Te("svg"), a = Te("path"), c = L(), m && m.c(), this.h()
         },
-        l(f) {
-            e = A(f, "SELECT", {
+        l(u) {
+            e = A(u, "SELECT", {
                 class: !0
             });
-            var u = M(e);
-            for (let v = 0; v < m.length; v += 1) m[v].l(u);
-            u.forEach(g), t = L(f), s = A(f, "DIV", {
+            var f = R(e);
+            for (let b = 0; b < g.length; b += 1) g[b].l(f);
+            f.forEach(_), t = V(u), s = A(u, "DIV", {
                 class: !0
             });
-            var h = M(s);
+            var h = R(s);
             r = A(h, "INPUT", {
                 id: !0,
                 type: !0,
                 placeholder: !0,
                 class: !0
-            }), o = L(h), a = De(h, "svg", {
+            }), o = V(h), i = De(h, "svg", {
                 xmlns: !0,
                 height: !0,
                 viewBox: !0,
                 width: !0,
                 class: !0
             });
-            var p = M(a);
-            i = De(p, "path", {
+            var p = R(i);
+            a = De(p, "path", {
                 d: !0,
                 fill: !0
-            }), M(i).forEach(g), p.forEach(g), c = L(h), b && b.l(h), h.forEach(g), this.h()
+            }), R(a).forEach(_), p.forEach(_), c = V(h), m && m.l(h), h.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "h-10 px-4 mx-4 border rounded bg-slate-50 border-slate-300"), $(r, "id", "sem-search-input"), $(r, "type", "text"), r.value = n[5], $(r, "placeholder", l = "Semantic search using " + n[6]), $(r, "class", "h-10 pl-10 pr-4 rounded-full border text-slate-800 placeholder-slate-500 bg-slate-50 border-slate-300 shadow-slate-300 accent-main"), $(i, "d", $s), $(i, "fill", "currentcolor"), $(a, "xmlns", "http://www.w3.org/2000/svg"), $(a, "height", "48"), $(a, "viewBox", "0 -960 960 960"), $(a, "width", "48"), $(a, "class", "absolute left-2 h-5 w-5 text-slate-800 pointer-events-none"), $(s, "class", "relative flex items-center")
+            v(e, "class", "h-10 px-4 mx-4 border rounded bg-slate-50 border-slate-300"), v(r, "id", "sem-search-input"), v(r, "type", "text"), r.value = n[5], v(r, "placeholder", l = "Semantic search using " + n[6]), v(r, "class", "h-10 pl-10 pr-4 rounded-full border text-slate-800 placeholder-slate-500 bg-slate-50 border-slate-300 shadow-slate-300 accent-main"), v(a, "d", ys), v(a, "fill", "currentcolor"), v(i, "xmlns", "http://www.w3.org/2000/svg"), v(i, "height", "48"), v(i, "viewBox", "0 -960 960 960"), v(i, "width", "48"), v(i, "class", "absolute left-2 h-5 w-5 text-slate-800 pointer-events-none"), v(s, "class", "relative flex items-center")
         },
-        m(f, u) {
-            F(f, e, u);
-            for (let h = 0; h < m.length; h += 1) m[h] && m[h].m(e, null);
-            F(f, t, u), F(f, s, u), C(s, r), C(s, o), C(s, a), C(a, i), C(s, c), b && b.m(s, null), d || (w = ae(r, "change", n[14]), d = !0)
+        m(u, f) {
+            T(u, e, f);
+            for (let h = 0; h < g.length; h += 1) g[h] && g[h].m(e, null);
+            T(u, t, f), T(u, s, f), y(s, r), y(s, o), y(s, i), y(i, a), y(s, c), m && m.m(s, null), d || ($ = ne(r, "change", n[14]), d = !0)
         },
-        p(f, u) {
-            if (u & 192) {
-                y = ie(f[7]);
+        p(u, f) {
+            if (f & 192) {
+                k = oe(u[7]);
                 let h;
-                for (h = 0; h < y.length; h += 1) {
-                    const p = Et(f, y, h);
-                    m[h] ? m[h].p(p, u) : (m[h] = It(p), m[h].c(), m[h].m(e, null))
+                for (h = 0; h < k.length; h += 1) {
+                    const p = Tt(u, k, h);
+                    g[h] ? g[h].p(p, f) : (g[h] = St(p), g[h].c(), g[h].m(e, null))
                 }
-                for (; h < m.length; h += 1) m[h].d(1);
-                m.length = y.length
+                for (; h < g.length; h += 1) g[h].d(1);
+                g.length = k.length
             }
-            u & 32 && r.value !== f[5] && (r.value = f[5]), u & 64 && l !== (l = "Semantic search using " + f[6]) && $(r, "placeholder", l), f[5] !== "" ? b ? b.p(f, u) : (b = Tt(f), b.c(), b.m(s, null)) : b && (b.d(1), b = null)
+            f & 32 && r.value !== u[5] && (r.value = u[5]), f & 64 && l !== (l = "Semantic search using " + u[6]) && v(r, "placeholder", l), u[5] !== "" ? m ? m.p(u, f) : (m = Ft(u), m.c(), m.m(s, null)) : m && (m.d(1), m = null)
         },
-        d(f) {
-            f && (g(e), g(t), g(s)), Pt(m, f), b && b.d(), d = !1, w()
+        d(u) {
+            u && (_(e), _(t), _(s)), Vt(g, u), m && m.d(), d = !1, $()
         }
     }
 }
 
-function It(n) {
-    let e, t = n[19] + "",
+function St(n) {
+    let e, t = n[18] + "",
         s, r;
     return {
         c() {
-            e = j("option"), s = ne(t), r = P(), this.h()
+            e = j("option"), s = re(t), r = L(), this.h()
         },
         l(l) {
             e = A(l, "OPTION", {});
-            var o = M(e);
-            s = oe(o, t), r = L(o), o.forEach(g), this.h()
+            var o = R(e);
+            s = le(o, t), r = V(o), o.forEach(_), this.h()
         },
         h() {
-            e.__value = n[6], ot(e, e.__value)
+            e.__value = n[6], at(e, e.__value)
         },
         m(l, o) {
-            F(l, e, o), C(e, s), C(e, r)
+            T(l, e, o), y(e, s), y(e, r)
         },
         p(l, o) {
-            o & 64 && (e.__value = l[6], ot(e, e.__value))
+            o & 64 && (e.__value = l[6], at(e, e.__value))
         },
         d(l) {
-            l && g(e)
+            l && _(e)
         }
     }
 }
 
-function Tt(n) {
-    let e, t = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-5 w-5 text-slate-800"><path d="${ws}" fill="currentcolor"></path></svg>`,
+function Ft(n) {
+    let e, t = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-5 w-5 text-slate-800"><path d="${Es}" fill="currentcolor"></path></svg>`,
         s, r;
     return {
         c() {
             e = j("button"), e.innerHTML = t, this.h()
         },
         l(l) {
             e = A(l, "BUTTON", {
                 class: !0,
                 "data-svelte-h": !0
-            }), ve(e) !== "svelte-wv2rtu" && (e.innerHTML = t), this.h()
+            }), be(e) !== "svelte-wv2rtu" && (e.innerHTML = t), this.h()
         },
         h() {
-            $(e, "class", "absolute right-2 p-1 rounded-full transition-colors hover:bg-slate-300")
+            v(e, "class", "absolute right-2 p-1 rounded-full transition-colors hover:bg-slate-300")
         },
         m(l, o) {
-            F(l, e, o), s || (r = ae(e, "click", n[9]), s = !0)
+            T(l, e, o), s || (r = ne(e, "click", n[9]), s = !0)
         },
-        p: q,
+        p: J,
         d(l) {
-            l && g(e), s = !1, r()
+            l && _(e), s = !1, r()
         }
     }
 }
 
-function fl(n) {
+function pl(n) {
     let e, t, s = "Error: dataset items could not be loaded",
         r, l, o;
-    return l = new Fs({
+    return l = new As({
         props: {
             $$slots: {
-                default: [pl]
+                default: [ml]
             },
             $$scope: {
                 ctx: n
             }
         }
     }), l.$on("click", n[9]), {
         c() {
-            e = j("div"), t = j("p"), t.textContent = s, r = P(), z(l.$$.fragment), this.h()
+            e = j("div"), t = j("p"), t.textContent = s, r = L(), K(l.$$.fragment), this.h()
         },
-        l(a) {
-            e = A(a, "DIV", {
+        l(i) {
+            e = A(i, "DIV", {
                 class: !0
             });
-            var i = M(e);
-            t = A(i, "P", {
+            var a = R(e);
+            t = A(a, "P", {
                 "data-svelte-h": !0
-            }), ve(t) !== "svelte-lcj0vm" && (t.textContent = s), r = L(i), J(l.$$.fragment, i), i.forEach(g), this.h()
+            }), be(t) !== "svelte-lcj0vm" && (t.textContent = s), r = V(a), W(l.$$.fragment, a), a.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "flex flex-col gap-5 justify-center align-middle text-center max-w-xs m-auto mt-10")
+            v(e, "class", "flex flex-col gap-5 justify-center align-middle text-center max-w-xs m-auto mt-10")
         },
-        m(a, i) {
-            F(a, e, i), C(e, t), C(e, r), G(l, e, null), o = !0
+        m(i, a) {
+            T(i, e, a), y(e, t), y(e, r), q(l, e, null), o = !0
         },
-        p(a, i) {
+        p(i, a) {
             const c = {};
-            i & 4194304 && (c.$$scope = {
-                dirty: i,
-                ctx: a
+            a & 2097152 && (c.$$scope = {
+                dirty: a,
+                ctx: i
             }), l.$set(c)
         },
-        i(a) {
-            o || (I(l.$$.fragment, a), o = !0)
+        i(i) {
+            o || (E(l.$$.fragment, i), o = !0)
         },
-        o(a) {
-            S(l.$$.fragment, a), o = !1
+        o(i) {
+            F(l.$$.fragment, i), o = !1
         },
-        d(a) {
-            a && g(e), K(l)
+        d(i) {
+            i && _(e), U(l)
         }
     }
 }
 
-function dl(n) {
+function _l(n) {
     let e, t;
-    return e = new cl({
+    return e = new dl({
         props: {
-            items: n[15]
+            items: n[0].page.items
         }
-    }), e.$on("selectItem", n[16]), {
+    }), e.$on("selectItem", n[15]), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(s) {
-            J(e.$$.fragment, s)
+            W(e.$$.fragment, s)
         },
         m(s, r) {
-            G(e, s, r), t = !0
+            q(e, s, r), t = !0
+        },
+        p(s, r) {
+            const l = {};
+            r & 1 && (l.items = s[0].page.items), e.$set(l)
         },
-        p: q,
         i(s) {
-            t || (I(e.$$.fragment, s), t = !0)
+            t || (E(e.$$.fragment, s), t = !0)
         },
         o(s) {
-            S(e.$$.fragment, s), t = !1
+            F(e.$$.fragment, s), t = !1
         },
         d(s) {
-            K(e, s)
+            U(e, s)
         }
     }
 }
 
-function hl(n) {
+function gl(n) {
     let e, t, s;
-    return t = new js({
+    return t = new Rs({
         props: {
             class: "animate-spin"
         }
     }), {
         c() {
-            e = j("div"), z(t.$$.fragment), this.h()
+            e = j("div"), K(t.$$.fragment), this.h()
         },
         l(r) {
             e = A(r, "DIV", {
                 class: !0
             });
-            var l = M(e);
-            J(t.$$.fragment, l), l.forEach(g), this.h()
+            var l = R(e);
+            W(t.$$.fragment, l), l.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "flex-grow flex justify-center items-center")
+            v(e, "class", "flex-grow flex justify-center items-center")
         },
         m(r, l) {
-            F(r, e, l), G(t, e, null), s = !0
+            T(r, e, l), q(t, e, null), s = !0
         },
-        p: q,
+        p: J,
         i(r) {
-            s || (I(t.$$.fragment, r), s = !0)
+            s || (E(t.$$.fragment, r), s = !0)
         },
         o(r) {
-            S(t.$$.fragment, r), s = !1
+            F(t.$$.fragment, r), s = !1
         },
         d(r) {
-            r && g(e), K(t)
+            r && _(e), U(t)
         }
     }
 }
 
-function pl(n) {
+function ml(n) {
     let e;
     return {
         c() {
-            e = ne("Try again")
+            e = re("Try again")
         },
         l(t) {
-            e = oe(t, "Try again")
+            e = le(t, "Try again")
         },
         m(t, s) {
-            F(t, e, s)
+            T(t, e, s)
         },
         d(t) {
-            t && g(e)
+            t && _(e)
         }
     }
 }
 
-function Dt(n) {
+function jt(n) {
     let e, t, s, r = 1 + n[3] * (n[2] - 1) + "",
-        l, o, a = Math.min(n[3] * n[2], n[0].page.total) + "",
-        i, c, d = n[0].page.total + "",
-        w, y, m = n[0].page.total > n[3] && Ft(n),
-        b = n[0].page.total > n[3] && St(n);
+        l, o, i = Math.min(n[3] * n[2], n[0].page.total) + "",
+        a, c, d = n[0].page.total + "",
+        $, k, g = n[0].page.total > n[3] && At(n),
+        m = n[0].page.total > n[3] && Mt(n);
     return {
         c() {
-            e = j("div"), m && m.c(), t = P(), s = j("span"), l = ne(r), o = ne(" - "), i = ne(a), c = ne(` of
-          `), w = ne(d), y = P(), b && b.c(), this.h()
+            e = j("div"), g && g.c(), t = L(), s = j("span"), l = re(r), o = re(" - "), a = re(i), c = re(` of
+          `), $ = re(d), k = L(), m && m.c(), this.h()
         },
-        l(f) {
-            e = A(f, "DIV", {
+        l(u) {
+            e = A(u, "DIV", {
                 class: !0
             });
-            var u = M(e);
-            m && m.l(u), t = L(u), s = A(u, "SPAN", {
+            var f = R(e);
+            g && g.l(f), t = V(f), s = A(f, "SPAN", {
                 class: !0
             });
-            var h = M(s);
-            l = oe(h, r), o = oe(h, " - "), i = oe(h, a), c = oe(h, ` of
-          `), w = oe(h, d), h.forEach(g), y = L(u), b && b.l(u), u.forEach(g), this.h()
+            var h = R(s);
+            l = le(h, r), o = le(h, " - "), a = le(h, i), c = le(h, ` of
+          `), $ = le(h, d), h.forEach(_), k = V(f), m && m.l(f), f.forEach(_), this.h()
         },
         h() {
-            $(s, "class", "mx-4"), $(e, "class", "w-full py-5 h-20 flex justify-center items-center text-slate-800")
+            v(s, "class", "mx-4"), v(e, "class", "w-full py-5 h-20 flex justify-center items-center text-slate-800")
         },
-        m(f, u) {
-            F(f, e, u), m && m.m(e, null), C(e, t), C(e, s), C(s, l), C(s, o), C(s, i), C(s, c), C(s, w), C(e, y), b && b.m(e, null)
+        m(u, f) {
+            T(u, e, f), g && g.m(e, null), y(e, t), y(e, s), y(s, l), y(s, o), y(s, a), y(s, c), y(s, $), y(e, k), m && m.m(e, null)
         },
-        p(f, u) {
-            f[0].page.total > f[3] ? m ? m.p(f, u) : (m = Ft(f), m.c(), m.m(e, t)) : m && (m.d(1), m = null), u & 12 && r !== (r = 1 + f[3] * (f[2] - 1) + "") && be(l, r), u & 13 && a !== (a = Math.min(f[3] * f[2], f[0].page.total) + "") && be(i, a), u & 1 && d !== (d = f[0].page.total + "") && be(w, d), f[0].page.total > f[3] ? b ? b.p(f, u) : (b = St(f), b.c(), b.m(e, null)) : b && (b.d(1), b = null)
+        p(u, f) {
+            u[0].page.total > u[3] ? g ? g.p(u, f) : (g = At(u), g.c(), g.m(e, t)) : g && (g.d(1), g = null), f & 12 && r !== (r = 1 + u[3] * (u[2] - 1) + "") && me(l, r), f & 13 && i !== (i = Math.min(u[3] * u[2], u[0].page.total) + "") && me(a, i), f & 1 && d !== (d = u[0].page.total + "") && me($, d), u[0].page.total > u[3] ? m ? m.p(u, f) : (m = Mt(u), m.c(), m.m(e, null)) : m && (m.d(1), m = null)
         },
-        d(f) {
-            f && g(e), m && m.d(), b && b.d()
+        d(u) {
+            u && _(e), g && g.d(), m && m.d()
         }
     }
 }
 
-function Ft(n) {
-    let e, t = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${ks}" fill="currentcolor"></path></svg>`,
-        s, r, l = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${ys}" fill="currentcolor"></path></svg>`,
-        o, a;
+function At(n) {
+    let e, t = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${Cs}" fill="currentcolor"></path></svg>`,
+        s, r, l = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${Is}" fill="currentcolor"></path></svg>`,
+        o, i;
     return {
         c() {
-            e = j("button"), e.innerHTML = t, s = P(), r = j("button"), r.innerHTML = l
+            e = j("button"), e.innerHTML = t, s = L(), r = j("button"), r.innerHTML = l
         },
-        l(i) {
-            e = A(i, "BUTTON", {
+        l(a) {
+            e = A(a, "BUTTON", {
                 "data-svelte-h": !0
-            }), ve(e) !== "svelte-18zo4xr" && (e.innerHTML = t), s = L(i), r = A(i, "BUTTON", {
+            }), be(e) !== "svelte-18zo4xr" && (e.innerHTML = t), s = V(a), r = A(a, "BUTTON", {
                 "data-svelte-h": !0
-            }), ve(r) !== "svelte-1n17f1n" && (r.innerHTML = l)
+            }), be(r) !== "svelte-1n17f1n" && (r.innerHTML = l)
         },
-        m(i, c) {
-            F(i, e, c), F(i, s, c), F(i, r, c), o || (a = [ae(e, "click", n[10]), ae(r, "click", n[11])], o = !0)
+        m(a, c) {
+            T(a, e, c), T(a, s, c), T(a, r, c), o || (i = [ne(e, "click", n[10]), ne(r, "click", n[11])], o = !0)
         },
-        p: q,
-        d(i) {
-            i && (g(e), g(s), g(r)), o = !1, Ne(a)
+        p: J,
+        d(a) {
+            a && (_(e), _(s), _(r)), o = !1, ze(i)
         }
     }
 }
 
-function St(n) {
-    let e, t = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${Es}" fill="currentcolor"></path></svg>`,
-        s, r, l = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${Cs}" fill="currentcolor"></path></svg>`,
-        o, a;
+function Mt(n) {
+    let e, t = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${Ts}" fill="currentcolor"></path></svg>`,
+        s, r, l = `<svg xmlns="http://www.w3.org/2000/svg" height="48" viewBox="0 -960 960 960" width="48" class="h-8 w-8 p-1 rounded-full transition-colors hover:bg-slate-300"><path d="${Ds}" fill="currentcolor"></path></svg>`,
+        o, i;
     return {
         c() {
-            e = j("button"), e.innerHTML = t, s = P(), r = j("button"), r.innerHTML = l
+            e = j("button"), e.innerHTML = t, s = L(), r = j("button"), r.innerHTML = l
         },
-        l(i) {
-            e = A(i, "BUTTON", {
+        l(a) {
+            e = A(a, "BUTTON", {
                 "data-svelte-h": !0
-            }), ve(e) !== "svelte-1d9o6d7" && (e.innerHTML = t), s = L(i), r = A(i, "BUTTON", {
+            }), be(e) !== "svelte-1d9o6d7" && (e.innerHTML = t), s = V(a), r = A(a, "BUTTON", {
                 "data-svelte-h": !0
-            }), ve(r) !== "svelte-92h5yb" && (r.innerHTML = l)
+            }), be(r) !== "svelte-92h5yb" && (r.innerHTML = l)
         },
-        m(i, c) {
-            F(i, e, c), F(i, s, c), F(i, r, c), o || (a = [ae(e, "click", n[12]), ae(r, "click", n[13])], o = !0)
+        m(a, c) {
+            T(a, e, c), T(a, s, c), T(a, r, c), o || (i = [ne(e, "click", n[12]), ne(r, "click", n[13])], o = !0)
         },
-        p: q,
-        d(i) {
-            i && (g(e), g(s), g(r)), o = !1, Ne(a)
+        p: J,
+        d(a) {
+            a && (_(e), _(s), _(r)), o = !1, ze(i)
         }
     }
 }
 
-function jt(n) {
+function Rt(n) {
     let e, t;
-    return e = new Ds({
+    return e = new js({
         props: {
             message: "Error while retrieving dataset items.",
             details: "Please look at the application logs for more information, and report this issue if the error persists."
         }
-    }), e.$on("confirm", n[17]), {
+    }), e.$on("confirm", n[16]), {
         c() {
-            z(e.$$.fragment)
+            K(e.$$.fragment)
         },
         l(s) {
-            J(e.$$.fragment, s)
+            W(e.$$.fragment, s)
         },
         m(s, r) {
-            G(e, s, r), t = !0
+            q(e, s, r), t = !0
         },
-        p: q,
+        p: J,
         i(s) {
-            t || (I(e.$$.fragment, s), t = !0)
+            t || (E(e.$$.fragment, s), t = !0)
         },
         o(s) {
-            S(e.$$.fragment, s), t = !1
+            F(e.$$.fragment, s), t = !1
         },
         d(s) {
-            K(e, s)
+            U(e, s)
         }
     }
 }
 
-function _l(n) {
-    let e, t, s, r, l = n[0].page && Ct(n),
-        o = n[4] && jt(n),
-        a = gl;
+function bl(n) {
+    let e, t, s, r, l = n[0].page && Dt(n),
+        o = n[4] && Rt(n),
+        i = vl;
     return {
         c() {
-            e = j("div"), l && l.c(), t = P(), o && o.c(), s = P(), this.h()
+            e = j("div"), l && l.c(), t = L(), o && o.c(), s = L(), this.h()
         },
-        l(i) {
-            e = A(i, "DIV", {
+        l(a) {
+            e = A(a, "DIV", {
                 class: !0
             });
-            var c = M(e);
-            l && l.l(c), t = L(c), o && o.l(c), s = L(c), c.forEach(g), this.h()
+            var c = R(e);
+            l && l.l(c), t = V(c), o && o.l(c), s = V(c), c.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "w-full px-20 bg-slate-50 flex flex-col text-slate-800 min-h-[calc(100vh-80px)]")
+            v(e, "class", "w-full px-20 bg-slate-50 flex flex-col text-slate-800 min-h-[calc(100vh-80px)]")
         },
-        m(i, c) {
-            F(i, e, c), l && l.m(e, null), C(e, t), o && o.m(e, null), C(e, s), r = !0
+        m(a, c) {
+            T(a, e, c), l && l.m(e, null), y(e, t), o && o.m(e, null), y(e, s), r = !0
         },
-        p(i, [c]) {
-            i[0].page ? l ? (l.p(i, c), c & 1 && I(l, 1)) : (l = Ct(i), l.c(), I(l, 1), l.m(e, t)) : l && (Z(), S(l, 1, 1, () => {
+        p(a, [c]) {
+            a[0].page ? l ? (l.p(a, c), c & 1 && E(l, 1)) : (l = Dt(a), l.c(), E(l, 1), l.m(e, t)) : l && (Z(), F(l, 1, 1, () => {
                 l = null
-            }), x()), i[4] ? o ? (o.p(i, c), c & 16 && I(o, 1)) : (o = jt(i), o.c(), I(o, 1), o.m(e, s)) : o && (Z(), S(o, 1, 1, () => {
+            }), x()), a[4] ? o ? (o.p(a, c), c & 16 && E(o, 1)) : (o = Rt(a), o.c(), E(o, 1), o.m(e, s)) : o && (Z(), F(o, 1, 1, () => {
                 o = null
             }), x())
         },
-        i(i) {
-            r || (I(l), I(o), I(a), r = !0)
+        i(a) {
+            r || (E(l), E(o), E(i), r = !0)
         },
-        o(i) {
-            S(l), S(o), S(a), r = !1
+        o(a) {
+            F(l), F(o), F(i), r = !1
         },
-        d(i) {
-            i && g(e), l && l.d(), o && o.d()
+        d(a) {
+            a && _(e), l && l.d(), o && o.d()
         }
     }
 }
-let gl = !1;
+let vl = !1;
 
-function ml(n, e, t) {
-    var V;
+function $l(n, e, t) {
     let {
         selectedDataset: s
     } = e, r = !1, l, o;
-    Se.subscribe(k => {
-        t(2, l = (k == null ? void 0 : k.currentPage) || ps), t(3, o = (k == null ? void 0 : k.pageSize) || _s)
+    Fe.subscribe(S => {
+        t(2, l = (S == null ? void 0 : S.currentPage) || ms), t(3, o = (S == null ? void 0 : S.pageSize) || bs)
     });
-    let a = !1,
-        i = "",
+    let i = !1,
+        a = "",
         c;
     const d = [];
     if ("embeddings" in s.tables)
-        for (const k of s.tables.embeddings) k.type == "search" && (c || (c = k.source), d.push(k.source));
-    const w = Ue();
+        for (const S of s.tables.embeddings) S.type == "search" && (c || (c = S.source), d.push(S.source));
+    const $ = Qe();
 
-    function y(k) {
-        w("selectItem", k)
+    function k(S) {
+        $("selectItem", S)
     }
 
-    function m() {
+    function g() {
         document.getElementById("sem-search-input").value = "", p()
     }
 
-    function b() {
-        l > 1 && (t(1, r = !0), Se.update(k => ({
-            ...k,
-            pageSize: (k == null ? void 0 : k.pageSize) || o,
+    function m() {
+        l > 1 && (t(1, r = !0), Fe.update(S => ({
+            ...S,
+            pageSize: (S == null ? void 0 : S.pageSize) || o,
             currentPage: 1
         })))
     }
 
-    function f() {
-        l > 1 && (t(1, r = !0), Se.update(k => ({
-            ...k,
-            pageSize: (k == null ? void 0 : k.pageSize) || o,
+    function u() {
+        l > 1 && (t(1, r = !0), Fe.update(S => ({
+            ...S,
+            pageSize: (S == null ? void 0 : S.pageSize) || o,
             currentPage: l - 1
         })))
     }
 
-    function u() {
-        var k;
-        (((k = s.page) == null ? void 0 : k.total) || 1) > l * o && (t(1, r = !0), Se.update(U => ({
-            ...U,
-            pageSize: (U == null ? void 0 : U.pageSize) || o,
+    function f() {
+        var S;
+        (((S = s.page) == null ? void 0 : S.total) || 1) > l * o && (t(1, r = !0), Fe.update(O => ({
+            ...O,
+            pageSize: (O == null ? void 0 : O.pageSize) || o,
             currentPage: l + 1
         })))
     }
 
     function h() {
-        var k;
-        (((k = s.page) == null ? void 0 : k.total) || 1) > l * o && (t(1, r = !0), Se.update(U => {
-            var W;
+        var S;
+        (((S = s.page) == null ? void 0 : S.total) || 1) > l * o && (t(1, r = !0), Fe.update(O => {
+            var G;
             return {
-                ...U,
-                pageSize: (U == null ? void 0 : U.pageSize) || o,
-                currentPage: Math.ceil((((W = s.page) == null ? void 0 : W.total) || 1) / o)
+                ...O,
+                pageSize: (O == null ? void 0 : O.pageSize) || o,
+                currentPage: Math.ceil((((G = s.page) == null ? void 0 : G.total) || 1) / o)
             }
         }))
     }
 
     function p() {
-        t(5, i = document.getElementById("sem-search-input").value);
-        let k = {
+        t(5, a = document.getElementById("sem-search-input").value);
+        let S = {
             model: c,
-            search: i
+            search: a
         };
-        t(1, r = !0), Se.update(U => ({
-            ...U,
+        t(1, r = !0), Fe.update(O => ({
+            ...O,
             currentPage: 1,
-            query: k
+            query: S
         }))
     }
-    let v = [];
-    (V = s.page) == null || V.items.forEach(k => {
-        let U = [];
-        U.push({
-            name: "id",
-            dtype: "int",
-            value: k.id
-        }), U.push({
-            name: "split",
-            dtype: "str",
-            value: k.split
-        }), Object.values(k.views).forEach(W => {
-            U.push({
-                name: W.id,
-                dtype: "image",
-                value: W.thumbnail
-            })
-        }), Object.values(k.features).forEach(W => {
-            U.push({
-                name: W.name,
-                dtype: W.dtype,
-                value: W.value
-            })
-        }), v.push(U)
-    });
-    const R = k => y(k.detail),
-        ee = () => t(4, a = !1);
-    return n.$$set = k => {
-        "selectedDataset" in k && t(0, s = k.selectedDataset)
+    const b = S => k(S.detail),
+        B = () => t(4, i = !1);
+    return n.$$set = S => {
+        "selectedDataset" in S && t(0, s = S.selectedDataset)
     }, n.$$.update = () => {
-        var k;
-        n.$$.dirty & 1 && (k = s.page) != null && k.items && t(1, r = !1)
-    }, [s, r, l, o, a, i, c, d, y, m, b, f, u, h, p, v, R, ee]
+        var S;
+        n.$$.dirty & 1 && (S = s.page) != null && S.items && t(1, r = !1)
+    }, [s, r, l, o, i, a, c, d, k, g, m, u, f, h, p, b, B]
 }
-class bl extends re {
+class wl extends te {
     constructor(e) {
-        super(), le(this, e, ml, _l, se, {
+        super(), se(this, e, $l, bl, ee, {
             selectedDataset: 0
         })
     }
 }
 
-function At(n) {
+function Bt(n) {
     let e, t, s;
-    return t = new bl({
+    return t = new wl({
         props: {
             selectedDataset: n[0]
         }
     }), t.$on("selectItem", n[2]), {
         c() {
-            e = j("div"), z(t.$$.fragment), this.h()
+            e = j("div"), K(t.$$.fragment), this.h()
         },
         l(r) {
             e = A(r, "DIV", {
                 class: !0
             });
-            var l = M(e);
-            J(t.$$.fragment, l), l.forEach(g), this.h()
+            var l = R(e);
+            W(t.$$.fragment, l), l.forEach(_), this.h()
         },
         h() {
-            $(e, "class", "pt-20 h-1 min-h-screen")
+            v(e, "class", "pt-20 h-1 min-h-screen")
         },
         m(r, l) {
-            F(r, e, l), G(t, e, null), s = !0
+            T(r, e, l), q(t, e, null), s = !0
         },
         p(r, l) {
             const o = {};
             l & 1 && (o.selectedDataset = r[0]), t.$set(o)
         },
         i(r) {
-            s || (I(t.$$.fragment, r), s = !0)
+            s || (E(t.$$.fragment, r), s = !0)
         },
         o(r) {
-            S(t.$$.fragment, r), s = !1
+            F(t.$$.fragment, r), s = !1
         },
         d(r) {
-            r && g(e), K(t)
+            r && _(e), U(t)
         }
     }
 }
 
-function vl(n) {
+function kl(n) {
     var r;
-    let e, t, s = ((r = n[0]) == null ? void 0 : r.page) && At(n);
+    let e, t, s = ((r = n[0]) == null ? void 0 : r.page) && Bt(n);
     return {
         c() {
-            s && s.c(), e = N()
+            s && s.c(), e = z()
         },
         l(l) {
-            s && s.l(l), e = N()
+            s && s.l(l), e = z()
         },
         m(l, o) {
-            s && s.m(l, o), F(l, e, o), t = !0
+            s && s.m(l, o), T(l, e, o), t = !0
         },
         p(l, [o]) {
-            var a;
-            (a = l[0]) != null && a.page ? s ? (s.p(l, o), o & 1 && I(s, 1)) : (s = At(l), s.c(), I(s, 1), s.m(e.parentNode, e)) : s && (Z(), S(s, 1, 1, () => {
+            var i;
+            (i = l[0]) != null && i.page ? s ? (s.p(l, o), o & 1 && E(s, 1)) : (s = Bt(l), s.c(), E(s, 1), s.m(e.parentNode, e)) : s && (Z(), F(s, 1, 1, () => {
                 s = null
             }), x())
         },
         i(l) {
-            t || (I(s), t = !0)
+            t || (E(s), t = !0)
         },
         o(l) {
-            S(s), t = !1
+            F(s), t = !1
         },
         d(l) {
-            l && g(e), s && s.d(l)
+            l && _(e), s && s.d(l)
         }
     }
 }
 
-function $l(n, e, t) {
+function yl(n, e, t) {
     let s;
     const r = async o => {
-        await ds(`/${s.name}/dataset/${o.detail}`)
+        await _s(`/${s.name}/dataset/${o.detail}`)
     }, l = o => r(o);
     {
         let o;
-        fs.subscribe(a => o = a.params.dataset), gs.subscribe(a => {
-            const i = a == null ? void 0 : a.find(c => c.name === o);
-            i && t(0, s = i)
+        ps.subscribe(i => o = i.params.dataset), vs.subscribe(i => {
+            const a = i == null ? void 0 : i.find(c => c.name === o);
+            a && t(0, s = a)
         })
     }
     return [s, r, l]
 }
-class Bl extends re {
+class Nl extends te {
     constructor(e) {
-        super(), le(this, e, $l, vl, se, {})
+        super(), se(this, e, yl, kl, ee, {})
     }
 }
 export {
-    Bl as component, Ml as universal
+    Nl as component, Ol as universal
 };
```

### Comparing `pixano-0.5.2/pixano/app/dist/_app/immutable/nodes/5.Bo-LObf-.js` & `pixano-0.5.3/pixano/app/dist/_app/immutable/nodes/5.BngP3_K5.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -72,15 +72,15 @@
     d as claim_component,
     m as mount_component,
     e as destroy_component,
     f as bind
 } from "../chunks/index.D__UofN6.js";
 import {
     p as page
-} from "../chunks/stores.titGXIKi.js";
+} from "../chunks/stores.baCeY990.js";
 import {
     d as getItemEmbeddings,
     e as getDatasetItem,
     p as postDatasetItem
 } from "../chunks/api.BxNj-TAm.js";
 import {
     j as setCtx,
@@ -112,50 +112,50 @@
     L as isHTMLInputElement,
     M as getGroup,
     N as isUndefined,
     O as isHTMLElement,
     h as flyAndScale,
     P as commonjsGlobal,
     Q as getDefaultExportFromCjs
-} from "../chunks/command.YXxPKXvy.js";
+} from "../chunks/command.CjKwrCHU.js";
 import {
     c as createDispatcher,
     B as Button,
     P as PrimaryButton
-} from "../chunks/PrimaryButton.2luo0sZd.js";
+} from "../chunks/PrimaryButton.CjwzDHMn.js";
 import {
     T as TooltipIconButton,
     R as Root$3,
     a as Trigger$2,
     b as Tooltip_content,
     C as ConfirmModal
-} from "../chunks/TooltipIconButton.h3qFl-sW.js";
+} from "../chunks/TooltipIconButton.DmW3ppx8.js";
 import {
     d as derived,
     w as writable,
     g as goto
-} from "../chunks/entry.BdqlkNrw.js";
+} from "../chunks/entry.BGJCdFkn.js";
 import {
     e as ensure_array_like,
     g as get_spread_update,
     a as get_spread_object,
     m as modelsStore$1,
     s as saveCurrentItemStore,
     d as datasetsStore,
     i as isLoadingNewItemStore
-} from "../chunks/datasetStores.BZ9GDOPp.js";
+} from "../chunks/datasetStores.Davxg0aA.js";
 import {
     I as Icon,
     L as Loader_2
-} from "../chunks/loader-2.Cz-VINyt.js";
+} from "../chunks/loader-2.yiAD6ux3.js";
 import {
     a as Check,
     C as Checkbox,
     W as WarningModal
-} from "../chunks/checkbox.OiMtEzVH.js";
+} from "../chunks/checkbox.DTaWBrBv.js";
 class InternMap extends Map {
     constructor(e, n = keyof) {
         if (super(), Object.defineProperties(this, {
                 _intern: {
                     value: new Map
                 },
                 _key: {
@@ -46482,17 +46482,15 @@
             n(0, t = b), Object.keys(b).length === 0 ? n(7, u = !0) : n(7, u = !1)
         }).then(() => isLoadingNewItemStore.set(!1)).catch(b => console.error(b))
     };
     page.subscribe(m => {
         n(4, s = m.params.dataset), n(9, l = m.params.itemId)
     }), datasetsStore.subscribe(m => {
         const g = m == null ? void 0 : m.find(b => b.name === s);
-        console.log({
-            value: m
-        }), g && n(1, r = g)
+        g && n(1, r = g)
     });
     async function d(m) {
         await postDatasetItem(r.id, m), i(r, l), saveCurrentItemStore.update(g => ({
             ...g,
             shouldSave: !1
         }))
     }
```

### Comparing `pixano-0.5.2/pixano/core/__init__.py` & `pixano-0.5.3/pixano/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/bbox.py` & `pixano-0.5.3/pixano/core/bbox.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/camera.py` & `pixano-0.5.3/pixano/core/camera.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/compressed_rle.py` & `pixano-0.5.3/pixano/core/compressed_rle.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/depth_image.py` & `pixano-0.5.3/pixano/core/depth_image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/gt_info.py` & `pixano-0.5.3/pixano/core/gt_info.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/image.py` & `pixano-0.5.3/pixano/core/image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/pixano_type.py` & `pixano-0.5.3/pixano/core/pixano_type.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/pose.py` & `pixano-0.5.3/pixano/core/pose.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/core/utils.py` & `pixano-0.5.3/pixano/core/utils.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/__init__.py` & `pixano-0.5.3/pixano/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/fields.py` & `pixano-0.5.3/pixano/data/fields.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/settings.py` & `pixano-0.5.3/pixano/data/settings.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/dataset/__init__.py` & `pixano-0.5.3/pixano/data/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/dataset/dataset.py` & `pixano-0.5.3/pixano/data/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/dataset/dataset_info.py` & `pixano-0.5.3/pixano/data/dataset/dataset_info.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/dataset/dataset_item.py` & `pixano-0.5.3/pixano/data/dataset/dataset_item.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/dataset/dataset_stat.py` & `pixano-0.5.3/pixano/data/dataset/dataset_stat.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/dataset/dataset_table.py` & `pixano-0.5.3/pixano/data/dataset/dataset_table.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/exporters/__init__.py` & `pixano-0.5.3/pixano/data/item/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 # This software is governed by the CeCILL-C license under French law and
 # abiding by the rules of distribution of free software. You can use,
 # modify and/ or redistribute the software under the terms of the CeCILL-C
 # license as circulated by CEA, CNRS and INRIA at the following URL
 #
 # http://www.cecill.info
 
-from pixano.data.exporters.coco_exporter import COCOExporter
-from pixano.data.exporters.exporter import Exporter
+from pixano.data.item.item_embedding import ItemEmbedding
+from pixano.data.item.item_feature import ItemFeature
+from pixano.data.item.item_object import ItemObject
+from pixano.data.item.item_view import ItemView
 
 __all__ = [
-    "Exporter",
-    "COCOExporter",
+    "ItemObject",
+    "ItemFeature",
+    "ItemView",
+    "ItemEmbedding",
 ]
```

### Comparing `pixano-0.5.2/pixano/data/exporters/coco_exporter.py` & `pixano-0.5.3/pixano/data/exporters/coco_exporter.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/exporters/exporter.py` & `pixano-0.5.3/pixano/data/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/importers/__init__.py` & `pixano-0.5.3/pixano/data/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/importers/coco_importer.py` & `pixano-0.5.3/pixano/data/importers/coco_importer.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/importers/dota_importer.py` & `pixano-0.5.3/pixano/data/importers/dota_importer.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/importers/image_importer.py` & `pixano-0.5.3/pixano/data/importers/image_importer.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/importers/importer.py` & `pixano-0.5.3/pixano/data/importers/importer.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/item/item_embedding.py` & `pixano-0.5.3/pixano/data/item/item_embedding.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/item/item_feature.py` & `pixano-0.5.3/pixano/data/item/item_feature.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/item/item_object.py` & `pixano-0.5.3/pixano/data/item/item_object.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/data/item/item_view.py` & `pixano-0.5.3/pixano/data/item/item_view.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/models/__init__.py` & `pixano-0.5.3/pixano/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/models/inference_model.py` & `pixano-0.5.3/pixano/models/inference_model.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/utils/__init__.py` & `pixano-0.5.3/pixano/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/utils/boxes.py` & `pixano-0.5.3/pixano/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/utils/image.py` & `pixano-0.5.3/pixano/utils/image.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/utils/labels.py` & `pixano-0.5.3/pixano/utils/labels.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pixano/utils/python.py` & `pixano-0.5.3/pixano/utils/python.py`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/LICENSE` & `pixano-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/README.md` & `pixano-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/pyproject.toml` & `pixano-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixano-0.5.2/PKG-INFO` & `pixano-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pixano
-Version: 0.5.2
+Version: 0.5.3
 Summary: Data-centric AI building blocks for computer vision applications
 Project-URL: Documentation, https://github.com/pixano/pixano#readme
 Project-URL: Issues, https://github.com/pixano/pixano/issues
 Project-URL: Source, https://github.com/pixano/pixano
 Author-email: Pixano Developers <pixano@cea.fr>
 License-Expression: CECILL-C
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pixano Version: 0.5.2 Summary: Data-centric AI
+Metadata-Version: 2.3 Name: pixano Version: 0.5.3 Summary: Data-centric AI
 building blocks for computer vision applications Project-URL: Documentation,
 https://github.com/pixano/pixano#readme Project-URL: Issues, https://
 github.com/pixano/pixano/issues Project-URL: Source, https://github.com/pixano/
 pixano Author-email: Pixano Developers
 cea.fr> License-Expression: CECILL-C License-File: LICENSE Keywords: computer
 vision,data annotation,data visualization,deep learning,machine learning
 Classifier: Development Status :: 4 - Beta Classifier: License :: CeCILL-C Free
```

