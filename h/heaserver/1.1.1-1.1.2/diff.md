# Comparing `tmp/heaserver-1.1.1.tar.gz` & `tmp/heaserver-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.1.1.tar", last modified: Wed Mar 27 00:00:06 2024, max compression
+gzip compressed data, was "heaserver-1.1.2.tar", last modified: Mon Apr  1 23:38:17 2024, max compression
```

## Comparing `heaserver-1.1.1.tar` & `heaserver-1.1.2.tar`

### file list

```diff
@@ -1,283 +1,287 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.399125 heaserver-1.1.1/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.1.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.1.1/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6032 2024-03-27 00:00:06.398055 heaserver-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4037 2024-03-26 23:59:17.000000 heaserver-1.1.1/README.md
--rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.1.1/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.036592 heaserver-1.1.1/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.036592 heaserver-1.1.1/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.068590 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34980 2023-12-16 23:04:09.000000 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19321 2024-03-26 22:51:02.000000 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.070590 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.037622 heaserver-1.1.1/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.038592 heaserver-1.1.1/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.073589 heaserver-1.1.1/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.081657 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.1.1/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.039592 heaserver-1.1.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.040590 heaserver-1.1.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.106658 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.134657 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5792 2023-12-16 23:04:09.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5497 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5166 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4626 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.136658 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.1.1/pytest.ini
--rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.1.1/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 00:00:06.399125 heaserver-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2870 2024-03-26 23:58:32.000000 heaserver-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.043590 heaserver-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.043590 heaserver-1.1.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.183686 heaserver-1.1.1/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.1.1/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.1.1/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    23214 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.194686 heaserver-1.1.1/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.1.1/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    25510 2024-03-26 23:43:40.000000 heaserver-1.1.1/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-26 23:28:53.000000 heaserver-1.1.1/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    30179 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.1.1/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4111 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    25881 2024-03-21 03:54:08.000000 heaserver-1.1.1/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.1.1/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.200685 heaserver-1.1.1/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.1.1/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.1/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.211718 heaserver-1.1.1/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    25567 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.1.1/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.1.1/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    28694 2024-01-21 22:50:36.000000 heaserver-1.1.1/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.1.1/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.235718 heaserver-1.1.1/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    40209 2024-02-05 21:29:09.000000 heaserver-1.1.1/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17482 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130412 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    17724 2024-03-26 22:51:02.000000 heaserver-1.1.1/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.1.1/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.1.1/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36296 2023-12-20 00:39:00.000000 heaserver-1.1.1/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.397055 heaserver-1.1.1/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     6032 2024-03-27 00:00:05.000000 heaserver-1.1.1/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16084 2024-03-27 00:00:06.000000 heaserver-1.1.1/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 00:00:05.000000 heaserver-1.1.1/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2024-03-27 00:00:05.000000 heaserver-1.1.1/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 00:00:05.000000 heaserver-1.1.1/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.046590 heaserver-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.047590 heaserver-1.1.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.293913 heaserver-1.1.1/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.330990 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.331991 heaserver-1.1.1/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    16500 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.336025 heaserver-1.1.1/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.343024 heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5351 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5619 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.362056 heaserver-1.1.1/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.394055 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    54698 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     4273 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.1.1/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7012 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5322 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:00:06.395055 heaserver-1.1.1/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.1.1/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.794462 heaserver-1.1.2/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.1.2/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.1.2/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6137 2024-04-01 23:38:17.793463 heaserver-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4142 2024-03-30 04:07:59.000000 heaserver-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.1.2/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.407276 heaserver-1.1.2/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.407276 heaserver-1.1.2/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.432173 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-03-29 22:12:16.000000 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19321 2024-03-26 22:51:02.000000 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.433718 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.408881 heaserver-1.1.2/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.408889 heaserver-1.1.2/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.436301 heaserver-1.1.2/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.443540 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.1.2/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.410451 heaserver-1.1.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.410451 heaserver-1.1.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.467624 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.495850 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5792 2023-12-16 23:04:09.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5495 2024-03-29 22:05:31.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5164 2024-03-29 21:51:34.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4626 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.497394 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.1.2/pytest.ini
+-rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.1.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 23:38:17.795462 heaserver-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2870 2024-04-01 23:37:33.000000 heaserver-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.412520 heaserver-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.413033 heaserver-1.1.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.549248 heaserver-1.1.2/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.1.2/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.1.2/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    23214 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.563844 heaserver-1.1.2/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.1.2/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    25510 2024-03-27 00:01:36.000000 heaserver-1.1.2/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.1.2/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    30179 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.1.2/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4111 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    26295 2024-03-30 02:37:24.000000 heaserver-1.1.2/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.1.2/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.570842 heaserver-1.1.2/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.1.2/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.2/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.583051 heaserver-1.1.2/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    25695 2024-03-30 03:25:05.000000 heaserver-1.1.2/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.1.2/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.1.2/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-03-30 02:36:21.000000 heaserver-1.1.2/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.1.2/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.611115 heaserver-1.1.2/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    40278 2024-03-30 02:41:55.000000 heaserver-1.1.2/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-03-29 21:46:53.000000 heaserver-1.1.2/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-03-29 21:51:53.000000 heaserver-1.1.2/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    17724 2024-03-26 22:51:02.000000 heaserver-1.1.2/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.1.2/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.1.2/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-03-30 03:45:19.000000 heaserver-1.1.2/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.792460 heaserver-1.1.2/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     6137 2024-04-01 23:38:17.000000 heaserver-1.1.2/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16482 2024-04-01 23:38:17.000000 heaserver-1.1.2/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 23:38:17.000000 heaserver-1.1.2/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      455 2024-04-01 23:38:17.000000 heaserver-1.1.2/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 23:38:17.000000 heaserver-1.1.2/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.414617 heaserver-1.1.2/tests/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.415135 heaserver-1.1.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.677908 heaserver-1.1.2/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.718030 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.719029 heaserver-1.1.2/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    16505 2024-03-29 21:06:36.000000 heaserver-1.1.2/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.723029 heaserver-1.1.2/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.730069 heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5351 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5617 2024-03-29 21:10:13.000000 heaserver-1.1.2/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.750069 heaserver-1.1.2/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.789104 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-03-30 04:01:04.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-03-30 04:04:43.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.1.2/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7012 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5322 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:38:17.791105 heaserver-1.1.2/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.1.2/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.1.1/LICENSE` & `heaserver-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/PKG-INFO` & `heaserver-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.1.1
+Version: 1.1.2
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.1.0
+Requires-Dist: heaobject~=1.1.1
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,14 +47,17 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.1.2
+* Added resolved permissions for desktop objects in WeSTL and Collection+JSON docs.
+
 ## Version 1.1.1
 * No longer errors out when accessing account information that the user is unauthorized to see.
 
 ## Version 1.1.0
 * AWS account objects are now populated with more information.
 * New heaobject with new APIs.
```

### Comparing `heaserver-1.1.1/README.md` & `heaserver-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.1.2
+* Added resolved permissions for desktop objects in WeSTL and Collection+JSON docs.
+
 ## Version 1.1.1
 * No longer errors out when accessing account information that the user is unauthorized to see.
 
 ## Version 1.1.0
 * AWS account objects are now populated with more information.
 * New heaobject with new APIs.
```

### Comparing `heaserver-1.1.1/RELEASING.md` & `heaserver-1.1.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         'invites': [],
         'modified': '2022-05-17T00:00:00+00:00',
         'name': 'VGVzdEZvbGRlci8=',
         'owner': user.NONE_USER,
         'shares': [],
         'source': 'AWS S3',
         'source_detail': None,
-        'type': 'heaobject.folder.AWSS3FolderFileItem',
+        'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
         'actual_object_id': 'VGVzdEZvbGRlci8=',
         'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlci8=',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'storage_class': 'STANDARD',
         'mime_type': 'application/x.item',
         'size': None,
@@ -55,15 +55,15 @@
         'invites': [],
         'modified': '2022-05-17T00:00:00+00:00',
         'name': 'VGVzdEZvbGRlcjIv',
         'owner': user.NONE_USER,
         'shares': [],
         'source': 'AWS S3',
         'source_detail': None,
