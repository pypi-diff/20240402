# Comparing `tmp/data_horizon-0.1.1.tar.gz` & `tmp/data_horizon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_horizon-0.1.1.tar", max compression
+gzip compressed data, was "data_horizon-0.1.2.tar", max compression
```

## Comparing `data_horizon-0.1.1.tar` & `data_horizon-0.1.2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0    11426 2024-03-27 13:27:20.941036 data_horizon-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2842 2024-03-27 13:27:59.020617 data_horizon-0.1.1/README.rst
--rw-r--r--   0        0        0      530 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/__init__.py
--rw-r--r--   0        0        0     2540 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/__init__.py
--rwxr-xr-x   0        0        0      815 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/__main__.py
--rw-r--r--   0        0        0      680 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/alembic.ini
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/__init__.py
--rw-r--r--   0        0        0     4168 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/handlers.py
--rw-r--r--   0        0        0      362 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/monitoring.py
--rw-r--r--   0        0        0      372 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/router.py
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/__init__.py
--rw-r--r--   0        0        0      997 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/__init__.py
--rw-r--r--   0        0        0     1252 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/auth.py
--rw-r--r--   0        0        0     6412 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/hwm.py
--rw-r--r--   0        0        0      975 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/hwm_history.py
--rw-r--r--   0        0        0     1029 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/namespace_history.py
--rw-r--r--   0        0        0     4183 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/namespaces.py
--rw-r--r--   0        0        0     3650 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/permission.py
--rw-r--r--   0        0        0      811 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/api/v1/router/users.py
--rw-r--r--   0        0        0     6148 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/.DS_Store
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/__init__.py
--rw-r--r--   0        0        0      669 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/factory.py
--rw-r--r--   0        0        0       58 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/README
--rwxr-xr-x   0        0        0      885 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/__main__.py
--rw-r--r--   0        0        0     2360 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/env.py
--rw-r--r--   0        0        0      510 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/script.py.mako
--rw-r--r--   0        0        0        0 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/.keep
--rw-r--r--   0        0        0     1498 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py
--rw-r--r--   0        0        0     1723 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py
--rw-r--r--   0        0        0     2283 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py
--rw-r--r--   0        0        0     2302 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py
--rw-r--r--   0        0        0     1684 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py
--rw-r--r--   0        0        0     1375 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py
--rw-r--r--   0        0        0     1877 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py
--rw-r--r--   0        0        0      670 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py
--rw-r--r--   0        0        0     2345 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py
--rw-r--r--   0        0        0     1799 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py
--rw-r--r--   0        0        0     2564 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py
--rw-r--r--   0        0        0      599 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/mixins/__init__.py
--rw-r--r--   0        0        0     1091 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/mixins/changed_by.py
--rw-r--r--   0        0        0      634 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/mixins/timestamp.py
--rw-r--r--   0        0        0      595 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/models/__init__.py
--rw-r--r--   0        0        0     1044 2024-03-27 13:27:20.945036 data_horizon-0.1.1/horizon/backend/db/models/base.py
--rw-r--r--   0        0        0     1112 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/credentials_cache.py
--rw-r--r--   0        0        0     1380 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/hwm.py
--rw-r--r--   0        0        0     1266 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/hwm_history.py
--rw-r--r--   0        0        0     1223 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/namespace.py
--rw-r--r--   0        0        0     1174 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/namespace_history.py
--rw-r--r--   0        0        0      723 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/namespace_user.py
--rw-r--r--   0        0        0      758 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/models/user.py
--rw-r--r--   0        0        0      554 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/__init__.py
--rw-r--r--   0        0        0     3797 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/base.py
--rw-r--r--   0        0        0      915 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/credentials_cache.py
--rw-r--r--   0        0        0     5178 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/hwm.py
--rw-r--r--   0        0        0     1312 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/hwm_history.py
--rw-r--r--   0        0        0     6275 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/namespace.py
--rw-r--r--   0        0        0     1102 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/namespace_history.py
--rw-r--r--   0        0        0     1509 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/db/repositories/user.py
--rw-r--r--   0        0        0      151 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/dependencies/__init__.py
--rw-r--r--   0        0        0     1636 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/dependencies/stub.py
--rwxr-xr-x   0        0        0      482 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/export_openapi_schema.py
--rw-r--r--   0        0        0     1555 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/__init__.py
--rw-r--r--   0        0        0     1600 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/application_version.py
--rw-r--r--   0        0        0      522 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/cors.py
--rw-r--r--   0        0        0      752 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/logging.py
--rw-r--r--   0        0        0      303 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/monitoring/__init__.py
--rw-r--r--   0        0        0     1337 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/monitoring/metrics.py
--rw-r--r--   0        0        0     2912 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/monitoring/stats.py
--rw-r--r--   0        0        0     4252 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/openapi.py
--rw-r--r--   0        0        0      629 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/request_id.py
--rw-r--r--   0        0        0      633 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/middlewares/static_files.py
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/providers/__init__.py
--rw-r--r--   0        0        0      160 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/providers/auth/__init__.py
--rw-r--r--   0        0        0     3119 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/providers/auth/base.py
--rw-r--r--   0        0        0     5817 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/providers/auth/cached_ldap.py
--rw-r--r--   0        0        0     3791 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/providers/auth/dummy.py
--rw-r--r--   0        0        0    10594 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/providers/auth/ldap.py
--rwxr-xr-x   0        0        0     2906 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/scripts/manage_admins.py
--rw-r--r--   0        0        0      215 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/services/__init__.py
--rw-r--r--   0        0        0      654 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/services/current_user.py
--rw-r--r--   0        0        0     1241 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/services/uow.py
--rw-r--r--   0        0        0     2136 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/__init__.py
--rw-r--r--   0        0        0     1078 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/auth/__init__.py
--rw-r--r--   0        0        0     2758 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/auth/cached_ldap.py
--rw-r--r--   0        0        0      567 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/auth/dummy.py
--rw-r--r--   0        0        0     1166 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/auth/jwt.py
--rw-r--r--   0        0        0     7103 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/auth/ldap.py
--rw-r--r--   0        0        0     1133 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/database.py
--rw-r--r--   0        0        0     2678 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/__init__.py
--rw-r--r--   0        0        0      704 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/application_version.py
--rw-r--r--   0        0        0     2102 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/cors.py
--rw-r--r--   0        0        0     2862 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/log/__init__.py
--rw-r--r--   0        0        0      924 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/log/colored.yml
--rw-r--r--   0        0        0      867 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/log/json.yml
--rw-r--r--   0        0        0      905 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/log/plain.yml
--rw-r--r--   0        0        0     2203 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/monitoring.py
--rw-r--r--   0        0        0     4495 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/openapi.py
--rw-r--r--   0        0        0     1048 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/request_id.py
--rw-r--r--   0        0        0     1025 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/settings/server/static_files.py
--rw-r--r--   0        0        0        0 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/static/.gitkeep
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/utils/__init__.py
--rw-r--r--   0        0        0      827 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/utils/jwt.py
--rw-r--r--   0        0        0      343 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/backend/utils/slug.py
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/__init__.py
--rw-r--r--   0        0        0      335 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/auth/__init__.py
--rw-r--r--   0        0        0     1743 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/auth/access_token.py
--rw-r--r--   0        0        0      795 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/auth/base.py
--rw-r--r--   0        0        0     1381 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/auth/login_password.py
--rw-r--r--   0        0        0     6433 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/base.py
--rw-r--r--   0        0        0    34597 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/client/sync.py
--rw-r--r--   0        0        0       99 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/__init__.py
--rw-r--r--   0        0        0      244 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/dto/__init__.py
--rw-r--r--   0        0        0     1003 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/dto/pagination.py
--rw-r--r--   0        0        0      583 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/dto/unset.py
--rw-r--r--   0        0        0      480 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/__init__.py
--rw-r--r--   0        0        0      729 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/base.py
--rw-r--r--   0        0        0     2261 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/registration.py
--rw-r--r--   0        0        0      700 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/__init__.py
--rw-r--r--   0        0        0      982 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/already_exists.py
--rw-r--r--   0        0        0      525 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/bad_request.py
--rw-r--r--   0        0        0     1203 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/invalid_request.py
--rw-r--r--   0        0        0      753 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/not_authorized.py
--rw-r--r--   0        0        0      939 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/not_found.py
--rw-r--r--   0        0        0      927 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/errors/schemas/permission_denied.py
--rw-r--r--   0        0        0      724 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/exceptions/__init__.py
--rw-r--r--   0        0        0      832 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/exceptions/auth.py
--rw-r--r--   0        0        0     1016 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/exceptions/bad_request.py
--rw-r--r--   0        0        0      550 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/exceptions/base.py
--rw-r--r--   0        0        0     2346 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/exceptions/entity.py
--rw-r--r--   0        0        0     1300 2024-03-27 13:27:20.949036 data_horizon-0.1.1/horizon/commons/exceptions/permission.py
--rw-r--r--   0        0        0      760 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/exceptions/service.py
--rw-r--r--   0        0        0      189 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/__init__.py
--rw-r--r--   0        0        0      293 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/ping.py
--rw-r--r--   0        0        0     1929 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/__init__.py
--rw-r--r--   0        0        0      305 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/auth.py
--rw-r--r--   0        0        0     4502 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/hwm.py
--rw-r--r--   0        0        0     1633 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/hwm_history.py
--rw-r--r--   0        0        0     2271 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/namespace.py
--rw-r--r--   0        0        0     1304 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/namespace_history.py
--rw-r--r--   0        0        0     1990 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/pagination.py
--rw-r--r--   0        0        0     2110 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/permission.py
--rw-r--r--   0        0        0      703 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/commons/schemas/v1/user.py
--rw-r--r--   0        0        0        0 2024-03-27 13:27:20.953036 data_horizon-0.1.1/horizon/py.typed
--rw-r--r--   0        0        0    14923 2024-03-27 13:27:20.953036 data_horizon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7288 1970-01-01 00:00:00.000000 data_horizon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11426 2024-04-02 09:28:21.174010 data_horizon-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2843 2024-04-02 09:28:50.678362 data_horizon-0.1.2/README.rst
+-rw-r--r--   0        0        0      530 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/__init__.py
+-rw-r--r--   0        0        0     2540 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/__init__.py
+-rwxr-xr-x   0        0        0      815 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/__main__.py
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/__init__.py
+-rw-r--r--   0        0        0     4168 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/handlers.py
+-rw-r--r--   0        0        0      362 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/monitoring.py
+-rw-r--r--   0        0        0      372 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/router.py
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/__init__.py
+-rw-r--r--   0        0        0     1252 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/auth.py
+-rw-r--r--   0        0        0     6454 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/hwm.py
+-rw-r--r--   0        0        0      975 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/hwm_history.py
+-rw-r--r--   0        0        0     1029 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/namespace_history.py
+-rw-r--r--   0        0        0     4226 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/namespaces.py
+-rw-r--r--   0        0        0     3650 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/permission.py
+-rw-r--r--   0        0        0      854 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/users.py
+-rw-r--r--   0        0        0     6148 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/db/.DS_Store
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/db/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/db/factory.py
+-rw-r--r--   0        0        0       58 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/README
+-rwxr-xr-x   0        0        0      868 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/__main__.py
+-rw-r--r--   0        0        0      673 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/alembic.ini
+-rw-r--r--   0        0        0     2360 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/env.py
+-rw-r--r--   0        0        0      510 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/.keep
+-rw-r--r--   0        0        0     1498 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py
+-rw-r--r--   0        0        0     1723 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py
+-rw-r--r--   0        0        0     2283 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py
+-rw-r--r--   0        0        0     2302 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py
+-rw-r--r--   0        0        0     1684 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py
+-rw-r--r--   0        0        0     1375 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py
+-rw-r--r--   0        0        0     1877 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py
+-rw-r--r--   0        0        0      670 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py
+-rw-r--r--   0        0        0     2345 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py
+-rw-r--r--   0        0        0     1799 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py
+-rw-r--r--   0        0        0     2564 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py
+-rw-r--r--   0        0        0      599 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/mixins/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/mixins/changed_by.py
+-rw-r--r--   0        0        0      634 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/mixins/timestamp.py
+-rw-r--r--   0        0        0      595 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/__init__.py
+-rw-r--r--   0        0        0     1044 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/base.py
+-rw-r--r--   0        0        0     1112 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/credentials_cache.py
+-rw-r--r--   0        0        0     1380 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/hwm.py
+-rw-r--r--   0        0        0     1266 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/hwm_history.py
+-rw-r--r--   0        0        0     1223 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/namespace.py
+-rw-r--r--   0        0        0     1174 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/namespace_history.py
+-rw-r--r--   0        0        0      723 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/namespace_user.py
+-rw-r--r--   0        0        0      758 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/user.py
+-rw-r--r--   0        0        0      554 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/__init__.py
+-rw-r--r--   0        0        0     3797 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/base.py
+-rw-r--r--   0        0        0      915 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/credentials_cache.py
+-rw-r--r--   0        0        0     5178 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/hwm.py
+-rw-r--r--   0        0        0     1312 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/hwm_history.py
+-rw-r--r--   0        0        0     6275 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/namespace.py
+-rw-r--r--   0        0        0     1102 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/namespace_history.py
+-rw-r--r--   0        0        0     1509 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/user.py
+-rw-r--r--   0        0        0      151 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/dependencies/__init__.py
+-rw-r--r--   0        0        0     1636 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/dependencies/stub.py
+-rwxr-xr-x   0        0        0      482 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/export_openapi_schema.py
+-rw-r--r--   0        0        0     1555 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/__init__.py
+-rw-r--r--   0        0        0     1600 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/application_version.py
+-rw-r--r--   0        0        0      522 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/cors.py
+-rw-r--r--   0        0        0      752 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/logging.py
+-rw-r--r--   0        0        0      303 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/monitoring/__init__.py
+-rw-r--r--   0        0        0     1337 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/monitoring/metrics.py
+-rw-r--r--   0        0        0     2912 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/monitoring/stats.py
+-rw-r--r--   0        0        0     4252 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/openapi.py
+-rw-r--r--   0        0        0      629 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/request_id.py
+-rw-r--r--   0        0        0      633 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/static_files.py
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/__init__.py
+-rw-r--r--   0        0        0     3119 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/base.py
+-rw-r--r--   0        0        0     5817 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/cached_ldap.py
+-rw-r--r--   0        0        0     3791 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/dummy.py
+-rw-r--r--   0        0        0    10594 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/ldap.py
+-rwxr-xr-x   0        0        0     3656 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/scripts/manage_admins.py
+-rw-r--r--   0        0        0      215 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/services/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/services/current_user.py
+-rw-r--r--   0        0        0     1241 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/services/uow.py
+-rw-r--r--   0        0        0     2136 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/cached_ldap.py
+-rw-r--r--   0        0        0      567 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/dummy.py
+-rw-r--r--   0        0        0     1166 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/jwt.py
+-rw-r--r--   0        0        0     7103 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/ldap.py
+-rw-r--r--   0        0        0     1133 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/database.py
+-rw-r--r--   0        0        0     2678 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/application_version.py
+-rw-r--r--   0        0        0     2102 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/cors.py
+-rw-r--r--   0        0        0     2862 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/__init__.py
+-rw-r--r--   0        0        0      924 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/colored.yml
+-rw-r--r--   0        0        0      867 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/json.yml
+-rw-r--r--   0        0        0      909 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/plain.yml
+-rw-r--r--   0        0        0     2203 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/monitoring.py
+-rw-r--r--   0        0        0     4495 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/openapi.py
+-rw-r--r--   0        0        0     1048 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/request_id.py
+-rw-r--r--   0        0        0     1025 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/static/.gitkeep
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/utils/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/utils/jwt.py
+-rw-r--r--   0        0        0      343 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/utils/slug.py
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/access_token.py
+-rw-r--r--   0        0        0      795 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/base.py
+-rw-r--r--   0        0        0     1381 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/login_password.py
+-rw-r--r--   0        0        0     6593 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/base.py
+-rw-r--r--   0        0        0    34597 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/client/sync.py
+-rw-r--r--   0        0        0       99 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/dto/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/dto/pagination.py
+-rw-r--r--   0        0        0      583 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/dto/unset.py
+-rw-r--r--   0        0        0      480 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/__init__.py
+-rw-r--r--   0        0        0      860 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/base.py
+-rw-r--r--   0        0        0     2261 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/registration.py
+-rw-r--r--   0        0        0      730 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/__init__.py
+-rw-r--r--   0        0        0      982 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/already_exists.py
+-rw-r--r--   0        0        0      525 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/bad_request.py
+-rw-r--r--   0        0        0     1217 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/invalid_request.py
+-rw-r--r--   0        0        0      753 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/not_authorized.py
+-rw-r--r--   0        0        0      939 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/not_found.py
+-rw-r--r--   0        0        0      927 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/permission_denied.py
+-rw-r--r--   0        0        0      724 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/auth.py
+-rw-r--r--   0        0        0     1016 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/bad_request.py
+-rw-r--r--   0        0        0      550 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/base.py
+-rw-r--r--   0        0        0     2346 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/entity.py
+-rw-r--r--   0        0        0     1300 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/permission.py
+-rw-r--r--   0        0        0      760 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/service.py
+-rw-r--r--   0        0        0      189 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/ping.py
+-rw-r--r--   0        0        0     1929 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/auth.py
+-rw-r--r--   0        0        0     4589 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/hwm.py
+-rw-r--r--   0        0        0     1700 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/hwm_history.py
+-rw-r--r--   0        0        0     2358 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/namespace.py
+-rw-r--r--   0        0        0     1371 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/namespace_history.py
+-rw-r--r--   0        0        0     2174 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/pagination.py
+-rw-r--r--   0        0        0     2209 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/permission.py
+-rw-r--r--   0        0        0      770 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/user.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/py.typed
+-rw-r--r--   0        0        0    14954 2024-04-02 09:28:21.186010 data_horizon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 data_horizon-0.1.2/PKG-INFO
```

### Comparing `data_horizon-0.1.1/LICENSE.txt` & `data_horizon-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/README.rst` & `data_horizon-0.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :target: https://codecov.io/gh/MobileTeleSystems/horizon
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/horizon/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/horizon/develop
 
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/1c0cce8a785056c5462e124793bd67075287d9ed/docs/_static/logo.svg
+.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/8367012cc94e07439ad04cac1fa30644b0567934/docs/_static/logo.svg
     :width: 400
     :alt: Horizon logo
     :target: https://github.com/MobileTeleSystems/horizon/
 
 What is Horizon?
 ----------------
 
