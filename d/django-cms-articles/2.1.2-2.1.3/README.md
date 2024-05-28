# Comparing `tmp/django_cms_articles-2.1.2.tar.gz` & `tmp/django_cms_articles-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cms_articles-2.1.2.tar", max compression
+gzip compressed data, was "django_cms_articles-2.1.3.tar", max compression
```

## Comparing `django_cms_articles-2.1.2.tar` & `django_cms_articles-2.1.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1507 2022-09-20 10:23:53.365187 django_cms_articles-2.1.2/LICENSE
--rw-r--r--   0        0        0     1189 2022-09-20 10:23:53.365187 django_cms_articles-2.1.2/README.md
--rw-r--r--   0        0        0       59 2022-09-20 11:07:46.821205 django_cms_articles-2.1.2/cms_articles/__init__.py
--rw-r--r--   0        0        0       93 2022-09-20 10:23:53.365187 django_cms_articles-2.1.2/cms_articles/admin/__init__.py
--rw-r--r--   0        0        0    19135 2022-12-30 15:26:17.765974 django_cms_articles-2.1.2/cms_articles/admin/article.py
--rw-r--r--   0        0        0      277 2022-09-20 10:23:53.365187 django_cms_articles-2.1.2/cms_articles/admin/attribute.py
--rw-r--r--   0        0        0      224 2022-09-20 11:07:46.825205 django_cms_articles-2.1.2/cms_articles/admin/category.py
--rw-r--r--   0        0        0     3029 2022-12-30 15:25:49.465921 django_cms_articles-2.1.2/cms_articles/admin/forms.py
--rw-r--r--   0        0        0     5230 2022-09-22 22:13:29.570734 django_cms_articles-2.1.2/cms_articles/api.py
--rw-r--r--   0        0        0      281 2022-09-22 21:48:17.595607 django_cms_articles-2.1.2/cms_articles/apps.py
--rw-r--r--   0        0        0     4409 2022-09-20 11:07:47.037209 django_cms_articles-2.1.2/cms_articles/archive.py
--rw-r--r--   0        0        0     1526 2022-09-20 11:07:46.993208 django_cms_articles-2.1.2/cms_articles/article_rendering.py
--rw-r--r--   0        0        0      359 2022-09-22 21:48:17.595607 django_cms_articles-2.1.2/cms_articles/cms_apps.py
--rw-r--r--   0        0        0     2628 2022-09-22 21:56:11.181288 django_cms_articles-2.1.2/cms_articles/cms_plugins.py
--rw-r--r--   0        0        0     2724 2022-09-22 21:48:17.595607 django_cms_articles-2.1.2/cms_articles/cms_toolbars.py
--rw-r--r--   0        0        0      485 2022-09-20 11:07:47.053209 django_cms_articles-2.1.2/cms_articles/conf/__init__.py
--rw-r--r--   0        0        0      830 2022-09-22 21:48:17.595607 django_cms_articles-2.1.2/cms_articles/conf/default_settings.py
--rw-r--r--   0        0        0       91 2022-09-20 11:07:47.077209 django_cms_articles-2.1.2/cms_articles/import_wordpress/__init__.py
--rw-r--r--   0        0        0     9759 2024-05-06 23:19:01.606972 django_cms_articles-2.1.2/cms_articles/import_wordpress/admin.py
--rw-r--r--   0        0        0      253 2022-09-22 21:48:17.595607 django_cms_articles-2.1.2/cms_articles/import_wordpress/apps.py
--rw-r--r--   0        0        0      655 2022-09-22 21:48:17.595607 django_cms_articles-2.1.2/cms_articles/import_wordpress/forms.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.2/cms_articles/import_wordpress/management/__init__.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.2/cms_articles/import_wordpress/management/commands/__init__.py
--rw-r--r--   0        0        0     1087 2024-05-06 21:26:07.209560 django_cms_articles-2.1.2/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py
--rw-r--r--   0        0        0    13873 2024-05-06 20:46:46.623419 django_cms_articles-2.1.2/cms_articles/import_wordpress/migrations/0001_initial.py
--rw-r--r--   0        0        0      995 2024-05-06 23:19:01.523971 django_cms_articles-2.1.2/cms_articles/import_wordpress/migrations/0002_update.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.2/cms_articles/import_wordpress/migrations/__init__.py
--rw-r--r--   0        0        0    14657 2024-05-28 21:04:23.537752 django_cms_articles-2.1.2/cms_articles/import_wordpress/models.py
--rw-r--r--   0        0        0     2183 2024-05-28 21:01:19.538054 django_cms_articles-2.1.2/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html
--rw-r--r--   0        0        0     1098 2022-09-20 10:23:53.369187 django_cms_articles-2.1.2/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html
--rwxr-xr-x   0        0        0     7073 2024-05-28 22:07:59.265098 django_cms_articles-2.1.2/cms_articles/import_wordpress/utils.py
--rw-r--r--   0        0        0    11767 2022-09-20 10:23:53.373187 django_cms_articles-2.1.2/cms_articles/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18344 2022-09-20 10:23:53.373187 django_cms_articles-2.1.2/cms_articles/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10495 2022-09-22 22:40:46.906000 django_cms_articles-2.1.2/cms_articles/migrations/0001_initial.py
--rw-r--r--   0        0        0      386 2022-09-22 22:40:46.605981 django_cms_articles-2.1.2/cms_articles/migrations/0002_remove_title_excerpt.py
--rw-r--r--   0        0        0     2254 2022-09-22 22:40:21.876400 django_cms_articles-2.1.2/cms_articles/migrations/0003_description_image.py
--rw-r--r--   0        0        0     4742 2022-09-22 22:40:46.821994 django_cms_articles-2.1.2/cms_articles/migrations/0004_categories.py
--rw-r--r--   0        0        0     1712 2022-09-22 22:40:46.693987 django_cms_articles-2.1.2/cms_articles/migrations/0005_attributes.py
--rw-r--r--   0        0        0     1282 2022-09-22 22:40:46.657984 django_cms_articles-2.1.2/cms_articles/migrations/0006_order_date.py
--rw-r--r--   0        0        0      971 2022-09-22 22:40:46.705987 django_cms_articles-2.1.2/cms_articles/migrations/0007_plugins.py
--rw-r--r--   0        0        0     2765 2022-09-22 22:40:46.817994 django_cms_articles-2.1.2/cms_articles/migrations/0008_cms_3_4.py
--rw-r--r--   0        0        0      997 2022-09-22 22:40:46.769991 django_cms_articles-2.1.2/cms_articles/migrations/0009_number_min_value.py
--rw-r--r--   0        0        0      402 2022-09-22 22:40:46.789992 django_cms_articles-2.1.2/cms_articles/migrations/0010_remove_article_revision_id.py
--rw-r--r--   0        0        0     1085 2022-09-22 22:40:46.833995 django_cms_articles-2.1.2/cms_articles/migrations/0011_attribute_site.py
--rw-r--r--   0        0        0     1327 2022-09-22 22:40:46.865997 django_cms_articles-2.1.2/cms_articles/migrations/0012_protect_keys.py
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.373187 django_cms_articles-2.1.2/cms_articles/migrations/__init__.py
--rw-r--r--   0        0        0      287 2022-09-20 10:23:53.373187 django_cms_articles-2.1.2/cms_articles/models/__init__.py
--rw-r--r--   0        0        0    23967 2022-12-30 15:26:47.710033 django_cms_articles-2.1.2/cms_articles/models/article.py
--rw-r--r--   0        0        0      619 2022-09-22 23:03:54.335412 django_cms_articles-2.1.2/cms_articles/models/attribute.py
--rw-r--r--   0        0        0      843 2023-11-25 22:48:33.472751 django_cms_articles-2.1.2/cms_articles/models/category.py
--rw-r--r--   0        0        0     4220 2022-09-20 11:07:47.569217 django_cms_articles-2.1.2/cms_articles/models/managers.py
--rw-r--r--   0        0        0     4540 2022-12-30 15:24:29.529780 django_cms_articles-2.1.2/cms_articles/models/plugins.py
--rw-r--r--   0        0        0      276 2022-09-20 11:07:47.581217 django_cms_articles-2.1.2/cms_articles/models/query.py
--rw-r--r--   0        0        0     4212 2022-12-30 15:23:52.297721 django_cms_articles-2.1.2/cms_articles/models/title.py
--rw-r--r--   0        0        0     4609 2022-12-30 13:29:58.468309 django_cms_articles-2.1.2/cms_articles/search_indexes.py
--rw-r--r--   0        0        0     1252 2022-09-22 22:28:00.384915 django_cms_articles-2.1.2/cms_articles/signals/__init__.py
--rw-r--r--   0        0        0      816 2022-09-20 11:07:47.813220 django_cms_articles-2.1.2/cms_articles/signals/article.py
--rw-r--r--   0        0        0     1939 2022-09-20 11:07:47.865221 django_cms_articles-2.1.2/cms_articles/signals/plugins.py
--rw-r--r--   0        0        0      892 2022-09-20 11:07:47.845221 django_cms_articles-2.1.2/cms_articles/signals/title.py
--rw-r--r--   0        0        0      717 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/static/cms_articles/css/changelist.css
--rw-r--r--   0        0        0     2262 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/static/cms_articles/js/changelist.js
--rw-r--r--   0        0        0      378 2022-12-29 16:48:51.328113 django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article/change_form.html
--rw-r--r--   0        0        0     3619 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article/change_list_lang.html
--rw-r--r--   0        0        0      661 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article/change_list_preview.html
--rw-r--r--   0        0        0      757 2022-12-29 16:48:51.328113 django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article_changelist.html
--rw-r--r--   0        0        0       77 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/templates/cms_articles/article/default.html
--rw-r--r--   0        0        0      558 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/templates/cms_articles/article_preview.html
--rw-r--r--   0        0        0     1144 2022-09-20 10:23:53.377187 django_cms_articles-2.1.2/cms_articles/templates/cms_articles/articles/default.html
--rw-r--r--   0        0        0     1219 2022-09-22 22:44:45.738639 django_cms_articles-2.1.2/cms_articles/templates/cms_articles/base.html
--rw-r--r--   0        0        0      730 2022-09-20 10:23:53.381187 django_cms_articles-2.1.2/cms_articles/templates/cms_articles/default.html
--rw-r--r--   0        0        0        0 2022-09-20 10:23:53.381187 django_cms_articles-2.1.2/cms_articles/templatetags/__init__.py
--rw-r--r--   0        0        0     8972 2022-12-30 15:23:35.569696 django_cms_articles-2.1.2/cms_articles/templatetags/cms_articles.py
--rw-r--r--   0        0        0        0 2022-09-22 22:29:38.096301 django_cms_articles-2.1.2/cms_articles/tests/__init__.py
--rw-r--r--   0        0        0      924 2022-09-22 21:32:42.470486 django_cms_articles-2.1.2/cms_articles/tests/fixtures.py
--rw-r--r--   0        0        0     3054 2022-09-22 23:26:09.567216 django_cms_articles-2.1.2/cms_articles/tests/settings.py
--rw-r--r--   0        0        0      417 2022-09-22 23:17:26.339321 django_cms_articles-2.1.2/cms_articles/tests/templates/default.html
--rw-r--r--   0        0        0      514 2022-12-29 16:48:51.332113 django_cms_articles-2.1.2/cms_articles/tests/test_api.py
--rw-r--r--   0        0        0      328 2022-09-20 11:07:47.885222 django_cms_articles-2.1.2/cms_articles/urls.py
--rw-r--r--   0        0        0      435 2022-09-20 11:07:47.897222 django_cms_articles-2.1.2/cms_articles/utils/__init__.py
--rw-r--r--   0        0        0      941 2022-09-20 11:07:47.933222 django_cms_articles-2.1.2/cms_articles/utils/article.py
--rw-r--r--   0        0        0     1016 2022-09-20 11:17:31.723767 django_cms_articles-2.1.2/cms_articles/utils/placeholder.py
--rw-r--r--   0        0        0     4694 2022-09-20 11:07:48.037224 django_cms_articles-2.1.2/cms_articles/views.py
--rw-r--r--   0        0        0     1608 2024-05-28 22:08:30.253510 django_cms_articles-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 django_cms_articles-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1507 2022-09-20 10:23:53.365187 django_cms_articles-2.1.3/LICENSE
+-rw-r--r--   0        0        0     1189 2022-09-20 10:23:53.365187 django_cms_articles-2.1.3/README.md
+-rw-r--r--   0        0        0       59 2022-09-20 11:07:46.821205 django_cms_articles-2.1.3/cms_articles/__init__.py
+-rw-r--r--   0        0        0       93 2022-09-20 10:23:53.365187 django_cms_articles-2.1.3/cms_articles/admin/__init__.py
+-rw-r--r--   0        0        0    19135 2022-12-30 15:26:17.765974 django_cms_articles-2.1.3/cms_articles/admin/article.py
+-rw-r--r--   0        0        0      277 2022-09-20 10:23:53.365187 django_cms_articles-2.1.3/cms_articles/admin/attribute.py
+-rw-r--r--   0        0        0      224 2022-09-20 11:07:46.825205 django_cms_articles-2.1.3/cms_articles/admin/category.py
+-rw-r--r--   0        0        0     3029 2022-12-30 15:25:49.465921 django_cms_articles-2.1.3/cms_articles/admin/forms.py
+-rw-r--r--   0        0        0     5230 2022-09-22 22:13:29.570734 django_cms_articles-2.1.3/cms_articles/api.py
+-rw-r--r--   0        0        0      281 2022-09-22 21:48:17.595607 django_cms_articles-2.1.3/cms_articles/apps.py
+-rw-r--r--   0        0        0     4409 2022-09-20 11:07:47.037209 django_cms_articles-2.1.3/cms_articles/archive.py
+-rw-r--r--   0        0        0     1526 2022-09-20 11:07:46.993208 django_cms_articles-2.1.3/cms_articles/article_rendering.py
+-rw-r--r--   0        0        0      359 2022-09-22 21:48:17.595607 django_cms_articles-2.1.3/cms_articles/cms_apps.py
+-rw-r--r--   0        0        0     2628 2022-09-22 21:56:11.181288 django_cms_articles-2.1.3/cms_articles/cms_plugins.py
+-rw-r--r--   0        0        0     2724 2022-09-22 21:48:17.595607 django_cms_articles-2.1.3/cms_articles/cms_toolbars.py
+-rw-r--r--   0        0        0      485 2022-09-20 11:07:47.053209 django_cms_articles-2.1.3/cms_articles/conf/__init__.py
+-rw-r--r--   0        0        0      830 2022-09-22 21:48:17.595607 django_cms_articles-2.1.3/cms_articles/conf/default_settings.py
+-rw-r--r--   0        0        0       91 2022-09-20 11:07:47.077209 django_cms_articles-2.1.3/cms_articles/import_wordpress/__init__.py
+-rw-r--r--   0        0        0     9759 2024-05-06 23:19:01.606972 django_cms_articles-2.1.3/cms_articles/import_wordpress/admin.py
+-rw-r--r--   0        0        0      253 2022-09-22 21:48:17.595607 django_cms_articles-2.1.3/cms_articles/import_wordpress/apps.py
+-rw-r--r--   0        0        0      655 2022-09-22 21:48:17.595607 django_cms_articles-2.1.3/cms_articles/import_wordpress/forms.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.3/cms_articles/import_wordpress/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.3/cms_articles/import_wordpress/management/commands/__init__.py
+-rw-r--r--   0        0        0     1087 2024-05-06 21:26:07.209560 django_cms_articles-2.1.3/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py
+-rw-r--r--   0        0        0    13873 2024-05-06 20:46:46.623419 django_cms_articles-2.1.3/cms_articles/import_wordpress/migrations/0001_initial.py
+-rw-r--r--   0        0        0      995 2024-05-06 23:19:01.523971 django_cms_articles-2.1.3/cms_articles/import_wordpress/migrations/0002_update.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.369187 django_cms_articles-2.1.3/cms_articles/import_wordpress/migrations/__init__.py
+-rw-r--r--   0        0        0    14714 2024-05-28 22:31:19.602504 django_cms_articles-2.1.3/cms_articles/import_wordpress/models.py
+-rw-r--r--   0        0        0     2183 2024-05-28 21:01:19.538054 django_cms_articles-2.1.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html
+-rw-r--r--   0        0        0     1098 2022-09-20 10:23:53.369187 django_cms_articles-2.1.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html
+-rwxr-xr-x   0        0        0     7073 2024-05-28 22:07:59.265098 django_cms_articles-2.1.3/cms_articles/import_wordpress/utils.py
+-rw-r--r--   0        0        0    11767 2022-09-20 10:23:53.373187 django_cms_articles-2.1.3/cms_articles/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18344 2022-09-20 10:23:53.373187 django_cms_articles-2.1.3/cms_articles/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10495 2022-09-22 22:40:46.906000 django_cms_articles-2.1.3/cms_articles/migrations/0001_initial.py
+-rw-r--r--   0        0        0      386 2022-09-22 22:40:46.605981 django_cms_articles-2.1.3/cms_articles/migrations/0002_remove_title_excerpt.py
+-rw-r--r--   0        0        0     2254 2022-09-22 22:40:21.876400 django_cms_articles-2.1.3/cms_articles/migrations/0003_description_image.py
+-rw-r--r--   0        0        0     4742 2022-09-22 22:40:46.821994 django_cms_articles-2.1.3/cms_articles/migrations/0004_categories.py
+-rw-r--r--   0        0        0     1712 2022-09-22 22:40:46.693987 django_cms_articles-2.1.3/cms_articles/migrations/0005_attributes.py
+-rw-r--r--   0        0        0     1282 2022-09-22 22:40:46.657984 django_cms_articles-2.1.3/cms_articles/migrations/0006_order_date.py
+-rw-r--r--   0        0        0      971 2022-09-22 22:40:46.705987 django_cms_articles-2.1.3/cms_articles/migrations/0007_plugins.py
+-rw-r--r--   0        0        0     2765 2022-09-22 22:40:46.817994 django_cms_articles-2.1.3/cms_articles/migrations/0008_cms_3_4.py
+-rw-r--r--   0        0        0      997 2022-09-22 22:40:46.769991 django_cms_articles-2.1.3/cms_articles/migrations/0009_number_min_value.py
+-rw-r--r--   0        0        0      402 2022-09-22 22:40:46.789992 django_cms_articles-2.1.3/cms_articles/migrations/0010_remove_article_revision_id.py
+-rw-r--r--   0        0        0     1085 2022-09-22 22:40:46.833995 django_cms_articles-2.1.3/cms_articles/migrations/0011_attribute_site.py
+-rw-r--r--   0        0        0     1327 2022-09-22 22:40:46.865997 django_cms_articles-2.1.3/cms_articles/migrations/0012_protect_keys.py
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.373187 django_cms_articles-2.1.3/cms_articles/migrations/__init__.py
+-rw-r--r--   0        0        0      287 2022-09-20 10:23:53.373187 django_cms_articles-2.1.3/cms_articles/models/__init__.py
+-rw-r--r--   0        0        0    23967 2022-12-30 15:26:47.710033 django_cms_articles-2.1.3/cms_articles/models/article.py
+-rw-r--r--   0        0        0      619 2022-09-22 23:03:54.335412 django_cms_articles-2.1.3/cms_articles/models/attribute.py
+-rw-r--r--   0        0        0      843 2023-11-25 22:48:33.472751 django_cms_articles-2.1.3/cms_articles/models/category.py
+-rw-r--r--   0        0        0     4220 2022-09-20 11:07:47.569217 django_cms_articles-2.1.3/cms_articles/models/managers.py
+-rw-r--r--   0        0        0     4540 2022-12-30 15:24:29.529780 django_cms_articles-2.1.3/cms_articles/models/plugins.py
+-rw-r--r--   0        0        0      276 2022-09-20 11:07:47.581217 django_cms_articles-2.1.3/cms_articles/models/query.py
+-rw-r--r--   0        0        0     4212 2022-12-30 15:23:52.297721 django_cms_articles-2.1.3/cms_articles/models/title.py
+-rw-r--r--   0        0        0     4609 2022-12-30 13:29:58.468309 django_cms_articles-2.1.3/cms_articles/search_indexes.py
+-rw-r--r--   0        0        0     1252 2022-09-22 22:28:00.384915 django_cms_articles-2.1.3/cms_articles/signals/__init__.py
+-rw-r--r--   0        0        0      816 2022-09-20 11:07:47.813220 django_cms_articles-2.1.3/cms_articles/signals/article.py
+-rw-r--r--   0        0        0     1939 2022-09-20 11:07:47.865221 django_cms_articles-2.1.3/cms_articles/signals/plugins.py
+-rw-r--r--   0        0        0      892 2022-09-20 11:07:47.845221 django_cms_articles-2.1.3/cms_articles/signals/title.py
+-rw-r--r--   0        0        0      717 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/static/cms_articles/css/changelist.css
+-rw-r--r--   0        0        0     2262 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/static/cms_articles/js/changelist.js
+-rw-r--r--   0        0        0      378 2022-12-29 16:48:51.328113 django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article/change_form.html
+-rw-r--r--   0        0        0     3619 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article/change_list_lang.html
+-rw-r--r--   0        0        0      661 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article/change_list_preview.html
+-rw-r--r--   0        0        0      757 2022-12-29 16:48:51.328113 django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article_changelist.html
+-rw-r--r--   0        0        0       77 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/templates/cms_articles/article/default.html
+-rw-r--r--   0        0        0      558 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/templates/cms_articles/article_preview.html
+-rw-r--r--   0        0        0     1144 2022-09-20 10:23:53.377187 django_cms_articles-2.1.3/cms_articles/templates/cms_articles/articles/default.html
+-rw-r--r--   0        0        0     1219 2022-09-22 22:44:45.738639 django_cms_articles-2.1.3/cms_articles/templates/cms_articles/base.html
+-rw-r--r--   0        0        0      730 2022-09-20 10:23:53.381187 django_cms_articles-2.1.3/cms_articles/templates/cms_articles/default.html
+-rw-r--r--   0        0        0        0 2022-09-20 10:23:53.381187 django_cms_articles-2.1.3/cms_articles/templatetags/__init__.py
+-rw-r--r--   0        0        0     8972 2022-12-30 15:23:35.569696 django_cms_articles-2.1.3/cms_articles/templatetags/cms_articles.py
+-rw-r--r--   0        0        0        0 2022-09-22 22:29:38.096301 django_cms_articles-2.1.3/cms_articles/tests/__init__.py
+-rw-r--r--   0        0        0      924 2022-09-22 21:32:42.470486 django_cms_articles-2.1.3/cms_articles/tests/fixtures.py
+-rw-r--r--   0        0        0     3054 2022-09-22 23:26:09.567216 django_cms_articles-2.1.3/cms_articles/tests/settings.py
+-rw-r--r--   0        0        0      417 2022-09-22 23:17:26.339321 django_cms_articles-2.1.3/cms_articles/tests/templates/default.html
+-rw-r--r--   0        0        0      514 2022-12-29 16:48:51.332113 django_cms_articles-2.1.3/cms_articles/tests/test_api.py
+-rw-r--r--   0        0        0      328 2022-09-20 11:07:47.885222 django_cms_articles-2.1.3/cms_articles/urls.py
+-rw-r--r--   0        0        0      435 2022-09-20 11:07:47.897222 django_cms_articles-2.1.3/cms_articles/utils/__init__.py
+-rw-r--r--   0        0        0      941 2022-09-20 11:07:47.933222 django_cms_articles-2.1.3/cms_articles/utils/article.py
+-rw-r--r--   0        0        0     1016 2022-09-20 11:17:31.723767 django_cms_articles-2.1.3/cms_articles/utils/placeholder.py
+-rw-r--r--   0        0        0     4694 2022-09-20 11:07:48.037224 django_cms_articles-2.1.3/cms_articles/views.py
+-rw-r--r--   0        0        0     1608 2024-05-28 22:31:58.559943 django_cms_articles-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 django_cms_articles-2.1.3/PKG-INFO
```

### Comparing `django_cms_articles-2.1.2/LICENSE` & `django_cms_articles-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/README.md` & `django_cms_articles-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/admin/article.py` & `django_cms_articles-2.1.3/cms_articles/admin/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/admin/forms.py` & `django_cms_articles-2.1.3/cms_articles/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/api.py` & `django_cms_articles-2.1.3/cms_articles/api.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/archive.py` & `django_cms_articles-2.1.3/cms_articles/archive.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/article_rendering.py` & `django_cms_articles-2.1.3/cms_articles/article_rendering.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/cms_plugins.py` & `django_cms_articles-2.1.3/cms_articles/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/cms_toolbars.py` & `django_cms_articles-2.1.3/cms_articles/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/conf/default_settings.py` & `django_cms_articles-2.1.3/cms_articles/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/admin.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/admin.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/forms.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/forms.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/management/commands/cms_import_wordpress.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/migrations/0001_initial.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/migrations/0002_update.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/migrations/0002_update.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/models.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from cms.models import Page
 from cms.models.fields import PageField
 from django.core.files import File as DjangoFile
 from django.core.files.temp import NamedTemporaryFile
 from django.db import models
 from django.utils.functional import cached_property
 from django.utils.text import slugify
