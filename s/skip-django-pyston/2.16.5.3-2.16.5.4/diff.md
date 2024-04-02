# Comparing `tmp/skip-django-pyston-2.16.5.3.tar.gz` & `tmp/skip-django-pyston-2.16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pyston-2.16.5.3.tar", last modified: Tue Feb 20 09:45:15 2024, max compression
+gzip compressed data, was "skip-django-pyston-2.16.5.4.tar", last modified: Tue Apr  2 14:13:32 2024, max compression
```

## Comparing `skip-django-pyston-2.16.5.3.tar` & `skip-django-pyston-2.16.5.4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.652149 skip-django-pyston-2.16.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-20 09:45:15.652149 skip-django-pyston-2.16.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.632149 skip-django-pyston-2.16.5.3/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.632149 skip-django-pyston-2.16.5.3/example/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.632149 skip-django-pyston-2.16.5.3/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.636149 skip-django-pyston-2.16.5.3/example/dj/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.636149 skip-django-pyston-2.16.5.3/example/dj/apps/app/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/dynamo/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/dynamo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.636149 skip-django-pyston-2.16.5.3/example/dj/apps/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/elasticsearch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/elasticsearch/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.636149 skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/0002_user_manual_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/0003_auto_20170729_2305.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/0004_issue_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.640149 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/extra_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/fieldsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/standard_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.640149 skip-django-pyston-2.16.5.3/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/dj/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.644149 skip-django-pyston-2.16.5.3/pyston/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.644149 skip-django-pyston-2.16.5.3/pyston/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.644149 skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.644149 skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.644149 skip-django-pyston-2.16.5.3/pyston/converters/
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/converters/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/converters/file_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.644149 skip-django-pyston-2.16.5.3/pyston/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/django_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16715 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/forms/
--rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/forms/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.632149 skip-django-pyston-2.16.5.3/pyston/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.632149 skip-django-pyston-2.16.5.3/pyston/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/metamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/order/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/django_sorters.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/sorters.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/order/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/requested_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/requested_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/requested_fields/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/requested_fields/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    41564 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    35172 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/templates/default_pdf_table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/templates/pyston/
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/templates/pyston/html_converter.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.648149 skip-django-pyston-2.16.5.3/pyston/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/utils/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/pyston/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 09:45:15.652149 skip-django-pyston-2.16.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-20 09:45:08.000000 skip-django-pyston-2.16.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:45:15.652149 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-20 09:45:15.000000 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-02-20 09:45:15.000000 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 09:45:15.000000 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 09:45:15.000000 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-20 09:45:15.000000 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-20 09:45:15.000000 skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0002_user_manual_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0003_auto_20170729_2305.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0004_issue_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/extra_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fieldsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/standard_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/converters/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/converters/file_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/django_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16820 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/forms/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/pyston/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/pyston/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/metamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/order/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/django_sorters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/sorters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/requested_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/requested_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/requested_fields/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/requested_fields/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41564 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35172 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/templates/default_pdf_table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/templates/pyston/
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/templates/pyston/html_converter.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/top_level.txt
```

### Comparing `skip-django-pyston-2.16.5.3/AUTHORS.txt` & `skip-django-pyston-2.16.5.4/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/LICENSE` & `skip-django-pyston-2.16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/PKG-INFO` & `skip-django-pyston-2.16.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pyston
-Version: 2.16.5.3
+Version: 2.16.5.4
 Summary: Pyston is a Django mini-framework creating APIs.
 Home-page: https://github.com/skip-pay/django-pyston
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pyston-2.16.5.3/README.md` & `skip-django-pyston-2.16.5.4/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/dynamo/models.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/dynamo/resource.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/elasticsearch/models.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/0001_initial.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/migrations/0003_auto_20170729_2305.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0003_auto_20170729_2305.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/models.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/resource.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/serializable.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/serializable.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/compatibility.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/compatibility.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/cors.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/cors.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/dynamo.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/dynamo.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/elasticsearch.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/extra_resource.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/extra_resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/factories.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/factories.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/fields.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/fieldsets.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fieldsets.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/filter.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/filter.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/order.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/serializer.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/serializer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/standard_operations.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/standard_operations.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/apps/app/tests/test_case.py` & `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/settings/base.py` & `skip-django-pyston-2.16.5.4/example/dj/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/urls.py` & `skip-django-pyston-2.16.5.4/example/dj/urls.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/example/dj/wsgi.py` & `skip-django-pyston-2.16.5.4/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/cache.py` & `skip-django-pyston-2.16.5.4/pyston/cache.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/conf.py` & `skip-django-pyston-2.16.5.4/pyston/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/filter.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/filter.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/order.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/paginator.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/paginator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/dynamo/resource.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/filters.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/order.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/contrib/elasticsearch/resource.py` & `skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/converters/__init__.py` & `skip-django-pyston-2.16.5.4/pyston/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/converters/extra.py` & `skip-django-pyston-2.16.5.4/pyston/converters/extra.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/converters/file_generators.py` & `skip-django-pyston-2.16.5.4/pyston/converters/file_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 if isinstance(val, str):
                     val = self._prepare_value(val)
                 output_stream.write('\t'.join(('\t' + force_text(val).lstrip()).splitlines(True)) + '\n\n')
             output_stream.write('---\n')
 
 
 if xlsxwriter:
