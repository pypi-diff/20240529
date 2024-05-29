# Comparing `tmp/lilya-0.7.1.tar.gz` & `tmp/lilya-0.7.2.tar.gz`

## Comparing `lilya-0.7.1.tar` & `lilya-0.7.2.tar`

### file list

```diff
@@ -1,150 +1,158 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/__main__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_utils.py
--rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/apps.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/background.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/compat.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/concurrency.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/context.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/controllers.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/crypto.py
--rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/datastructures.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/encoders.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/enums.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/environments.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/exceptions.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/logging.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/py.typed
--rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/requests.py
--rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/responses.py
--rw-r--r--   0        0        0    53033 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/routing.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/staticfiles.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/status.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/transformers.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/types.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/websockets.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/__init__.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_connection.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_encoders.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_events.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_exception_handlers.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_helpers.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_message.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_module_loading.py
--rw-r--r--   0        0        0    16818 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_parsers.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_path.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_path_transformers.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_representation.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_responses.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/v1/controllers.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/_internal/_templates/project_template_simple/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/__init__.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/base.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/cli.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/constants.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/env.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/parsers.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/templates.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/_constants.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/createapp.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/createproject.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/list.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/run.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/runserver.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/terminal/__init__.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/terminal/base.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/terminal/print.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/cli/terminal/terminal.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/conf/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/conf/enums.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/conf/exceptions.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/conf/functional.py
--rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/conf/global_settings.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/app_settings.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/asyncexit.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/authentication.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/base.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/compression.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/cors.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/csrf.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/exceptions.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/httpsredirect.py
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/server_error.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/sessions.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/trustedhost.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/styles/__init__.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/middleware/styles/errors.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/permissions/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/permissions/base.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/permissions/deny_all.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/protocols/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/protocols/authentication.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/protocols/middleware.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/protocols/permissions.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/templating/__init__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/templating/base.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/templating/jinja.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/testclient/__init__.py
--rw-r--r--   0        0        0    32033 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/testclient/base.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 lilya-0.7.1/lilya/testclient/helpers.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lilya-0.7.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 lilya-0.7.1/LICENSE
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 lilya-0.7.1/README.md
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 lilya-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 lilya-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/__main__.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_utils.py
+-rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/app.py
+-rw-r--r--   0        0        0    29533 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/apps.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/background.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/compat.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/concurrency.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/context.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/controllers.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/crypto.py
+-rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/datastructures.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/encoders.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/enums.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/environments.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/exceptions.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/logging.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/py.typed
+-rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/requests.py
+-rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/responses.py
+-rw-r--r--   0        0        0    53033 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/routing.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/staticfiles.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/status.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/transformers.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/types.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/websockets.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/__init__.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_connection.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_encoders.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_events.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_exception_handlers.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_helpers.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_message.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_module_loading.py
+-rw-r--r--   0        0        0    16818 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_parsers.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_path.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_path_transformers.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_representation.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_responses.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/_internal/_templates/project_template_simple/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/__init__.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/base.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/cli.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/constants.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/env.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/parsers.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/templates.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/list.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/run.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/terminal/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/terminal/base.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/terminal/print.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/cli/terminal/terminal.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/conf/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/conf/enums.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/conf/exceptions.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/conf/functional.py
+-rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/conf/global_settings.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/app_settings.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/asyncexit.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/authentication.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/base.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/compression.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/cors.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/csrf.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/exceptions.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/httpsredirect.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/server_error.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/sessions.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/trustedhost.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/styles/__init__.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/middleware/styles/errors.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/permissions/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/permissions/base.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/permissions/deny_all.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/protocols/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/protocols/authentication.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/protocols/middleware.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/protocols/permissions.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/templating/__init__.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/templating/base.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/templating/jinja.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/__init__.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/exceptions.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/_internal/__init__.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/_internal/inputs.py
+-rw-r--r--   0        0        0    15340 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/_internal/transport.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/_internal/types.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/_internal/utils.py
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 lilya-0.7.2/lilya/testclient/_internal/websockets.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lilya-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 lilya-0.7.2/LICENSE
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 lilya-0.7.2/README.md
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 lilya-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 lilya-0.7.2/PKG-INFO
```