+from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 from filer.fields.folder import FilerFolderField
 from filer.models import File, Folder
 
 from cms_articles.api import add_content, create_article, publish_article
 from cms_articles.conf import settings
 
@@ -180,15 +181,15 @@
         if options.article_publish:
             self.article = publish_article(
                 article=self.article,
                 language=options.language,
                 changed_by=self.created_by.user or self.created_by.login,
             )
             public = self.article.get_public_object()
-            public.creation_date = self.pub_date
+            public.creation_date = self.pub_date or now()
             public.save()
         if options.article_redirects:
             create_redirect(self.link, self.article.get_absolute_url())
         self.save()
         return self.article
 
     def get_or_import_page(self, options):
@@ -222,15 +223,15 @@
         self.page.creation_date = self.post_date
         self.page.save()
         content = "\n".join("<p>{}</p>".format(p) for p in self.content.split("\n\n"))
         add_content(self.page, language=options.language, slot=options.page_slot, content=content)
         if options.page_publish:
             self.page.publish(options.language)
             public = self.page.get_public_object()
-            public.creation_date = self.pub_date
+            public.creation_date = self.pub_date or now()
             public.save()
         if options.page_redirects:
             create_redirect(self.link, self.page.get_absolute_url())
         self.save()
         return self.page
 
     def get_or_import_file(self, options):
