# Comparing `tmp/spaceone-identity-2.0.dev98.tar.gz` & `tmp/spaceone-identity-2.0.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-identity-2.0.dev98.tar", last modified: Sat Jan  6 23:17:15 2024, max compression
+gzip compressed data, was "spaceone-identity-2.0.dev99.tar", last modified: Sat Jan  6 23:47:59 2024, max compression
```

## Comparing `spaceone-identity-2.0.dev98.tar` & `spaceone-identity-2.0.dev99.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.099354 spaceone-identity-2.0.dev98/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-06 23:17:15.099354 spaceone-identity-2.0.dev98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 23:17:15.099354 spaceone-identity-2.0.dev98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.067354 spaceone-identity-2.0.dev98/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.067354 spaceone-identity-2.0.dev98/spaceone/identity/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.067354 spaceone-identity-2.0.dev98/spaceone/identity/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.067354 spaceone-identity-2.0.dev98/spaceone/identity/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/connector/external_auth_plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/connector/smtp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.071354 spaceone-identity-2.0.dev98/spaceone/identity/error/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_project_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_smtp.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/error/error_workspace_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.071354 spaceone-identity-2.0.dev98/spaceone/identity/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.071354 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/external_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/project_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/trusted_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/workspace_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.075354 spaceone-identity-2.0.dev98/spaceone/identity/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/lib/cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/lib/key_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.063354 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.075354 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/provider/aws.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/provider/azure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/provider/google_cloud.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.075354 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/role/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/role/domain_admin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/role/workspace_member.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/role/workspace_owner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.075354 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_secret_access_key.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_secret_assume_role.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_service_account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_trusted_account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_secret_client_secret.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_secret_subscription_id.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_service_account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_trusted_account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/email_smtp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_cloud_service_account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_cloud_trusted_account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_secret_oauth2_credentials.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_secret_project_id.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.079354 spaceone-identity-2.0.dev98/spaceone/identity/manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/app_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/client_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/domain_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/domain_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/email_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/external_auth_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/managed_resource_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.079354 spaceone-identity-2.0.dev98/spaceone/identity/manager/mfa_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/mfa_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/mfa_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/mfa_manager/email_mfa_manger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/project_group_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/project_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/provider_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/role_binding_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/role_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/service_account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/system_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/external_token_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/grant_token_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/local_token_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/mfa_token_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/trusted_account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/user_group_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/user_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/workspace_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/manager/workspace_user_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/app/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/app/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/app/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/domain/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/domain/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/domain/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/endpoint/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/endpoint/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.083354 spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/provider/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/provider/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/provider/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/role/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/schema/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/schema/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/schema/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/system/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/system/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.087354 spaceone-identity-2.0.dev98/spaceone/identity/model/token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/token/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/token/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.091354 spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.091354 spaceone-identity-2.0.dev98/spaceone/identity/model/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.091354 spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.091354 spaceone-identity-2.0.dev98/spaceone/identity/model/user_profile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/user_profile/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.091354 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.091354 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace_user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace_user/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/model/workspace_user/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.095354 spaceone-identity-2.0.dev98/spaceone/identity/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/app_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/endpoint_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/external_auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/project_group_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/provider_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/role_binding_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/role_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/schema_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15826 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/service_account_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/trusted_account_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/user_group_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/user_profile_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/workspace_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/service/workspace_user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.099354 spaceone-identity-2.0.dev98/spaceone/identity/template/
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/authentication_code_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/authentication_code_jp.html
--rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/authentication_code_ko.html
--rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    14902 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ja.html
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ko.html
--rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_user_added_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_user_added_ja.html
--rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_user_added_ko.html
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_pw_forgotten_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_pw_forgotten_ja.html
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_pw_forgotten_ko.html
--rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_user_added_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_user_added_ja.html
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_user_added_ko.html
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/verification_MFA_code_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/verification_MFA_code_jp.html
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/verification_MFA_code_ko.html
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/verification_code_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/verification_code_ja.html
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-01-06 23:17:06.000000 spaceone-identity-2.0.dev98/spaceone/identity/template/verification_code_ko.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:17:15.099354 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-06 23:17:14.000000 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-01-06 23:17:15.000000 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 23:17:14.000000 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 23:17:14.000000 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-06 23:17:14.000000 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-06 23:17:14.000000 spaceone-identity-2.0.dev98/spaceone_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.979731 spaceone-identity-2.0.dev99/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-06 23:47:59.975731 spaceone-identity-2.0.dev99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 23:47:59.979731 spaceone-identity-2.0.dev99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.943731 spaceone-identity-2.0.dev99/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.943731 spaceone-identity-2.0.dev99/spaceone/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.943731 spaceone-identity-2.0.dev99/spaceone/identity/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.943731 spaceone-identity-2.0.dev99/spaceone/identity/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/connector/external_auth_plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/connector/smtp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.947731 spaceone-identity-2.0.dev99/spaceone/identity/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_project_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_smtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/error/error_workspace_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.947731 spaceone-identity-2.0.dev99/spaceone/identity/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.951731 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/project_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/trusted_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/workspace_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.951731 spaceone-identity-2.0.dev99/spaceone/identity/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/lib/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/lib/key_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.939731 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.951731 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/provider/aws.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/provider/azure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/provider/google_cloud.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.951731 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/role/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/role/domain_admin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/role/workspace_member.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/role/workspace_owner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.955731 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_secret_access_key.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_secret_assume_role.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_service_account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_trusted_account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_secret_client_secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_secret_subscription_id.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_service_account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_trusted_account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/email_smtp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_cloud_service_account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_cloud_trusted_account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_secret_oauth2_credentials.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_secret_project_id.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/app_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/client_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/domain_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/domain_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/email_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/external_auth_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/managed_resource_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/manager/mfa_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/mfa_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/mfa_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/mfa_manager/email_mfa_manger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/project_group_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/provider_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/role_binding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/role_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/service_account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/system_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/external_token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/grant_token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/local_token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/mfa_token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/trusted_account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/user_group_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/user_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/workspace_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/manager/workspace_user_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/model/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/app/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/app/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/app/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/model/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/domain/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/domain/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/domain/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.959731 spaceone-identity-2.0.dev99/spaceone/identity/model/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/endpoint/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/endpoint/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/provider/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/provider/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/provider/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/role/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.963731 spaceone-identity-2.0.dev99/spaceone/identity/model/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/schema/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/schema/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/schema/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/system/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/system/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/token/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/token/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/user_profile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/user_profile/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.967731 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.971731 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace_user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace_user/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/model/workspace_user/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.971731 spaceone-identity-2.0.dev99/spaceone/identity/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/endpoint_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/external_auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/project_group_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/provider_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/role_binding_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/role_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/schema_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15826 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/service_account_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/trusted_account_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/user_group_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/user_profile_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/workspace_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/service/workspace_user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.975731 spaceone-identity-2.0.dev99/spaceone/identity/template/
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/authentication_code_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/authentication_code_jp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/authentication_code_ko.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14902 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ja.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ko.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14448 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_user_added_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_user_added_ja.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_user_added_ko.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_pw_forgotten_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_pw_forgotten_ja.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_pw_forgotten_ko.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_user_added_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_user_added_ja.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_user_added_ko.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/verification_MFA_code_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/verification_MFA_code_jp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/verification_MFA_code_ko.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/verification_code_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/verification_code_ja.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-01-06 23:47:52.000000 spaceone-identity-2.0.dev99/spaceone/identity/template/verification_code_ko.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 23:47:59.975731 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-06 23:47:59.000000 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2024-01-06 23:47:59.000000 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 23:47:59.000000 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 23:47:59.000000 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-06 23:47:59.000000 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-06 23:47:59.000000 spaceone-identity-2.0.dev99/spaceone_identity.egg-info/top_level.txt
```

### Comparing `spaceone-identity-2.0.dev98/setup.py` & `spaceone-identity-2.0.dev99/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/conf/global_conf.py` & `spaceone-identity-2.0.dev99/spaceone/identity/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/connector/external_auth_plugin_connector.py` & `spaceone-identity-2.0.dev99/spaceone/identity/connector/external_auth_plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/connector/smtp_connector.py` & `spaceone-identity-2.0.dev99/spaceone/identity/connector/smtp_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/error/error_authentication.py` & `spaceone-identity-2.0.dev99/spaceone/identity/error/error_authentication.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/error/error_mfa.py` & `spaceone-identity-2.0.dev99/spaceone/identity/error/error_mfa.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/error/error_project_group.py` & `spaceone-identity-2.0.dev99/spaceone/identity/error/error_project_group.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/error/error_role.py` & `spaceone-identity-2.0.dev99/spaceone/identity/error/error_role.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/error/error_user.py` & `spaceone-identity-2.0.dev99/spaceone/identity/error/error_user.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/__init__.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/app.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/app.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/domain.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/domain.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/endpoint.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/endpoint.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/external_auth.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/external_auth.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/project.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/project.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/project_group.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/project_group.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/provider.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/provider.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/role.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/role.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/role_binding.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/role_binding.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/schema.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/schema.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/service_account.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/service_account.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/system.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/system.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/token.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/token.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/trusted_account.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/trusted_account.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/user.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/user.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/user_group.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/user_group.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/user_profile.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/user_profile.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/workspace.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/workspace.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/interface/grpc/workspace_user.py` & `spaceone-identity-2.0.dev99/spaceone/identity/interface/grpc/workspace_user.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/lib/key_generator.py` & `spaceone-identity-2.0.dev99/spaceone/identity/lib/key_generator.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_secret_assume_role.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_secret_assume_role.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_service_account.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_service_account.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/aws_trusted_account.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/aws_trusted_account.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_secret_client_secret.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_secret_client_secret.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_service_account.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_service_account.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/azure_trusted_account.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/azure_trusted_account.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/email_smtp.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/email_smtp.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_cloud_service_account.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_cloud_service_account.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_cloud_trusted_account.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_cloud_trusted_account.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/managed_resource/schema/google_secret_oauth2_credentials.yaml` & `spaceone-identity-2.0.dev99/spaceone/identity/managed_resource/schema/google_secret_oauth2_credentials.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/app_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/app_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/client_secret_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/client_secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/config_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/domain_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/domain_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/domain_secret_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/domain_secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/email_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/email_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/external_auth_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/external_auth_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/managed_resource_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/managed_resource_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/mfa_manager/base.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/mfa_manager/base.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/mfa_manager/email_mfa_manger.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/mfa_manager/email_mfa_manger.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/project_group_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/project_group_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/project_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/project_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/provider_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/provider_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/role_binding_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/role_binding_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/role_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/role_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/schema_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/secret_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/service_account_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/service_account_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/system_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/system_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/base.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/base.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/external_token_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/external_token_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/grant_token_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/grant_token_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/local_token_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/local_token_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/token_manager/mfa_token_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/token_manager/mfa_token_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/trusted_account_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/trusted_account_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/user_group_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/user_group_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/user_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/user_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/workspace_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/workspace_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/manager/workspace_user_manager.py` & `spaceone-identity-2.0.dev99/spaceone/identity/manager/workspace_user_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/__init__.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/app/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/app/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/app/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/app/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/app/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/app/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/domain/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/domain/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/domain/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/domain/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/domain/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/domain/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/external_auth/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/external_auth/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/project/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/project/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/project/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/project/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/project/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/project/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/project_group/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/project_group/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/provider/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/provider/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/provider/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/provider/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/provider/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/provider/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/role/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/role/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/role/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/role/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/role/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/role/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/role_binding/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/role_binding/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/schema/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/schema/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/schema/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/schema/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/schema/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/schema/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/service_account/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/service_account/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/token/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/token/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/trusted_account/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/trusted_account/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user_group/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user_group/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/user_profile/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/user_profile/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/database.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/workspace/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/workspace/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/workspace_user/request.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/workspace_user/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/model/workspace_user/response.py` & `spaceone-identity-2.0.dev99/spaceone/identity/model/workspace_user/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/app_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/app_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/domain_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/domain_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             raise ERROR_DOMAIN_ADMIN_ROLE_IS_NOT_DEFINED()
 
         # create admin user
         params_admin = params.admin.dict()
         params_admin["auth_type"] = "LOCAL"
         params_admin["domain_id"] = domain_vo.domain_id
         params_admin["role_type"] = "DOMAIN_ADMIN"