-    class XlsxGenerator:
+    class XlsxGenerator:  # noqa: F811
 
         def _prepare_value(self, value):
             return value.replace('&nbsp;', ' ')
 
         def generate(self, header, data, output_stream):
             wb = xlsxwriter.Workbook(output_stream, {'strings_to_formulas': False, 'strings_to_urls': False})
             ws = wb.add_worksheet()
@@ -143,15 +143,15 @@
                         ws.write(row, col, val)
                     else:
                         ws.write(row, col, val)
                 row += 1
             wb.close()
 
 if pisa:
-    class PdfGenerator:
+    class PdfGenerator:  # noqa: F811
 
         encoding = 'utf-8'
 
         def generate(self, header, data, output_stream):
             def fetch_resources(uri, rel):
                 urls = {
                     django_settings.MEDIA_ROOT: settings.MEDIA_URL,
```

### Comparing `skip-django-pyston-2.16.5.3/pyston/data_processor.py` & `skip-django-pyston-2.16.5.4/pyston/data_processor.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/exception.py` & `skip-django-pyston-2.16.5.4/pyston/exception.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/filters/django_filters.py` & `skip-django-pyston-2.16.5.4/pyston/filters/django_filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/filters/filters.py` & `skip-django-pyston-2.16.5.4/pyston/filters/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/filters/managers.py` & `skip-django-pyston-2.16.5.4/pyston/filters/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,31 +194,32 @@
         if current_identifier not in filters_fields_rfs:
             return None
 
         suffix = LOOKUP_SEP.join(identifiers_suffix)
 
         model_field = get_field_or_none(model, current_identifier)
         model_method = get_method_or_none(model, current_identifier)
+        model_attribute = getattr(model, current_identifier, None)
         model_filter_filter = self._get_default_model_field_filter_class(model_field) if model_field else None
 
         if model_filter_filter and (not suffix or suffix in model_filter_filter.get_suffixes()):
             return model_filter_filter(
                 identifiers_prefix, [current_identifier], identifiers_suffix, model, field=model_field
             )
         elif model_field and model_field.is_relation and model_field.related_model:
             # recursive search for filter via related model fields
             next_model = model_field.related_model
             next_resource = get_resource_or_none(request, next_model, getattr(resource, 'resource_typemapper', None))
             return self._get_filter_recursive(
                 identifiers_prefix + [identifiers[0]], identifiers[1:], next_model, next_resource, request,
                 filters_fields_rfs[current_identifier].subfieldset
             )
-        elif model_method:
+        elif model_method or model_attribute:
             return self._get_method_filter(
-                model_method, identifiers_prefix, [current_identifier], identifiers_suffix,
+                model_method or model_attribute, identifiers_prefix, [current_identifier], identifiers_suffix,
                 model, resource, request, filters_fields_rfs
             )
         else:
             return None
 
     def _get_filters_fields_rfs(self, model, resource):
         return resource.get_filter_fields_rfs() if resource else get_allowed_filter_fields_rfs_from_model(model)
```

### Comparing `skip-django-pyston-2.16.5.3/pyston/filters/parser.py` & `skip-django-pyston-2.16.5.4/pyston/filters/parser.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/filters/utils.py` & `skip-django-pyston-2.16.5.4/pyston/filters/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/forms/__init__.py` & `skip-django-pyston-2.16.5.4/pyston/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/forms/postgres.py` & `skip-django-pyston-2.16.5.4/pyston/forms/postgres.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/locale/cs/LC_MESSAGES/django.mo` & `skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/locale/cs/LC_MESSAGES/django.po` & `skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/metamodel.py` & `skip-django-pyston-2.16.5.4/pyston/metamodel.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/order/django_sorters.py` & `skip-django-pyston-2.16.5.4/pyston/order/django_sorters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/order/managers.py` & `skip-django-pyston-2.16.5.4/pyston/order/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,27 +143,34 @@
         identifiers_suffix = identifiers[1:]
 
         if current_identifier not in order_fields_rfs:
             raise OrderIdentifierError
 
         model_field = get_field_or_none(model, current_identifier)
         model_method = get_method_or_none(model, current_identifier)
+        model_attribute = getattr(model, current_identifier, None)
 
         if model_field and not identifiers_suffix and (not model_field.is_relation or model_field.related_model):
             return DjangoSorter(identifiers_prefix + identifiers, direction)
         elif model_field and model_field.is_relation and model_field.related_model:
             next_model = model_field.related_model
             next_resource = get_resource_or_none(request, next_model, getattr(resource, 'resource_typemapper', None))
             return self._get_sorter_recursive(
                 identifiers_prefix + [identifiers[0]], identifiers[1:], direction,
                 next_model, next_resource, request, order_fields_rfs[current_identifier].subfieldset
             )
-        elif model_method and not identifiers_suffix:
+        elif (model_method or model_attribute) and not identifiers_suffix:
             return self._get_sorter_from_method(
-                model_method, identifiers_prefix, identifiers, direction, model, resource, request, order_fields_rfs
+                model_method or model_attribute,
+                identifiers_prefix,
+                identifiers, direction,
+                model,
+                resource,
+                request,
+                order_fields_rfs,
             )
 
 
 class BaseParserModelOrderManager(BaseModelOrderManager):
 
     parsers = [DefaultOrderParser()]
```

### Comparing `skip-django-pyston-2.16.5.3/pyston/order/parsers.py` & `skip-django-pyston-2.16.5.4/pyston/order/parsers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/paginator.py` & `skip-django-pyston-2.16.5.4/pyston/paginator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/patch.py` & `skip-django-pyston-2.16.5.4/pyston/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/requested_fields/managers.py` & `skip-django-pyston-2.16.5.4/pyston/requested_fields/managers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/requested_fields/parser.py` & `skip-django-pyston-2.16.5.4/pyston/requested_fields/parser.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/resource.py` & `skip-django-pyston-2.16.5.4/pyston/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/response.py` & `skip-django-pyston-2.16.5.4/pyston/response.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/serializer.py` & `skip-django-pyston-2.16.5.4/pyston/serializer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/templates/default_pdf_table.html` & `skip-django-pyston-2.16.5.4/pyston/templates/default_pdf_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/templates/pyston/html_converter.html` & `skip-django-pyston-2.16.5.4/pyston/templates/pyston/html_converter.html`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/utils/__init__.py` & `skip-django-pyston-2.16.5.4/pyston/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/utils/compatibility.py` & `skip-django-pyston-2.16.5.4/pyston/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/utils/datastructures.py` & `skip-django-pyston-2.16.5.4/pyston/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/utils/decorators.py` & `skip-django-pyston-2.16.5.4/pyston/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/utils/files.py` & `skip-django-pyston-2.16.5.4/pyston/utils/files.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/pyston/utils/helpers.py` & `skip-django-pyston-2.16.5.4/pyston/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/setup.py` & `skip-django-pyston-2.16.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/PKG-INFO` & `skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pyston
-Version: 2.16.5.3
+Version: 2.16.5.4
 Summary: Pyston is a Django mini-framework creating APIs.
 Home-page: https://github.com/skip-pay/django-pyston
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pyston-2.16.5.3/skip_django_pyston.egg-info/SOURCES.txt` & `skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/SOURCES.txt`

 * *Files identical despite different names*