@@ -43,15 +43,15 @@
 
 Goals
 -----
 
 * Allow users to save and fetch High Water Mark (*HWM*) items. These are ``name+type+value`` triples with few optional fields.
 * Avoid confusion between different user's data by separating HWMs to different *namespaces*. Each HWM is bound to namespace.
 * Allow users to get HWM change history, to determine who and when changed a specific HWM value and other fields.
-* Provide RBAC model to ensure that interaction with ``HWMs`` and ``Namespaces`` are governed by role assigned to each user. Role are assigned per namespace.
+* Provide RBAC model to ensure that interaction with ``HWMs`` and ``Namespaces`` are governed by role assigned to each user. Roles are assigned per namespace.
 
 Non-goals
 ---------
 
 * This is not a *data* storage, it is not designed to store raw table rows. It is designed to store only HWM values.
 * Attaching machine-readable metadata for HWMs (like ``process``, ``origin``) is not supported. This should be stored somewhere else.
```

### Comparing `data_horizon-0.1.1/horizon/__init__.py` & `data_horizon-0.1.2/horizon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
 # _raw_version could contain pre-release version, like 0.0.1dev123
 # value is updated automatically by `poetry version ...` and poetry-bumpversion plugin
-_raw_version = "0.1.1"
+_raw_version = "0.1.2"
 
 # version always contain only release number like 0.0.1
 __version__ = ".".join(_raw_version.split(".")[:3])  # noqa: WPS410
 
 # version tuple always contains only integer parts, like (0, 0, 1)
 __version_tuple__ = tuple(map(int, __version__.split(".")))