+        params_admin["role_id"] = "managed-domain-admin"
         params_admin["reset_password"] = params_admin.get("reset_password", True)
         if params_admin.get("email") is None:
             params_admin["email"] = params_admin["user_id"]
 
         user_service = UserService()
         user_vo = user_service.create_user(params_admin)
```

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/endpoint_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/endpoint_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/external_auth_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/external_auth_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/project_group_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/project_group_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/project_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/project_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/provider_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/provider_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/role_binding_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/role_binding_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/role_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/role_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/schema_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/schema_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/service_account_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/service_account_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/system_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/system_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
         # create admin user
         _LOGGER.debug(f"[init] Create admin user: {params.admin.user_id}")
         params_admin = params.admin.dict()
         params_admin["auth_type"] = "LOCAL"
         params_admin["domain_id"] = root_domain_vo.domain_id
         params_admin["role_type"] = "DOMAIN_ADMIN"
+        params_admin["role_id"] = "managed-domain-admin"
         user_vo = self.user_mgr.create_user(params_admin, check_user_id=False)
 
         # create default role
         role_mgr = RoleManager()
         role_mgr.list_roles({}, root_domain_vo.domain_id)
         role_vos = self.role_manager.filter_roles(
             domain_id=root_domain_vo.domain_id, role_type="DOMAIN_ADMIN"
```

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/token_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/token_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/trusted_account_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/trusted_account_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/user_group_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/user_group_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/user_profile_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/user_profile_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/user_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/user_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/workspace_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/workspace_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/service/workspace_user_service.py` & `spaceone-identity-2.0.dev99/spaceone/identity/service/workspace_user_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/authentication_code_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/authentication_code_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/authentication_code_jp.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/authentication_code_jp.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/authentication_code_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/authentication_code_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ja.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ja.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_pw_forgotten_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_user_added_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_user_added_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_user_added_ja.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_user_added_ja.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/reset_pwd_link_when_user_added_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/reset_pwd_link_when_user_added_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_pw_forgotten_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_pw_forgotten_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_pw_forgotten_ja.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_pw_forgotten_ja.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_pw_forgotten_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_pw_forgotten_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_user_added_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_user_added_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_user_added_ja.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_user_added_ja.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/temp_pwd_when_user_added_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/temp_pwd_when_user_added_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/verification_MFA_code_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/verification_MFA_code_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/verification_MFA_code_jp.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/verification_MFA_code_jp.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/verification_MFA_code_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/verification_MFA_code_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/verification_code_en.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/verification_code_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/verification_code_ja.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/verification_code_ja.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone/identity/template/verification_code_ko.html` & `spaceone-identity-2.0.dev99/spaceone/identity/template/verification_code_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-identity-2.0.dev98/spaceone_identity.egg-info/SOURCES.txt` & `spaceone-identity-2.0.dev99/spaceone_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

