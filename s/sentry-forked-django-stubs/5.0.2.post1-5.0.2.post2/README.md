# Comparing `tmp/sentry_forked_django_stubs-5.0.2.post1.tar.gz` & `tmp/sentry_forked_django_stubs-5.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_forked_django_stubs-5.0.2.post1.tar", last modified: Tue May 28 21:42:54 2024, max compression
+gzip compressed data, was "sentry_forked_django_stubs-5.0.2.post2.tar", last modified: Wed May 29 16:35:25 2024, max compression
```

## Comparing `sentry_forked_django_stubs-5.0.2.post1.tar` & `sentry_forked_django_stubs-5.0.2.post2.tar`

### file list

```diff
@@ -1,835 +1,835 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.390339 sentry_forked_django_stubs-5.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-28 21:42:54.390339 sentry_forked_django_stubs-5.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.282339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.282339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/apps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/apps/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.282339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.282339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/locale/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.282339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/urls/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.282339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.286339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.286339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.286339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.286339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.290339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.290339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.290339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/management/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/prefetch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.294339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.298339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.302339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.302339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.306339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.306339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.306339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.306339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.306339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.310339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.310339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.310339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.314339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.318339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.318339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.318339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.322339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/expressions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.322339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.322339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.322339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.322339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sitemaps/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sitemaps/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.326339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.330339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.330339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.330339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.330339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/syndication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.330339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.330339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.334339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/redis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.334339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.334339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/compatibility/django_4_0.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/files.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.334339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.338339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/locks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/move.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.338339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/filesystem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/handler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/memory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/temp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.338339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.338339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.342339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.342339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.346339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/optimizemigration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/sql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/templates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.346339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.346339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/servers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/signing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.346339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.346339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.350339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.350339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.350339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.354339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.354339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.354339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.358339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.358339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.362339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.362339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/
--rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/generated.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.362339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/manager.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.366339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.366339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.366339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20507 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/formsets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/renderers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.366339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/cookie.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.366339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/locale.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/security.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.370339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.370339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/django.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/context_processors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/engine.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/library.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.370339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/smartif.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.374339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/static.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.374339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/selenium.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/signals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/testcases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.374339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/conf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.382339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/_os.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/archive.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/choices.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/dates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/duration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/encoding.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/formats.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/functional.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/hashable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/inspect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/jslex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/log.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/safestring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/text.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/timesince.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/timezone.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.382339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.382339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/debug.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.386339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.386339 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/i18n.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/static.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.386339 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.386339 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22288 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/django/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.386339 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 runner    (1001) docker     (127)    17822 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15376 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.390339 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    25137 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/manytomany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    49280 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.390339 sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-28 21:42:54.000000 sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30466 2024-05-28 21:42:54.000000 sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:42:54.000000 sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 21:42:54.000000 sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 21:42:54.000000 sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:42:54.390339 sentry_forked_django_stubs-5.0.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:42:54.390339 sentry_forked_django_stubs-5.0.2.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-28 21:42:50.000000 sentry_forked_django_stubs-5.0.2.post1/tests/test_error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.556435 sentry_forked_django_stubs-5.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-29 16:35:25.556435 sentry_forked_django_stubs-5.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.440434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.440434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/apps/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.440434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.440434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.444434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.444434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.444434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.444434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.448434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.448434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.448434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.452434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.452434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.452434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.452434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.452434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/prefetch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.456434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.460434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.460434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.460434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.460434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.460434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.460434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.464434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.464434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.468434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.468434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.468434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.468434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.472434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.472434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.472434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.476434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.476434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.480434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.480434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.480434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.480434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.480434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.480434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.484434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.484434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.484434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.488434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/expressions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.488434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.488434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.488434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.488434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.492434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.492434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.492434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.492434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.492434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.492434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sitemaps/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/syndication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.496434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.500434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/redis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.500434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.500434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/compatibility/django_4_0.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.500434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.504434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.504434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.504434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.504434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.508434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.508434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.512434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/optimizemigration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.512434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.512434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/signing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.512434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.512434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.516435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.516435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.516435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.520434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.520434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.520434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.524434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.524434 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.528435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.528435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/generated.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.528435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.532435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.532435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.532435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20507 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.532435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/cookie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.536435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.536435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.536435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/engine.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/library.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.540435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/smartif.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.540435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.540435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/selenium.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/testcases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.540435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/conf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.548435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/_os.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/archive.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/choices.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/duration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/formats.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/functional.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/timezone.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.548435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.548435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/debug.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.552435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.552435 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/static.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.552435 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.552435 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22288 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/django/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.552435 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17822 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15376 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.556435 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25137 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/manytomany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49280 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.556435 sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-29 16:35:25.000000 sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30466 2024-05-29 16:35:25.000000 sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:35:25.000000 sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-29 16:35:25.000000 sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 16:35:25.000000 sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:35:25.556435 sentry_forked_django_stubs-5.0.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:35:25.556435 sentry_forked_django_stubs-5.0.2.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-29 16:35:21.000000 sentry_forked_django_stubs-5.0.2.post2/tests/test_error_handling.py
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/LICENSE.md` & `sentry_forked_django_stubs-5.0.2.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/PKG-INFO` & `sentry_forked_django_stubs-5.0.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-forked-django-stubs
-Version: 5.0.2.post1
+Version: 5.0.2.post2
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/README.md` & `sentry_forked_django_stubs-5.0.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/apps/config.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/apps/config.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/apps/registry.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/apps/registry.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/global_settings.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/global_settings.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/conf/urls/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/conf/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/checks.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/checks.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/decorators.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/decorators.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/filters.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/filters.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/helpers.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/helpers.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/options.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/sites.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/sites.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/templatetags/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/tests.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/views/main.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/views/main.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admin/widgets.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admin/widgets.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/admindocs/views.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/admin.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/admin.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/backends.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/backends.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/base_user.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/base_user.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/context_processors.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/decorators.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/decorators.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/forms.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/forms.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/hashers.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/hashers.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/middleware.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/middleware.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/mixins.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/password_validation.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/password_validation.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/tokens.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/tokens.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/auth/views.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/admin.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/fields.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/forms.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/management/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/contenttypes/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/admin/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/backends/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/aggregates.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/fields.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/functions.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/lookups.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/feeds.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/fields.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/forms/widgets.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/datasource.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/envelope.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/feature.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/field.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/geometries.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/layer.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/libgdal.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/libgdal.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/band.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/raster/source.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/gdal/srs.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geoip2/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/collections.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/coordseq.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/geometry.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/libgeos.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/linestring.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/mutable_list.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/point.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/polygon.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prepared.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/predicates.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/measure.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/measure.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/gis/utils/layermapping.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/api.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/messages/storage/cookie.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/messages/storage/cookie.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/general.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/general.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/mixins.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/mixins.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/aggregates/statistics.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/aggregates/statistics.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/constraints.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/constraints.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/array.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/array.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/hstore.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/hstore.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/fields/ranges.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/fields/ranges.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/array.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/forms/ranges.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/indexes.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/indexes.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/lookups.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/search.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/search.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/postgres/validators.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/postgres/validators.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/backends/db.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sessions/base_session.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sessions/base_session.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sitemaps/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sitemaps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sitemaps/views.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sitemaps/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/sites/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/finders.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/handlers.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/staticfiles/storage.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/contrib/syndication/views.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/contrib/syndication/views.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/db.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/memcached.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/memcached.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/cache/backends/redis.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/cache/backends/redis.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/caches.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/messages.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/registry.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/registry.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/csrf.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/csrf.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/security/sessions.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/templates.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/templates.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/translation.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/checks/urls.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/exceptions.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/filesystem.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/storage/memory.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/storage/memory.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/uploadedfile.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/uploadedfile.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/uploadhandler.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/files/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/asgi.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/asgi.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/exception.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/handlers/wsgi.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/handlers/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/backends/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/mail/message.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/mail/message.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/color.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/diffsettings.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/inspectdb.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/inspectdb.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/loaddata.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/loaddata.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/makemessages.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/makemessages.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/makemigrations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/makemigrations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/migrate.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/commands/runserver.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/commands/runserver.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/templates.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/templates.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/management/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/paginator.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/paginator.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/json.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/pyyaml.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/serializers/xml_serializer.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/servers/basehttp.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/servers/basehttp.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/signing.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/signing.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/core/validators.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/core/validators.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/client.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/creation.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/creation.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/introspection.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/introspection.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/base/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/base/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/ddl_references.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/ddl_references.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/dummy/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/dummy/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/compiler.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/introspection.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/mysql/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/client.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/oracle/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/client.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/features.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/features.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/postgresql/schema.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/sqlite3/operations.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/sqlite3/operations.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/backends/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/autodetector.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/autodetector.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/exceptions.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/executor.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/executor.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/graph.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/graph.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/loader.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/migration.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/migration.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/fields.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/special.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/special.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/operations/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/operations/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/questioner.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/recorder.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/recorder.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/serializer.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/serializer.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/state.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/state.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/migrations/writer.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/aggregates.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/constraints.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/constraints.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/deletion.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/deletion.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/enums.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/enums.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/expressions.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/expressions.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/files.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/files.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/generated.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/generated.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/json.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/json.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/mixins.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/related.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/related.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/related_descriptors.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/related_lookups.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/fields/reverse_related.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/comparison.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/comparison.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Any, ClassVar
 
 from django.db.models import Func