-        'type': 'heaobject.folder.AWSS3FolderFileItem',
+        'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
         'actual_object_id': 'VGVzdEZvbGRlcjIv',
         'actual_object_uri': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlcjIv',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
         'storage_class': 'STANDARD',
         'mime_type': 'application/x.item',
         'size': None,
```

### Comparing `heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.1.2/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.1.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.1.2/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     'permissions': [Permission.VIEWER.name]
                 }
             ],
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
-            "manager_ids": [''],
+            "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': []
         }
     ]}
 
 content = {
```

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
-            "manager_ids": [''],
-            "member_ids": [TEST_USER],
+            "manager_ids": [TEST_USER],
+            "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
             'created': None,
             'modified': None,
             'admin_ids': []
         }
     ]}
```

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.1.2/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/setup.py` & `heaserver-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.1.1',
+      version='1.1.2',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=find_namespace_packages(where='src'),
       package_data={'heaserver.service': ['py.typed', 'jsonschemafiles/*']},
       install_requires=[
-          'heaobject~=1.1.0',
+          'heaobject~=1.1.1',
           'aiohttp[speedups]~=3.8.6',
           'hea-aiohttp-remotes~=1.2.1',  # replace with aiohttp-remotes if they incorporate our patch.
           'motor~=3.2.0',
           'motor-types~=1.0.0b2',
           'accept-types~=0.4.1',
           'mongoquery~=1.4.2',
           'jsonschema~=4.17.3',
```

### Comparing `heaserver-1.1.1/src/heaserver/service/__init__.py` & `heaserver-1.1.2/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/activity.py` & `heaserver-1.1.2/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/aiohttp.py` & `heaserver-1.1.2/src/heaserver/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/appfactory.py` & `heaserver-1.1.2/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/appproperty.py` & `heaserver-1.1.2/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/backgroundtasks.py` & `heaserver-1.1.2/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/caching.py` & `heaserver-1.1.2/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/client.py` & `heaserver-1.1.2/src/heaserver/service/client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/config.py` & `heaserver-1.1.2/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/aws.py` & `heaserver-1.1.2/src/heaserver/service/db/aws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.1.2/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/database.py` & `heaserver-1.1.2/src/heaserver/service/db/database.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/dbapi2.py` & `heaserver-1.1.2/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/mongo.py` & `heaserver-1.1.2/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.1.2/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.1.2/src/heaserver/service/db/mongoservicelib.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .. import response
 from ..heaobjectsupport import new_heaobject_from_type, has_permissions, RESTPermissionGroup
 from ..appproperty import HEA_DB, HEA_CACHE
 from .mongo import MongoContext
 from heaobject.error import DeserializeException
 from aiohttp.web import Request, StreamResponse, Response, HTTPError
 from typing import Any, AsyncGenerator, Literal, IO
-from heaobject.root import DesktopObject, DesktopObjectDict, desktop_object_from_dict
+from heaobject.root import DesktopObject, DesktopObjectDict, desktop_object_from_dict, Permission
 from heaobject.user import NONE_USER
 from heaserver.service.oidcclaimhdrs import SUB
 from pymongo.errors import WriteError
 from collections.abc import Sequence, Mapping
 
 
 async def get_dict(request: Request, collection: str,
@@ -54,15 +54,20 @@
     :param request: the HTTP request, which must have an id value in the match_info mapping. Required.
     :param collection: the Mongo collection name. Required.
     :param volume_id: the id string of the volume containing the requested HEA object. If None, the root volume is
     assumed.
     :return: a Response with the requested HEA object or Not Found.
     """
     result = await get_dict(request, collection, volume_id)
-    return await response.get(request, desktop_object_from_dict(result).to_dict() if result is not None else None)
+    if result is None:
+        return await response.get(request, None)
+    else:
+        obj = desktop_object_from_dict(result)
+        sub = request.headers.get(SUB, NONE_USER)
+        return await response.get(request, obj.to_dict(), obj.get_permissions(sub))
 
 
 async def get_content(request: Request, collection: str, volume_id: str | None = None) -> StreamResponse:
     """
     Gets the HEA object's associated content.
 
     :param request: the HTTP request. Required.
@@ -159,20 +164,25 @@
         cache_key = (sub, collection, None, tuple((key, val) for key, val in (sort or {}).items()))
         cached_value = request.app[HEA_CACHE].get(cache_key)
     else:
         cached_value = None
     if mongoattributes is None and cached_value is not None:
         return await response.get_all(request, cached_value)
     else:
+        objs: list[DesktopObject] = []
         l: list[DesktopObjectDict] = []
         async for obj in _get_all_gen(request, collection, volume_id, mongoattributes, sort):
+            objs.append(obj)
             l.append(obj.to_dict())
         if mongoattributes is None and not request.query:
             request.app[HEA_CACHE][cache_key] = l
-        return await response.get_all(request, l)
+        perms: list[list[Permission]] = []
+        for obj in objs:
+            perms.append(obj.get_permissions(sub))
+        return await response.get_all(request, l, perms)
 
 async def get_all_dict(request: Request,
                        collection: str,
                        volume_id: str | None = None,
                        mongoattributes: Any | None = None,
                        sort: dict[str, Literal[-1, 1]] | None = None) -> list[DesktopObjectDict]:
     """
@@ -233,18 +243,19 @@
         async with MongoContext(request, volume_id) as mongo:
             result = await mongo.get(request, collection, var_parts='id', sub=request.headers.get(SUB))
             if result is not None:
                 obj = heaobject.root.desktop_object_from_dict(result)
                 permitted = has_permissions(obj=obj, sub=request.headers.get(SUB, NONE_USER), permissions=RESTPermissionGroup.GETTER_PERMS)
                 if not permitted:
                     return response.status_not_found()
+                request.app[HEA_CACHE][cache_key] = result
+                return await response.get_multiple_choices(request, result if include_desktop_object_ else None, permissions=[obj.get_permissions(sub)])
             else:
                 return response.status_not_found()
-            request.app[HEA_CACHE][cache_key] = result
-            return await response.get_multiple_choices(request, result if include_desktop_object_ else None)
+
 
 
 async def post(request: Request, collection: str, type_: type[DesktopObject], default_content: IO | None = None, volume_id: str | None = None) -> Response:
     """
     Posts the provided HEA object.
 
     :param request: the HTTP request.
```

### Comparing `heaserver-1.1.1/src/heaserver/service/expression.py` & `heaserver-1.1.2/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/functional.py` & `heaserver-1.1.2/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.1.2/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/jsonschema.py` & `heaserver-1.1.2/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.1.2/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.1.2/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.1.2/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.1.2/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.1.2/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/messagebroker.py` & `heaserver-1.1.2/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/mimetypes.py` & `heaserver-1.1.2/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.1.2/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/openapi.py` & `heaserver-1.1.2/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/__init__.py` & `heaserver-1.1.2/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/cj.py` & `heaserver-1.1.2/src/heaserver/service/representor/cj.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,17 @@
         parameter contains the index of the item, or None if the link is global. The second parameter
         contains the link as a heaserver.service.representor.Link object.
         :return: a Collection+JSON dict.
         """
         wstl = wstl_obj['wstl']
         collection: dict[str, Any] = {}
         collection['version'] = '1.0'
-        collection['href'] = wstl.get('hea', {}).get('href', '#')
+        wstl_hea = wstl.get('hea', {})
+        collection['href'] = wstl_hea.get('href', '#')
+        collection['permissions'] = wstl_hea.get('permissions', [[]] * len(wstl.get('data', [])))
 
         content = _get_content(wstl)
         if content:
             collection['content'] = content
         tvars = {}
         items = tuple(item for item in _get_items(request, wstl, link_callback=link_callback, tvars=tvars))
         if items:
```

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/factory.py` & `heaserver-1.1.2/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.1.2/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/representor.py` & `heaserver-1.1.2/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/wstljson.py` & `heaserver-1.1.2/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.1.2/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/response.py` & `heaserver-1.1.2/src/heaserver/service/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 from hashlib import md5
 from heaobject.user import NONE_USER
 
 from .representor.factory import formats_from_request
 from . import requestproperty, appproperty
 from .appproperty import HEA_BACKGROUND_TASKS
 from .oidcclaimhdrs import SUB
-from .representor import factory as representor_factory
 from .representor.representor import Link
 from yarl import URL
 import logging
 from typing import Union, Optional, Any
 from collections.abc import Iterable, Mapping, Sequence
 from .aiohttp import SupportsAsyncRead
 from .wstl import RuntimeWeSTLDocumentBuilder
-from heaobject.root import DesktopObjectDict
+from heaobject.root import DesktopObjectDict, Permission
 from multidict import istr, CIMultiDict, CIMultiDictProxy
 from .caching_strategy import CachingStrategy
 
 TEXT_PLAIN_HTTP_HEADERS: Union[Mapping[Union[str, istr], str], None] = {hdrs.CONTENT_TYPE: 'text/plain; charset=UTF-8'}
 NO_CACHE_HEADERS = {hdrs.CACHE_CONTROL: 'no-cache, no-store, must-revalidate', hdrs.PRAGMA: 'no-cache', hdrs.EXPIRES: '0'}
 
 
@@ -233,32 +232,33 @@
     this function will encode it to bytes using UTF-8 encoding.
     :return: aiohttp.web.Response object with a 409 status code.
     """
     body_ = body.encode() if isinstance(body, str) else body
     return web.HTTPConflict(body=body_)
 
 
-async def get(request: web.Request, data: Optional[DesktopObjectDict]) -> web.Response:
+async def get(request: web.Request, data: Optional[DesktopObjectDict], permissions: Sequence[Permission] | None = None) -> web.Response:
     """
     Create and return a HTTP response object in response to a GET request for one or more HEA desktop object resources.
 
     :param request: the HTTP request (required).
     :param data: a HEA desktop object dict. May be None if you want no data to be included in the response.
     :return: aiohttp.web.Response object, with status code 200, containing a body with the HEA desktop object, or
     status code 404 if the data argument is None.
     """
     if data:
-        return await _handle_get_result(request, data)
+        return await _handle_get_result(request, data, [permissions] if permissions is not None else None)
     else:
         return web.HTTPNotFound()
 
 
 async def get_multiple_choices(request: web.Request,
                                result: DesktopObjectDict | None = None,
-                               caching_strategy: CachingStrategy = None) -> web.Response:
+                               caching_strategy: CachingStrategy = None,
+                               permissions: Sequence[Sequence[Permission]] = None) -> web.Response:
     """
     Create and return a HTTP response to a GET request with available links for opening the requested desktop
     object, possibly with a representation of the object. Unlike with typical GET requests, this function generates a
     successful response with status code 300 to indicate that the endpoint is for the purpose of client-side content
     negotiation. More information about content negotiation is available from
     https://developer.mozilla.org/en-US/docs/Web/HTTP/Content_negotiation.
 
@@ -293,15 +293,16 @@
     def link_callback(action_index: int, link: Link):
         nonlocal default_url
         if default_url is None or 'default' in link.rel:
             default_url = link.href
     try:
         body, mime_type = await wstl_builder.represent_from_request(request,
                                                                     [result] if result else None,
-                                                                    link_callback=link_callback)
+                                                                    link_callback=link_callback,
+                                                                    permissions=permissions)
         _logger.debug('Response body is %s', body)
         etag = _compute_etag(body)
         if request.if_none_match and etag in request.if_none_match:
             return web.HTTPNotModified()
         response = status_multiple_choices(default_url=default_url if default_url else '#', body=body,
                                            content_type=mime_type)
         if caching_strategy:
@@ -335,24 +336,24 @@
     :param request: the HTTP request (required).
     :param run_time_docs: a list of run-time WeSTL documents containing data.
     :return: aiohttp.web.Response object with a body containing the object in a JSON array of objects.
     """
     return await _handle_get_result_from_wstl(request, run_time_docs)
 
 
-async def get_all(request: web.Request, data: Sequence[DesktopObjectDict]) -> web.Response:
+async def get_all(request: web.Request, data: Sequence[DesktopObjectDict], permissions: Sequence[Sequence[Permission]] | None = None) -> web.Response:
     """
     Create and return a Response object in response to a GET request for all HEA desktop object resources in a
     collection.
 
     :param request: the HTTP request (required).
     :param data: a list of HEA desktop object dicts.
     :return: aiohttp.web.Response object with a body containing the object in a JSON array of objects.
     """
-    return await _handle_get_result(request, data)
+    return await _handle_get_result(request, data, permissions)
 
 
 async def get_options(request: web.Request, methods: Iterable[str]) -> web.Response:
     """
     Create and return a Response object in response to an OPTIONS request.
 
     :param request: the HTTP request (required).
@@ -447,15 +448,16 @@
     """
     if result:
         return web.HTTPNoContent()
     else:
         return web.HTTPNotFound()
 
 
-async def _handle_get_result(request: web.Request, data: Union[DesktopObjectDict, Sequence[DesktopObjectDict]]) -> web.Response:
+async def _handle_get_result(request: web.Request, data: Union[DesktopObjectDict, Sequence[DesktopObjectDict]],
+                             permissions: Sequence[Sequence[Permission]] | None = None) -> web.Response:
     """
     Handle the result from a get request. Returns a Response object, the body of which will always contain a list of
     JSON objects.
 
     :param request: the HTTP request object. Cannot be None.
     :param data: the retrieved HEA desktop objects as a dict or a list of dicts, with each dict representing a
     desktop object with its attributes as name-value pairs.
@@ -463,15 +465,15 @@
     code 404 (Not Found).
     """
     logger = logging.getLogger(__name__)
     if data is not None:
         wstl_builder = request[requestproperty.HEA_WSTL_BUILDER]
         wstl_builder.href = str(request.url)
         try:
-            body, mime_type = await wstl_builder.represent_from_request(request, data if isinstance(data, Sequence) else [data])
+            body, mime_type = await wstl_builder.represent_from_request(request, data if isinstance(data, Sequence) else [data], permissions=permissions)
             return await _to_response(request, body, mime_type)
         except ValueError as e:
             logger.exception('Invalid input data %s', wstl_builder)
             return status_not_acceptable(str(e))
     else:
         return status_not_found()
```

### Comparing `heaserver-1.1.1/src/heaserver/service/runner.py` & `heaserver-1.1.2/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.1.2/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.1.2/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.1.2/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/collection.py` & `heaserver-1.1.2/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/docker.py` & `heaserver-1.1.2/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.1.2/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.1.2/src/heaserver/service/testcase/expectedvalues.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from dataclasses import dataclass
 import uritemplate
 
 from .collection import CollectionKey, query_fixture_collection
 from ..uritemplate import tvars as extra_tvars
 from enum import Enum
 from heaobject.root import is_primitive, is_primitive_list, is_heaobject_dict_list, is_heaobject_dict, HEAObjectDict, \
-    Primitive, HEAObjectDictValue, MemberObjectDict, Union, DesktopObjectDict
+    HEAObjectDictValue, Union, DesktopObjectDict, desktop_object_from_dict, Permission
+from heaobject.user import NONE_USER
 from datetime import date, time
 from heaserver.service.representor.cj import add_extended_property_values
 from heaserver.service.expression import get_eval_for
 
 
 class Action:
     def __init__(self,
@@ -123,15 +124,16 @@
     logger_.debug('Transforming into template %s', data)
     return _create_template({**data, **{'description': 'A description'}}, exclude=None)
 
 
 def expected_one_wstl(fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
                       coll: str | CollectionKey,
                       wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
-                      get_actions: Optional[List[Action]] = None) -> List[Dict[str, Any]]:
+                      get_actions: Optional[List[Action]] = None,
+                      sub=NONE_USER) -> List[Dict[str, Any]]:
     """
     Create a run-time WeSTL document from a data test fixture. The document will contain the first HEAObject dict in
     the given collection, and will contain a single action.
 
     :param fixtures: mongodb collection name/key -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name or key to use. Required.
     :param wstl_builder: a runtime WeSTL document builder object. Required.
@@ -156,26 +158,30 @@
             raise ValueError(f'Action {action_name} does not exist')
         action = {**action,
                   'href': action_url if action_url else "http://localhost:8080",
                   'rel': action_rel if action_rel else []}
         if itemif is not None:
             action.setdefault('hea', {})['itemIf'] = itemif
         actions.append(action)
+    desktop_objects = [desktop_object_from_dict(obj)]
     return [{
         'wstl': {
-            'data': [_wstl_data_transform(obj)],
-            'hea': {'href': str(URL(href_) / str(obj['id']))},
+            'data': [desktop_object.to_dict() for desktop_object in desktop_objects],
+            'hea': {'href': str(URL(href_) / str(obj['id'])),
+                    'permissions': [[perm.name for perm in desktop_object.get_permissions(sub)] for desktop_object in desktop_objects]
+                    },
             'actions': actions,
             'title': wstl_builder.design_time_document['wstl']['title']}}]
 
 
 def expected_one(fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
                  coll: str | CollectionKey,
                  wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
-                 get_actions: Optional[List[Action]] = None) -> List[Dict[str, Dict[str, Any]]]:
+                 get_actions: Optional[List[Action]] = None,
+                 sub=NONE_USER) -> List[Dict[str, Dict[str, Any]]]:
     """
     Create a Collection+JSON document with the first HEAObject from a mongodb collection in the given data test fixture.
 
     :param fixtures: mongodb collection name -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name to use. Required.
     :param wstl_builder: a runtime WeSTL document builder object. Required.
     :param default_db_manager_cls: The database manager to use if the collection key is a string. Required.
@@ -281,19 +287,21 @@
                     q['data'].append(rtn)
                 queries.append(q)
         return queries
 
     item_link_ = item_link()
 
     data_: List[Dict[str, Any]] = []
+    perms = desktop_object_from_dict(obj).get_permissions(sub)
     for x, y in obj.items():
         _data_append(data_, x, y)
     collection: Dict[str, Any] = {
         'collection': {
             'href': str(href),
+            'permissions': [[perm.name for perm in perms]],
             'items': [{'data': data_,
                        'links': item_links()}],
             'version': '1.0'}}
     if item_link_:
         if 'rel' in item_link_:
             collection['collection']['items'][0]['rel'] = item_link_['rel']
         collection['collection']['items'][0]['href'] = item_link_['href']
@@ -312,30 +320,31 @@
 
 
 def expected_opener_body(
     fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
     coll: str | CollectionKey,
     wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
     get_actions: Optional[List[Action]] = None,
-    opener_link: Optional[Link] = None) -> Optional[List[Dict[str, Any]]]:
+    opener_link: Optional[Link] = None,
+    sub=NONE_USER) -> Optional[List[Dict[str, Any]]]:
     """
     Create a Collection+JSON document with the first HEAObject from a mongodb collection in the given data test fixture,
     including an opener link.
 
     :param fixtures: mongodb collection name/key -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name or key to use. Required.
     :param wstl_builder: a runtime WeSTL document builder object. Required.
     :param default_db_manager_cls: The database manager to use if the collection key is a string. Required.
     :param get_actions: the actions to include in the body of GET calls.
     :param opener_link: link for an opener choice. If None or omitted, this function will return None.
     :return: a list containing the first object in the fixture and mongodb collection as a Collection+JSON template as
     a dict, or None if no opener link was passed in.
     """
     if opener_link:
-        body = expected_one(fixtures, coll, wstl_builder, get_actions=get_actions)
+        body = expected_one(fixtures, coll, wstl_builder, get_actions=get_actions, sub=sub)
         coll_ = body[0]['collection']
         coll_.pop('template', None)
         coll_['href'] = coll_['href'] + '/opener'
         coll_['items'][0]['links'] = [
             {'prompt': 'Open', 'href': opener_link.url, 'rel': ' '.join(opener_link.rel or [])}]
         logging.getLogger(__name__).debug('Expected opener body is %s', body)
         return body
@@ -346,15 +355,15 @@
 
 def expected_one_duplicate_form(
     fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
     coll: str | CollectionKey,
     wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
     duplicate_action_name: str,
     duplicate_action_rel: Optional[List[str]] = None,
-    actions: list[Action] | None = None) -> List[Dict[str, Any]]:
+    actions: list[Action] | None = None, sub = NONE_USER) -> List[Dict[str, Any]]:
     """
     Create a Collection+JSON document with the first HEAObject from the given mongodb collection in the given data test
     fixture. The returned Collection+JSON document will contain the HEAObject in the data section and a template
     for duplicating the HEAObject.
 
     :param fixtures: mongodb collection name/key -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name or key to use. Required.
@@ -364,21 +373,22 @@
     these objects do not support duplication.
     :param duplicate_action_rel: list of rel strings for the action. Optional.
     :return: a list of Collection+JSON templates as dicts.
     """
     if not duplicate_action_name:
         return None
     return _expected_one_form(fixtures, coll, wstl_builder, duplicate_action_name,
-                              duplicate_action_rel, suffix='/duplicator', actions=actions)
+                              duplicate_action_rel, suffix='/duplicator', actions=actions, sub=sub)
 
 
 def expected_all_wstl(fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
                       coll: str | CollectionKey,
                       wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
-                      get_all_actions: Optional[List[Action]] = None) -> List[Dict[str, Dict[str, Any]]]:
+                      get_all_actions: Optional[List[Action]] = None,
+                      sub = NONE_USER) -> List[Dict[str, Dict[str, Any]]]:
     """
     Create a run-time WeSTL document from a data test fixture. The document will contain all HEAObject dicts in
     the given collection, and it will contain a single action.
 
     :param fixtures: mongodb collection name/key -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name or key to use. Required.
     :param wstl_builder: a runtime WeSTL document builder object. Required.
@@ -405,29 +415,32 @@
                 if optionsFromUrl is not None:
                     optionsFromUrlPath = optionsFromUrl['path']
                     optionsFromUrl['href'] = 'http://localhost:8080' + ('/' if optionsFromUrlPath else '') + optionsFromUrlPath
             if itemif is not None:
                 action.setdefault('hea', {})['itemIf'] = itemif
             result.append(action)
         return result
-
+    desktop_objects = [desktop_object_from_dict(o) for o in query_fixture_collection(fixtures, coll)]
     return [{
         'wstl': {
-            'data': _wstl_data_transform(query_fixture_collection(fixtures, coll)),
+            'data': [obj.to_dict() for obj in desktop_objects],
             'actions': runtime_actions(),
             'title': wstl_builder.design_time_document['wstl']['title'],
-            'hea': {'href': href_ if href_ else '#'}
+            'hea': {'href': href_ if href_ else '#',
+                    'permissions': [[perm.name for perm in obj.get_permissions(sub)] for obj in desktop_objects]
+                    }
         }
     }]
 
 
 def expected_all(fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
                  coll: str | CollectionKey,
                  wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
-                 get_all_actions: Optional[List[Action]] = None) -> List[Dict[str, Any]]:
+                 get_all_actions: Optional[List[Action]] = None,
+                 sub=NONE_USER) -> List[Dict[str, Any]]:
     """
     Create a list of Collection+JSON documents with all HEAObjects from a mongodb collection in the given data test fixture.
 
     :param fixtures: mongodb collection name/key -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name or key to use. Required.
     :param wstl_builder: a runtime WeSTL document builder object. Required.
     :param default_db_manager_cls: The database manager to use if the collection key is a string. Required.