```

### Comparing `data_horizon-0.1.1/horizon/backend/__init__.py` & `data_horizon-0.1.2/horizon/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/__main__.py` & `data_horizon-0.1.2/horizon/backend/__main__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/alembic.ini` & `data_horizon-0.1.2/horizon/backend/db/migrations/alembic.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [alembic]
-script_location = %(here)s/db/migrations
+script_location = %(here)s
 file_template = %%(year)d-%%(month).2d-%%(day).2d_%%(rev)s_%%(slug)s
-prepend_sys_path = %(here)s/../..
+prepend_sys_path = %(here)s/../../../../
 version_path_separator = os
 
 [post_write_hooks]
 
 [loggers]
 keys = root,sqlalchemy,alembic
```

### Comparing `data_horizon-0.1.1/horizon/backend/api/handlers.py` & `data_horizon-0.1.2/horizon/backend/api/handlers.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/__init__.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/auth.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/auth.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/hwm.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/hwm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
+# mypy: disable-error-code="pydantic-orm"
 
 from fastapi import APIRouter, Depends, status
 from typing_extensions import Annotated
 
 from horizon.backend.db.models import NamespaceUserRoleInt, User
 from horizon.backend.services import UnitOfWork, current_user
 from horizon.commons.errors import get_error_responses