### Comparing `lilya-0.7.1/lilya/_utils.py` & `lilya-0.7.2/lilya/_utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/apps.py` & `lilya-0.7.2/lilya/app.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/background.py` & `lilya-0.7.2/lilya/background.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/compat.py` & `lilya-0.7.2/lilya/compat.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/concurrency.py` & `lilya-0.7.2/lilya/concurrency.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/context.py` & `lilya-0.7.2/lilya/context.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/controllers.py` & `lilya-0.7.2/lilya/controllers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/crypto.py` & `lilya-0.7.2/lilya/crypto.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/datastructures.py` & `lilya-0.7.2/lilya/datastructures.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/enums.py` & `lilya-0.7.2/lilya/enums.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/environments.py` & `lilya-0.7.2/lilya/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import os
 import warnings
 from pathlib import Path
-from typing import Any, Callable, Generator, TypeVar
-from typing import cast as tcast
+from typing import Any, Callable, Generator, TypeVar, cast as tcast
 
 from multidict import MultiDict
 
 from lilya.exceptions import EnvironmentError
 from lilya.types import Empty
 
 Cast = Callable[..., Any]
```

### Comparing `lilya-0.7.1/lilya/exceptions.py` & `lilya-0.7.2/lilya/exceptions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/logging.py` & `lilya-0.7.2/lilya/logging.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/requests.py` & `lilya-0.7.2/lilya/requests.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/responses.py` & `lilya-0.7.2/lilya/responses.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/routing.py` & `lilya-0.7.2/lilya/routing.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/staticfiles.py` & `lilya-0.7.2/lilya/staticfiles.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/status.py` & `lilya-0.7.2/lilya/status.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/types.py` & `lilya-0.7.2/lilya/types.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/websockets.py` & `lilya-0.7.2/lilya/websockets.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_connection.py` & `lilya-0.7.2/lilya/_internal/_connection.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_encoders.py` & `lilya-0.7.2/lilya/_internal/_encoders.py`

 * *Files 23% similar despite different names*

```diff
@@ -90,22 +90,31 @@
 def register_encoder(encoder: Encoder[Any] | type[Encoder[Any]]) -> None:
     if is_class_and_subclass(encoder, Encoder):
         encoder = encoder()  # type: ignore
     ENCODER_TYPES.add(cast(Encoder[Any], encoder))
 
 
 def json_encoder(value: Any) -> Any:
-    result: Any = None
+    """
+    Encode a value to a JSON-compatible format using a list of encoder types.
+
+    Parameters:
+    value (Any): The value to encode.
+    encoder_types (List[Type[EncoderType]]): A list of encoder type classes to use for encoding.
+
+    Returns:
+    Any: The JSON-compatible encoded value.
+
+    Raises:
+    ValueError: If the value is not serializable by any provided encoder type.
+    """
 
     for encoder in ENCODER_TYPES:
         try:
-            if not encoder.is_type(value):
-                continue
-            result = encoder.serialize(value)
-            break
+            if encoder.is_type(value):
+                return encoder.serialize(value)
         except (TypeError, AttributeError):
+            # Log the exception if necessary for debugging
             continue
 
