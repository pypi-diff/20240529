# Comparing `tmp/ludic-0.4.5.tar.gz` & `tmp/ludic-0.4.6.tar.gz`

## Comparing `ludic-0.4.5.tar` & `ludic-0.4.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.5/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.5/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.5/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.5/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.5/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/catalog.md
--rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/getting-started.md
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/click_to_load.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/__init__.py
--rw-r--r--   0        0        0    16518 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/attrs.py
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/components.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/format.py
--rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/forms.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/headers.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/icons.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/items.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/messages.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/tables.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/typography.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/collect.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/themes.py
--rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/types.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/__init__.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/parsers.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/responses.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_components.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/styles/test_styles.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.5/LICENCE
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.5/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.6/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.6/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.6/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/catalog.md
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/getting-started.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/click_to_load.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/__init__.py
+-rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/attrs.py
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/components.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/format.py
+-rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/types.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/headers.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/icons.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/items.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/collect.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/themes.py
+-rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/responses.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_components.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.6/LICENCE
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.6/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.6/PKG-INFO
```

### Comparing `ludic-0.4.5/.pre-commit-config.yaml` & `ludic-0.4.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/CONTRIBUTING.md` & `ludic-0.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/mkdocs.yaml` & `ludic-0.4.6/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/.github/workflows/publish.yaml` & `ludic-0.4.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/.github/workflows/test.yaml` & `ludic-0.4.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/catalog.md` & `ludic-0.4.6/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/components.md` & `ludic-0.4.6/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/getting-started.md` & `ludic-0.4.6/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/htmx.md` & `ludic-0.4.6/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/index.md` & `ludic-0.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/styles.md` & `ludic-0.4.6/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/web-framework.md` & `ludic-0.4.6/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/docs/assets/ludic.png` & `ludic-0.4.6/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/README.md` & `ludic-0.4.6/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/__init__.py` & `ludic-0.4.6/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/bulk_update.py` & `ludic-0.4.6/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/click_to_edit.py` & `ludic-0.4.6/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/click_to_load.py` & `ludic-0.4.6/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/delete_row.py` & `ludic-0.4.6/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/edit_row.py` & `ludic-0.4.6/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/infinite_scroll.py` & `ludic-0.4.6/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/examples/lazy_loading.py` & `ludic-0.4.6/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/attrs.py` & `ludic-0.4.6/ludic/attrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     xmlns: str
 
 
 class MetaAttrs(HtmlAttrs, total=False):
     name: str
     content: str
     charset: str
+    property: str
 
 
 class StyleAttrs(HtmlAndEventAttrs, total=False):
     media: str
     type: Literal["text/css"]
