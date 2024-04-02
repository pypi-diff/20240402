# Comparing `tmp/lilya-0.3.0.tar.gz` & `tmp/lilya-0.3.1.tar.gz`

## Comparing `lilya-0.3.0.tar` & `lilya-0.3.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/__main__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_utils.py
--rw-r--r--   0        0        0    28911 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/apps.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/background.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/compat.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/concurrency.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/context.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/controllers.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/crypto.py
--rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/datastructures.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/encoders.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/enums.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/exceptions.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/logging.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/py.typed
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/requests.py
--rw-r--r--   0        0        0    16901 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/responses.py
--rw-r--r--   0        0        0    52914 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/routing.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/staticfiles.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/status.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/transformers.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/types.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/websockets.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/__init__.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_connection.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_encoders.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_events.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_exception_handlers.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_helpers.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_message.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_module_loading.py
--rw-r--r--   0        0        0    16818 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_parsers.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_path.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_path_transformers.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_representation.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_responses.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/_internal/_templates/project_template_simple/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/__init__.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/base.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/cli.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/constants.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/env.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/parsers.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/templates.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/_constants.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/createapp.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/createproject.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/list.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/run.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/runserver.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/terminal/__init__.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/terminal/base.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/terminal/print.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/cli/terminal/terminal.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/conf/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/conf/enums.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/conf/exceptions.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/conf/functional.py
--rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/conf/global_settings.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/__init__.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/asyncexit.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/authentication.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/base.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/compression.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/cors.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/csrf.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/exceptions.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/httpsredirect.py
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/server_error.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/sessions.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/trustedhost.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/styles/__init__.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/middleware/styles/errors.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/permissions/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/permissions/base.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/permissions/deny_all.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/protocols/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/protocols/authentication.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/protocols/middleware.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/protocols/permissions.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/templating/__init__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/templating/base.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/templating/jinja.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/testclient/__init__.py
--rw-r--r--   0        0        0    32033 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/testclient/base.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 lilya-0.3.0/lilya/testclient/helpers.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lilya-0.3.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 lilya-0.3.0/LICENSE
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 lilya-0.3.0/README.md
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 lilya-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 lilya-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/__main__.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_utils.py
+-rw-r--r--   0        0        0    28911 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/apps.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/background.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/compat.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/concurrency.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/context.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/controllers.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/crypto.py
+-rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/datastructures.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/encoders.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/enums.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/exceptions.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/logging.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/py.typed
+-rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/requests.py
+-rw-r--r--   0        0        0    16901 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/responses.py
+-rw-r--r--   0        0        0    52914 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/routing.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/staticfiles.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/status.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/transformers.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/types.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/websockets.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/__init__.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_connection.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_encoders.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_events.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_exception_handlers.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_helpers.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_message.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_module_loading.py
+-rw-r--r--   0        0        0    16818 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_parsers.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_path.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_path_transformers.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_representation.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_responses.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/_internal/_templates/project_template_simple/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/base.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/cli.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/constants.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/env.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/parsers.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/templates.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/list.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/run.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/terminal/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/terminal/base.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/terminal/print.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/cli/terminal/terminal.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/conf/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/conf/enums.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/conf/exceptions.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/conf/functional.py
+-rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/conf/global_settings.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/__init__.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/asyncexit.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/authentication.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/base.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/compression.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/cors.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/csrf.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/exceptions.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/httpsredirect.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/server_error.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/sessions.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/trustedhost.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/styles/__init__.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/middleware/styles/errors.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/permissions/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/permissions/base.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/permissions/deny_all.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/protocols/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/protocols/authentication.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/protocols/middleware.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/protocols/permissions.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/templating/__init__.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/templating/base.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/templating/jinja.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/testclient/__init__.py
+-rw-r--r--   0        0        0    32033 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/testclient/base.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 lilya-0.3.1/lilya/testclient/helpers.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lilya-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 lilya-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 lilya-0.3.1/README.md
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 lilya-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 lilya-0.3.1/PKG-INFO
```

### Comparing `lilya-0.3.0/lilya/_utils.py` & `lilya-0.3.1/lilya/_utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/apps.py` & `lilya-0.3.1/lilya/apps.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/background.py` & `lilya-0.3.1/lilya/background.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/compat.py` & `lilya-0.3.1/lilya/compat.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/concurrency.py` & `lilya-0.3.1/lilya/concurrency.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/context.py` & `lilya-0.3.1/lilya/context.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/controllers.py` & `lilya-0.3.1/lilya/controllers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/crypto.py` & `lilya-0.3.1/lilya/crypto.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/datastructures.py` & `lilya-0.3.1/lilya/datastructures.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/enums.py` & `lilya-0.3.1/lilya/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,16 @@
     JSON = "application/json"
     HTML = "text/html"
     TEXT = "text/plain"
     MESSAGE_PACK = "application/x-msgpack"
     TEXT_CHARSET = "text/plain; charset=utf-8"
     PNG = "image/png"
     OCTET = "application/octet-stream"