-    if result is None:
-        raise ValueError(f"object of type {type(value)} is not json serializable.")
-
-    return result
+    # If no encoder was found, raise a ValueError
+    raise ValueError(f"Object of type '{type(value).__name__}' is not JSON serializable.")
```

### Comparing `lilya-0.7.1/lilya/_internal/_events.py` & `lilya-0.7.2/lilya/_internal/_events.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_exception_handlers.py` & `lilya-0.7.2/lilya/_internal/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_helpers.py` & `lilya-0.7.2/lilya/_internal/_helpers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_module_loading.py` & `lilya-0.7.2/lilya/_internal/_module_loading.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_parsers.py` & `lilya-0.7.2/lilya/_internal/_parsers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_path.py` & `lilya-0.7.2/lilya/_internal/_path.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_path_transformers.py` & `lilya-0.7.2/lilya/_internal/_path_transformers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_representation.py` & `lilya-0.7.2/lilya/_internal/_representation.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_responses.py` & `lilya-0.7.2/lilya/_internal/_responses.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_urls.py` & `lilya-0.7.2/lilya/_internal/_urls.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template/.gitignore.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template/Makefile.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/main.py-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/serve.py-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template/project_name/urls.py-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl` & `lilya-0.7.2/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/base.py` & `lilya-0.7.2/lilya/cli/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/cli.py` & `lilya-0.7.2/lilya/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/env.py` & `lilya-0.7.2/lilya/cli/env.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/templates.py` & `lilya-0.7.2/lilya/cli/templates.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/utils.py` & `lilya-0.7.2/lilya/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/createapp.py` & `lilya-0.7.2/lilya/cli/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/createdeployment.py` & `lilya-0.7.2/lilya/cli/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/createproject.py` & `lilya-0.7.2/lilya/cli/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/list.py` & `lilya-0.7.2/lilya/cli/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/run.py` & `lilya-0.7.2/lilya/cli/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/runserver.py` & `lilya-0.7.2/lilya/cli/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/show_urls.py` & `lilya-0.7.2/lilya/cli/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/shell/base.py` & `lilya-0.7.2/lilya/cli/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/shell/ipython.py` & `lilya-0.7.2/lilya/cli/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/shell/ptpython.py` & `lilya-0.7.2/lilya/cli/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/directives/operations/shell/utils.py` & `lilya-0.7.2/lilya/cli/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/terminal/base.py` & `lilya-0.7.2/lilya/cli/terminal/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/terminal/print.py` & `lilya-0.7.2/lilya/cli/terminal/print.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/cli/terminal/terminal.py` & `lilya-0.7.2/lilya/cli/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/conf/__init__.py` & `lilya-0.7.2/lilya/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/conf/functional.py` & `lilya-0.7.2/lilya/conf/functional.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/conf/global_settings.py` & `lilya-0.7.2/lilya/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/app_settings.py` & `lilya-0.7.2/lilya/middleware/app_settings.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/asyncexit.py` & `lilya-0.7.2/lilya/middleware/asyncexit.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/authentication.py` & `lilya-0.7.2/lilya/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/base.py` & `lilya-0.7.2/lilya/middleware/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/compression.py` & `lilya-0.7.2/lilya/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/cors.py` & `lilya-0.7.2/lilya/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/csrf.py` & `lilya-0.7.2/lilya/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/exceptions.py` & `lilya-0.7.2/lilya/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/httpsredirect.py` & `lilya-0.7.2/lilya/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/server_error.py` & `lilya-0.7.2/lilya/middleware/server_error.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/sessions.py` & `lilya-0.7.2/lilya/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/trustedhost.py` & `lilya-0.7.2/lilya/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/wsgi.py` & `lilya-0.7.2/lilya/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/middleware/styles/errors.py` & `lilya-0.7.2/lilya/middleware/styles/errors.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/permissions/base.py` & `lilya-0.7.2/lilya/permissions/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/permissions/deny_all.py` & `lilya-0.7.2/lilya/permissions/deny_all.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/protocols/authentication.py` & `lilya-0.7.2/lilya/protocols/authentication.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/protocols/middleware.py` & `lilya-0.7.2/lilya/protocols/middleware.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/protocols/permissions.py` & `lilya-0.7.2/lilya/protocols/permissions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/templating/base.py` & `lilya-0.7.2/lilya/templating/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/templating/jinja.py` & `lilya-0.7.2/lilya/templating/jinja.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/lilya/testclient/helpers.py` & `lilya-0.7.2/lilya/testclient/helpers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/LICENSE` & `lilya-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/README.md` & `lilya-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `lilya-0.7.1/pyproject.toml` & `lilya-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -88,26 +88,28 @@
     "pydantic>=2.6.0,<3",
     "pytest>=7.2.2,<9.0.0",
     "pytest-asyncio>=0.23.2",
     "pytest-cov>=4.0.0,<5.0.0",
     "pytest-mock>=3.12.0",
     "python-multipart>=0.0.6",
     "requests>=2.28.2",
-    "mypy==1.9.0",
+    "mypy==1.10.0",
     "ipython",
     "ptpython",
+    "ipdb",
+    "pdbpp",
 ]
 
 [tool.hatch.version]
 path = "lilya/__init__.py"
 
 
 [tool.hatch.envs.default]
 dependencies = [
-    "mypy==1.9.0",
+    "mypy==1.10.0",
     "ruff>=0.3.0,<5.0.0",
     "pre-commit>=3.3.1,<4.0.0",
     "devtools>=0.12.2",
     "ipython",
     "ptpython",
     "twine",
 ]
@@ -140,17 +142,18 @@
 [tool.hatch.envs.test]
 features = ['testing']
 template = "test"
 installer = "pip"
 
 [tool.hatch.envs.test.scripts]
 # needs docker services running
-test = "LILYA_SETTINGS_MODULE='tests.settings.TestSettings' pytest -s -vv {args} --disable-pytest-warnings"
+test = "LILYA_SETTINGS_MODULE='tests.settings.TestSettings' pytest {args} --disable-pytest-warnings"
+test_man = "LILYA_SETTINGS_MODULE='tests.settings.TestSettings' pytest {args} --disable-pytest-warnings -s -vv"
 coverage = "LILYA_SETTINGS_MODULE='tests.settings.TestSettings' pytest --cov=lilya --cov=tests --cov-report=term-missing:skip-covered --cov-report=html tests {args}"
-check_types = "mypy -p lilya"
+check_types = "mypy -p lilya --show-traceback"
 
 
 [project.scripts]
 lilya = "lilya.__main__:run_cli"
 
 [tool.mypy]
 strict = true
@@ -163,15 +166,15 @@
 show_error_codes = true
 disallow_incomplete_defs = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 no_implicit_optional = false
 strict_equality = false
 strict_optional = false
-disable_error_code = "attr-defined,has-type,override"
+disable_error_code = "attr-defined,has-type,override,misc,safe-super"
 exclude = ["lilya/compat.py"]
 
 [tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
```

