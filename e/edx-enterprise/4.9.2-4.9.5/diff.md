# Comparing `tmp/edx-enterprise-4.9.2.tar.gz` & `tmp/edx-enterprise-4.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-4.9.2.tar", last modified: Wed Jan 10 12:51:03 2024, max compression
+gzip compressed data, was "edx-enterprise-4.9.5.tar", last modified: Mon Jan 15 12:40:10 2024, max compression
```

## Comparing `edx-enterprise-4.9.2.tar` & `edx-enterprise-4.9.5.tar`

### file list

```diff
@@ -1,829 +1,831 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.538303 edx-enterprise-4.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)   145032 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)   196797 2024-01-10 12:51:03.538303 edx-enterprise-4.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.430303 edx-enterprise-4.9.2/consent/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.430303 edx-enterprise-4.9.2/consent/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.430303 edx-enterprise-4.9.2/consent/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.430303 edx-enterprise-4.9.2/consent/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.430303 edx-enterprise-4.9.2/consent/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/0004_datasharingconsenttextoverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/0005_auto_20230707_0755.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/0006_alter_historicaldatasharingconsent_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    15248 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/consent/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.434303 edx-enterprise-4.9.2/edx_enterprise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   196797 2024-01-10 12:51:02.000000 edx-enterprise-4.9.2/edx_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    42717 2024-01-10 12:51:03.000000 edx-enterprise-4.9.2/edx_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 12:51:02.000000 edx-enterprise-4.9.2/edx_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 12:51:02.000000 edx-enterprise-4.9.2/edx_enterprise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-10 12:51:02.000000 edx-enterprise-4.9.2/edx_enterprise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-10 12:51:02.000000 edx-enterprise-4.9.2/edx_enterprise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.438303 edx-enterprise-4.9.2/enterprise/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.438303 edx-enterprise-4.9.2/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (127)    38370 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30441 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39729 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/admin/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.438303 edx-enterprise-4.9.2/enterprise/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.438303 edx-enterprise-4.9.2/enterprise/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    63112 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.442303 edx-enterprise-4.9.2/enterprise/api/v1/views/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/analytics_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/base_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/coupon_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_catalog_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_api_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_branding_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_sso_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    28693 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/pending_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api/v1/views/plotly_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/api_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/braze.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/enterprise_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/lms.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/open_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/api_client/sso_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/conf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/conf/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/conf/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/conf/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    41500 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/conf/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/conf/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/conf/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/conf/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   104293 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/conf/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/conf/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/conf/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/conf/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    45236 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/conf/locale/es_419/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/config/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/heartbeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/heartbeat/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/heartbeat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/heartbeat/throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/heartbeat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/heartbeat/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    41500 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)   104293 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    45236 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.446303 edx-enterprise-4.9.2/enterprise/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.450303 edx-enterprise-4.9.2/enterprise/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/backfill_learner_role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/bulk_update_catalog_query_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/create_enterprise_course_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/create_missing_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/email_drip_for_missing_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/fix_dsc_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/manufacture_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/migrate_enterprise_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/monthly_impact_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/reencrypt_enterprise_customer_reporting_config_passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/revert_enrollment_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/save_enterprise_customer_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/seed_enterprise_devstack_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/unlink_enterprise_customer_learners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/update_config_last_errored_at.py
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/management/commands/update_role_assignments_with_customers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.466303 edx-enterprise-4.9.2/enterprise/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0001_auto_20210111_1253.py
--rw-r--r--   0 runner    (1001) docker     (127)    52500 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0095_auto_20200507_1138.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0096_enterprise_catalog_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0097_auto_20200619_1130.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0098_auto_20200629_1756.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0099_auto_20200702_1537.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0101_move_data_to_saved_for_later.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0102_auto_20200708_1615.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0103_remove_marked_done.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0104_sync_query_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0105_add_branding_config_color_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0106_move_branding_config_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0107_remove_branding_config_banner_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0110_add_default_contract_discount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0112_auto_20200914_0926.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0113_auto_20200914_2054.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0114_auto_20201020_0142.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0116_auto_20201116_0400.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0116_auto_20201208_1759.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0117_auto_20201215_0258.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0124_auto_20210301_1309.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0125_add_config_for_role_assign_backfill.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0126_auto_20210308_1522.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0127_enterprisecatalogquery_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0129_enterprisecatalogquery_uuid_unique.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0130_lms_customer_lp_search_help_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0131_auto_20210517_0924.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0132_auto_20210608_1921.py
--rw-r--r--   0 runner    (1001) docker     (127)    26436 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0133_auto_20210608_1931.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0136_auto_20210629_2129.py
--rw-r--r--   0 runner    (1001) docker     (127)    16936 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0137_enrollment_email_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0139_auto_20210803_1854.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0140_update_enrollment_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0142_auto_20210907_2059.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0143_auto_20210908_0559.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0144_auto_20211011_1030.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0145_auto_20211013_1018.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0146_enterprise_customer_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0147_auto_20211129_1949.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0148_auto_20211129_2114.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0150_invite_key_expiry_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0151_add_is_active_to_invite_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0152_add_should_inactivate_other_customers.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0153_add_enable_browse_and_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0156_add_is_active_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0157_make_field_nullable_before_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0158_remove_is_active_from_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0159_add_enable_learner_portal_offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0163_auto_20220928_1611.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0166_auto_20221209_0819.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0167_auto_20230209_2108.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0168_auto_20230222_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0169_auto_20230222_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0170_auto_20230301_1627.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0171_auto_20230503_1413.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0172_auto_20230517_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0173_auto_20230531_1459.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0174_auto_20230608_2041.py
--rw-r--r--   0 runner    (1001) docker     (127)    19527 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0175_auto_20230629_2330.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0176_auto_20230712_1751.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0177_auto_20230712_1925.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0178_auto_20230808_0923.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0179_restore_historical_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0180_chatgptresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0181_enterprisecustomerssoconfiguration_historicalenterprisecustomerssoconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0182_auto_20230829_1741.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0183_auto_20230906_1435.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0184_auto_20230914_2057.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0185_auto_20230921_1007.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0186_auto_20230921_1828.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0187_auto_20230926_1627.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0188_alter_learnercreditenterprisecourseenrollment_enterprise_course_enrollment_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0189_auto_20231002_0902.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0190_auto_20231003_0719.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0191_auto_20231006_0948.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0192_auto_20231009_1302.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0193_auto_20231005_1708.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0194_auto_20231013_1359.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0195_auto_20231130_1837.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0196_backfill_sso_marked_authorized.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/0197_auto_20231130_2239.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/migrations/unique_constraints_pending_users.py
--rw-r--r--   0 runner    (1001) docker     (127)   152269 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.470303 edx-enterprise-4.9.2/enterprise/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/static/enterprise/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.470303 edx-enterprise-4.9.2/enterprise/static/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.470303 edx-enterprise-4.9.2/enterprise/static/enterprise/bundles/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/bundles/main-admin.style.css
--rw-r--r--   0 runner    (1001) docker     (127)   295145 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/bundles/main.style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.470303 edx-enterprise-4.9.2/enterprise/static/enterprise/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/course_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/enterprise_customer.js
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/enterprise_login_page.js
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/enterprise_selection_page.js
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/manage_learners.js
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/static/enterprise/js/program_enrollment_landing_page.js
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.418303 edx-enterprise-4.9.2/enterprise/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise/templates/enterprise/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_decline_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_policy.html
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_user_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/manage_learners.html
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/oauth_authorization_failed.html
--rw-r--r--   0 runner    (1001) docker     (127)    27091 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/oauth_authorization_successful.html
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/setup_auth_org_id.html
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_customer_login_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_customer_select_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/grant_data_sharing_permissions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise/templates/enterprise/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/templatetags/alert_messages.html
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/templatetags/course_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/templatetags/expand_button.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/templatetags/fa_icon.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise/templates/enterprise/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templates/enterprise/widgets/segment-io-django.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/templatetags/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/toggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/tpa_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    87041 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)   112485 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise/views_error_codes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise_learner_portal/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise_learner_portal/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.474303 edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/enterprise_learner_portal/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/enterprise_learner_portal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/integrated_channels/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/integrated_channels/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/integrated_channels/api/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.478303 edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/api/v1/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/logs/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/logs/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/logs/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/api/v1/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/moodle/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/moodle/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/moodle/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/blackboard/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.482303 edx-enterprise-4.9.2/integrated_channels/blackboard/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    39044 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.486303 edx-enterprise-4.9.2/integrated_channels/blackboard/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.486303 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0016_auto_20230719_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0017_alter_historicalblackboardenterprisecustomerconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.486303 edx-enterprise-4.9.2/integrated_channels/blackboard/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/blackboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.490303 edx-enterprise-4.9.2/integrated_channels/canvas/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.490303 edx-enterprise-4.9.2/integrated_channels/canvas/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    38633 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.490303 edx-enterprise-4.9.2/integrated_channels/canvas/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.494303 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0031_auto_20230719_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0032_alter_historicalcanvasenterprisecustomerconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.494303 edx-enterprise-4.9.2/integrated_channels/canvas/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/canvas/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/catalog_service_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.494303 edx-enterprise-4.9.2/integrated_channels/cornerstone/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.494303 edx-enterprise-4.9.2/integrated_channels/cornerstone/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.494303 edx-enterprise-4.9.2/integrated_channels/cornerstone/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.498303 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0017_alter_cornerstonelearnerdatatransmissionaudit_course_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0028_auto_20230719_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0029_alter_historicalcornerstoneenterprisecustomerconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0030_auto_20231010_1654.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.502303 edx-enterprise-4.9.2/integrated_channels/cornerstone/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/cornerstone/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.502303 edx-enterprise-4.9.2/integrated_channels/degreed/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.502303 edx-enterprise-4.9.2/integrated_channels/degreed/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.502303 edx-enterprise-4.9.2/integrated_channels/degreed/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.506303 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0030_auto_20230719_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0031_alter_historicaldegreedenterprisecustomerconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.506303 edx-enterprise-4.9.2/integrated_channels/degreed/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed/transmitters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.506303 edx-enterprise-4.9.2/integrated_channels/degreed2/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.506303 edx-enterprise-4.9.2/integrated_channels/degreed2/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    25286 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.506303 edx-enterprise-4.9.2/integrated_channels/degreed2/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.510303 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0008_degreed2learnerdatatransmissionaudit_course_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0022_auto_20230719_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0023_alter_historicaldegreed2enterprisecustomerconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.510303 edx-enterprise-4.9.2/integrated_channels/degreed2/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/degreed2/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.510303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.510303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/channel_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.514303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32575 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    41034 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.514303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.514303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/assign_skills_to_degreed_courses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/remove_null_catalog_transmission_audits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.518303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0002_learnerdatatransmissionaudit_subsection_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0005_auto_20211005_1052.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0006_contentmetadataitemtransmission_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0007_delete_learnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0011_contentmetadataitemtransmission_plugin_configuration_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0012_alter_contentmetadataitemtransmission_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_content_title.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0019_merge_20220928_1842.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0021_remove_contentmetadataitemtransmission_api_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0029_genericenterprisecustomerpluginconfiguration_show_course_price.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33134 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20241 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.518303 edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    23097 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/lms_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.522303 edx-enterprise-4.9.2/integrated_channels/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.522303 edx-enterprise-4.9.2/integrated_channels/moodle/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19906 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.522303 edx-enterprise-4.9.2/integrated_channels/moodle/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/exporters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.526303 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0026_auto_20230719_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0027_alter_historicalmoodleenterprisecustomerconfiguration_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0028_auto_20230928_1530.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0028_auto_20231116_1826.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0029_auto_20231106_1233.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0030_merge_0028_auto_20231116_1826_0029_auto_20231106_1233.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.526303 edx-enterprise-4.9.2/integrated_channels/moodle/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/moodle/transmitters/learner_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.526303 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.526303 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.526303 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.530303 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactorsenterprisecustomerconfiguration_deleted_at.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0014_alter_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.530303 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/transmitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/transmitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/transmitters/content_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/sap_success_factors/transmitters/learner_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.530303 edx-enterprise-4.9.2/integrated_channels/xapi/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.530303 edx-enterprise-4.9.2/integrated_channels/xapi/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.530303 edx-enterprise-4.9.2/integrated_channels/xapi/management/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.530303 edx-enterprise-4.9.2/integrated_channels/xapi/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/management/commands/send_course_completions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/management/commands/send_course_enrollments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.534303 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.534303 edx-enterprise-4.9.2/integrated_channels/xapi/statements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/statements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/statements/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/statements/learner_course_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/statements/learner_course_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/integrated_channels/xapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 12:51:03.538303 edx-enterprise-4.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/celery53.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)    25030 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/doc.in
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28622 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/edx-platform-constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/js_test.in
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/js_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/test-master.in
--rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-10 12:51:03.538303 edx-enterprise-4.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4028 2024-01-10 12:49:54.000000 edx-enterprise-4.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.417964 edx-enterprise-4.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)   145268 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35136 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)   197153 2024-01-15 12:40:10.417964 edx-enterprise-4.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.321963 edx-enterprise-4.9.5/consent/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.321963 edx-enterprise-4.9.5/consent/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.321963 edx-enterprise-4.9.5/consent/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.321963 edx-enterprise-4.9.5/consent/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.321963 edx-enterprise-4.9.5/consent/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/0002_migrate_to_new_data_sharing_consent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/0003_historicaldatasharingconsent_history_change_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/0004_datasharingconsenttextoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/0005_auto_20230707_0755.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/0006_alter_historicaldatasharingconsent_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15248 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/consent/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.325963 edx-enterprise-4.9.5/edx_enterprise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   197153 2024-01-15 12:40:09.000000 edx-enterprise-4.9.5/edx_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    42884 2024-01-15 12:40:10.000000 edx-enterprise-4.9.5/edx_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 12:40:09.000000 edx-enterprise-4.9.5/edx_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 12:40:09.000000 edx-enterprise-4.9.5/edx_enterprise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-15 12:40:09.000000 edx-enterprise-4.9.5/edx_enterprise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-15 12:40:09.000000 edx-enterprise-4.9.5/edx_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.329963 edx-enterprise-4.9.5/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.329963 edx-enterprise-4.9.5/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    38370 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30441 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39729 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/admin/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.329963 edx-enterprise-4.9.5/enterprise/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.329963 edx-enterprise-4.9.5/enterprise/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63112 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.333963 edx-enterprise-4.9.5/enterprise/api/v1/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/analytics_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/base_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/coupon_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_catalog_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_api_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_branding_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_sso_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28693 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/pending_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api/v1/views/plotly_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.333963 edx-enterprise-4.9.5/enterprise/api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/braze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15569 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/enterprise_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/lms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/open_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/api_client/sso_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/conf/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/conf/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.333963 edx-enterprise-4.9.5/enterprise/conf/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    41500 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/conf/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/conf/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/conf/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/conf/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   104293 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/conf/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/conf/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/conf/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/conf/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    45236 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/conf/locale/es_419/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/config/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/heartbeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/heartbeat/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/heartbeat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/heartbeat/throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/heartbeat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/heartbeat/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    41500 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)   104293 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    45236 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.337963 edx-enterprise-4.9.5/enterprise/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.341963 edx-enterprise-4.9.5/enterprise/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/backfill_learner_role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/bulk_update_catalog_query_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/create_enterprise_course_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/create_missing_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/email_drip_for_missing_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/fix_dsc_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/manufacture_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/migrate_enterprise_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/monthly_impact_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/reencrypt_enterprise_customer_reporting_config_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/revert_enrollment_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/save_enterprise_customer_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/seed_enterprise_devstack_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/unlink_enterprise_customer_learners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/update_config_last_errored_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/management/commands/update_role_assignments_with_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.353963 edx-enterprise-4.9.5/enterprise/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0001_auto_20210111_1253.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52500 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0095_auto_20200507_1138.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0096_enterprise_catalog_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0097_auto_20200619_1130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0098_auto_20200629_1756.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0099_auto_20200702_1537.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0101_move_data_to_saved_for_later.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0102_auto_20200708_1615.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0103_remove_marked_done.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0104_sync_query_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0105_add_branding_config_color_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0106_move_branding_config_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0107_remove_branding_config_banner_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0110_add_default_contract_discount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0112_auto_20200914_0926.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0113_auto_20200914_2054.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0114_auto_20201020_0142.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0116_auto_20201116_0400.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0116_auto_20201208_1759.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0117_auto_20201215_0258.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0124_auto_20210301_1309.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0125_add_config_for_role_assign_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0126_auto_20210308_1522.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0127_enterprisecatalogquery_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0129_enterprisecatalogquery_uuid_unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0130_lms_customer_lp_search_help_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0131_auto_20210517_0924.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0132_auto_20210608_1921.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26436 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0133_auto_20210608_1931.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0136_auto_20210629_2129.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16936 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0137_enrollment_email_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0139_auto_20210803_1854.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0140_update_enrollment_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0142_auto_20210907_2059.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0143_auto_20210908_0559.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0144_auto_20211011_1030.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0145_auto_20211013_1018.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0146_enterprise_customer_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0147_auto_20211129_1949.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0148_auto_20211129_2114.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0150_invite_key_expiry_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0151_add_is_active_to_invite_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0152_add_should_inactivate_other_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0153_add_enable_browse_and_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0156_add_is_active_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0157_make_field_nullable_before_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0158_remove_is_active_from_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0159_add_enable_learner_portal_offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0163_auto_20220928_1611.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0166_auto_20221209_0819.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0167_auto_20230209_2108.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0168_auto_20230222_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0169_auto_20230222_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0170_auto_20230301_1627.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0171_auto_20230503_1413.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0172_auto_20230517_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0173_auto_20230531_1459.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0174_auto_20230608_2041.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19527 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0175_auto_20230629_2330.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0176_auto_20230712_1751.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0177_auto_20230712_1925.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0178_auto_20230808_0923.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0179_restore_historical_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0180_chatgptresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0181_enterprisecustomerssoconfiguration_historicalenterprisecustomerssoconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0182_auto_20230829_1741.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0183_auto_20230906_1435.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0184_auto_20230914_2057.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0185_auto_20230921_1007.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0186_auto_20230921_1828.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0187_auto_20230926_1627.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0188_alter_learnercreditenterprisecourseenrollment_enterprise_course_enrollment_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0189_auto_20231002_0902.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0190_auto_20231003_0719.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0191_auto_20231006_0948.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0192_auto_20231009_1302.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0193_auto_20231005_1708.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0194_auto_20231013_1359.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0195_auto_20231130_1837.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0196_backfill_sso_marked_authorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/0197_auto_20231130_2239.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/migrations/unique_constraints_pending_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152269 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.353963 edx-enterprise-4.9.5/enterprise/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/static/enterprise/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.353963 edx-enterprise-4.9.5/enterprise/static/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/admin/enterprise_customer_catalog.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.357963 edx-enterprise-4.9.5/enterprise/static/enterprise/bundles/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/bundles/main-admin.style.css
+-rw-r--r--   0 runner    (1001) docker     (127)   295145 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/bundles/main.style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.357963 edx-enterprise-4.9.5/enterprise/static/enterprise/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/course_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/enterprise_customer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/enterprise_login_page.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/enterprise_selection_page.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/grant_data_sharing_permissions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/manage_learners.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/static/enterprise/js/program_enrollment_landing_page.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.309963 edx-enterprise-4.9.5/enterprise/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.357963 edx-enterprise-4.9.5/enterprise/templates/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_decline_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_policy.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_top_paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_user_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/_enterprise_customer_sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/enterprise_course_enrollments_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/manage_learners.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/oauth_authorization_failed.html
+-rw-r--r--   0 runner    (1001) docker     (127)    27091 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/oauth_authorization_successful.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/setup_auth_org_id.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/transmit_courses_metadata.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_course_enrollment_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_customer_login_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_customer_select_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_error_page_with_messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_program_enrollment_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/grant_data_sharing_permissions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise/templates/enterprise/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/templatetags/alert_messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/templatetags/course_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/templatetags/expand_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/templatetags/fa_icon.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise/templates/enterprise/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templates/enterprise/widgets/segment-io-django.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/templatetags/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/toggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/tpa_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87041 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112485 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise/views_error_codes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise_learner_portal/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise_learner_portal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/enterprise_learner_portal/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/enterprise_learner_portal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/integrated_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/integrated_channels/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.361963 edx-enterprise-4.9.5/integrated_channels/api/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/logs/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/logs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/logs/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.365963 edx-enterprise-4.9.5/integrated_channels/api/v1/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/moodle/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/moodle/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/moodle/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.369963 edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.369963 edx-enterprise-4.9.5/integrated_channels/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.369963 edx-enterprise-4.9.5/integrated_channels/blackboard/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39044 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.369963 edx-enterprise-4.9.5/integrated_channels/blackboard/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.369963 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    18816 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0016_auto_20230719_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0017_alter_historicalblackboardenterprisecustomerconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.373963 edx-enterprise-4.9.5/integrated_channels/blackboard/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/blackboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.373963 edx-enterprise-4.9.5/integrated_channels/canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.373963 edx-enterprise-4.9.5/integrated_channels/canvas/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38633 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.373963 edx-enterprise-4.9.5/integrated_channels/canvas/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.377963 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0003_delete_canvasglobalconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0031_auto_20230719_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0032_alter_historicalcanvasenterprisecustomerconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.377963 edx-enterprise-4.9.5/integrated_channels/canvas/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/canvas/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/catalog_service_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.377963 edx-enterprise-4.9.5/integrated_channels/cornerstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.377963 edx-enterprise-4.9.5/integrated_channels/cornerstone/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.381963 edx-enterprise-4.9.5/integrated_channels/cornerstone/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.385964 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0002_cornerstoneglobalconfiguration_subject_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0004_cornerstoneglobalconfiguration_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0017_alter_cornerstonelearnerdatatransmissionaudit_course_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0028_auto_20230719_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0029_alter_historicalcornerstoneenterprisecustomerconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0030_auto_20231010_1654.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0031_cornerstoneapirequestlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.385964 edx-enterprise-4.9.5/integrated_channels/cornerstone/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/cornerstone/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.385964 edx-enterprise-4.9.5/integrated_channels/degreed/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.385964 edx-enterprise-4.9.5/integrated_channels/degreed/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.385964 edx-enterprise-4.9.5/integrated_channels/degreed/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.389963 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0030_auto_20230719_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0031_alter_historicaldegreedenterprisecustomerconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.389963 edx-enterprise-4.9.5/integrated_channels/degreed/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed/transmitters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.389963 edx-enterprise-4.9.5/integrated_channels/degreed2/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.389963 edx-enterprise-4.9.5/integrated_channels/degreed2/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25286 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.389963 edx-enterprise-4.9.5/integrated_channels/degreed2/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.393963 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0008_degreed2learnerdatatransmissionaudit_course_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0022_auto_20230719_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0023_alter_historicaldegreed2enterprisecustomerconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.393963 edx-enterprise-4.9.5/integrated_channels/degreed2/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/degreed2/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.393963 edx-enterprise-4.9.5/integrated_channels/integrated_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.397963 edx-enterprise-4.9.5/integrated_channels/integrated_channel/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/channel_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.397963 edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32575 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38816 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.397963 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.397963 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/assign_skills_to_degreed_courses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/remove_null_catalog_transmission_audits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.401964 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0002_learnerdatatransmissionaudit_subsection_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0005_auto_20211005_1052.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0006_contentmetadataitemtransmission_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0007_delete_learnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0011_contentmetadataitemtransmission_plugin_configuration_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0012_alter_contentmetadataitemtransmission_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_content_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0019_merge_20220928_1842.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0021_remove_contentmetadataitemtransmission_api_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0029_genericenterprisecustomerpluginconfiguration_show_course_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0030_integratedchannelapirequestlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34767 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20241 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.401964 edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23097 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/lms_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.401964 edx-enterprise-4.9.5/integrated_channels/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.405964 edx-enterprise-4.9.5/integrated_channels/moodle/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.405964 edx-enterprise-4.9.5/integrated_channels/moodle/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/exporters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.409963 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0026_auto_20230719_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0027_alter_historicalmoodleenterprisecustomerconfiguration_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0028_auto_20230928_1530.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0028_auto_20231116_1826.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0029_auto_20231106_1233.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0030_merge_0028_auto_20231116_1826_0029_auto_20231106_1233.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.409963 edx-enterprise-4.9.5/integrated_channels/moodle/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/moodle/transmitters/learner_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.409963 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.409963 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.409963 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0009_sapsuccessfactorsenterprisecustomerconfiguration_deleted_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0014_alter_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/transmitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/transmitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/transmitters/content_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/sap_success_factors/transmitters/learner_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/xapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/xapi/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/xapi/management/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/xapi/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/management/commands/send_course_completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/management/commands/send_course_enrollments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.413964 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0004_auto_20190830_0710.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.417964 edx-enterprise-4.9.5/integrated_channels/xapi/statements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/statements/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/statements/learner_course_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/statements/learner_course_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/integrated_channels/xapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:40:10.417964 edx-enterprise-4.9.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/celery53.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25030 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/doc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28622 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/edx-platform-constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/js_test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/js_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/test-master.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-15 12:40:10.421964 edx-enterprise-4.9.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4028 2024-01-15 12:39:03.000000 edx-enterprise-4.9.5/setup.py
```

### Comparing `edx-enterprise-4.9.2/CHANGELOG.rst` & `edx-enterprise-4.9.5/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,29 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[4.9.5]
+--------
+
+feat: replacing non encrypted fields of moodle config model with encrypted ones
+
+[4.9.4]
+--------
+
+feat: Add model for integrated channel API request log table (ENT-8018)
+
+[4.9.3]
+--------
+
+fix: Remove SAP debug logs
+
 [4.9.2]
 --------
 
 refactor: learner data transmission audit record  to utilize the existing records (ENT-8005)
 
 [4.9.1]
 --------