+    MULTIPART = "multipart/form-data"
+    URLENCODED = "application/x-www-form-urlencoded"
 
 
 class WebSocketState(IntEnum):
     CONNECTING = 0
     CONNECTED = 1
     DISCONNECTED = 2
```

### Comparing `lilya-0.3.0/lilya/exceptions.py` & `lilya-0.3.1/lilya/exceptions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/logging.py` & `lilya-0.3.1/lilya/logging.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/requests.py` & `lilya-0.3.1/lilya/requests.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Connection,
     empty_receive,
     empty_send,
 )
 from lilya._internal._parsers import FormParser, MultiPartException, MultiPartParser
 from lilya.compat import AsyncResourceHandler
 from lilya.datastructures import FormData
-from lilya.enums import Event, ScopeType
+from lilya.enums import Event, MediaType, ScopeType
 from lilya.exceptions import HTTPException
 from lilya.types import Empty, Message, Receive, Scope, Send
 
 try:
     from multipart.multipart import parse_options_header
 except ModuleNotFoundError:  # pragma: nocover
     parse_options_header = None
@@ -37,14 +37,15 @@
         "_receive",
         "_send",
         "_stream_consumed",
         "_is_disconnected",
         "_json",
         "_content_type",
         "_body",
+        "_media",
     )
 
     _form: FormData | None = None
 
     def __init__(
         self, scope: Scope, receive: Receive = empty_receive, send: Send = empty_send
     ) -> None:
@@ -58,18 +59,27 @@
         """
         super().__init__(scope)
         assert scope["type"] == ScopeType.HTTP
         self._receive = receive
         self._send = send
         self._stream_consumed = False
         self._is_disconnected = False
+        self._media = Empty
         self._json = Empty
         self._content_type = Empty
         self._body = Empty
 
+    def _assert_multipart(self) -> None:
+        """
+        Asserts if the multipart python package is installed.
+        """
+        assert (
+            parse_options_header is not None
+        ), "The `python-multipart` library must be installed to use form parsing."
+
     @property
     def method(self) -> str:
         """
         Get the HTTP method of the request.
 
         Returns:
             str: The HTTP method (e.g., "GET", "POST").