```

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/hwm_history.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/namespace_history.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/namespaces.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/namespaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
+# mypy: disable-error-code="pydantic-orm"
+
 from fastapi import APIRouter, Depends, HTTPException, status
 from typing_extensions import Annotated
 
 from horizon.backend.db.models import NamespaceUserRoleInt, User
 from horizon.backend.services import UnitOfWork, current_user
 from horizon.commons.errors import get_error_responses
 from horizon.commons.schemas.v1 import (
```

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/permission.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/api/v1/router/users.py` & `data_horizon-0.1.2/horizon/backend/api/v1/router/users.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
+# mypy: disable-error-code="pydantic-orm"
+
 from typing import Union
 
 from fastapi import APIRouter, Depends
 from typing_extensions import Annotated
 
 from horizon.backend.db.models import User
 from horizon.backend.services import current_user
```

### Comparing `data_horizon-0.1.1/horizon/backend/db/.DS_Store` & `data_horizon-0.1.2/horizon/backend/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/factory.py` & `data_horizon-0.1.2/horizon/backend/db/factory.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/__main__.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/bin/env python3
 
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
+
+from __future__ import annotations
+
 import os
 import sys
 from pathlib import Path
-from typing import List, Optional
 
 from alembic.config import CommandLine
 
 here = Path(__file__).resolve()