```

### Comparing `edx-enterprise-4.9.2/LICENSE` & `edx-enterprise-4.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/MANIFEST.in` & `edx-enterprise-4.9.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/PKG-INFO` & `edx-enterprise-4.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 4.9.2
+Version: 4.9.5
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -91,14 +91,29 @@
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
         
+        [4.9.5]
+        --------
+        
+        feat: replacing non encrypted fields of moodle config model with encrypted ones
+        
+        [4.9.4]
+        --------
+        
+        feat: Add model for integrated channel API request log table (ENT-8018)
+        
+        [4.9.3]
+        --------
+        
+        fix: Remove SAP debug logs
+        
         [4.9.2]
         --------
         
         refactor: learner data transmission audit record  to utilize the existing records (ENT-8005)
         
         [4.9.1]
         --------
```

### Comparing `edx-enterprise-4.9.2/README.rst` & `edx-enterprise-4.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/__init__.py` & `edx-enterprise-4.9.5/consent/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/admin/__init__.py` & `edx-enterprise-4.9.5/consent/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/api/permissions.py` & `edx-enterprise-4.9.5/consent/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/api/v1/views.py` & `edx-enterprise-4.9.5/consent/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/errors.py` & `edx-enterprise-4.9.5/consent/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/helpers.py` & `edx-enterprise-4.9.5/consent/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/migrations/0001_initial.py` & `edx-enterprise-4.9.5/consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/migrations/0002_migrate_to_new_data_sharing_consent.py` & `edx-enterprise-4.9.5/consent/migrations/0002_migrate_to_new_data_sharing_consent.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/migrations/0004_datasharingconsenttextoverrides.py` & `edx-enterprise-4.9.5/consent/migrations/0004_datasharingconsenttextoverrides.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/migrations/0005_auto_20230707_0755.py` & `edx-enterprise-4.9.5/consent/migrations/0005_auto_20230707_0755.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/migrations/0006_alter_historicaldatasharingconsent_options.py` & `edx-enterprise-4.9.5/consent/migrations/0006_alter_historicaldatasharingconsent_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/mixins.py` & `edx-enterprise-4.9.5/consent/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/consent/models.py` & `edx-enterprise-4.9.5/consent/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/edx_enterprise.egg-info/PKG-INFO` & `edx-enterprise-4.9.5/edx_enterprise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-enterprise
-Version: 4.9.2
+Version: 4.9.5
 Summary: Your project description goes here
 Home-page: https://github.com/openedx/edx-enterprise
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: enterprise
         ==========