@@ -492,29 +505,32 @@
                     'href': url if url else str(URL(href_) / ''),
                     'rel': ' '.join(rel)
                 })
         return links
 
     items = []
     collection = query_fixture_collection(fixtures, coll)
+    perms: list[list[Permission]] = []
     for f in collection:
+        obj = desktop_object_from_dict(f)
+        perms.append(obj.get_permissions(sub))
         data_: List[Dict[str, Any]] = []
-        id_ = f['id']
         item_link_ = item_link(f)
         for x, y in f.items():
             _data_append(data_, x, y)
         item = {'data': data_,
                 'links': item_links(f)}
         if item_link_:
             if 'rel' in item_link_:
                 item['rel'] = item_link_['rel']
             item['href'] = item_link_['href']
         items.append(item)
 
     collection_doc = {'collection': {'href': str(wstl_builder.href if wstl_builder.href else '#'),
+                                     'permissions': [[p.name for p in perm] for perm in perms],
                                      'items': items,
                                      'version': '1.0'}}
     for action, action_name, rel, itemif in ((wstl_builder.find_action(a.name), a.name, a.rel, a.itemif) for a in get_all_actions_):
         if action is None:
             raise ValueError(f'Invalid action name in get_all_actions {action_name}')
         if len(set(i['type'] for i in collection)) < 2 and (itemif is None or get_eval_for(f).eval(itemif)):
             _set_collection_template(action, collection_doc, f, len(collection), rel)