-config_path = here.parent.parent.parent / "alembic.ini"
+config_path = here.parent / "alembic.ini"
 
 
-def main(prog_name: Optional[str] = None, args: Optional[List[str]] = None):
+def main(prog_name: str | None = None, args: list[str] | None = None):
     """Run alembic and pass the command line arguments to it."""
     if args is None:
         args = sys.argv.copy()
         prog_name = args.pop(0)
 
     if not prog_name:
         prog_name = os.fspath(here)
```

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/env.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py` & `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/mixins/changed_by.py` & `data_horizon-0.1.2/horizon/backend/db/mixins/changed_by.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/mixins/timestamp.py` & `data_horizon-0.1.2/horizon/backend/db/mixins/timestamp.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/__init__.py` & `data_horizon-0.1.2/horizon/backend/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/base.py` & `data_horizon-0.1.2/horizon/backend/db/models/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/credentials_cache.py` & `data_horizon-0.1.2/horizon/backend/db/models/credentials_cache.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/hwm.py` & `data_horizon-0.1.2/horizon/backend/db/models/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/hwm_history.py` & `data_horizon-0.1.2/horizon/backend/db/models/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/namespace.py` & `data_horizon-0.1.2/horizon/backend/db/models/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/namespace_history.py` & `data_horizon-0.1.2/horizon/backend/db/models/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/namespace_user.py` & `data_horizon-0.1.2/horizon/backend/db/models/namespace_user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/models/user.py` & `data_horizon-0.1.2/horizon/backend/db/models/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/__init__.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/base.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/credentials_cache.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/credentials_cache.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/hwm.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/hwm_history.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/namespace.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/namespace_history.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/db/repositories/user.py` & `data_horizon-0.1.2/horizon/backend/db/repositories/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/dependencies/stub.py` & `data_horizon-0.1.2/horizon/backend/dependencies/stub.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/__init__.py` & `data_horizon-0.1.2/horizon/backend/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/application_version.py` & `data_horizon-0.1.2/horizon/backend/middlewares/application_version.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/cors.py` & `data_horizon-0.1.2/horizon/backend/middlewares/cors.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/logging.py` & `data_horizon-0.1.2/horizon/backend/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/monitoring/metrics.py` & `data_horizon-0.1.2/horizon/backend/middlewares/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/monitoring/stats.py` & `data_horizon-0.1.2/horizon/backend/middlewares/monitoring/stats.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/openapi.py` & `data_horizon-0.1.2/horizon/backend/middlewares/openapi.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/request_id.py` & `data_horizon-0.1.2/horizon/backend/middlewares/request_id.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/middlewares/static_files.py` & `data_horizon-0.1.2/horizon/backend/middlewares/static_files.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/providers/auth/base.py` & `data_horizon-0.1.2/horizon/backend/providers/auth/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/providers/auth/cached_ldap.py` & `data_horizon-0.1.2/horizon/backend/providers/auth/cached_ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/providers/auth/dummy.py` & `data_horizon-0.1.2/horizon/backend/providers/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/providers/auth/ldap.py` & `data_horizon-0.1.2/horizon/backend/providers/auth/ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/services/current_user.py` & `data_horizon-0.1.2/horizon/backend/services/current_user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/services/uow.py` & `data_horizon-0.1.2/horizon/backend/services/uow.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/__init__.py` & `data_horizon-0.1.2/horizon/backend/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/auth/__init__.py` & `data_horizon-0.1.2/horizon/backend/settings/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/auth/cached_ldap.py` & `data_horizon-0.1.2/horizon/backend/settings/auth/cached_ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/auth/dummy.py` & `data_horizon-0.1.2/horizon/backend/settings/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/auth/jwt.py` & `data_horizon-0.1.2/horizon/backend/settings/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/auth/ldap.py` & `data_horizon-0.1.2/horizon/backend/settings/auth/ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/database.py` & `data_horizon-0.1.2/horizon/backend/settings/database.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/__init__.py` & `data_horizon-0.1.2/horizon/backend/settings/server/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/application_version.py` & `data_horizon-0.1.2/horizon/backend/settings/server/application_version.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/cors.py` & `data_horizon-0.1.2/horizon/backend/settings/server/cors.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/log/__init__.py` & `data_horizon-0.1.2/horizon/backend/settings/server/log/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/log/colored.yml` & `data_horizon-0.1.2/horizon/backend/settings/server/log/colored.yml`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/log/json.yml` & `data_horizon-0.1.2/horizon/backend/settings/server/log/json.yml`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/log/plain.yml` & `data_horizon-0.1.2/horizon/backend/settings/server/log/plain.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   correlation_id:
     (): asgi_correlation_id.CorrelationIdFilter
     uuid_length: 32
     default_value: '-'
 
 formatters:
   plain:
-    (): log.Formatter
+    (): logging.Formatter
     # Add correlation_id to log records
     fmt: '%(asctime)s.%(msecs)03d %(name)s:%(lineno)d [%(levelname)s] %(correlation_id)s %(message)s'
     datefmt: '%Y-%m-%d %H:%M:%S'
 
 handlers:
   main:
     class: logging.StreamHandler
```

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/monitoring.py` & `data_horizon-0.1.2/horizon/backend/settings/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/openapi.py` & `data_horizon-0.1.2/horizon/backend/settings/server/openapi.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/request_id.py` & `data_horizon-0.1.2/horizon/backend/settings/server/request_id.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/settings/server/static_files.py` & `data_horizon-0.1.2/horizon/backend/settings/server/static_files.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/backend/utils/jwt.py` & `data_horizon-0.1.2/horizon/backend/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/client/auth/access_token.py` & `data_horizon-0.1.2/horizon/client/auth/access_token.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/client/auth/base.py` & `data_horizon-0.1.2/horizon/client/auth/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/client/auth/login_password.py` & `data_horizon-0.1.2/horizon/client/auth/login_password.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/client/base.py` & `data_horizon-0.1.2/horizon/client/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 import warnings
 from typing import Any, Generic, Optional, Tuple, TypeVar
 from urllib.parse import urlparse
 
 from pydantic import AnyHttpUrl, BaseModel, PrivateAttr, ValidationError
 from pydantic import __version__ as pydantic_version
 from pydantic import parse_obj_as, validator