@@ -93,25 +103,48 @@
 
         Returns:
             Receive: The send.
         """
         return self._send
 
     @property
+    def media(self) -> dict[str, Any]:
+        """
+        Gathers the information about the media for the request
+        and returns a dictionary type.
+        """
+        self._assert_multipart()
+        if self._media is Empty:
+            content_type_header = self.headers.get("Content-type", "")
+            content_type, opts = parse_options_header(content_type_header)
+            self._media = dict(opts, content_type=content_type)  # type: ignore
+        return cast(Dict[str, Any], self._media)
+
+    @property
+    def charset(self) -> str:
+        """
+        Get a charset for the scope.
+        """
+        return cast(str, self.media.get("charset", "utf-8"))
+
+    @property
     def content_type(self) -> tuple[str, dict[str, str]]:
         """
         Get the content type of the request.
 
         Returns:
             Tuple[str, Dict[str, str]]: The content type as a tuple containing a string
             and a dictionary of parameters.
         """
+        self._assert_multipart()
+
         if self._content_type is Empty:
-            self._content_type = self.headers.get("Content-Type", "")
-        return cast(Tuple[str, Dict[str, str]], self._content_type)
+            content_type = self.headers.get("Content-Type", "")
+            self._content_type, _ = parse_options_header(content_type)
+        return cast(Tuple[str, Dict[str, str]], self._content_type.decode(self.charset))
 
     async def stream(self) -> AsyncGenerator[bytes, None]:
         """
         Stream the request body in asynchronous chunks.
 
         Yields:
             AsyncGenerator[bytes, None]: Bytes representing chunks of the request body.
@@ -141,18 +174,15 @@
         """
         Read the entire request body.
 
         Returns:
             bytes: The request body as bytes.
         """
         if self._body is Empty:
-            chunks: list[bytes] = []
-            async for chunk in self.stream():
-                chunks.append(chunk)
-            self._body = b"".join(chunks)  # type: ignore
+            self._body = b"".join([chunk async for chunk in self.stream()])  # type: ignore
         return cast(bytes, self._body)
 
     async def json(self) -> Any:
         """
         Parse the request body as JSON.
 
         Returns:
@@ -162,14 +192,41 @@
             if "_body" in self.scope:
                 body = self.scope["_body"]
             else:
                 body = self.scope["_body"] = await self.body() or b"null"
             self._json = json.loads(body)
         return self._json
 
+    async def text(self) -> Any:
+        """
+        Returns the body in as a string.
+        """
+        body = await self.body()
+        try:
+            return body.decode(self.charset)
+        except (LookupError, ValueError) as exc:
+            raise exc
+
+    async def data(self, *, raise_exception: bool = False) -> str | bytes | Any:
+        """
+        Returns any form or multipart forms from the request
+        or simply returns a JSON or text/plain format.
+        """
+        try:
+            if self.content_type in (MediaType.MULTIPART, MediaType.URLENCODED):
+                return await self.form()
+            if self.content_type == MediaType.JSON:
+                return await self.json()  # type: ignore
+        except ValueError as e:
+            if raise_exception:
+                raise e
+            return await self.body()
+        else:
+            return await self.text()
+
     async def _get_form(
         self,
         *,
         max_files: int | float = 1000,
         max_fields: int | float = 1000,
     ) -> FormData:
         """