@@ -529,15 +545,16 @@
                     wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
                     duplicate_action_name: str | None,
                     href: Optional[Union[str, URL]],
                     get_actions: Optional[List[Action]] = None,
                     get_all_actions: Optional[List[Action]] = None,
                     opener_link: Optional[Link] = None,
                     duplicate_action_actions: list[Action] | None = None,
-                    exclude: list[str] | None = None) -> Dict[str, Any]:
+                    exclude: list[str] | None = None,
+                    sub = NONE_USER) -> Dict[str, Any]:
     """
     Generate a dict of all the expected values for passing into the mongotestcase and mockmongotestcase
     get_test_case_cls function.
 
     :param fixtures: the data to load into the database, as a map of collection name -> list of desktop object dicts.
     Required.
     :param coll: the collection name to use. Required.
@@ -559,32 +576,32 @@
         body_put_ = body_put(fixtures, coll)
         content_id = next((e.get('value') for e in body_put_['template']['data'] if e['name'] == 'id'), None)
         result['body_put'] = body_put_
         result['content_id'] = content_id
     if not exclude or ('body_post' not in exclude):
         result['body_post'] = body_post(fixtures, coll)
     if not exclude or ('expected_one_wstl' not in exclude):
-        result['expected_one_wstl'] = expected_one_wstl(fixtures, coll, wstl_builder_, get_actions=get_actions)
+        result['expected_one_wstl'] = expected_one_wstl(fixtures, coll, wstl_builder_, get_actions=get_actions, sub=sub)
     if not exclude or ('expected_one' not in exclude):
-        result['expected_one'] = expected_one(fixtures, coll, wstl_builder_, get_actions=get_actions)
+        result['expected_one'] = expected_one(fixtures, coll, wstl_builder_, get_actions=get_actions, sub=sub)
     if not exclude or ('expected_one_duplicate_form' not in exclude):
         result['expected_one_duplicate_form'] = expected_one_duplicate_form(fixtures, coll, wstl_builder_,
                                                                    duplicate_action_name,
-                                                                   actions=duplicate_action_actions)
+                                                                   actions=duplicate_action_actions, sub=sub)
     if not exclude or ('expected_all_wstl' not in exclude):
-        result['expected_all_wstl'] = expected_all_wstl(fixtures, coll, wstl_builder_,
-                                               get_all_actions=get_all_actions)
+        result['expected_all_wstl'] = expected_all_wstl(fixtures, coll, wstl_builder_, get_all_actions=get_all_actions,
+                                                        sub=sub)
     if not exclude or ('expected_all' not in exclude):
         result['expected_all'] = expected_all(fixtures, coll, wstl_builder_,
-                                     get_all_actions=get_all_actions)
+                                     get_all_actions=get_all_actions, sub=sub)
     if not exclude or ('expected_opener' not in exclude):
         result['expected_opener'] = opener_link.url if opener_link is not None else None
     if not exclude or ('expected_opener_body' not in exclude):
         result['expected_opener_body'] = expected_opener_body(fixtures, coll, wstl_builder_,
-                                                     get_actions=get_actions, opener_link=opener_link)
+                                                     get_actions=get_actions, opener_link=opener_link, sub=sub)
     return result
 
 
 def _create_template(d: DesktopObjectDict, exclude=('id',)) -> Dict[str, Dict[str, List[Dict[str, Any]]]]:
     return {'template': {'data': [z for x, y in d.items() if (not exclude or x not in exclude) for z in
                                   _nvpjson_property_to_cj_part_generator(x, y)]}}
 
@@ -674,15 +691,16 @@
 def _expected_one_form(
     fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
     coll: str | CollectionKey,
     wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
     action_name: str,
     action_rel: Optional[List[str]] = None,
     suffix: str = None,
-    actions: Optional[List[Action]] = None) -> List[Dict[str, Any]]:
+    actions: Optional[List[Action]] = None,
+    sub = NONE_USER) -> List[Dict[str, Any]]:
     """
     Create a Collection+JSON document with the first HEAObject from the given mongodb collection in the given data test
     fixture. The returned Collection+JSON document will contain the HEAObject in the data section and a template
     containing that HEAObject's values.
 
     :param fixtures: mongodb collection name/key -> list of HEAObject dicts. Required.
     :param coll: the mongodb collection name or key to use. Required.