-from pydantic.generics import GenericModel
+
+if pydantic_version >= "2":
+    from pydantic import BaseModel as GenericModel
+else:
+    from pydantic.generics import GenericModel  # type: ignore[no-redef] # noqa: WPS440
 from typing_extensions import Protocol
 
 import horizon
 from horizon.client.auth.base import BaseAuth
 from horizon.commons.errors import get_response_for_status_code
 from horizon.commons.errors.base import APIErrorSchema
 
@@ -54,17 +58,17 @@
 
     class Config:
         arbitrary_types_allowed = True
 
     @classmethod
     def session_class(cls) -> type[SessionClass]:
         # Get `Session` from `SyncClient(BaseClient[Session])`
-        if pydantic_version < "2":
-            return cls.__bases__[0].__annotations__["session"].__args__[0]
-        return cls.model_fields["session"].annotation.__args__[0]
+        if pydantic_version >= "2":
+            return cls.model_fields["session"].annotation.__args__[0]  # type: ignore[union-attr]
+        return cls.__bases__[0].__annotations__["session"].__args__[0]
 
     @validator("base_url")
     def _validate_url(cls, value: AnyHttpUrl):
         """``http://localhost:8000/`` -> ``http://localhost:8000``"""
         if value.path:
             return urlparse(str(value))._replace(path=value.path.rstrip("/")).geturl()  # noqa: WPS437
         return value
```

### Comparing `data_horizon-0.1.1/horizon/client/sync.py` & `data_horizon-0.1.2/horizon/client/sync.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/dto/pagination.py` & `data_horizon-0.1.2/horizon/commons/dto/pagination.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/dto/unset.py` & `data_horizon-0.1.2/horizon/commons/dto/unset.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/errors/base.py` & `data_horizon-0.1.2/horizon/commons/errors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Any, Generic, TypeVar
 
 from pydantic import BaseModel
 from pydantic import __version__ as pydantic_version
-from pydantic.generics import GenericModel
+
+if pydantic_version >= "2":
+    from pydantic import BaseModel as GenericModel
+else:
+    from pydantic.generics import GenericModel  # type: ignore[no-redef] # noqa: WPS440
 
 from horizon.commons.dto.unset import Unset
 
 
 class BaseErrorSchema(BaseModel):
     code: str
     message: str
```

### Comparing `data_horizon-0.1.1/horizon/commons/errors/registration.py` & `data_horizon-0.1.2/horizon/commons/errors/registration.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/__init__.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 
 __all__ = [
     "AlreadyExistsSchema",
     "InvalidRequestSchema",
     "NotAuthorizedSchema",
     "NotFoundSchema",
     "BadRequestError",
+    "PermissionDeniedSchema",
 ]