+from django.db.models.expressions import Combinable
 from django.db.models.fields import Field
 from django.db.models.fields.json import JSONField
 
 class Cast(Func):
-    def __init__(self, expression: Any, output_field: str | Field) -> None: ...
+    def __init__(self, expression: Combinable | str, output_field: str | Field) -> None: ...
 
 class Coalesce(Func): ...
 
 class Collate(Func):
-    def __init__(self, expression: Any, collation: str) -> None: ...
+    def __init__(self, expression: Combinable | str, collation: str) -> None: ...
 
 class Greatest(Func): ...
 
 class JSONObject(Func):
     def __init__(self, **fields: Any) -> None: ...
     output_field: ClassVar[JSONField]
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/datetime.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/datetime.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import tzinfo
 from typing import Any, ClassVar
 
 from django.db import models
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Func, Transform
-from django.db.models.expressions import Expression
+from django.db.models.expressions import Combinable
 from django.db.models.fields import Field
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 
 class TimezoneMixin:
     tzinfo: Any
     def get_tzname(self) -> str | None: ...
 
 class Extract(TimezoneMixin, Transform):
     lookup_name: str
     output_field: ClassVar[models.IntegerField]
     def __init__(
-        self, expression: Any, lookup_name: str | None = ..., tzinfo: Any | None = ..., **extra: Any
+        self, expression: Combinable | str, lookup_name: str | None = ..., tzinfo: Any | None = ..., **extra: Any
     ) -> None: ...
 
 class ExtractYear(Extract): ...
 class ExtractIsoYear(Extract): ...
 class ExtractMonth(Extract): ...
 class ExtractDay(Extract): ...
 class ExtractWeek(Extract): ...