### Comparing `lilya-0.7.1/PKG-INFO` & `lilya-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lilya
-Version: 0.7.1
+Version: 0.7.2
 Summary: Yet another ASGI toolkit that delivers
 Project-URL: Homepage, https://github.com/dymmond/lilya
 Project-URL: Documentation, https://lilya.dev
 Project-URL: Changelog, https://lilya.dev/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/lilya
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -63,18 +63,20 @@
 Requires-Dist: anyio[trio]<5.0.0,>=3.6.2; extra == 'testing'
 Requires-Dist: autoflake<3.0.0,>=2.0.2; extra == 'testing'
 Requires-Dist: edgy[postgres]<1.0.0,>=0.9.2; extra == 'testing'
 Requires-Dist: email-validator>=2.1.0.post1; extra == 'testing'
 Requires-Dist: flask<4.0.0,>=3.0.2; extra == 'testing'
 Requires-Dist: httpx<1.0.0,>=0.25.2; extra == 'testing'
 Requires-Dist: httpx>=0.22.0; extra == 'testing'
+Requires-Dist: ipdb; extra == 'testing'
 Requires-Dist: ipython; extra == 'testing'
 Requires-Dist: jinja2<4.0.0,>=3.1.3; extra == 'testing'
 Requires-Dist: msgspec<0.20.0,>=0.18.6; extra == 'testing'
-Requires-Dist: mypy==1.9.0; extra == 'testing'
+Requires-Dist: mypy==1.10.0; extra == 'testing'
+Requires-Dist: pdbpp; extra == 'testing'
 Requires-Dist: ptpython; extra == 'testing'
 Requires-Dist: pydantic<3,>=2.6.0; extra == 'testing'
 Requires-Dist: pytest-asyncio>=0.23.2; extra == 'testing'
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'testing'
 Requires-Dist: pytest-mock>=3.12.0; extra == 'testing'
 Requires-Dist: pytest<9.0.0,>=7.2.2; extra == 'testing'
 Requires-Dist: python-multipart>=0.0.6; extra == 'testing'
```