```

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/already_exists.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/already_exists.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/bad_request.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/bad_request.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/invalid_request.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/invalid_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
     if pydantic_version >= "2":
         url: str
         ctx: dict = Field(default_factory=dict, alias="context")
         input: Any = Field(default=None)
 
     class Config:
-        # pydantic v1
-        allow_population_by_field_name = True
-        # pydantic v2
-        populate_by_name = True
+        if pydantic_version >= "2":
+            populate_by_name = True
+        else:
+            allow_population_by_field_name = True
 
 
 @register_error_response(
     exception=ValidationError,
     status=http.HTTPStatus.UNPROCESSABLE_ENTITY,
 )
 class InvalidRequestSchema(BaseErrorSchema):
```

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/not_authorized.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/not_authorized.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/not_found.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/not_found.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/errors/schemas/permission_denied.py` & `data_horizon-0.1.2/horizon/commons/errors/schemas/permission_denied.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/__init__.py` & `data_horizon-0.1.2/horizon/commons/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/auth.py` & `data_horizon-0.1.2/horizon/commons/exceptions/auth.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/bad_request.py` & `data_horizon-0.1.2/horizon/commons/exceptions/bad_request.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/base.py` & `data_horizon-0.1.2/horizon/commons/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/entity.py` & `data_horizon-0.1.2/horizon/commons/exceptions/entity.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/permission.py` & `data_horizon-0.1.2/horizon/commons/exceptions/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/exceptions/service.py` & `data_horizon-0.1.2/horizon/commons/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/__init__.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/hwm.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/hwm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 from datetime import datetime
 from typing import Any, List, Optional, Union
 
-from pydantic import BaseModel, Field, root_validator, validator
+from pydantic import BaseModel, Field
+from pydantic import __version__ as pydantic_version
+from pydantic import root_validator, validator
 
 from horizon.commons.dto import Unset
 from horizon.commons.schemas.v1.pagination import PaginateQueryV1
 
 MAX_NAME_LENGTH = 2048
 MAX_TYPE_LENGTH = 64
 
@@ -26,18 +28,18 @@
         default=None,
         description="Expression used to calculate HWM value. Can be any string",
     )
     changed_at: datetime = Field(description="Timestamp of last change of the HWM data")
     changed_by: Optional[str] = Field(default=None, description="Latest user who changed the HWM data")
 
     class Config:
-        # pydantic v1
-        orm_mode = True
-        # pydantic v2
-        from_attributes = True
+        if pydantic_version >= "2":
+            from_attributes = True
+        else:
+            orm_mode = True
 
 
 class HWMListResponseV1(BaseModel):
     hwms: List[HWMResponseV1]
 
 
 class HWMPaginateQueryV1(PaginateQueryV1):
```

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/hwm_history.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/hwm_history.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
 from datetime import datetime
 from typing import Any, Optional
 
 from pydantic import BaseModel, Field
+from pydantic import __version__ as pydantic_version
 
 from horizon.commons.schemas.v1.pagination import PaginateQueryV1
 
 
 class HWMHistoryPaginateQueryV1(PaginateQueryV1):
     """Query params for HWM pagination request."""
 
@@ -33,11 +34,11 @@
         description="Expression used to calculate HWM value. Can be any string",
     )
     action: str = Field(description="Action performed on the HWM record")
     changed_at: datetime = Field(description="Timestamp of a change of the HWM data")
     changed_by: Optional[str] = Field(default=None, description="User who changed the HWM data")
 
     class Config:
-        # pydantic v1
-        orm_mode = True
-        # pydantic v2
-        from_attributes = True
+        if pydantic_version >= "2":
+            from_attributes = True
+        else:
+            orm_mode = True
```

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/namespace.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/namespace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 from datetime import datetime
 from enum import Enum
 from typing import Optional, Union
 
-from pydantic import BaseModel, Field, root_validator
+from pydantic import BaseModel, Field
+from pydantic import __version__ as pydantic_version
+from pydantic import root_validator
 
 from horizon.commons.dto import Unset
 from horizon.commons.schemas.v1.pagination import PaginateQueryV1
 
 MAX_NAME_LENGTH = 256
 
 
@@ -25,18 +27,18 @@
     name: str = Field(description="Namespace name, unique in the entire database")
     description: str = Field(description="Namespace description")
     owned_by: str = Field(description="The namespace owner")
     changed_at: datetime = Field(description="Timestamp of last change of the namespace data")
     changed_by: Optional[str] = Field(default=None, description="Latest user who changed the namespace data")
 
     class Config:
-        # pydantic v1
-        orm_mode = True
-        # pydantic v2
-        from_attributes = True
+        if pydantic_version >= "2":
+            from_attributes = True
+        else:
+            orm_mode = True
 
 
 class NamespacePaginateQueryV1(PaginateQueryV1):
     """Query params for namespace pagination request."""
 
     name: Optional[str] = Field(default=None, min_length=1, max_length=MAX_NAME_LENGTH)
```

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/namespace_history.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/namespace_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel, Field
+from pydantic import __version__ as pydantic_version
 
 from horizon.commons.schemas.v1.pagination import PaginateQueryV1
 
 
 class NamespaceHistoryPaginateQueryV1(PaginateQueryV1):
     """Query params for Namespace pagination request."""
 
@@ -26,11 +27,11 @@
     description: str = Field(description="Namespace description")
     owned_by: Optional[str] = Field(default=None, description="The namespace owner")
     action: str = Field(description="Action performed on the namespace record")
     changed_at: datetime = Field(description="Timestamp of a change of the namespace data")
     changed_by: Optional[str] = Field(default=None, description="User who changed the namespace data")
 
     class Config:
-        # pydantic v1
-        orm_mode = True
-        # pydantic v2
-        from_attributes = True
+        if pydantic_version >= "2":
+            from_attributes = True
+        else:
+            orm_mode = True
```

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/pagination.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/pagination.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 from typing import Generic, List, Optional, TypeVar
 
 from pydantic import BaseModel, Field