@@ -37,22 +37,22 @@
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class TruncBase(TimezoneMixin, Transform):
     kind: str
     tzinfo: Any
 
     def __init__(
-        self, expression: Expression, output_field: Field | None = ..., tzinfo: tzinfo | None = ..., **extra: Any
+        self, expression: Combinable | str, output_field: Field | None = ..., tzinfo: tzinfo | None = ..., **extra: Any
     ) -> None: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...  # type: ignore[override]
 
 class Trunc(TruncBase):
     def __init__(
         self,
-        expression: Expression,
+        expression: Combinable | str,
         kind: str,
         output_field: Field | None = ...,
         tzinfo: tzinfo | None = ...,
         **extra: Any,
     ) -> None: ...
 
 class TruncYear(TruncBase): ...
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/text.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/text.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,42 +28,42 @@
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Concat(Func):
     def __init__(self, *expressions: Any, **extra: Any) -> None: ...
 
 class Left(Func):
     output_field: ClassVar[models.CharField]
-    def __init__(self, expression: Expression | str, length: Expression | int, **extra: Any) -> None: ...
+    def __init__(self, expression: Combinable | str, length: Expression | int, **extra: Any) -> None: ...
     def get_substr(self) -> Substr: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Length(Transform):
     output_field: ClassVar[models.IntegerField]
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Lower(Transform): ...
 
 class LPad(Func):
     output_field: ClassVar[models.CharField]
     def __init__(
-        self, expression: Expression | str, length: Expression | int | None, fill_text: Expression = ..., **extra: Any
+        self, expression: Combinable | str, length: Expression | int | None, fill_text: Expression = ..., **extra: Any
     ) -> None: ...
 
 class LTrim(Transform): ...
 class MD5(OracleHashMixin, Transform): ...
 
 class Ord(Transform):
     output_field: ClassVar[models.IntegerField]
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_mysql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Repeat(Func):
     output_field: ClassVar[models.CharField]