@@ -91,14 +91,29 @@
            This project adheres to Semantic Versioning (http://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ----------
         
+        [4.9.5]
+        --------
+        
+        feat: replacing non encrypted fields of moodle config model with encrypted ones
+        
+        [4.9.4]
+        --------
+        
+        feat: Add model for integrated channel API request log table (ENT-8018)
+        
+        [4.9.3]
+        --------
+        
+        fix: Remove SAP debug logs
+        
         [4.9.2]
         --------
         
         refactor: learner data transmission audit record  to utilize the existing records (ENT-8005)
         
         [4.9.1]
         --------
```

### Comparing `edx-enterprise-4.9.2/edx_enterprise.egg-info/SOURCES.txt` & `edx-enterprise-4.9.5/edx_enterprise.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -453,14 +453,15 @@
 integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py
 integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py
 integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py
 integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py
 integrated_channels/cornerstone/migrations/0028_auto_20230719_1621.py
 integrated_channels/cornerstone/migrations/0029_alter_historicalcornerstoneenterprisecustomerconfiguration_options.py
 integrated_channels/cornerstone/migrations/0030_auto_20231010_1654.py
+integrated_channels/cornerstone/migrations/0031_cornerstoneapirequestlogs.py
 integrated_channels/cornerstone/migrations/__init__.py
 integrated_channels/cornerstone/transmitters/__init__.py
 integrated_channels/cornerstone/transmitters/content_metadata.py
 integrated_channels/cornerstone/transmitters/learner_data.py
 integrated_channels/degreed/__init__.py
 integrated_channels/degreed/apps.py
 integrated_channels/degreed/client.py
@@ -593,14 +594,15 @@
 integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py
 integrated_channels/integrated_channel/migrations/0024_genericenterprisecustomerpluginconfiguration_deleted_at.py
 integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py
 integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py
 integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py
 integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py
 integrated_channels/integrated_channel/migrations/0029_genericenterprisecustomerpluginconfiguration_show_course_price.py
+integrated_channels/integrated_channel/migrations/0030_integratedchannelapirequestlogs.py
 integrated_channels/integrated_channel/migrations/__init__.py
 integrated_channels/integrated_channel/transmitters/__init__.py
 integrated_channels/integrated_channel/transmitters/content_metadata.py
 integrated_channels/integrated_channel/transmitters/learner_data.py
 integrated_channels/moodle/__init__.py
 integrated_channels/moodle/apps.py
 integrated_channels/moodle/client.py
```

### Comparing `edx-enterprise-4.9.2/edx_enterprise.egg-info/requires.txt` & `edx-enterprise-4.9.5/edx_enterprise.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/admin/__init__.py` & `edx-enterprise-4.9.5/enterprise/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/admin/actions.py` & `edx-enterprise-4.9.5/enterprise/admin/actions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/admin/forms.py` & `edx-enterprise-4.9.5/enterprise/admin/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/admin/paginator.py` & `edx-enterprise-4.9.5/enterprise/admin/paginator.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/admin/utils.py` & `edx-enterprise-4.9.5/enterprise/admin/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/admin/views.py` & `edx-enterprise-4.9.5/enterprise/admin/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/__init__.py` & `edx-enterprise-4.9.5/enterprise/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/filters.py` & `edx-enterprise-4.9.5/enterprise/api/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/pagination.py` & `edx-enterprise-4.9.5/enterprise/api/pagination.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/throttles.py` & `edx-enterprise-4.9.5/enterprise/api/throttles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/utils.py` & `edx-enterprise-4.9.5/enterprise/api/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/decorators.py` & `edx-enterprise-4.9.5/enterprise/api/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/fields.py` & `edx-enterprise-4.9.5/enterprise/api/v1/fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/permissions.py` & `edx-enterprise-4.9.5/enterprise/api/v1/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/serializers.py` & `edx-enterprise-4.9.5/enterprise/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/urls.py` & `edx-enterprise-4.9.5/enterprise/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/analytics_summary.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/analytics_summary.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/base_views.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/base_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/coupon_codes.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/coupon_codes.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_catalog_query.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_course_enrollment.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_api_credentials.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_api_credentials.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_branding_configuration.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_branding_configuration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_catalog.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_catalog.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_invite_key.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_reporting.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_reporting.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_sso_configuration.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_sso_configuration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_customer_user.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/enterprise_subsidy_fulfillment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/notifications.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/notifications.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/pending_enterprise_customer_user.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/pending_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api/v1/views/plotly_auth.py` & `edx-enterprise-4.9.5/enterprise/api/v1/views/plotly_auth.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/braze.py` & `edx-enterprise-4.9.5/enterprise/api_client/braze.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/client.py` & `edx-enterprise-4.9.5/enterprise/api_client/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/discovery.py` & `edx-enterprise-4.9.5/enterprise/api_client/discovery.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/ecommerce.py` & `edx-enterprise-4.9.5/enterprise/api_client/ecommerce.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/enterprise.py` & `edx-enterprise-4.9.5/enterprise/api_client/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/enterprise_catalog.py` & `edx-enterprise-4.9.5/enterprise/api_client/enterprise_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
         query_params = {'course_run_ids': content_ids}
         api_url = self.get_api_url(f"{self.ENTERPRISE_CUSTOMER_ENDPOINT}/{enterprise_uuid}/contains_content_items")
         response = self.client.get(api_url, params=query_params)
         response.raise_for_status()
         return response.json()['contains_content_items']
 
     @UserAPIClient.refresh_token
-    def get_content_metadata_content_identifier(self, enterprise_uuid, content_id):  # pylint: disable=inconsistent-return-statements
+    def get_content_metadata_content_identifier(self, enterprise_uuid, content_id):
         """
         Return all content metadata contained in the catalogs associated with the
         given EnterpriseCustomer and content_id.
         """
         try:
             api_url = self.get_api_url(
                 f"{self.CONTENT_METADATA_IDENTIFIER_ENDPOINT.format(enterprise_uuid, content_id)}"
```

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/lms.py` & `edx-enterprise-4.9.5/enterprise/api_client/lms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/open_ai.py` & `edx-enterprise-4.9.5/enterprise/api_client/open_ai.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/api_client/sso_orchestrator.py` & `edx-enterprise-4.9.5/enterprise/api_client/sso_orchestrator.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/apps.py` & `edx-enterprise-4.9.5/enterprise/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/conf/locale/en/LC_MESSAGES/django.po` & `edx-enterprise-4.9.5/enterprise/conf/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/conf/locale/en/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.9.5/enterprise/conf/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/conf/locale/eo/LC_MESSAGES/django.po` & `edx-enterprise-4.9.5/enterprise/conf/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/conf/locale/eo/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.9.5/enterprise/conf/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/conf/locale/es_419/LC_MESSAGES/django.po` & `edx-enterprise-4.9.5/enterprise/conf/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/config/models.py` & `edx-enterprise-4.9.5/enterprise/config/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/constants.py` & `edx-enterprise-4.9.5/enterprise/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/decorators.py` & `edx-enterprise-4.9.5/enterprise/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/errors.py` & `edx-enterprise-4.9.5/enterprise/errors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/forms.py` & `edx-enterprise-4.9.5/enterprise/forms.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/heartbeat/checks.py` & `edx-enterprise-4.9.5/enterprise/heartbeat/checks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/heartbeat/exceptions.py` & `edx-enterprise-4.9.5/enterprise/heartbeat/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/heartbeat/utils.py` & `edx-enterprise-4.9.5/enterprise/heartbeat/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/heartbeat/views.py` & `edx-enterprise-4.9.5/enterprise/heartbeat/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/locale/en/LC_MESSAGES/django.po` & `edx-enterprise-4.9.5/enterprise/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/locale/en/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.9.5/enterprise/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/locale/eo/LC_MESSAGES/django.po` & `edx-enterprise-4.9.5/enterprise/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/locale/eo/LC_MESSAGES/djangojs.po` & `edx-enterprise-4.9.5/enterprise/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/locale/es_419/LC_MESSAGES/django.po` & `edx-enterprise-4.9.5/enterprise/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/logging.py` & `edx-enterprise-4.9.5/enterprise/logging.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/backfill_learner_role_assignments.py` & `edx-enterprise-4.9.5/enterprise/management/commands/backfill_learner_role_assignments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/bulk_update_catalog_query_id.py` & `edx-enterprise-4.9.5/enterprise/management/commands/bulk_update_catalog_query_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/create_enterprise_course_enrollments.py` & `edx-enterprise-4.9.5/enterprise/management/commands/create_enterprise_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/create_missing_dsc_records.py` & `edx-enterprise-4.9.5/enterprise/management/commands/create_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/email_drip_for_missing_dsc_records.py` & `edx-enterprise-4.9.5/enterprise/management/commands/email_drip_for_missing_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py` & `edx-enterprise-4.9.5/enterprise/management/commands/ensure_singular_active_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/fix_dsc_records.py` & `edx-enterprise-4.9.5/enterprise/management/commands/fix_dsc_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/manufacture_data.py` & `edx-enterprise-4.9.5/enterprise/management/commands/manufacture_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/migrate_enterprise_catalogs.py` & `edx-enterprise-4.9.5/enterprise/management/commands/migrate_enterprise_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/monthly_impact_report.py` & `edx-enterprise-4.9.5/enterprise/management/commands/monthly_impact_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py` & `edx-enterprise-4.9.5/enterprise/management/commands/nudge_dormant_enrolled_enterprise_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/reencrypt_enterprise_customer_reporting_config_passwords.py` & `edx-enterprise-4.9.5/enterprise/management/commands/reencrypt_enterprise_customer_reporting_config_passwords.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/revert_enrollment_objects.py` & `edx-enterprise-4.9.5/enterprise/management/commands/revert_enrollment_objects.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/save_enterprise_customer_users.py` & `edx-enterprise-4.9.5/enterprise/management/commands/save_enterprise_customer_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/seed_enterprise_devstack_data.py` & `edx-enterprise-4.9.5/enterprise/management/commands/seed_enterprise_devstack_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/unlink_enterprise_customer_learners.py` & `edx-enterprise-4.9.5/enterprise/management/commands/unlink_enterprise_customer_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/update_config_last_errored_at.py` & `edx-enterprise-4.9.5/enterprise/management/commands/update_config_last_errored_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/management/commands/update_role_assignments_with_customers.py` & `edx-enterprise-4.9.5/enterprise/management/commands/update_role_assignments_with_customers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/messages.py` & `edx-enterprise-4.9.5/enterprise/messages.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/middleware.py` & `edx-enterprise-4.9.5/enterprise/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0001_auto_20210111_1253.py` & `edx-enterprise-4.9.5/enterprise/migrations/0001_auto_20210111_1253.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py` & `edx-enterprise-4.9.5/enterprise/migrations/0001_squashed_0092_auto_20200312_1650.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py` & `edx-enterprise-4.9.5/enterprise/migrations/0093_add_use_enterprise_catalog_flag.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py` & `edx-enterprise-4.9.5/enterprise/migrations/0094_add_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0095_auto_20200507_1138.py` & `edx-enterprise-4.9.5/enterprise/migrations/0095_auto_20200507_1138.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0096_enterprise_catalog_admin_role.py` & `edx-enterprise-4.9.5/enterprise/migrations/0096_enterprise_catalog_admin_role.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0097_auto_20200619_1130.py` & `edx-enterprise-4.9.5/enterprise/migrations/0097_auto_20200619_1130.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0098_auto_20200629_1756.py` & `edx-enterprise-4.9.5/enterprise/migrations/0098_auto_20200629_1756.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0099_auto_20200702_1537.py` & `edx-enterprise-4.9.5/enterprise/migrations/0099_auto_20200702_1537.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py` & `edx-enterprise-4.9.5/enterprise/migrations/0100_add_licensed_enterprise_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0101_move_data_to_saved_for_later.py` & `edx-enterprise-4.9.5/enterprise/migrations/0101_move_data_to_saved_for_later.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0102_auto_20200708_1615.py` & `edx-enterprise-4.9.5/enterprise/migrations/0102_auto_20200708_1615.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0104_sync_query_field.py` & `edx-enterprise-4.9.5/enterprise/migrations/0104_sync_query_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0105_add_branding_config_color_fields.py` & `edx-enterprise-4.9.5/enterprise/migrations/0105_add_branding_config_color_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0106_move_branding_config_colors.py` & `edx-enterprise-4.9.5/enterprise/migrations/0106_move_branding_config_colors.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0107_remove_branding_config_banner_fields.py` & `edx-enterprise-4.9.5/enterprise/migrations/0107_remove_branding_config_banner_fields.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py` & `edx-enterprise-4.9.5/enterprise/migrations/0108_add_licensed_enrollment_is_revoked.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py` & `edx-enterprise-4.9.5/enterprise/migrations/0109_remove_use_enterprise_catalog_sample.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0110_add_default_contract_discount.py` & `edx-enterprise-4.9.5/enterprise/migrations/0110_add_default_contract_discount.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py` & `edx-enterprise-4.9.5/enterprise/migrations/0111_pendingenterprisecustomeradminuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0112_auto_20200914_0926.py` & `edx-enterprise-4.9.5/enterprise/migrations/0112_auto_20200914_0926.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0113_auto_20200914_2054.py` & `edx-enterprise-4.9.5/enterprise/migrations/0113_auto_20200914_2054.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0114_auto_20201020_0142.py` & `edx-enterprise-4.9.5/enterprise/migrations/0114_auto_20201020_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py` & `edx-enterprise-4.9.5/enterprise/migrations/0115_enterpriseanalyticsuser_historicalenterpriseanalyticsuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0116_auto_20201116_0400.py` & `edx-enterprise-4.9.5/enterprise/migrations/0116_auto_20201116_0400.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0116_auto_20201208_1759.py` & `edx-enterprise-4.9.5/enterprise/migrations/0116_auto_20201208_1759.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0117_auto_20201215_0258.py` & `edx-enterprise-4.9.5/enterprise/migrations/0117_auto_20201215_0258.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py` & `edx-enterprise-4.9.5/enterprise/migrations/0120_systemwiderole_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py` & `edx-enterprise-4.9.5/enterprise/migrations/0121_systemwiderole_add_ent_cust_field.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py` & `edx-enterprise-4.9.5/enterprise/migrations/0122_remove_field_sync_enterprise_catalog_query.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py` & `edx-enterprise-4.9.5/enterprise/migrations/0123_enterprisecustomeridentityprovider_default_provider.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0124_auto_20210301_1309.py` & `edx-enterprise-4.9.5/enterprise/migrations/0124_auto_20210301_1309.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0125_add_config_for_role_assign_backfill.py` & `edx-enterprise-4.9.5/enterprise/migrations/0125_add_config_for_role_assign_backfill.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0126_auto_20210308_1522.py` & `edx-enterprise-4.9.5/enterprise/migrations/0126_auto_20210308_1522.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py` & `edx-enterprise-4.9.5/enterprise/migrations/0128_enterprisecatalogquery_generate_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0130_lms_customer_lp_search_help_text.py` & `edx-enterprise-4.9.5/enterprise/migrations/0130_lms_customer_lp_search_help_text.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0131_auto_20210517_0924.py` & `edx-enterprise-4.9.5/enterprise/migrations/0131_auto_20210517_0924.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0132_auto_20210608_1921.py` & `edx-enterprise-4.9.5/enterprise/migrations/0132_auto_20210608_1921.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0133_auto_20210608_1931.py` & `edx-enterprise-4.9.5/enterprise/migrations/0133_auto_20210608_1931.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py` & `edx-enterprise-4.9.5/enterprise/migrations/0134_enterprisecustomerreportingconfiguration_enable_compression.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py` & `edx-enterprise-4.9.5/enterprise/migrations/0135_adminnotification_adminnotificationfilter_adminnotificationread.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0136_auto_20210629_2129.py` & `edx-enterprise-4.9.5/enterprise/migrations/0136_auto_20210629_2129.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0137_enrollment_email_update.py` & `edx-enterprise-4.9.5/enterprise/migrations/0137_enrollment_email_update.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py` & `edx-enterprise-4.9.5/enterprise/migrations/0138_bulkcatalogqueryupdatecommandconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0139_auto_20210803_1854.py` & `edx-enterprise-4.9.5/enterprise/migrations/0139_auto_20210803_1854.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0140_update_enrollment_sources.py` & `edx-enterprise-4.9.5/enterprise/migrations/0140_update_enrollment_sources.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py` & `edx-enterprise-4.9.5/enterprise/migrations/0141_make_enterprisecatalogquery_title_unique.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0142_auto_20210907_2059.py` & `edx-enterprise-4.9.5/enterprise/migrations/0142_auto_20210907_2059.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0143_auto_20210908_0559.py` & `edx-enterprise-4.9.5/enterprise/migrations/0143_auto_20210908_0559.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0144_auto_20211011_1030.py` & `edx-enterprise-4.9.5/enterprise/migrations/0144_auto_20211011_1030.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0145_auto_20211013_1018.py` & `edx-enterprise-4.9.5/enterprise/migrations/0145_auto_20211013_1018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0146_enterprise_customer_invite_key.py` & `edx-enterprise-4.9.5/enterprise/migrations/0146_enterprise_customer_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0147_auto_20211129_1949.py` & `edx-enterprise-4.9.5/enterprise/migrations/0147_auto_20211129_1949.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0148_auto_20211129_2114.py` & `edx-enterprise-4.9.5/enterprise/migrations/0148_auto_20211129_2114.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py` & `edx-enterprise-4.9.5/enterprise/migrations/0149_invite_key_required_default_expiry_backfill.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0150_invite_key_expiry_required.py` & `edx-enterprise-4.9.5/enterprise/migrations/0150_invite_key_expiry_required.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0151_add_is_active_to_invite_key.py` & `edx-enterprise-4.9.5/enterprise/migrations/0151_add_is_active_to_invite_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0152_add_should_inactivate_other_customers.py` & `edx-enterprise-4.9.5/enterprise/migrations/0152_add_should_inactivate_other_customers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0153_add_enable_browse_and_request.py` & `edx-enterprise-4.9.5/enterprise/migrations/0153_add_enable_browse_and_request.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py` & `edx-enterprise-4.9.5/enterprise/migrations/0154_alter_systemwideenterpriseuserroleassignment_unique_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py` & `edx-enterprise-4.9.5/enterprise/migrations/0155_add_is_relinkable_to_enterprise_customer_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0156_add_is_active_role_assignment.py` & `edx-enterprise-4.9.5/enterprise/migrations/0156_add_is_active_role_assignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0157_make_field_nullable_before_removal.py` & `edx-enterprise-4.9.5/enterprise/migrations/0157_make_field_nullable_before_removal.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0158_remove_is_active_from_role_assignment.py` & `edx-enterprise-4.9.5/enterprise/migrations/0158_remove_is_active_from_role_assignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0159_add_enable_learner_portal_offers.py` & `edx-enterprise-4.9.5/enterprise/migrations/0159_add_enable_learner_portal_offers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py` & `edx-enterprise-4.9.5/enterprise/migrations/0160_add_enable_portal_learner_credit_management_screen.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py` & `edx-enterprise-4.9.5/enterprise/migrations/0161_alter_enterprisecustomerreportingconfiguration_data_type.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py` & `edx-enterprise-4.9.5/enterprise/migrations/0162_add_enable_executive_education_2U_fulfillment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0163_auto_20220928_1611.py` & `edx-enterprise-4.9.5/enterprise/migrations/0163_auto_20220928_1611.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py` & `edx-enterprise-4.9.5/enterprise/migrations/0164_enterprisecatalogquery_include_exec_ed_2u_courses.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py` & `edx-enterprise-4.9.5/enterprise/migrations/0165_alter_enterprisecustomerreportingconfiguration_pgp_encryption_key.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0166_auto_20221209_0819.py` & `edx-enterprise-4.9.5/enterprise/migrations/0166_auto_20221209_0819.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0167_auto_20230209_2108.py` & `edx-enterprise-4.9.5/enterprise/migrations/0167_auto_20230209_2108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0168_auto_20230222_1621.py` & `edx-enterprise-4.9.5/enterprise/migrations/0168_auto_20230222_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0169_auto_20230222_1621.py` & `edx-enterprise-4.9.5/enterprise/migrations/0169_auto_20230222_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0170_auto_20230301_1627.py` & `edx-enterprise-4.9.5/enterprise/migrations/0170_auto_20230301_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0171_auto_20230503_1413.py` & `edx-enterprise-4.9.5/enterprise/migrations/0171_auto_20230503_1413.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0172_auto_20230517_1550.py` & `edx-enterprise-4.9.5/enterprise/migrations/0172_auto_20230517_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0173_auto_20230531_1459.py` & `edx-enterprise-4.9.5/enterprise/migrations/0173_auto_20230531_1459.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0174_auto_20230608_2041.py` & `edx-enterprise-4.9.5/enterprise/migrations/0174_auto_20230608_2041.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0175_auto_20230629_2330.py` & `edx-enterprise-4.9.5/enterprise/migrations/0175_auto_20230629_2330.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0176_auto_20230712_1751.py` & `edx-enterprise-4.9.5/enterprise/migrations/0176_auto_20230712_1751.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0177_auto_20230712_1925.py` & `edx-enterprise-4.9.5/enterprise/migrations/0177_auto_20230712_1925.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0178_auto_20230808_0923.py` & `edx-enterprise-4.9.5/enterprise/migrations/0178_auto_20230808_0923.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0179_restore_historical_table.py` & `edx-enterprise-4.9.5/enterprise/migrations/0179_restore_historical_table.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0180_chatgptresponse.py` & `edx-enterprise-4.9.5/enterprise/migrations/0180_chatgptresponse.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0181_enterprisecustomerssoconfiguration_historicalenterprisecustomerssoconfiguration.py` & `edx-enterprise-4.9.5/enterprise/migrations/0181_enterprisecustomerssoconfiguration_historicalenterprisecustomerssoconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0182_auto_20230829_1741.py` & `edx-enterprise-4.9.5/enterprise/migrations/0182_auto_20230829_1741.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0183_auto_20230906_1435.py` & `edx-enterprise-4.9.5/enterprise/migrations/0183_auto_20230906_1435.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0184_auto_20230914_2057.py` & `edx-enterprise-4.9.5/enterprise/migrations/0184_auto_20230914_2057.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0185_auto_20230921_1007.py` & `edx-enterprise-4.9.5/enterprise/migrations/0185_auto_20230921_1007.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0186_auto_20230921_1828.py` & `edx-enterprise-4.9.5/enterprise/migrations/0186_auto_20230921_1828.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0187_auto_20230926_1627.py` & `edx-enterprise-4.9.5/enterprise/migrations/0187_auto_20230926_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0188_alter_learnercreditenterprisecourseenrollment_enterprise_course_enrollment_and_more.py` & `edx-enterprise-4.9.5/enterprise/migrations/0188_alter_learnercreditenterprisecourseenrollment_enterprise_course_enrollment_and_more.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0189_auto_20231002_0902.py` & `edx-enterprise-4.9.5/enterprise/migrations/0189_auto_20231002_0902.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0190_auto_20231003_0719.py` & `edx-enterprise-4.9.5/enterprise/migrations/0190_auto_20231003_0719.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0191_auto_20231006_0948.py` & `edx-enterprise-4.9.5/enterprise/migrations/0191_auto_20231006_0948.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0192_auto_20231009_1302.py` & `edx-enterprise-4.9.5/enterprise/migrations/0192_auto_20231009_1302.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0193_auto_20231005_1708.py` & `edx-enterprise-4.9.5/enterprise/migrations/0193_auto_20231005_1708.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0194_auto_20231013_1359.py` & `edx-enterprise-4.9.5/enterprise/migrations/0194_auto_20231013_1359.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0195_auto_20231130_1837.py` & `edx-enterprise-4.9.5/enterprise/migrations/0195_auto_20231130_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0196_backfill_sso_marked_authorized.py` & `edx-enterprise-4.9.5/enterprise/migrations/0196_backfill_sso_marked_authorized.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/0197_auto_20231130_2239.py` & `edx-enterprise-4.9.5/enterprise/migrations/0197_auto_20231130_2239.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/migrations/unique_constraints_pending_users.py` & `edx-enterprise-4.9.5/enterprise/migrations/unique_constraints_pending_users.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/models.py` & `edx-enterprise-4.9.5/enterprise/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/roles_api.py` & `edx-enterprise-4.9.5/enterprise/roles_api.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/rules.py` & `edx-enterprise-4.9.5/enterprise/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/settings/test.py` & `edx-enterprise-4.9.5/enterprise/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/signals.py` & `edx-enterprise-4.9.5/enterprise/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/admin/enterprise_customer_catalog.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/admin/enterprise_customer_catalog.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/bundles/main.style.css` & `edx-enterprise-4.9.5/enterprise/static/enterprise/bundles/main.style.css`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/course_modal.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/course_modal.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/enterprise_customer.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/enterprise_customer.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/enterprise_login_page.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/enterprise_login_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/enterprise_selection_page.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/enterprise_selection_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/grant_data_sharing_permissions.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/grant_data_sharing_permissions.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/manage_learners.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/manage_learners.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/static/enterprise/js/program_enrollment_landing_page.js` & `edx-enterprise-4.9.5/enterprise/static/enterprise/js/program_enrollment_landing_page.js`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/tasks.py` & `edx-enterprise-4.9.5/enterprise/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_decline_modal.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_decline_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_policy_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_top_paragraph.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_top_paragraph.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/_data_sharing_user_input.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/_data_sharing_user_input.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/_enterprise_customer_sidebar.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/_enterprise_customer_sidebar.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/clear_learners_data_sharing_consent.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/manage_learners.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/manage_learners.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/oauth_authorization_failed.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/oauth_authorization_failed.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/oauth_authorization_successful.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/oauth_authorization_successful.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/setup_auth_org_id.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/setup_auth_org_id.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/admin/transmit_courses_metadata.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/admin/transmit_courses_metadata.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/base.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/base.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_course_enrollment_page.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_course_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_customer_login_page.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_customer_login_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_customer_select_form.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_customer_select_form.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/enterprise_program_enrollment_page.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/enterprise_program_enrollment_page.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/grant_data_sharing_permissions.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/grant_data_sharing_permissions.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/templatetags/course_modal.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/templatetags/course_modal.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templates/enterprise/widgets/segment-io-django.html` & `edx-enterprise-4.9.5/enterprise/templates/enterprise/widgets/segment-io-django.html`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/templatetags/enterprise.py` & `edx-enterprise-4.9.5/enterprise/templatetags/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/toggles.py` & `edx-enterprise-4.9.5/enterprise/toggles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/tpa_pipeline.py` & `edx-enterprise-4.9.5/enterprise/tpa_pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/urls.py` & `edx-enterprise-4.9.5/enterprise/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/utils.py` & `edx-enterprise-4.9.5/enterprise/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/validators.py` & `edx-enterprise-4.9.5/enterprise/validators.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/views.py` & `edx-enterprise-4.9.5/enterprise/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise/views_error_codes.txt` & `edx-enterprise-4.9.5/enterprise/views_error_codes.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/serializers.py` & `edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise_learner_portal/api/v1/views.py` & `edx-enterprise-4.9.5/enterprise_learner_portal/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/enterprise_learner_portal/utils.py` & `edx-enterprise-4.9.5/enterprise_learner_portal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/blackboard/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/canvas/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/cornerstone/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/degreed/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/degreed/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/degreed2/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/degreed2/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/logs/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/logs/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/logs/urls.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/logs/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/logs/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/logs/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/mixins.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/moodle/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/moodle/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/serializers.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/sap_success_factors/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/sap_success_factors/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/urls.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/api/v1/views.py` & `edx-enterprise-4.9.5/integrated_channels/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/apps.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/client.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0001_initial_squashed_0014_alter_blackboardlearnerassessmentdatatransmissionaudit_enterprise_course_enrollment_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0002_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0003_alter_blackboardlearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0004_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0005_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0006_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0007_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0008_auto_20220913_2018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0009_auto_20220929_1720.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0010_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0011_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0012_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0013_alter_blackboardlearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0014_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0015_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0016_auto_20230719_1621.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0016_auto_20230719_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/migrations/0017_alter_historicalblackboardenterprisecustomerconfiguration_options.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/migrations/0017_alter_historicalblackboardenterprisecustomerconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/models.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/blackboard/views.py` & `edx-enterprise-4.9.5/integrated_channels/blackboard/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/client.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0001_initial.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0002_auto_20200806_1632.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0004_adding_learner_data_to_canvas.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0005_auto_20200909_1534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0006_canvaslearnerassessmentdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0007_auto_20210222_2225.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0008_auto_20210707_0815.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0009_auto_20210708_1639.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0010_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0011_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0012_alter_canvasenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0013_auto_20211221_1535.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0014_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0015_auto_20220127_1605.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0016_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0017_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0018_alter_canvaslearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0019_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0020_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0021_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0022_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0023_auto_20220913_2018.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0024_auto_20220929_1720.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0025_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0026_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0027_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0028_alter_canvaslearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0029_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0030_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0031_auto_20230719_1621.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0031_auto_20230719_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/migrations/0032_alter_historicalcanvasenterprisecustomerconfiguration_options.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/migrations/0032_alter_historicalcanvasenterprisecustomerconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/models.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/utils.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/canvas/views.py` & `edx-enterprise-4.9.5/integrated_channels/canvas/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/catalog_service_utils.py` & `edx-enterprise-4.9.5/integrated_channels/catalog_service_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/client.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0001_initial.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0003_auto_20190621_1000.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0005_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0006_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0007_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0008_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0009_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0010_cornerstonecoursekey.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0011_auto_20211103_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0012_alter_cornerstoneenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0013_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0014_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0015_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0016_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0018_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0019_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0020_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0021_cornerstonelearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0022_cornerstonelearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0023_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0024_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0025_alter_cornerstonelearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0026_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0027_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0028_auto_20230719_1621.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0028_auto_20230719_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0029_alter_historicalcornerstoneenterprisecustomerconfiguration_options.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0029_alter_historicalcornerstoneenterprisecustomerconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/migrations/0030_auto_20231010_1654.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/migrations/0030_auto_20231010_1654.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/models.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from integrated_channels.cornerstone.exporters.content_metadata import CornerstoneContentMetadataExporter
 from integrated_channels.cornerstone.exporters.learner_data import CornerstoneLearnerExporter
 from integrated_channels.cornerstone.transmitters.content_metadata import CornerstoneContentMetadataTransmitter
 from integrated_channels.cornerstone.transmitters.learner_data import CornerstoneLearnerTransmitter
 from integrated_channels.integrated_channel.models import (
     EnterpriseCustomerPluginConfiguration,
+    IntegratedChannelAPIRequestLogs,
     LearnerDataTransmissionAudit,
 )
 from integrated_channels.utils import is_valid_url
 
 LOGGER = getLogger(__name__)
 User = auth.get_user_model()
 
@@ -314,7 +315,40 @@
         blank=False,
         null=False,
         help_text=_('This is the course key that is being sent to our partners.')
     )
 
     class Meta:
         app_label = 'cornerstone'
+
+
+class CornerstoneAPIRequestLogs(IntegratedChannelAPIRequestLogs):
+    """
+     A model to track basic information about every API call we make from the integrated channels.
+    """
+    user_agent = models.CharField(max_length=255)
+    user_ip = models.GenericIPAddressField(blank=True, null=True)
+
+    class Meta:
+        app_label = 'cornerstone'
+
+    def __str__(self):
+        """
+        Return a human-readable string representation of the object.
+        """
+        return (
+            f'<CornerstoneAPIRequestLogs {self.id}'
+            f' for enterprise customer {self.enterprise_customer}, '
+            f', enterprise_customer_configuration_id: {self.enterprise_customer_configuration_id}>'
+            f', endpoint: {self.endpoint}'
+            f', time_taken: {self.time_taken}'
+            f', user_agent: {self.user_agent}'
+            f', user_ip: {self.user_ip}'
+            f', api_record.body: {self.api_record.body}'
+            f', api_record.status_code: {self.api_record.status_code}'
+        )
+
+    def __repr__(self):
+        """
+        Return uniquely identifying string representation.
+        """
+        return self.__str__()
```

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/utils.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/cornerstone/views.py` & `edx-enterprise-4.9.5/integrated_channels/cornerstone/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/client.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0001_initial.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0002_auto_20180104_0103.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0003_auto_20180109_0712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0004_auto_20180306_1251.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0005_auto_20180807_1302.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0006_upgrade_django_simple_history.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0008_auto_20191001_0742.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0009_auto_20210119_1546.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0010_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0011_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0012_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0013_alter_degreedenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0014_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0015_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0016_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0017_alter_degreedlearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0018_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0019_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0020_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0021_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0022_degreedlearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0023_degreedlearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0024_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0025_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0026_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0027_alter_degreedlearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0028_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0029_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0030_auto_20230719_1621.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0030_auto_20230719_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/migrations/0031_alter_historicaldegreedenterprisecustomerconfiguration_options.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/migrations/0031_alter_historicaldegreedenterprisecustomerconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/models.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/degreed/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/apps.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/apps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/client.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0001_initial.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0002_auto_20211101_2021.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0003_alter_degreed2enterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0004_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0005_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0006_auto_20220214_1627.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0007_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0009_alter_degreed2learnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0010_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0011_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0012_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0013_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0014_degreed2learnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0015_degreed2learnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0016_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0017_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0018_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0019_alter_degreed2learnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0020_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0021_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0022_auto_20230719_1621.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0022_auto_20230719_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/migrations/0023_alter_historicaldegreed2enterprisecustomerconfiguration_options.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/migrations/0023_alter_historicaldegreed2enterprisecustomerconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/models.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/degreed2/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/degreed2/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/channel_settings.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/channel_settings.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/client.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/exporters/learner_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,19 +393,14 @@
             channel_name,
             skip_transmitted,
             TransmissionAudit,
             grade,
         )
         enrollment_ids_to_export = [enrollment.id for enrollment in enrollments_permitted]
 
-        LOGGER.info(
-            f"[Debug-SAP]: course_run_id:{course_run_id}, channel_name: {channel_name}"
-            f"lms_user_for_filter:{lms_user_for_filter}, grade:{grade} "
-            f"enrollment_ids_to_export: {enrollment_ids_to_export}"
-        )
         for enterprise_enrollment in enrollments_permitted:
             lms_user_id = enterprise_enrollment.enterprise_customer_user.user_id
             user_email = enterprise_enrollment.enterprise_customer_user.user_email
             enterprise_customer_uuid = enterprise_enrollment.enterprise_customer_user.enterprise_customer.uuid
             course_id = enterprise_enrollment.course_id
 
             course_details, error_message = LearnerExporterUtility.get_course_details_by_id(course_id)
@@ -456,26 +451,15 @@
                 completed_date=completed_date_from_api,
                 grade=grade_from_api,
                 content_title=course_details.display_name,
                 progress_status=progress_status,
                 course_completed=_is_course_completed,
                 grade_percent=grade_percent,
             )
-            LOGGER.info(
-                generate_formatted_log(
-                    channel_name,
-                    enterprise_customer_uuid,
-                    lms_user_id,
-                    course_id,
-                    f", [Debug-SAP]: _is_course_completed: {_is_course_completed}, progress_status:{progress_status}"
-                    f",completed_date_from_api: {completed_date_from_api}, grade_from_api:{grade_from_api}"
-                    f"is_passing_from_api: {is_passing_from_api}, grade_percent:{grade_percent}"
-                    f"passed_timestamp:{passed_timestamp}, records: {records}",
-                )
-            )
+
             if records:
                 # There are some cases where we won't receive a record from the above
                 # method; right now, that should only happen if we have an Enterprise-linked
                 # user for the integrated channel, and transmission of that user's
                 # data requires an upstream user identifier that we don't have (due to a
                 # failure of SSO or similar). In such a case, `get_learner_data_record`
                 # would return None, and we'd simply skip yielding it here.
@@ -485,20 +469,14 @@
                     try:
                         enrollment_ids_to_export.pop(enrollment_ids_to_export.index(enterprise_enrollment.id))
                     except ValueError:
                         pass
 
                     yield record
 
-        LOGGER.info(generate_formatted_log(
-            channel_name, None, lms_user_for_filter, course_run_id,
-            f'[Debug-SAP]: export finished. Did not export records for EnterpriseCourseEnrollment objects: '
-            f' {enrollment_ids_to_export}.'
-        ))
-
     def _filter_out_pre_transmitted_enrollments(
             self,
             enrollments_to_process,
             channel_name,
             grade,
             transmission_audit
     ):
@@ -542,50 +520,23 @@
         enrollment_queryset = EnterpriseCourseEnrollment.objects.select_related(
             'enterprise_customer_user'
         ).filter(
             enterprise_customer_user__enterprise_customer=self.enterprise_customer,
             enterprise_customer_user__active=True,
         )
         if lms_user_for_filter and course_run_id:
-            LOGGER.info(
-                generate_formatted_log(
-                    channel_name,
-                    self.enterprise_customer.uuid,
-                    lms_user_for_filter,
-                    course_run_id,
-                    f"[Debug-SAP]: enrollments to process before filtering: {list(enrollment_queryset)}",
-                )
-            )
             enrollment_queryset = enrollment_queryset.filter(
                 course_id=course_run_id,
                 enterprise_customer_user__user_id=lms_user_for_filter.id,
             )
-            LOGGER.info(
-                generate_formatted_log(
-                    channel_name,
-                    self.enterprise_customer.uuid,
-                    lms_user_for_filter,
-                    course_run_id,
-                    f"[Debug-SAP]: enrollments to process after filtering: {list(enrollment_queryset)}",
-                )
-            )
             LOGGER.info(generate_formatted_log(
                 channel_name, self.enterprise_customer.uuid, lms_user_for_filter, course_run_id,
                 'get_enrollments_to_process run for single learner and course.'))
         enrollment_queryset = enrollment_queryset.order_by('course_id')
         # return resolved list instead of queryset
-        LOGGER.info(
-            generate_formatted_log(
-                channel_name,
-                self.enterprise_customer.uuid,
-                lms_user_for_filter,
-                course_run_id,
-                f"[Debug-SAP]: enrollments to process: {list(enrollment_queryset)}",
-            )
-        )
         return list(enrollment_queryset)
 
     def get_learner_assessment_data_records(
             self,
             enterprise_enrollment,
             assessment_grade_data
     ):
```

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/assign_skills_to_degreed_courses.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/assign_skills_to_degreed_courses.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_course_end_dates.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_missing_csod_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_missing_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/backfill_remote_action_timestamps.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/cleanup_duplicate_assignment_records.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/mark_orphaned_content_metadata_audits.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/remove_null_catalog_transmission_audits.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/remove_null_catalog_transmission_audits.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/reset_csod_remote_deleted_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/reset_sapsf_learner_transmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/transmit_content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/transmit_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/transmit_subsection_learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/unlink_inactive_sap_learners.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/management/commands/update_content_transmission_catalogs.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0001_squashed_0007_auto_20190925_0730.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0003_contentmetadataitemtransmission_content_last_changed.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0004_contentmetadataitemtransmission_enterprise_customer_catalog_uuid.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0008_genericlearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0009_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0010_genericenterprisecustomerpluginconfiguration.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0013_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0014_genericenterprisecustomerpluginconfiguration_dry_run_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0015_auto_20220718_2113.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0016_contentmetadataitemtransmission_marked_for.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0017_contentmetadataitemtransmission_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0018_genericlearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0020_auto_20220929_1712.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0022_alter_contentmetadataitemtransmission_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0023_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0025_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0026_genericenterprisecustomerpluginconfiguration_last_modified_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0027_orphanedcontenttransmissions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0028_alter_contentmetadataitemtransmission_unique_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/migrations/0029_genericenterprisecustomerpluginconfiguration_show_course_price.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/migrations/0029_genericenterprisecustomerpluginconfiguration_show_course_price.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/models.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -875,7 +875,51 @@
     content_id = models.CharField(max_length=255, blank=False, null=False)
     transmission = models.ForeignKey(
         ContentMetadataItemTransmission,
         related_name='orphaned_record',
         on_delete=models.CASCADE,
     )
     resolved = models.BooleanField(default=False)
+
+
+class IntegratedChannelAPIRequestLogs(TimeStampedModel):
+    """
+     A model to track basic information about every API call we make from the integrated channels.
+    """
+    enterprise_customer = models.ForeignKey(
+        EnterpriseCustomer, on_delete=models.CASCADE)
+    enterprise_customer_configuration_id = models.IntegerField(
+        blank=False, null=False, help_text='ID from the EnterpriseCustomerConfiguration model')
+    endpoint = models.TextField(blank=False, null=False)
+    payload = models.TextField(blank=False, null=False)
+    time_taken = models.DurationField(blank=False, null=False)
+    api_record = models.OneToOneField(
+        ApiResponseRecord,
+        blank=True,
+        null=True,
+        on_delete=models.CASCADE,
+        help_text=_(
+            'Data pertaining to the transmissions API request response.')
+    )
+
+    class Meta:
+        app_label = 'integrated_channel'
+
+    def __str__(self):
+        """
+        Return a human-readable string representation of the object.
+        """
+        return (
+            f'<IntegratedChannelAPIRequestLog {self.id}'
+            f' for enterprise customer {self.enterprise_customer}, '
+            f', enterprise_customer_configuration_id: {self.enterprise_customer_configuration_id}>'
+            f', endpoint: {self.endpoint}'
+            f', time_taken: {self.time_taken}'
+            f', api_record.body: {self.api_record.body}'
+            f', api_record.status_code: {self.api_record.status_code}'
+        )
+
+    def __repr__(self):
+        """
+        Return uniquely identifying string representation.
+        """
+        return self.__str__()
```

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/tasks.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/integrated_channel/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/integrated_channel/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/lms_utils.py` & `edx-enterprise-4.9.5/integrated_channels/lms_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/admin/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     """
     class Meta:
         model = MoodleEnterpriseCustomerConfiguration
         fields = '__all__'
 
     def clean(self):
         cleaned_data = super().clean()
-        cleaned_username = cleaned_data.get('username')
-        cleaned_password = cleaned_data.get('password')
-        cleaned_token = cleaned_data.get('token')
+        cleaned_username = cleaned_data.get('decrypted_username')
+        cleaned_password = cleaned_data.get('decrypted_password')
+        cleaned_token = cleaned_data.get('decrypted_token')
         if cleaned_token and (cleaned_username or cleaned_password):
             raise ValidationError(_('Cannot set both a Username/Password and Token'))
         if (cleaned_username and not cleaned_password) or (cleaned_password and not cleaned_username):
             raise ValidationError(_('Must set both a Username and Password, not just one'))
 
 
 @admin.register(MoodleEnterpriseCustomerConfiguration)
```

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/client.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,27 +180,28 @@
             'service': self.enterprise_configuration.service_short_name
         }
 
         decrypted_username = self.enterprise_configuration.decrypted_username
         username = self.enterprise_configuration.username
         decrypted_password = self.enterprise_configuration.decrypted_password
         password = self.enterprise_configuration.password