@@ -181,17 +238,15 @@
             max_fields (Union[int, float]): Maximum number of fields allowed
                 in the form data.
 
         Returns:
             FormData: The parsed form data.
         """
         if self._form is None:
-            assert (
-                parse_options_header is not None
-            ), "The `python-multipart` library must be installed to use form parsing."
+            self._assert_multipart()
             content_type_header = self.headers.get("Content-Type")
             content_type: bytes
             content_type, _ = parse_options_header(content_type_header)
             if content_type == b"multipart/form-data":
                 try:
                     multipart_parser = MultiPartParser(
                         self.headers,
```

### Comparing `lilya-0.3.0/lilya/responses.py` & `lilya-0.3.1/lilya/responses.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/routing.py` & `lilya-0.3.1/lilya/routing.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/staticfiles.py` & `lilya-0.3.1/lilya/staticfiles.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/status.py` & `lilya-0.3.1/lilya/status.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/types.py` & `lilya-0.3.1/lilya/types.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/websockets.py` & `lilya-0.3.1/lilya/websockets.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_connection.py` & `lilya-0.3.1/lilya/_internal/_connection.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_encoders.py` & `lilya-0.3.1/lilya/_internal/_encoders.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_events.py` & `lilya-0.3.1/lilya/_internal/_events.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_exception_handlers.py` & `lilya-0.3.1/lilya/_internal/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_helpers.py` & `lilya-0.3.1/lilya/_internal/_helpers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_module_loading.py` & `lilya-0.3.1/lilya/_internal/_module_loading.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_parsers.py` & `lilya-0.3.1/lilya/_internal/_parsers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_path.py` & `lilya-0.3.1/lilya/_internal/_path.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_path_transformers.py` & `lilya-0.3.1/lilya/_internal/_path_transformers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_representation.py` & `lilya-0.3.1/lilya/_internal/_representation.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_responses.py` & `lilya-0.3.1/lilya/_internal/_responses.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_urls.py` & `lilya-0.3.1/lilya/_internal/_urls.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template/.gitignore.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template/Makefile.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/main.py-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/serve.py-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template/project_name/urls.py-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl` & `lilya-0.3.1/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/base.py` & `lilya-0.3.1/lilya/cli/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/cli.py` & `lilya-0.3.1/lilya/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/env.py` & `lilya-0.3.1/lilya/cli/env.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/templates.py` & `lilya-0.3.1/lilya/cli/templates.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/utils.py` & `lilya-0.3.1/lilya/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/createapp.py` & `lilya-0.3.1/lilya/cli/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/createdeployment.py` & `lilya-0.3.1/lilya/cli/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/createproject.py` & `lilya-0.3.1/lilya/cli/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/list.py` & `lilya-0.3.1/lilya/cli/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/run.py` & `lilya-0.3.1/lilya/cli/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/runserver.py` & `lilya-0.3.1/lilya/cli/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/show_urls.py` & `lilya-0.3.1/lilya/cli/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/shell/base.py` & `lilya-0.3.1/lilya/cli/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/shell/ipython.py` & `lilya-0.3.1/lilya/cli/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/shell/ptpython.py` & `lilya-0.3.1/lilya/cli/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/directives/operations/shell/utils.py` & `lilya-0.3.1/lilya/cli/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/terminal/base.py` & `lilya-0.3.1/lilya/cli/terminal/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/terminal/print.py` & `lilya-0.3.1/lilya/cli/terminal/print.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/cli/terminal/terminal.py` & `lilya-0.3.1/lilya/cli/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/conf/__init__.py` & `lilya-0.3.1/lilya/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/conf/functional.py` & `lilya-0.3.1/lilya/conf/functional.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/conf/global_settings.py` & `lilya-0.3.1/lilya/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/asyncexit.py` & `lilya-0.3.1/lilya/middleware/asyncexit.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/authentication.py` & `lilya-0.3.1/lilya/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/base.py` & `lilya-0.3.1/lilya/middleware/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/compression.py` & `lilya-0.3.1/lilya/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/cors.py` & `lilya-0.3.1/lilya/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/csrf.py` & `lilya-0.3.1/lilya/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/exceptions.py` & `lilya-0.3.1/lilya/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/httpsredirect.py` & `lilya-0.3.1/lilya/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/server_error.py` & `lilya-0.3.1/lilya/middleware/server_error.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/sessions.py` & `lilya-0.3.1/lilya/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/trustedhost.py` & `lilya-0.3.1/lilya/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/wsgi.py` & `lilya-0.3.1/lilya/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/middleware/styles/errors.py` & `lilya-0.3.1/lilya/middleware/styles/errors.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/permissions/base.py` & `lilya-0.3.1/lilya/permissions/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/permissions/deny_all.py` & `lilya-0.3.1/lilya/permissions/deny_all.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/protocols/authentication.py` & `lilya-0.3.1/lilya/protocols/authentication.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/protocols/middleware.py` & `lilya-0.3.1/lilya/protocols/middleware.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/protocols/permissions.py` & `lilya-0.3.1/lilya/protocols/permissions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/templating/base.py` & `lilya-0.3.1/lilya/templating/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/templating/jinja.py` & `lilya-0.3.1/lilya/templating/jinja.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/testclient/base.py` & `lilya-0.3.1/lilya/testclient/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/lilya/testclient/helpers.py` & `lilya-0.3.1/lilya/testclient/helpers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/LICENSE` & `lilya-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/README.md` & `lilya-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lilya-0.3.0/pyproject.toml` & `lilya-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -74,25 +74,25 @@
 ]
 
 test = [
     "a2wsgi>=1.10.0,<2.0.0",
     "autoflake>=2.0.2,<3.0.0",
     "anyio[trio]>=3.6.2,<5.0.0",
     "asyncio[trio]>=3.4.3,<4.0.0",
-    "black==24.1.1,<25.0",
+    "black==24.3.0,<25.0",
     "edgy[postgres]>=0.9.2,<1.0.0",
     "email-validator>=2.1.0.post1",
     "flask>=3.0.2,<4.0.0",
     "freezegun>=1.4.0,<2.0.0",
     "httpx>=0.25.2,<1.0.0",
     "isort>=5.12.0,<6.0.0",
     "jinja2>=3.1.3,<4.0.0",
     "mako>=1.3.2,<2.0.0",
     "msgspec>=0.18.6,<0.20.0",
-    "mypy==1.8.0",
+    "mypy==1.9.0",
     "pydantic>=2.6.0,<3",
     "pytest>=7.2.2,<9.0.0",
     "pytest-asyncio>=0.23.2",
     "pytest-cov>=4.0.0,<5.0.0",
     "pytest-mock>=3.12.0",
     "python-multipart>=0.0.6",
     "requests>=2.28.2",
```

### Comparing `lilya-0.3.0/PKG-INFO` & `lilya-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lilya
-Version: 0.3.0
+Version: 0.3.1
 Summary: Yet another ASGI toolkit that delivers
 Project-URL: Homepage, https://github.com/dymmond/lilya
 Project-URL: Documentation, https://lilya.dev
 Project-URL: Changelog, https://lilya.dev/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/lilya
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -75,25 +75,25 @@
 Provides-Extra: ptpython
 Requires-Dist: ptpython>=3.0.23; extra == 'ptpython'
 Provides-Extra: test
 Requires-Dist: a2wsgi<2.0.0,>=1.10.0; extra == 'test'
 Requires-Dist: anyio[trio]<5.0.0,>=3.6.2; extra == 'test'
 Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
 Requires-Dist: autoflake<3.0.0,>=2.0.2; extra == 'test'
-Requires-Dist: black<25.0,==24.1.1; extra == 'test'
+Requires-Dist: black<25.0,==24.3.0; extra == 'test'
 Requires-Dist: edgy[postgres]<1.0.0,>=0.9.2; extra == 'test'
 Requires-Dist: email-validator>=2.1.0.post1; extra == 'test'
 Requires-Dist: flask<4.0.0,>=3.0.2; extra == 'test'
 Requires-Dist: freezegun<2.0.0,>=1.4.0; extra == 'test'
 Requires-Dist: httpx<1.0.0,>=0.25.2; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
 Requires-Dist: jinja2<4.0.0,>=3.1.3; extra == 'test'
 Requires-Dist: mako<2.0.0,>=1.3.2; extra == 'test'
 Requires-Dist: msgspec<0.20.0,>=0.18.6; extra == 'test'
-Requires-Dist: mypy==1.8.0; extra == 'test'
+Requires-Dist: mypy==1.9.0; extra == 'test'
 Requires-Dist: pydantic<3,>=2.6.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.23.2; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'test'
 Requires-Dist: pytest-mock>=3.12.0; extra == 'test'
 Requires-Dist: pytest<9.0.0,>=7.2.2; extra == 'test'
 Requires-Dist: python-multipart>=0.0.6; extra == 'test'
 Requires-Dist: requests>=2.28.2; extra == 'test'
```