-    def __init__(self, expression: Expression | str, number: Expression | int | None, **extra: Any) -> None: ...
+    def __init__(self, expression: Combinable | str, number: Expression | int | None, **extra: Any) -> None: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Replace(Func):
     def __init__(self, expression: Combinable | str, text: Value, replacement: Value = ..., **extra: Any) -> None: ...
 
 class Reverse(Transform):
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
@@ -87,14 +87,14 @@
     def as_postgresql(
         self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any
     ) -> _AsSqlType: ...
 
 class Substr(Func):
     output_field: ClassVar[models.CharField]
     def __init__(
-        self, expression: Expression | str, pos: Expression | int, length: Expression | int | None = ..., **extra: Any
+        self, expression: Combinable | str, pos: Expression | int, length: Expression | int | None = ..., **extra: Any
     ) -> None: ...
     def as_sqlite(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
     def as_oracle(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper, **extra_context: Any) -> _AsSqlType: ...
 
 class Trim(Transform): ...
 class Upper(Transform): ...
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/functions/window.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/functions/window.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/indexes.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/indexes.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/lookups.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/manager.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/manager.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/options.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/options.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/query.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/query.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/query_utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/query_utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/signals.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/signals.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/compiler.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/datastructures.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/query.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/query.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/subqueries.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/subqueries.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/sql/where.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/sql/where.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/models/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/models/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/transaction.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/transaction.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/db/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/db/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/dispatch/dispatcher.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/dispatch/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/boundfield.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/boundfield.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/fields.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/forms.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/forms.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/formsets.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/formsets.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/models.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/models.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/renderers.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/renderers.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/forms/widgets.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/multipartparser.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/multipartparser.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/request.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/request.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/http/response.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/http/response.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/cache.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/cache.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/common.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/csrf.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/csrf.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/middleware/security.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/shortcuts.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/shortcuts.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/django.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/backends/jinja2.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/backends/jinja2.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/context.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/context.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/context_processors.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/defaultfilters.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/defaultfilters.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/defaulttags.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/engine.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/engine.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/library.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loader.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loader_tags.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loader_tags.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/cached.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/loaders/filesystem.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/response.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/response.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/smartif.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/template/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/template/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/cache.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/i18n.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/i18n.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/static.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/templatetags/tz.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/templatetags/tz.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/client.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/client.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/html.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/html.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/runner.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/runner.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/selenium.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/signals.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/testcases.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/testcases.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/test/utils.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/test/utils.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/conf.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/conf.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/converters.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/converters.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/urls/resolvers.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/urls/resolvers.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/archive.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/archive.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/autoreload.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/autoreload.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/cache.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/choices.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/choices.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/connection.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/connection.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/crypto.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/crypto.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/datastructures.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/dateformat.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/dateformat.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/deconstruct.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/deconstruct.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/decorators.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/decorators.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/deprecation.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/deprecation.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/encoding.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/encoding.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/feedgenerator.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/feedgenerator.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/formats.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/formats.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/functional.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/functional.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/html.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/html.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/http.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/http.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/jslex.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/log.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/log.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/regex_helper.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/safestring.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/safestring.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/termcolors.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/termcolors.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/text.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/text.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/timezone.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/timezone.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/trans_null.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/trans_null.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/translation/trans_real.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/translation/trans_real.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/tree.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/tree.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/utils/version.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/utils/version.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/debug.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/debug.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/decorators/http.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/decorators/http.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/defaults.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/__init__.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/base.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/base.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/dates.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/detail.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/edit.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/edit.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/generic/list.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/generic/list.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/django-stubs/views/i18n.pyi` & `sentry_forked_django_stubs-5.0.2.post2/django-stubs/views/i18n.pyi`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/config.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/config.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/django/context.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/django/context.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/lib/fullnames.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/lib/helpers.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/main.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/main.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/fields.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/fields.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/forms.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/forms.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/functional.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/functional.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/init_create.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/managers.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/managers.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/manytomany.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/manytomany.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/meta.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/meta.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/models.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/models.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/orm_lookups.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/querysets.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/querysets.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/request.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/request.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/mypy_django_plugin/transformers/settings.py` & `sentry_forked_django_stubs-5.0.2.post2/mypy_django_plugin/transformers/settings.py`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/pyproject.toml` & `sentry_forked_django_stubs-5.0.2.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/PKG-INFO` & `sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-forked-django-stubs
-Version: 5.0.2.post1
+Version: 5.0.2.post2
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/sentry_forked_django_stubs.egg-info/SOURCES.txt` & `sentry_forked_django_stubs-5.0.2.post2/sentry_forked_django_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_forked_django_stubs-5.0.2.post1/setup.py` & `sentry_forked_django_stubs-5.0.2.post2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "compatible-mypy": ["mypy~=1.10.0"],
     "redis": ["redis"],
     "oracle": ["oracledb"],
 }
 
 setup(
     name="sentry-forked-django-stubs",
-    version="5.0.2-1",
+    version="5.0.2-2",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
```

### Comparing `sentry_forked_django_stubs-5.0.2.post1/tests/test_error_handling.py` & `sentry_forked_django_stubs-5.0.2.post2/tests/test_error_handling.py`

 * *Files identical despite different names*