@@ -691,50 +709,51 @@
     :param action_name: the name of the action that causes creation of the template. Required.
     :param action_rel: list of rel strings for the action. Optional.
     :return: a list of Collection+JSON templates as dicts.
     """
     action = wstl_builder.find_action(action_name)
     if action is None:
         raise ValueError(f'Action {action_name} does not exist')
-    obj = query_fixture_collection(fixtures, coll)[0]
-    id_ = str(obj['id'])
+    obj_dict = query_fixture_collection(fixtures, coll)[0]
+    id_ = str(obj_dict['id'])
     href = URL(wstl_builder.href if wstl_builder.href else '') / (id_ + (suffix if suffix else ''))
 
-    data_ = _heaobject_dict_to_collection_plus_json_data(obj)
+    data_ = _heaobject_dict_to_collection_plus_json_data(obj_dict)
 
     def get_link(a: Action):
         action_ = wstl_builder.find_action(a.name)
         if action_ is None:
             raise ValueError(f'Action {a.name} does not exist')
         if a.url is not None:
             match = extra_tvars(route=a.url, url=str(href))
         else:
             match = {}
-        return {'href': uritemplate.expand(a.url, {k: v for k, v in (match | obj).items()
+        return {'href': uritemplate.expand(a.url, {k: v for k, v in (match | obj_dict).items()
                                                    if isinstance(v, (int, float, str))}) if a.url else str(href),
                 'rel': ' '.join(a.rel or []),
                 'prompt': action_['prompt']}
 
     def set_default_values_from_headata_links():
         for link in links_:
             field_name = next((r.removeprefix('headata-') for r in link['rel'].split() if r.startswith('headata-')),
                               None)
             if field_name:
                 for d in template_data:
                     if d['name'] == field_name:
                         d['value'] = link['href']
 
     links_ = [get_link(a) for a in actions or []]
-    template_data = [d for d in _template_data_generator(action, obj)]
+    template_data = [d for d in _template_data_generator(action, obj_dict)]
     set_default_values_from_headata_links()
-
+    obj = desktop_object_from_dict(obj_dict)
     return [{
         'collection': {
             'version': '1.0',
             'href': str(href),
+            'permissions': [[perm.name for perm in obj.get_permissions(sub)]],
             'items': [
                 {
                     'data': data_,
                     'links': links_
                 }],
             'template': {
                 'prompt': action.get('prompt', None),
@@ -746,40 +765,14 @@
 def _heaobject_dict_to_collection_plus_json_data(obj):
     data_: List[Dict[str, Any]] = []
     for x, y in obj.items():
         _data_append(data_, x, y)
     return data_
 
 
-def _wstl_data_transform(data: HEAObjectDictValue) -> HEAObjectDictValue:
-    """
-    Recursively goes through HEA object dicts, lists of HEA object dicts, primitive lists, and primitives, and replaces
-    any enums and dates with strings as if the dicts had been serialized to JSON and deserialized back to dicts.
-
-    :param data: HEA object dict, list of HEA object dicts, primitive list, or primitive.
-    :return: a deep copy of the same data except with enums and dates replaced with strings.
-    """
-    if is_heaobject_dict_list(data):
-        return [cast(MemberObjectDict, _wstl_data_transform(elt)) for elt in cast(List[MemberObjectDict], data)]
-    elif is_heaobject_dict(data):
-        return {x: cast(Union[Primitive, List[Primitive]], _wstl_data_transform(y)) for x, y in
-                cast(MemberObjectDict, data).items()}
-    elif is_primitive_list(data):
-        return [cast(Primitive, _wstl_data_transform(d)) for d in cast(List[Primitive], data)]
-    elif is_primitive(data):
-        if isinstance(data, Enum):
-            return str(data)
-        elif isinstance(data, date):
-            return data.isoformat()
-        else:
-            return data
-    else:
-        raise ValueError(str(data))
-
-
 def _data_append(data: List[Dict[str, Any]], x: str, y: HEAObjectDictValue):
     if is_heaobject_dict(y):
         for xprime, yprime in cast(HEAObjectDict, y).items():
             _data_append_part(data, xprime, yprime, {'section': x})
     elif is_heaobject_dict_list(y):
         for i, yprime_ in enumerate(cast(List[HEAObjectDict], y)):
             for xprimeprime, yprimeprime in yprime_.items():
```

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.1.2/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                               href: Optional[str | URL] = None,
                               get_actions: Optional[list[Action]] = None,
                               get_all_actions: Optional[list[Action]] = None,
                               expected_opener: Optional[Link] = None,
                               registry_docker_image: Optional[RegistryContainerConfig] = None,
                               other_docker_images: Iterable[DockerContainerConfig] | None = None,
                               port: Optional[int] = None,
-                              sub: Optional[str] = NONE_USER,
+                              sub = NONE_USER,
                               exclude: Optional[list[str]] = None,
                               duplicate_action_actions: list[Action] | None = None,
                               package_name: str | None = None) -> Type[MicroserviceTestCase]:
     """
     Create a test case class for testing a specific HEA microservice.
 
     :param coll: the name of the collection that the microservice uses (required).