-from pydantic.generics import GenericModel
+from pydantic import __version__ as pydantic_version
+
+if pydantic_version >= "2":
+    from pydantic import BaseModel as GenericModel
+else:
+    from pydantic.generics import GenericModel  # type: ignore[no-redef] # noqa: WPS440
 
 from horizon.commons.dto import Pagination
 
 
 class PaginateQueryV1(BaseModel):
     """Basic class with pagination query params."""
```

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/permission.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/permission.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,18 @@
 
     permissions: List[PermissionUpdateRequestItemV1] = Field(
         description="A list of modifications to the namespace's permissions."
         " Each entry specifies a user and the role they should have or be removed from.",
     )
 
     @validator("permissions")
-    def _ensure_unique_usernames_and_single_owner(cls, permissions):
+    def _ensure_unique_usernames_and_single_owner(
+        cls,
+        permissions: List[PermissionUpdateRequestItemV1],
+    ) -> List[PermissionUpdateRequestItemV1]:
         seen: Set[str] = set()
         owner_count = 0
         for perm in permissions:
             username, role = perm.username, perm.role
 
             if username in seen:
                 raise ValueError(f"Duplicate username detected: {username}. Each username must appear only once.")
```

### Comparing `data_horizon-0.1.1/horizon/commons/schemas/v1/user.py` & `data_horizon-0.1.2/horizon/commons/schemas/v1/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from pydantic import BaseModel, Field
+from pydantic import __version__ as pydantic_version
 
 
 class UserResponseV1(BaseModel):
     """User info response."""
 
     id: int = Field(description="Internal user id, not for external usage")
     username: str = Field(description="User name, unique in the entire database")
 
     class Config:
-        # pydantic v1
-        orm_mode = True
-        # pydantic v2
-        from_attributes = True
+        if pydantic_version >= "2":
+            from_attributes = True
+        else:
+            orm_mode = True
 
 
 class UserResponseV1WithAdmin(UserResponseV1):
     """Extended user info response including is_admin."""
 
     is_admin: bool = Field(description="Indicates if the user is a superadmin")
```

### Comparing `data_horizon-0.1.1/pyproject.toml` & `data_horizon-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "data-horizon"
-version = "0.1.1"
+version = "0.1.2"
 license = "Apache-2.0"
 description = "Horizon REST API + client"
 authors = ["DataOps.ETL <onetools@mts.ru>"]
 readme = "README.rst"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Pydantic",
@@ -208,15 +208,15 @@
 furo = {version = "^2024.1.29", python = ">=3.8"}
 sphinx-copybutton = {version = "^0.5.2", python = ">=3.8"}
 sphinxcontrib-towncrier = {version = "^0.4.0a0", python = ">=3.8"}
 towncrier = {version = "^23.11.0", python = ">=3.8"}
 sphinx-issues = {version = ">=3.0.1,<5.0.0", python = ">=3.8"}
 sphinx-design = {version = "^0.5.0", python = ">=3.8"}
 sphinx-favicon = {version = "^1.0.1", python = ">=3.8"}
-sphinx-argparse = {version = "^0.2.5", python = ">=3.8"}
+sphinx-argparse = {version = ">=0.2.5,<0.5.0", python = ">=3.8"}
 # uncomment after https://github.com/zqmillet/sphinx-plantuml/pull/4
 # sphinx-plantuml = {version = "^1.0.0", python = ">=3.8"}
 
 [tool.poetry.plugins."tricoder_package_spy.register"]
 "data-horizon" = "horizon"
 
 [tool.poetry_bumpversion.file."horizon/__init__.py"]
@@ -276,14 +276,15 @@
 [tool.isort]
 profile = "black"
 known_first_party = ["horizon", "tests"]
 
 [tool.mypy]
 python_version = "3.8"
 plugins = ["pydantic.mypy", "sqlalchemy.ext.mypy.plugin"]
+strict_optional = true
 
 [[tool.mypy.overrides]]
 module = "sqlalchemy_utils"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "authlib.*"
```

### Comparing `data_horizon-0.1.1/PKG-INFO` & `data_horizon-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-horizon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Horizon REST API + client
 License: Apache-2.0
 Keywords: Horizon,REST,API,HWM
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -100,15 +100,15 @@
     :target: https://codecov.io/gh/MobileTeleSystems/horizon
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/horizon/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/horizon/develop
 
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/1c0cce8a785056c5462e124793bd67075287d9ed/docs/_static/logo.svg
+.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/8367012cc94e07439ad04cac1fa30644b0567934/docs/_static/logo.svg
     :width: 400
     :alt: Horizon logo
     :target: https://github.com/MobileTeleSystems/horizon/
 
 What is Horizon?
 ----------------
 
@@ -119,15 +119,15 @@
 
 Goals
 -----
 
 * Allow users to save and fetch High Water Mark (*HWM*) items. These are ``name+type+value`` triples with few optional fields.
 * Avoid confusion between different user's data by separating HWMs to different *namespaces*. Each HWM is bound to namespace.
 * Allow users to get HWM change history, to determine who and when changed a specific HWM value and other fields.
-* Provide RBAC model to ensure that interaction with ``HWMs`` and ``Namespaces`` are governed by role assigned to each user. Role are assigned per namespace.
+* Provide RBAC model to ensure that interaction with ``HWMs`` and ``Namespaces`` are governed by role assigned to each user. Roles are assigned per namespace.
 
 Non-goals
 ---------
 
 * This is not a *data* storage, it is not designed to store raw table rows. It is designed to store only HWM values.
 * Attaching machine-readable metadata for HWMs (like ``process``, ``origin``) is not supported. This should be stored somewhere else.
```