```

### Comparing `ludic-0.4.5/ludic/base.py` & `ludic-0.4.6/ludic/base.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/components.py` & `ludic-0.4.6/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/format.py` & `ludic-0.4.6/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/html.py` & `ludic-0.4.6/ludic/html.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/types.py` & `ludic-0.4.6/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/utils.py` & `ludic-0.4.6/ludic/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import lru_cache
 from typing import (
     Annotated,
     Any,
     TypeVar,
     get_args,
     get_origin,
     get_type_hints,
@@ -29,14 +30,15 @@
 
     for base in getattr(cls_or_obj, "__orig_bases__", []):
         if issubclass(get_origin(base), BaseElement):
             return get_args(base)
     return None
 
 
+@lru_cache
 def get_element_attrs_annotations(
     cls_or_obj: Any, include_extras: bool = False
 ) -> dict[str, Any]:
     """Get the annotations of the element.
 
     Args:
         cls_or_obj (type[Any]): The element to get the annotations of.
```

### Comparing `ludic-0.4.5/ludic/catalog/buttons.py` & `ludic-0.4.6/ludic/catalog/buttons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/forms.py` & `ludic-0.4.6/ludic/catalog/forms.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/headers.py` & `ludic-0.4.6/ludic/catalog/headers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/icons.py` & `ludic-0.4.6/ludic/catalog/icons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/items.py` & `ludic-0.4.6/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/layouts.py` & `ludic-0.4.6/ludic/catalog/layouts.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/lists.py` & `ludic-0.4.6/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/loaders.py` & `ludic-0.4.6/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/messages.py` & `ludic-0.4.6/ludic/catalog/messages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/navigation.py` & `ludic-0.4.6/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/pages.py` & `ludic-0.4.6/ludic/catalog/pages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/quotes.py` & `ludic-0.4.6/ludic/catalog/quotes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/tables.py` & `ludic-0.4.6/ludic/catalog/tables.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/typography.py` & `ludic-0.4.6/ludic/catalog/typography.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/catalog/utils.py` & `ludic-0.4.6/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/styles/collect.py` & `ludic-0.4.6/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/styles/themes.py` & `ludic-0.4.6/ludic/styles/themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/styles/types.py` & `ludic-0.4.6/ludic/styles/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/styles/utils.py` & `ludic-0.4.6/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/app.py` & `ludic-0.4.6/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/datastructures.py` & `ludic-0.4.6/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/endpoints.py` & `ludic-0.4.6/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/exceptions.py` & `ludic-0.4.6/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/parsers.py` & `ludic-0.4.6/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/requests.py` & `ludic-0.4.6/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/responses.py` & `ludic-0.4.6/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/ludic/web/routing.py` & `ludic-0.4.6/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/test_components.py` & `ludic-0.4.6/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/test_elements.py` & `ludic-0.4.6/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/test_examples.py` & `ludic-0.4.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/test_exceptions.py` & `ludic-0.4.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/test_formatting.py` & `ludic-0.4.6/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/test_types.py` & `ludic-0.4.6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/styles/__init__.py` & `ludic-0.4.6/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/styles/test_styles.py` & `ludic-0.4.6/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/tests/styles/test_themes.py` & `ludic-0.4.6/tests/styles/test_themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/.gitignore` & `ludic-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/LICENCE` & `ludic-0.4.6/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/README.md` & `ludic-0.4.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -13,17 +13,32 @@
 
 ## Features
 
 - Seamless **&lt;/&gt; htmx** integration for rapid web development in **pure Python**
 - **Type-Guided components** utilizing Python's typing system
 - Uses the power of **Starlette** and **Async** for high-performance web development
 - Build HTML with the ease and power of Python **f-strings**
-- Add CSS styling to your components with **themes**
+- Add CSS styling to your components with **Themes**
+- Create simple, responsive layouts adopted from the **Every Layout Book**
 
-## Ideals
+## Comparison
+
+Here is a table comparing Ludic to other similar tools:
+
+| Feature                     | Ludic       | FastUI      | Reflex      |
+|-----------------------------|-------------|-------------|-------------|
+| HTML rendering              | Server Side | Client Side | Client Side |
+| Uses a template engine      | No          | No          | No          |
+| UI interactivity            | [</> htmx](https://htmx.org)* | [React](https://react.dev/) | [React](https://react.dev/) |
+| Backend framework           | [Starlette](https://www.starlette.io)*  | [FastAPI](https://fastapi.tiangolo.com) | [FastAPI](https://fastapi.tiangolo.com) |
+| Client-Server Communication | [HTML + REST](https://htmx.org/essays/how-did-rest-come-to-mean-the-opposite-of-rest/) | [JSON + REST](https://github.com/pydantic/FastUI?tab=readme-ov-file#the-principle-long-version) | [WebSockets](https://reflex.dev/blog/2024-03-21-reflex-architecture/) |
+
+<sup>(*) HTMX as well as Starlette are optional dependencies for Ludic, it does not enforce any frontend or backend frameworks. At it's core, Ludic only generates HTML and allows registering CSS.</sup>
+
+## Motivation
 
 This framework allows HTML generation in Python while utilizing Python's typing system. Our goal is to enable the creation of dynamic web applications with reusable components, all while offering a greater level of type safety than raw HTML.
 
 **Key Ideas:**
 
 - **Type-Guided HTML**: Catch potential HTML structural errors at development time thanks to type hints. The framework enforces stricter rules than standard HTML, promoting well-structured and maintainable code.
 - **Composable Components**: Define reusable, dynamic HTML components in pure Python. This aligns with modern web development practices, emphasizing modularity.
@@ -70,14 +85,20 @@
 
 Similar to Starlette, you'll also want to install an [ASGI](https://asgi.readthedocs.io/en/latest/) server:
 
 ```
 pip install uvicorn
 ```
 
+You can also use a basic cookiecutter template to get quickly started:
+
+```
+cookiecutter gh:paveldedik/ludic-template
+```
+
 ## Full Example
 
 **components.py**:
 
 ```python
 from typing import override
```

### Comparing `ludic-0.4.5/pyproject.toml` & `ludic-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.5/PKG-INFO` & `ludic-0.4.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.5
+Version: 0.4.6
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
@@ -47,17 +47,32 @@
 
 ## Features
 
 - Seamless **&lt;/&gt; htmx** integration for rapid web development in **pure Python**
 - **Type-Guided components** utilizing Python's typing system
 - Uses the power of **Starlette** and **Async** for high-performance web development
 - Build HTML with the ease and power of Python **f-strings**
-- Add CSS styling to your components with **themes**
+- Add CSS styling to your components with **Themes**
+- Create simple, responsive layouts adopted from the **Every Layout Book**
 
-## Ideals
+## Comparison
+
+Here is a table comparing Ludic to other similar tools:
+
+| Feature                     | Ludic       | FastUI      | Reflex      |
+|-----------------------------|-------------|-------------|-------------|
+| HTML rendering              | Server Side | Client Side | Client Side |
+| Uses a template engine      | No          | No          | No          |
+| UI interactivity            | [</> htmx](https://htmx.org)* | [React](https://react.dev/) | [React](https://react.dev/) |
+| Backend framework           | [Starlette](https://www.starlette.io)*  | [FastAPI](https://fastapi.tiangolo.com) | [FastAPI](https://fastapi.tiangolo.com) |
+| Client-Server Communication | [HTML + REST](https://htmx.org/essays/how-did-rest-come-to-mean-the-opposite-of-rest/) | [JSON + REST](https://github.com/pydantic/FastUI?tab=readme-ov-file#the-principle-long-version) | [WebSockets](https://reflex.dev/blog/2024-03-21-reflex-architecture/) |
+
+<sup>(*) HTMX as well as Starlette are optional dependencies for Ludic, it does not enforce any frontend or backend frameworks. At it's core, Ludic only generates HTML and allows registering CSS.</sup>
+
+## Motivation
 
 This framework allows HTML generation in Python while utilizing Python's typing system. Our goal is to enable the creation of dynamic web applications with reusable components, all while offering a greater level of type safety than raw HTML.
 
 **Key Ideas:**
 
 - **Type-Guided HTML**: Catch potential HTML structural errors at development time thanks to type hints. The framework enforces stricter rules than standard HTML, promoting well-structured and maintainable code.
 - **Composable Components**: Define reusable, dynamic HTML components in pure Python. This aligns with modern web development practices, emphasizing modularity.
@@ -104,14 +119,20 @@
 
 Similar to Starlette, you'll also want to install an [ASGI](https://asgi.readthedocs.io/en/latest/) server:
 
 ```
 pip install uvicorn
 ```
 
+You can also use a basic cookiecutter template to get quickly started:
+
+```
+cookiecutter gh:paveldedik/ludic-template
+```
+
 ## Full Example
 
 **components.py**:
 
 ```python
 from typing import override
```