+        use_encrypted_user_data = getattr(settings, 'FEATURES', {}).get('USE_ENCRYPTED_USER_DATA', False)
 
         response = requests.post(
             urljoin(
                 self.enterprise_configuration.moodle_base_url,
                 'login/token.php',
             ),
             params=querystring,
             headers={
                 'Content-Type': 'application/x-www-form-urlencoded',
             },
             data={
-                "username": decrypted_username if settings.FEATURES.get('USE_ENCRYPTED_USER_DATA', False) else username,
-                "password": decrypted_password if settings.FEATURES.get('USE_ENCRYPTED_USER_DATA', False) else password,
+                "username": decrypted_username if use_encrypted_user_data else username,
+                "password": decrypted_password if use_encrypted_user_data else password,
             },
         )
 
         try:
             data = response.json()
             token = data['token']
             return token
```

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0001_initial.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0002_moodlelearnerdatatransmissionaudit.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0003_auto_20201006_1706.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0004_auto_20201105_1921.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0005_auto_20210708_1446.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0006_auto_20210909_1536.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0007_auto_20210923_1727.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0008_alter_moodleenterprisecustomerconfiguration_enterprise_customer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0009_auto_20220126_1837.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0010_auto_20220131_1539.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0011_auto_20220302_2231.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0012_alter_moodlelearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0013_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0014_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0015_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0016_auto_20220523_1625.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0017_moodlelearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0018_moodlelearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0019_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0020_auto_20221031_1855.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0021_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0022_auto_20221220_1527.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0023_alter_moodlelearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0024_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0025_auto_20230112_2002.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0026_auto_20230719_1621.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0026_auto_20230719_1621.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0027_alter_historicalmoodleenterprisecustomerconfiguration_options.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0027_alter_historicalmoodleenterprisecustomerconfiguration_options.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0028_auto_20230928_1530.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0028_auto_20230928_1530.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0028_auto_20231116_1826.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0028_auto_20231116_1826.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/migrations/0029_auto_20231106_1233.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/migrations/0029_auto_20231106_1233.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/models.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             obj: The instance of MoodleEnterpriseCustomerConfiguration
                 being rendered with this admin form.
         """
         missing_items = {'missing': []}
         incorrect_items = {'incorrect': []}
         if not self.moodle_base_url:
             missing_items.get('missing').append('moodle_base_url')
-        if not self.token and not (self.username and self.password):
+        if not self.decrypted_token and not (self.decrypted_username and self.decrypted_password):
             missing_items.get('missing').append('token OR username and password')
         if not self.service_short_name:
             missing_items.get('missing').append('service_short_name')
         if not is_valid_url(self.moodle_base_url):
             incorrect_items.get('incorrect').append('moodle_base_url')
         if len(self.display_name) > 20:
             incorrect_items.get('incorrect').append('display_name')
```

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/moodle/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/moodle/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/client.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/constants.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/constants.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/exporters/utils.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0001_squashed_0022_auto_20200206_1046_squashed_0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_enterprise_course_enrollment_id.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0002_alter_sapsuccessfactorsenterprisecustomerconfiguration_display_name.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0003_alter_sapsuccessfactorslearnerdatatransmissionaudit_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0004_auto_20220324_1550_squashed_0006_auto_20220330_1157.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0005_sapsuccessfactorsenterprisecustomerconfiguration_dry_run_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0006_sapsuccessfactorslearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0007_sapsuccessfactorslearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0008_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0010_move_and_recrete_completed_timestamp.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0011_alter_sapsuccessfactorslearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0012_auto_20230105_2122.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0013_sapsuccessfactorsenterprisecustomerconfiguration_last_modified_at.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/migrations/0014_alter_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/migrations/0014_alter_sapsuccessfactorsenterprisecustomerconfiguration_show_course_price.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/models.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/transmitters/content_metadata.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/transmitters/content_metadata.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/sap_success_factors/transmitters/learner_data.py` & `edx-enterprise-4.9.5/integrated_channels/sap_success_factors/transmitters/learner_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/utils.py` & `edx-enterprise-4.9.5/integrated_channels/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/admin/__init__.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/client.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/management/commands/send_course_completions.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/management/commands/send_course_completions.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/management/commands/send_course_enrollments.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/management/commands/send_course_enrollments.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0001_initial.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0002_auto_20180726_0142.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0003_auto_20190807_1006.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0005_auto_20220324_1550.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0006_auto_20220325_1757.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0007_auto_20220405_2311.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0008_xapilearnerdatatransmissionaudit_friendly_status_message.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0009_xapilearnerdatatransmissionaudit_api_record.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0010_auto_20221021_0159.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/migrations/0011_alter_xapilearnerdatatransmissionaudit_index_together.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/models.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/statements/base.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/statements/base.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/statements/learner_course_completion.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/statements/learner_course_completion.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/statements/learner_course_enrollment.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/statements/learner_course_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/integrated_channels/xapi/utils.py` & `edx-enterprise-4.9.5/integrated_channels/xapi/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/base.in` & `edx-enterprise-4.9.5/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/ci.txt` & `edx-enterprise-4.9.5/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/common_constraints.txt` & `edx-enterprise-4.9.5/requirements/common_constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/constraints.txt` & `edx-enterprise-4.9.5/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/dev.in` & `edx-enterprise-4.9.5/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/dev.txt` & `edx-enterprise-4.9.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/doc.txt` & `edx-enterprise-4.9.5/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/edx-platform-constraints.txt` & `edx-enterprise-4.9.5/requirements/edx-platform-constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/js_test.txt` & `edx-enterprise-4.9.5/requirements/js_test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/test-master.txt` & `edx-enterprise-4.9.5/requirements/test-master.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/test.in` & `edx-enterprise-4.9.5/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/requirements/test.txt` & `edx-enterprise-4.9.5/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-4.9.2/setup.py` & `edx-enterprise-4.9.5/setup.py`

 * *Files identical despite different names*