@@ -252,15 +253,15 @@
         if self.parent:
             folder = self.parent.get_or_create_folder(options)
         else:
             folder = options.file_folder
         # import file
         self.file = FileImporter().import_file(file_obj=django_file, folder=folder)
         # set date and owner
-        self.file.created_at = self.pub_date
+        self.file.created_at = self.post_date
         self.file.owner = self.created_by.user
         self.file.save()
         # return imported file
         self.save()
         return self.file
 
     def get_or_create_folder(self, options):
```

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/cms_import.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/templates/cms_articles/import_wordpress/form.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/import_wordpress/utils.py` & `django_cms_articles-2.1.3/cms_articles/import_wordpress/utils.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/locale/cs/LC_MESSAGES/django.mo` & `django_cms_articles-2.1.3/cms_articles/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/locale/cs/LC_MESSAGES/django.po` & `django_cms_articles-2.1.3/cms_articles/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0001_initial.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0003_description_image.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0003_description_image.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0004_categories.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0004_categories.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0005_attributes.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0005_attributes.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0006_order_date.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0006_order_date.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0007_plugins.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0007_plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0008_cms_3_4.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0008_cms_3_4.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0009_number_min_value.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0009_number_min_value.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0011_attribute_site.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0011_attribute_site.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/migrations/0012_protect_keys.py` & `django_cms_articles-2.1.3/cms_articles/migrations/0012_protect_keys.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/models/article.py` & `django_cms_articles-2.1.3/cms_articles/models/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/models/attribute.py` & `django_cms_articles-2.1.3/cms_articles/models/attribute.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/models/category.py` & `django_cms_articles-2.1.3/cms_articles/models/category.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/models/managers.py` & `django_cms_articles-2.1.3/cms_articles/models/managers.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/models/plugins.py` & `django_cms_articles-2.1.3/cms_articles/models/plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/models/title.py` & `django_cms_articles-2.1.3/cms_articles/models/title.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/search_indexes.py` & `django_cms_articles-2.1.3/cms_articles/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/signals/__init__.py` & `django_cms_articles-2.1.3/cms_articles/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/signals/article.py` & `django_cms_articles-2.1.3/cms_articles/signals/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/signals/plugins.py` & `django_cms_articles-2.1.3/cms_articles/signals/plugins.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/signals/title.py` & `django_cms_articles-2.1.3/cms_articles/signals/title.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/static/cms_articles/css/changelist.css` & `django_cms_articles-2.1.3/cms_articles/static/cms_articles/css/changelist.css`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/static/cms_articles/js/changelist.js` & `django_cms_articles-2.1.3/cms_articles/static/cms_articles/js/changelist.js`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article/change_list_lang.html` & `django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article/change_list_lang.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article/change_list_preview.html` & `django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article/change_list_preview.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/admin/cms_articles/article_changelist.html` & `django_cms_articles-2.1.3/cms_articles/templates/admin/cms_articles/article_changelist.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/cms_articles/article_preview.html` & `django_cms_articles-2.1.3/cms_articles/templates/cms_articles/article_preview.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/cms_articles/articles/default.html` & `django_cms_articles-2.1.3/cms_articles/templates/cms_articles/articles/default.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/cms_articles/base.html` & `django_cms_articles-2.1.3/cms_articles/templates/cms_articles/base.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templates/cms_articles/default.html` & `django_cms_articles-2.1.3/cms_articles/templates/cms_articles/default.html`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/templatetags/cms_articles.py` & `django_cms_articles-2.1.3/cms_articles/templatetags/cms_articles.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/tests/fixtures.py` & `django_cms_articles-2.1.3/cms_articles/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/tests/settings.py` & `django_cms_articles-2.1.3/cms_articles/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/tests/test_api.py` & `django_cms_articles-2.1.3/cms_articles/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/utils/article.py` & `django_cms_articles-2.1.3/cms_articles/utils/article.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/utils/placeholder.py` & `django_cms_articles-2.1.3/cms_articles/utils/placeholder.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/cms_articles/views.py` & `django_cms_articles-2.1.3/cms_articles/views.py`

 * *Files identical despite different names*

### Comparing `django_cms_articles-2.1.2/pyproject.toml` & `django_cms_articles-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 multi_line_output = 3
 profile = "black"
 skip_glob = "*migrations*"
 use_parentheses = true
 
 [tool.poetry]
 name = "django-cms-articles"
-version = "2.1.2"
+version = "2.1.3"
 description = "django CMS application for managing articles"
 authors = ["Jakub Dorňák <jakub.dornak@qbsoftware.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{include = "cms_articles"}]
 repository = "https://github.com/misli/django-cms-articles"
 classifiers = [
```

### Comparing `django_cms_articles-2.1.2/PKG-INFO` & `django_cms_articles-2.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cms-articles
-Version: 2.1.2
+Version: 2.1.3
 Summary: django CMS application for managing articles
 Home-page: https://github.com/misli/django-cms-articles
 License: BSD-3-Clause
 Author: Jakub Dorňák
 Author-email: jakub.dornak@qbsoftware.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