@@ -244,15 +244,16 @@
     coll_ = coll if isinstance(coll, CollectionKey) else CollectionKey(name=coll, db_manager_cls=db_manager_cls)
     expected_values_ = {k: v for k, v in expected_values(fixtures, coll_, wstl.builder(package=wstl_package),
                                                          duplicate_action_name, href,
                                                          get_actions=get_actions,
                                                          get_all_actions=get_all_actions,
                                                          opener_link=expected_opener,
                                                          duplicate_action_actions=duplicate_action_actions,
-                                                         exclude=exclude_).items() if v is not None}
+                                                         exclude=exclude_,
+                                                         sub=sub).items() if v is not None}
 
     class ExpectedValuesMicroserviceTestCase(MicroserviceTestCase):
         def __init__(self, methodName: str = 'runTest') -> None:
             super().__init__(package_name=package_name, coll=coll, desktop_objects=fixtures,
                              db_manager_cls=db_manager_cls,
                              wstl_package=wstl_package, href=href, content=content, content_type=content_type,
                              put_content_status=put_content_status, registry_docker_image=registry_docker_image,
```

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/mixin.py` & `heaserver-1.1.2/src/heaserver/service/testcase/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2389,9 +2389,11 @@
         return sorted((_ordered_one(k, v) for k, v in obj.items()))
     if isinstance(obj, list):
         try:
             return sorted(_ordered(x) for x in obj)
         except TypeError as t:
             print('obj is {}'.format(obj))
             raise t
+    elif isinstance(obj, date):
+        return obj.isoformat()
     else:
         return str(obj)
```

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.1.2/src/heaserver/service/testcase/mockaws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.1.2/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.1.2/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.1.2/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.1.2/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/testenv.py` & `heaserver-1.1.2/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/testcase/util.py` & `heaserver-1.1.2/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/uritemplate.py` & `heaserver-1.1.2/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/util.py` & `heaserver-1.1.2/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/src/heaserver/service/wstl.py` & `heaserver-1.1.2/src/heaserver/service/wstl.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 import logging
 import pkgutil
 import json
 import jsonmerge  # type: ignore
 from collections import abc
 from aiohttp.web import Request, Response
 from typing import Optional, Callable, Any, Coroutine, Union
-from heaobject.root import DesktopObjectDict
+from heaobject.root import DesktopObjectDict, Permission
 
 from . import appproperty, requestproperty, jsonschemavalidator, jsonschema
 from .representor.representor import Link
 from yarl import URL
 from .util import check_duplicates, DuplicateError
 
 DEFAULT_DESIGN_TIME_WSTL = {
@@ -343,15 +343,16 @@
         run_time_wstl_copy = copy.deepcopy(self.__run_time_wstl)
         if data is not None:
             run_time_wstl_copy['wstl']['data'] = data if isinstance(data, abc.Sequence) else [data]
         return await from_mime_type(mime_type).formats(request, run_time_wstl_copy, link_callback=link_callback)
 
     async def represent_from_request(self, request: Request,
                                      data: DesktopObjectDict | abc.Sequence[DesktopObjectDict] | None,
-                                     link_callback: abc.Callable[[int, Link], None] = None) -> tuple[bytes, str]:
+                                     link_callback: abc.Callable[[int, Link], None] = None,
+                                     permissions: abc.Sequence[abc.Sequence[Permission]] | None = None) -> tuple[bytes, str]:
         """
         Generates a run-time WeSTL document with the given data and the builder's attributes, and it applies the
         heaserver.service.representor class with the mime type requested in the HTTP request's Accept header to format
         the run-time document.
 
         :param request: the HTTP request (required).
         :param data: the desktop object data to include in the response.
@@ -361,16 +362,27 @@
         parameter contains the link as a heaserver.service.representor.Link object. The purpose of this
         callback is to access parameterized links after their parameters have been filled in.
         :return: a tuple of the formatted document and the document's mime type.
         :raises ValueError: if the request has an invalid Accept header.
         """
         from heaserver.service.representor.factory import formats_from_request
         run_time_wstl_copy = copy.deepcopy(self.__run_time_wstl)
+        wstl = run_time_wstl_copy['wstl']
         if data is not None:
-            run_time_wstl_copy['wstl']['data'] = data if isinstance(data, abc.Sequence) else [data]
+            if 'hea' not in wstl:
+                wstl['hea'] = {}
+            hea = wstl['hea']
+            if isinstance(data, abc.Sequence):
+                wstl['data'] = data
+            else:
+                wstl['data'] = [data]
+            if permissions:
+                hea['permissions'] = [[perm.name for perm in perms] for perms in permissions]
+            else:
+                hea['permissions'] = [[]] * len(wstl['data'])
         return await formats_from_request(request, run_time_wstl_copy, link_callback=link_callback)
 
     def find_by_target(self, val: str):
         return [tran for tran in self.__run_time_wstl['wstl']['actions'] if 'target' in tran and val in tran['target']]
 
     @property
     def design_time_document(self) -> dict[str, Any]:
```

### Comparing `heaserver-1.1.1/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.1.2/src/heaserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.1.1
+Version: 1.1.2
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.1.0
+Requires-Dist: heaobject~=1.1.1
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,14 +47,17 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.1.2
+* Added resolved permissions for desktop objects in WeSTL and Collection+JSON docs.
+
 ## Version 1.1.1
 * No longer errors out when accessing account information that the user is unauthorized to see.
 
 ## Version 1.1.0
 * AWS account objects are now populated with more information.
 * New heaobject with new APIs.
```

### Comparing `heaserver-1.1.1/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.1.2/src/heaserver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -222,24 +222,28 @@
 tests/heaserver/servicetest/representor/test_cj.py
 tests/heaserver/servicetest/representor/test_factory.py
 tests/heaserver/servicetest/representor/test_nvpjson.py
 tests/heaserver/servicetest/representor/test_supports_links.py
 tests/heaserver/servicetest/representor/test_wstljson.py
 tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
 tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
 tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
 tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
 tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
 tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
 tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
 tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
 tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
 tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
 tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
 tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
 tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
 tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
 tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
 tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
 tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
 tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
 tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
```

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.1.2/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.1.2/tests/heaserver/servicetest/componenttestcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 content1 = {
     CollectionKey(name=service.MONGODB_COMPONENT_COLLECTION): {
         '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog'
     }
 }
 
 
-def _test_case_generator(coll, fixtures, duplicate_action_name, content=None, sub=None):
+def _test_case_generator(coll, fixtures, duplicate_action_name, content=None, sub=NONE_USER):
     return get_test_case_cls_default(coll=coll, fixtures=fixtures, duplicate_action_name=duplicate_action_name,
                                      db_manager_cls=heaserver.service.testcase.mockmongo.MockMongoManager,
                                      wstl_package=service.__package__, content=content, content_type='text/plain',
                                      put_content_status=204,
                                      href='http://localhost:8080/components',
                                      get_actions=[expectedvalues.Action(name='component-get-properties',
                                                                         rel=['hea-properties']),
```

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.1.2/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.1.2/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.1.2/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.1.2/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
-            "manager_ids": [''],
-            "member_ids": [TEST_USER],
+            "manager_ids": [TEST_USER],
+            "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
             'admin_ids': []
         }
     ]}
 
 content = {
```

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,24 +36,25 @@
             'plain_list': [1, 2, 3, 4]
         }
         self.maxDiff = None
 
     async def test_formats_default(self):
         b = wstl.builder('servicetest', resource='representor/all.json')
         actual, _ = await b.represent_from_request(self.__request(), None)
-        expected = '[{"collection": {"href": "#", "version": "1.0"}}]'
+        expected = '[{"collection": {"href": "#", "permissions": [], "version": "1.0"}}]'
         self._assert_json_string_equals(expected, actual)
 
     async def test_formats_data(self):
         runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all.json')
         runtime_wstl_builder.href = 'http://localhost/test'
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection":
                           {"version": "1.0",
                            "href": "http://localhost/test",
+                           "permissions": [[]],
                            "items": [
                                {"data": [
                                    {"name": "items", "value": [], "prompt": "items", "display": true},
                                    {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                    {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                    {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                    {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -80,23 +81,96 @@
                                    {"name": "plain_list", "prompt": "plain_list", "value": [1, 2, 3, 4], "display": true}
                                    ],
                                    "links": []
                                }
                            ]}}]'''
         self._assert_json_string_equals(expected, actual)
 
+    async def test_formats_two_items_empty_permissions(self):
+        runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all.json')
+        runtime_wstl_builder.href = 'http://localhost/test'
+        actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), [self.__body, self.__body])
+        expected = '''[{"collection":
+                          {"version": "1.0",
+                           "href": "http://localhost/test",
+                           "permissions": [[], []],
+                           "items": [
+                               {"data": [
+                                   {"name": "items", "value": [], "prompt": "items", "display": true},
+                                   {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
+                                   {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
+                                   {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
+                                   {"name": "description", "value": null, "prompt": "description", "display": true},
+                                   {"name": "display_name", "value": "Reximus", "prompt": "display_name", "display": true},
+                                   {"name": "id", "value": "1", "prompt": "id", "display": false},
+                                   {"name": "invites", "value": [], "prompt": "invites", "display": true},
+                                   {"name": "modified", "value": null, "prompt": "modified", "display": true},
+                                   {"name": "name", "value": "reximus", "prompt": "name", "display": true},
+                                   {"name": "owner", "value": "system|none", "prompt": "owner", "display": true},
+                                   {"name": "shares", "value": [], "prompt": "shares", "display": true},
+                                   {"name": "source_uri", "value": null, "prompt": "source_uri", "display": true},
+                                   {"name": "type", "value": "heaobject.folder.Folder", "prompt": "type", "display": true},
+                                   {"name": "version", "value": null, "prompt": "version", "display": true},
+                                   {"section": "nested_dict", "name": "foo", "value": "oof", "prompt": "foo", "display": true},
+                                   {"section": "nested_dict", "name": "baz", "value": "zab", "prompt": "baz", "display": true},
+                                   {"section": "nested_dict", "name": "type", "value": "heaobject.registry.Component", "prompt": "type", "display": true},
+                                   {"section": "nested_list", "index": 0, "name": "foo", "value": "oof", "prompt": "foo", "display": true},
+                                   {"section": "nested_list", "index": 0, "name": "baz", "value": "zab", "prompt": "baz", "display": true},
+                                   {"section": "nested_list", "index": 0, "name": "type", "value": "heaobject.registry.Component", "prompt": "type", "display": true},
+                                   {"section": "nested_list", "index": 1, "name": "foo", "value": "oof", "prompt": "foo", "display": true},
+                                   {"section": "nested_list", "index": 1, "name": "baz", "value": "zab", "prompt": "baz", "display": true},
+                                   {"section": "nested_list", "index": 1, "name": "type", "value": "heaobject.registry.Component", "prompt": "type", "display": true},
+                                   {"name": "empty_nested_list", "prompt": "empty_nested_list", "value": [], "display": true},
+                                   {"name": "plain_list", "prompt": "plain_list", "value": [1, 2, 3, 4], "display": true}
+                                   ],
+                                   "links": []
+                               },
+                               {"data": [
+                                   {"name": "items", "value": [], "prompt": "items", "display": true},
+                                   {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
+                                   {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
+                                   {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
+                                   {"name": "description", "value": null, "prompt": "description", "display": true},
+                                   {"name": "display_name", "value": "Reximus", "prompt": "display_name", "display": true},
+                                   {"name": "id", "value": "1", "prompt": "id", "display": false},
+                                   {"name": "invites", "value": [], "prompt": "invites", "display": true},
+                                   {"name": "modified", "value": null, "prompt": "modified", "display": true},
+                                   {"name": "name", "value": "reximus", "prompt": "name", "display": true},
+                                   {"name": "owner", "value": "system|none", "prompt": "owner", "display": true},
+                                   {"name": "shares", "value": [], "prompt": "shares", "display": true},
+                                   {"name": "source_uri", "value": null, "prompt": "source_uri", "display": true},
+                                   {"name": "type", "value": "heaobject.folder.Folder", "prompt": "type", "display": true},
+                                   {"name": "version", "value": null, "prompt": "version", "display": true},
+                                   {"section": "nested_dict", "name": "foo", "value": "oof", "prompt": "foo", "display": true},
+                                   {"section": "nested_dict", "name": "baz", "value": "zab", "prompt": "baz", "display": true},
+                                   {"section": "nested_dict", "name": "type", "value": "heaobject.registry.Component", "prompt": "type", "display": true},
+                                   {"section": "nested_list", "index": 0, "name": "foo", "value": "oof", "prompt": "foo", "display": true},
+                                   {"section": "nested_list", "index": 0, "name": "baz", "value": "zab", "prompt": "baz", "display": true},
+                                   {"section": "nested_list", "index": 0, "name": "type", "value": "heaobject.registry.Component", "prompt": "type", "display": true},
+                                   {"section": "nested_list", "index": 1, "name": "foo", "value": "oof", "prompt": "foo", "display": true},
+                                   {"section": "nested_list", "index": 1, "name": "baz", "value": "zab", "prompt": "baz", "display": true},
+                                   {"section": "nested_list", "index": 1, "name": "type", "value": "heaobject.registry.Component", "prompt": "type", "display": true},
+                                   {"name": "empty_nested_list", "prompt": "empty_nested_list", "value": [], "display": true},
+                                   {"name": "plain_list", "prompt": "plain_list", "value": [1, 2, 3, 4], "display": true}
+                                   ],
+                                   "links": []
+                               }
+                           ]}}]'''
+        self._assert_json_string_equals(expected, actual)
+
     async def test_formats_data_with_item_href(self):
         runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all_cj_item_href.json')
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-open', path='foo/bar/{id}',
                                                  root='http://localhost:8080')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection":
                          {"version": "1.0",
                           "href": "http://localhost/test",
+                          "permissions": [[]],
                           "items": [
                               {"data": [
                                   {"name": "items", "value": [], "prompt": "items", "display": true},
                                   {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                   {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                   {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                   {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -134,14 +208,15 @@
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-open', path='foo/bar/{id}',
                                                  root='http://localhost:8080')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection":
                           {"version": "1.0",
                            "href": "http://localhost/test",
+                           "permissions": [[]],
                            "items": [
                                {"data": [
                                    {"name": "items", "value": [], "prompt": "items", "display": true},
                                    {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                    {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                    {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                    {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -178,14 +253,15 @@
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-open', path='foo/bar/{id}',
                                                  root='http://localhost:8080', itemif='True')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection":
                           {"version": "1.0",
                            "href": "http://localhost/test",
+                           "permissions": [[]],
                            "items": [
                                {"data": [
                                    {"name": "items", "value": [], "prompt": "items", "display": true},
                                    {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                    {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                    {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                    {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -222,14 +298,15 @@
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-open', path='/foo/bar/{id}',
                                                  root='http://localhost:8080', itemif='False')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection":
                           {"version": "1.0",
                            "href": "http://localhost/test",
+                           "permissions": [[]],
                            "items": [
                                {"data": [
                                    {"name": "items", "value": [], "prompt": "items", "display": true},
                                    {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                    {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                    {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                    {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -263,14 +340,15 @@
         runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all_cj_toplevel_link_for_item.json')
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-open', path='foo/bar', root='http://localhost:8080')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection": {
                           "version": "1.0",
                           "href": "http://localhost/test",
+                          "permissions": [[]],
                           "items": [
                               {"data": [
                                   {"name": "items", "value": [], "prompt": "items", "display": true},
                                   {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                   {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                   {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                   {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -308,14 +386,15 @@
         runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all_cj_toplevel_link_for_list.json')
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-list', path='foo/bar', root='http://localhost/test')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection": {
                                   "version": "1.0",
                                   "href": "http://localhost/test",
+                                  "permissions": [[]],
                                   "items": [
                                       {"data": [
                                           {"name": "items", "value": [], "prompt": "items", "display": true},
                                           {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                           {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                           {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                           {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -353,14 +432,15 @@
         runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all_cj_queries.json')
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-search', path='foo/bar', root='http://localhost/test')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection": {
                               "version": "1.0",
                               "href": "http://localhost/test",
+                              "permissions": [[]],
                               "items": [
                                   {"data": [
                                       {"name": "items", "value": [], "prompt": "items", "display": true},
                                       {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                       {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                       {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                       {"name": "description", "value": null, "prompt": "description", "display": true},
@@ -412,14 +492,15 @@
         runtime_wstl_builder = wstl.builder('servicetest.representor', resource='all_cj_template.json')
         runtime_wstl_builder.href = 'http://localhost/test'
         runtime_wstl_builder.add_run_time_action('data-adapter-search', path='/foo/bar', root='http://localhost/test')
         actual, _ = await runtime_wstl_builder.represent_from_request(self.__request(), self.__body)
         expected = '''[{"collection": {
                                   "version": "1.0",
                                   "href": "http://localhost/test",
+                                  "permissions": [[]],
                                   "items": [
                                       {"data": [
                                           {"name": "items", "value": [], "prompt": "items", "display": true},
                                           {"name": "created", "value": "2021-12-02T17:31:15.630000", "prompt": "created", "display": true},
                                           {"name": "derived_by_uri", "value": null, "prompt": "derived_by_uri", "display": true},
                                           {"name": "derived_from_uris", "value": [], "prompt": "derived_from_uris", "display": true},
                                           {"name": "description", "value": null, "prompt": "description", "display": true},
```

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files 23% similar despite different names*

```diff
@@ -46,24 +46,33 @@
         self._assert_json_string_equals('[{"wstl": {"hea": {"href": "http://localhost/test"}, "actions": [{"name": "data-adapter-list", "type": "safe", "target": "list", "prompt": "Data adapters", "href": "/folders/{folder_id}/items/{id}", "rel": []}]}}]', actual)
 
     async def test_formats_data_but_no_actions(self):
         wstl_builder = wstl.builder('servicetest', resource='representor/all.json')
         wstl_builder.href = 'http://localhost/test'
         actual, _ = await wstl_builder.represent_from_request(self.__request, self.__body)
         self._assert_json_string_equals(
-            '[{"wstl": {"hea": {"href": "http://localhost/test"}, "data": [{"items": [], "created": null, "derived_by_uri": null, "derived_from_uris": [], "description": null, "display_name": "Reximus", "id": null, "invites": [], "modified": null, "name": "reximus", "owner": "system|none", "shares": [], "source_uri": null, "type": "heaobject.folder.Folder", "version": null}], "actions": []}}]',
+            '[{"wstl": {"hea": {"href": "http://localhost/test", "permissions": [[]]}, "data": [{"items": [], "created": null, "derived_by_uri": null, "derived_from_uris": [], "description": null, "display_name": "Reximus", "id": null, "invites": [], "modified": null, "name": "reximus", "owner": "system|none", "shares": [], "source_uri": null, "type": "heaobject.folder.Folder", "version": null}], "actions": []}}]',
             actual)
 
     async def test_formats(self):
         wstl_builder = wstl.builder('servicetest', resource='representor/all.json')
         wstl_builder.add_run_time_action(name='data-adapter-list', path='folders/{folder_id}/items/{id}')
         wstl_builder.href = 'http://localhost/test'
         actual, _ = await wstl_builder.represent_from_request(self.__request, self.__body)
         self._assert_json_string_equals(
-            '[{"wstl": {"hea": {"href": "http://localhost/test"}, "data": [{"items": [], "created": null, "derived_by_uri": null, "derived_from_uris": [], "description": null, "display_name": "Reximus", "id": null, "invites": [], "modified": null, "name": "reximus", "owner": "system|none", "shares": [], "source_uri": null, "type": "heaobject.folder.Folder", "version": null}], "actions": [{"name": "data-adapter-list", "type": "safe", "target": "list", "prompt": "Data adapters", "href": "/folders/{folder_id}/items/{id}", "rel": []}]}}]',
+            '[{"wstl": {"hea": {"href": "http://localhost/test", "permissions": [[]]}, "data": [{"items": [], "created": null, "derived_by_uri": null, "derived_from_uris": [], "description": null, "display_name": "Reximus", "id": null, "invites": [], "modified": null, "name": "reximus", "owner": "system|none", "shares": [], "source_uri": null, "type": "heaobject.folder.Folder", "version": null}], "actions": [{"name": "data-adapter-list", "type": "safe", "target": "list", "prompt": "Data adapters", "href": "/folders/{folder_id}/items/{id}", "rel": []}]}}]',
+            actual)
+
+    async def test_formats_two_desktop_objects_empty_permissions(self):
+        wstl_builder = wstl.builder('servicetest', resource='representor/all.json')
+        wstl_builder.add_run_time_action(name='data-adapter-list', path='folders/{folder_id}/items/{id}')
+        wstl_builder.href = 'http://localhost/test'
+        actual, _ = await wstl_builder.represent_from_request(self.__request, [self.__body, self.__body])
+        self._assert_json_string_equals(
+            '[{"wstl": {"hea": {"href": "http://localhost/test", "permissions": [[], []]}, "data": [{"items": [], "created": null, "derived_by_uri": null, "derived_from_uris": [], "description": null, "display_name": "Reximus", "id": null, "invites": [], "modified": null, "name": "reximus", "owner": "system|none", "shares": [], "source_uri": null, "type": "heaobject.folder.Folder", "version": null}, {"items": [], "created": null, "derived_by_uri": null, "derived_from_uris": [], "description": null, "display_name": "Reximus", "id": null, "invites": [], "modified": null, "name": "reximus", "owner": "system|none", "shares": [], "source_uri": null, "type": "heaobject.folder.Folder", "version": null}], "actions": [{"name": "data-adapter-list", "type": "safe", "target": "list", "prompt": "Data adapters", "href": "/folders/{folder_id}/items/{id}", "rel": []}]}}]',
             actual)
 
     async def test_formats_nothing(self):
         wstl_builder = wstl.builder('servicetest', resource='representor/all.json')
         wstl_builder.href = 'http://localhost/test'
         actual, _ = await wstl_builder.represent_from_request(self.__request, None)
         self._assert_json_string_equals(
```

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.1.2/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/service.py` & `heaserver-1.1.2/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_client.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_response.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_util.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.1.2/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.1.1/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.1.2/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

