# Comparing `tmp/matrix_synapse-1.99.0.tar.gz` & `tmp/matrix_synapse-1.99.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix_synapse-1.99.0.tar", max compression
+gzip compressed data, was "matrix_synapse-1.99.0rc1.tar", max compression
```

## Comparing `matrix_synapse-1.99.0.tar` & `matrix_synapse-1.99.0rc1.tar`

### file list

```diff
@@ -1,1478 +1,1478 @@
--rw-r--r--   0        0        0     1611 2024-01-16 15:31:37.046680 matrix_synapse-1.99.0/AUTHORS.rst
--rw-r--r--   0        0        0   194250 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/CHANGES.md
--rw-r--r--   0        0        0      171 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    12715 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/Cargo.lock
--rw-r--r--   0        0        0      185 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/Cargo.toml
--rw-r--r--   0        0        0      283 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/INSTALL.md
--rw-r--r--   0        0        0    34523 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/LICENSE
--rw-r--r--   0        0        0    11376 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/README.rst
--rw-r--r--   0        0        0      257 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/UPGRADE.rst
--rw-r--r--   0        0        0     1497 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/book.toml
--rw-r--r--   0        0        0      791 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/build_rust.py
--rw-r--r--   0        0        0       12 2024-01-16 15:31:37.050680 matrix_synapse-1.99.0/changelog.d/.gitignore
--rw-r--r--   0        0        0       74 2024-01-16 15:31:37.054680 matrix_synapse-1.99.0/demo/.gitignore
--rwxr-xr-x   0        0        0      350 2024-01-16 15:31:37.054680 matrix_synapse-1.99.0/demo/clean.sh
--rwxr-xr-x   0        0        0     4440 2024-01-16 15:31:37.054680 matrix_synapse-1.99.0/demo/start.sh
--rwxr-xr-x   0        0        0      262 2024-01-16 15:31:37.054680 matrix_synapse-1.99.0/demo/stop.sh
--rw-r--r--   0        0        0      655 2024-01-16 15:31:37.054680 matrix_synapse-1.99.0/docs/.sample_config_header.yaml
--rw-r--r--   0        0        0     1699 2024-01-16 15:31:37.054680 matrix_synapse-1.99.0/docs/CAPTCHA_SETUP.md
--rw-r--r--   0        0        0     3101 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/README.md
--rw-r--r--   0        0        0     6076 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/SUMMARY.md
--rw-r--r--   0        0        0      664 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/README.rst
--rw-r--r--   0        0        0     1273 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/account_validity.md
--rw-r--r--   0        0        0     6691 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/event_reports.md
--rw-r--r--   0        0        0     1612 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/experimental_features.md
--rw-r--r--   0        0        0     7123 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/media_admin_api.md
--rw-r--r--   0        0        0     2183 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/purge_history_api.md
--rw-r--r--   0        0        0     2641 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/register_api.md
--rw-r--r--   0        0        0      832 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/room_membership.md
--rw-r--r--   0        0        0    35435 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/rooms.md
--rw-r--r--   0        0        0     1124 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/server_notices.md
--rw-r--r--   0        0        0     4325 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/statistics.md
--rw-r--r--   0        0        0    41604 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/user_admin_api.md
--rw-r--r--   0        0        0      480 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/admin_api/version_api.md
--rw-r--r--   0        0        0     2896 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/ancient_architecture_notes.md
--rw-r--r--   0        0        0     1250 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/application_services.md
--rw-r--r--   0        0        0     3583 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/architecture.md
--rw-r--r--   0        0        0      843 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/auth_chain_diff.dot
--rw-r--r--   0        0        0    42427 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/auth_chain_diff.dot.png
--rw-r--r--   0        0        0     7076 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/auth_chain_difference_algorithm.md
--rw-r--r--   0        0        0    91114 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/changelogs/CHANGES-2019.md
--rw-r--r--   0        0        0   178146 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/changelogs/CHANGES-2020.md
--rw-r--r--   0        0        0   220505 2024-01-16 15:31:37.058680 matrix_synapse-1.99.0/docs/changelogs/CHANGES-2021.md
--rw-r--r--   0        0        0   267174 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/changelogs/CHANGES-2022.md
--rw-r--r--   0        0        0   257821 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/changelogs/CHANGES-pre-1.0.md
--rw-r--r--   0        0        0       55 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/changelogs/README.md
--rw-r--r--   0        0        0     4424 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/code_style.md
--rw-r--r--   0        0        0     7328 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/consent_tracking.md
--rw-r--r--   0        0        0     4991 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/delegate.md
--rw-r--r--   0        0        0     2554 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/deprecation_policy.md
--rw-r--r--   0        0        0     2079 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/cas.md
--rw-r--r--   0        0        0    23858 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/contributing_guide.md
--rw-r--r--   0        0        0    17629 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/database_schema.md
--rw-r--r--   0        0        0     1725 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/demo.md
--rw-r--r--   0        0        0    10639 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/dependencies.md
--rw-r--r--   0        0        0     1947 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/experimental_features.md
--rw-r--r--   0        0        0     7135 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/git.md
--rw-r--r--   0        0        0    72228 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/img/git/branches.jpg
--rw-r--r--   0        0        0   110840 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/img/git/clean.png
--rw-r--r--   0        0        0    29667 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/img/git/squash.png
--rw-r--r--   0        0        0      594 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/internal_documentation/README.md
--rw-r--r--   0        0        0     1567 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/releases.md
--rw-r--r--   0        0        0     2016 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/reviews.md
--rw-r--r--   0        0        0     4991 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/room-dag-concepts.md
--rw-r--r--   0        0        0     1839 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/saml.md
--rw-r--r--   0        0        0    11035 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/synapse_architecture/cancellation.md
--rw-r--r--   0        0        0    18006 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/synapse_architecture/faster_joins.md
--rw-r--r--   0        0        0     9698 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/development/synapse_architecture/streams.md
--rw-r--r--   0        0        0     7908 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/favicon.png
--rw-r--r--   0        0        0     3946 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/favicon.svg
--rw-r--r--   0        0        0     3677 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/federate.md
--rw-r--r--   0        0        0     3844 2024-01-16 15:31:37.062680 matrix_synapse-1.99.0/docs/jwt.md
--rw-r--r--   0        0        0    13642 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/log_contexts.md
--rw-r--r--   0        0        0     3246 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/manhole.md
--rw-r--r--   0        0        0     2920 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/media_repository.md
--rw-r--r--   0        0        0     8429 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/message_retention_policies.md
--rw-r--r--   0        0        0    19859 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/metrics-howto.md
--rw-r--r--   0        0        0     3330 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/account_data_callbacks.md
--rw-r--r--   0        0        0     2192 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/account_validity_callbacks.md
--rw-r--r--   0        0        0      950 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/add_extra_fields_to_client_events_unsigned.md
--rw-r--r--   0        0        0     3121 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/background_update_controller_callbacks.md
--rw-r--r--   0        0        0     2090 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/index.md
--rw-r--r--   0        0        0    11738 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/password_auth_provider_callbacks.md
--rw-r--r--   0        0        0     1131 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/porting_legacy_module.md
--rw-r--r--   0        0        0     4323 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/presence_router_callbacks.md
--rw-r--r--   0        0        0    19226 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/spam_checker_callbacks.md
--rw-r--r--   0        0        0    14496 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/third_party_rules_callbacks.md
--rw-r--r--   0        0        0     6604 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/modules/writing_a_module.md
--rw-r--r--   0        0        0    27540 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/openid.md
--rw-r--r--   0        0        0     4018 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/opentracing.md
--rw-r--r--   0        0        0     6075 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/other/running_synapse_on_single_board_computers.md
--rw-r--r--   0        0        0     5268 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/password_auth_providers.md
--rw-r--r--   0        0        0     9365 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/postgres.md
--rw-r--r--   0        0        0     9293 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/presence_router_module.md
--rw-r--r--   0        0        0      724 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/privacy_policy_templates/en/1.0.html
--rw-r--r--   0        0        0      154 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/privacy_policy_templates/en/success.html
--rw-r--r--   0        0        0     1540 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/replication.md
--rw-r--r--   0        0        0     9927 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/reverse_proxy.md
--rw-r--r--   0        0        0      661 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/room_and_user_statistics.md
--rw-r--r--   0        0        0     1725 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/sample_config.yaml
--rw-r--r--   0        0        0     2732 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/sample_log_config.yaml
--rw-r--r--   0        0        0     2731 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/server_notices.md
--rw-r--r--   0        0        0     2763 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/setup/forward_proxy.md
--rw-r--r--   0        0        0    20830 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/setup/installation.md
--rw-r--r--   0        0        0     6613 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/setup/turn/coturn.md
--rw-r--r--   0        0        0     7264 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/setup/turn/eturnal.md
--rw-r--r--   0        0        0     3729 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/spam_checker.md
--rw-r--r--   0        0        0    11780 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/sso_mapping_providers.md
--rw-r--r--   0        0        0     2509 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/structured_logging.md
--rw-r--r--   0        0        0     1131 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/synctl_workers.md
--rw-r--r--   0        0        0     4240 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/README.md
--rw-r--r--   0        0        0      887 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/system/matrix-synapse-worker@.service
--rw-r--r--   0        0        0      813 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/system/matrix-synapse.service
--rw-r--r--   0        0        0      100 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/system/matrix-synapse.target
--rw-r--r--   0        0        0      137 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/workers/background_worker.yaml
--rw-r--r--   0        0        0      544 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/workers/event_persister.yaml
--rw-r--r--   0        0        0      141 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/workers/federation_sender.yaml
--rw-r--r--   0        0        0      254 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/workers/generic_worker.yaml
--rw-r--r--   0        0        0      238 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/workers/media_worker.yaml
--rw-r--r--   0        0        0      122 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/systemd-with-workers/workers/pusher_worker.yaml
--rw-r--r--   0        0        0     9614 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/tcp_replication.md
--rw-r--r--   0        0        0    13804 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/templates.md
--rw-r--r--   0        0        0     6528 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/turn-howto.md
--rw-r--r--   0        0        0    98187 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/upgrade.md
--rw-r--r--   0        0        0      278 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/usage/administration/README.md
--rw-r--r--   0        0        0     2433 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/usage/administration/admin_api/README.md
--rw-r--r--   0        0        0     2468 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/usage/administration/admin_api/background_updates.md
--rw-r--r--   0        0        0     7159 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/usage/administration/admin_api/federation.md
--rw-r--r--   0        0        0     7442 2024-01-16 15:31:37.066680 matrix_synapse-1.99.0/docs/usage/administration/admin_api/registration_tokens.md
--rw-r--r--   0        0        0    11809 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/admin_faq.md
--rw-r--r--   0        0        0     1181 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/database_maintenance_tools.md
--rw-r--r--   0        0        0    13290 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/monitoring/reporting_homeserver_usage_statistics.md
--rw-r--r--   0        0        0     4674 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/monthly_active_users.md
--rw-r--r--   0        0        0     3211 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/request_log.md
--rw-r--r--   0        0        0     2399 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/state_groups.md
--rw-r--r--   0        0        0     6420 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/understanding_synapse_through_grafana_graphs.md
--rw-r--r--   0        0        0     6180 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/administration/useful_sql_for_admins.md
--rw-r--r--   0        0        0      231 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/README.md
--rw-r--r--   0        0        0   159563 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/config_documentation.md
--rw-r--r--   0        0        0      715 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/homeserver_sample_config.md
--rw-r--r--   0        0        0      695 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/logging_sample_config.md
--rw-r--r--   0        0        0      532 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/README.md
--rw-r--r--   0        0        0     6992 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/refresh_tokens.md
--rw-r--r--   0        0        0      207 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/single_sign_on/README.md
--rw-r--r--   0        0        0      377 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/single_sign_on/cas.md
--rw-r--r--   0        0        0      338 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/single_sign_on/saml.md
--rw-r--r--   0        0        0     6558 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/user_directory.md
--rw-r--r--   0        0        0     1976 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/README.md
--rw-r--r--   0        0        0      161 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/indent-section-headers.css
--rw-r--r--   0        0        0      252 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/remove-nav-buttons.css
--rw-r--r--   0        0        0     1118 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/table-of-contents.css
--rw-r--r--   0        0        0     4564 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/table-of-contents.js
--rw-r--r--   0        0        0    15431 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/theme/index.hbs
--rw-r--r--   0        0        0     1902 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/version-picker.css
--rw-r--r--   0        0        0     4705 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/version-picker.js
--rw-r--r--   0        0        0       35 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/website_files/version.js
--rw-r--r--   0        0        0     2951 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/welcome_and_overview.md
--rw-r--r--   0        0        0    32956 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/docs/workers.md
--rw-r--r--   0        0        0     2723 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/mypy.ini
--rw-r--r--   0        0        0    15757 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/pyproject.toml
--rw-r--r--   0        0        0     1082 2024-01-16 15:31:37.070680 matrix_synapse-1.99.0/rust/Cargo.toml
--rw-r--r--   0        0        0     1300 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/build.rs
--rw-r--r--   0        0        0     3082 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/acl/mod.rs
--rw-r--r--   0        0        0    14484 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/events/internal_metadata.rs
--rw-r--r--   0        0        0     1340 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/events/mod.rs
--rw-r--r--   0        0        0     1264 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/lib.rs
--rw-r--r--   0        0        0    29332 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/push/base_rules.rs
--rw-r--r--   0        0        0    20793 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/push/evaluator.rs
--rw-r--r--   0        0        0    26288 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/push/mod.rs
--rw-r--r--   0        0        0     7617 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/rust/src/push/utils.rs
--rwxr-xr-x   0        0        0     7512 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/build_debian_packages.py
--rwxr-xr-x   0        0        0     2320 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/check-newsfragment.sh
--rwxr-xr-x   0        0        0     1009 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/check_line_terminators.sh
--rwxr-xr-x   0        0        0     1923 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/check_locked_deps_have_sdists.py
--rwxr-xr-x   0        0        0    16670 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/check_pydantic_models.py
--rwxr-xr-x   0        0        0     3458 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/check_schema_delta.py
--rwxr-xr-x   0        0        0    10667 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/complement.sh
--rwxr-xr-x   0        0        0      538 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/config-lint.sh
--rwxr-xr-x   0        0        0      362 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/database-save.sh
--rwxr-xr-x   0        0        0     2848 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/docker_update_debian_changelog.sh
--rwxr-xr-x   0        0        0      532 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/dump_macaroon.py
--rwxr-xr-x   0        0        0    11976 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/federation_client.py
--rwxr-xr-x   0        0        0     1049 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/generate_sample_config.sh
--rwxr-xr-x   0        0        0     4146 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/lint.sh
--rwxr-xr-x   0        0        0    11444 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/make_full_schema.sh
--rw-r--r--   0        0        0    12678 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/mypy_synapse_plugin.py
--rwxr-xr-x   0        0        0      308 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/next_github_number.sh
--rwxr-xr-x   0        0        0    30919 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/release.py
--rwxr-xr-x   0        0        0     6790 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/schema_versions.py
--rwxr-xr-x   0        0        0     5177 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/scripts-dev/sign_json.py
--rw-r--r--   0        0        0     3285 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/__init__.py
--rw-r--r--   0        0        0      982 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/__init__.py
--rwxr-xr-x   0        0        0     2781 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/export_signing_key.py
--rwxr-xr-x   0        0        0     2336 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/generate_config.py
--rwxr-xr-x   0        0        0     1409 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/generate_log_config.py
--rwxr-xr-x   0        0        0     1491 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/generate_signing_key.py
--rwxr-xr-x   0        0        0     9751 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/generate_workers_map.py
--rwxr-xr-x   0        0        0     2076 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/hash_password.py
--rwxr-xr-x   0        0        0     3780 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/move_remote_media_to_new_store.py
--rw-r--r--   0        0        0     9110 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/register_new_matrix_user.py
--rw-r--r--   0        0        0     5987 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/review_recent_signups.py
--rwxr-xr-x   0        0        0    50656 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/synapse_port_db.py
--rwxr-xr-x   0        0        0    11921 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/synctl.py
--rw-r--r--   0        0        0     3746 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/_scripts/update_synapse_database.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/api/__init__.py
--rw-r--r--   0        0        0     6131 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/api/auth/__init__.py
--rw-r--r--   0        0        0    15587 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/api/auth/base.py
--rw-r--r--   0        0        0    10501 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/api/auth/internal.py
--rw-r--r--   0        0        0    15240 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/api/auth/msc3861_delegated.py
--rw-r--r--   0        0        0     6033 2024-01-16 15:31:37.074680 matrix_synapse-1.99.0/synapse/api/auth_blocking.py
--rw-r--r--   0        0        0     8272 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/constants.py
--rw-r--r--   0        0        0    28545 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/errors.py
--rw-r--r--   0        0        0    19926 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/filtering.py
--rw-r--r--   0        0        0     3164 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/presence.py
--rw-r--r--   0        0        0    17536 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/ratelimiting.py
--rw-r--r--   0        0        0    13368 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/room_versions.py
--rw-r--r--   0        0        0     2307 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/api/urls.py
--rw-r--r--   0        0        0     1900 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/__init__.py
--rw-r--r--   0        0        0    26657 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/_base.py
--rw-r--r--   0        0        0    12533 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/admin_cmd.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/appservice.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/client_reader.py
--rw-r--r--   0        0        0     7238 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/complement_fork_starter.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/event_creator.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/federation_reader.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/federation_sender.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/frontend_proxy.py
--rw-r--r--   0        0        0    13527 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/generic_worker.py
--rw-r--r--   0        0        0    14883 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/homeserver.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/media_repository.py
--rw-r--r--   0        0        0     8572 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/phone_stats_home.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/pusher.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/synchrotron.py
--rw-r--r--   0        0        0      905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/app/user_dir.py
--rw-r--r--   0        0        0    15399 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/appservice/__init__.py
--rw-r--r--   0        0        0    19987 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/appservice/api.py
--rw-r--r--   0        0        0    21253 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/appservice/scheduler.py
--rw-r--r--   0        0        0      907 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/__init__.py
--rw-r--r--   0        0        0     1896 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/__main__.py
--rw-r--r--   0        0        0    36463 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/_base.py
--rw-r--r--   0        0        0     6184 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/_base.pyi
--rw-r--r--   0        0        0     3389 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/_util.py
--rw-r--r--   0        0        0     4577 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/account_validity.py
--rw-r--r--   0        0        0     4856 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/api.py
--rw-r--r--   0        0        0     7595 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/appservice.py
--rw-r--r--   0        0        0     2834 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/auth.py
--rw-r--r--   0        0        0     1397 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/background_updates.py
--rw-r--r--   0        0        0     8416 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/cache.py
--rw-r--r--   0        0        0     1875 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/captcha.py
--rw-r--r--   0        0        0     3367 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/cas.py
--rw-r--r--   0        0        0     2669 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/consent.py
--rw-r--r--   0        0        0     6499 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/database.py
--rw-r--r--   0        0        0    15124 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/emailconfig.py
--rw-r--r--   0        0        0    16905 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/experimental.py
--rw-r--r--   0        0        0     3720 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/federation.py
--rw-r--r--   0        0        0     3282 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/homeserver.py
--rw-r--r--   0        0        0     1786 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/jwt.py
--rw-r--r--   0        0        0    15126 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/key.py
--rw-r--r--   0        0        0    12101 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/logger.py
--rw-r--r--   0        0        0     2676 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/metrics.py
--rw-r--r--   0        0        0     1393 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/modules.py
--rw-r--r--   0        0        0     6319 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/oembed.py
--rw-r--r--   0        0        0    16521 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/oidc.py
--rw-r--r--   0        0        0     2923 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/password_auth_providers.py
--rw-r--r--   0        0        0     2411 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/push.py
--rw-r--r--   0        0        0     7527 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/ratelimiting.py
--rw-r--r--   0        0        0     1799 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/redis.py
--rw-r--r--   0        0        0    12343 2024-01-16 15:31:37.078680 matrix_synapse-1.99.0/synapse/config/registration.py
--rw-r--r--   0        0        0    10645 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/repository.py
--rw-r--r--   0        0        0     5945 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/retention.py
--rw-r--r--   0        0        0     3288 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/room.py
--rw-r--r--   0        0        0     5529 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/room_directory.py
--rw-r--r--   0        0        0     9260 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/saml2.py
--rw-r--r--   0        0        0    39285 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/server.py
--rw-r--r--   0        0        0     3185 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/server_notices.py
--rw-r--r--   0        0        0     2680 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/spam_checker.py
--rw-r--r--   0        0        0     4109 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/sso.py
--rw-r--r--   0        0        0     1746 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/stats.py
--rw-r--r--   0        0        0     1217 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/third_party_event_rules.py
--rw-r--r--   0        0        0     7551 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/tls.py
--rw-r--r--   0        0        0     2405 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/tracer.py
--rw-r--r--   0        0        0     1501 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/user_directory.py
--rw-r--r--   0        0        0     1299 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/voip.py
--rw-r--r--   0        0        0    24262 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/config/workers.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/crypto/__init__.py
--rw-r--r--   0        0        0    10738 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/crypto/context_factory.py
--rw-r--r--   0        0        0     6241 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/crypto/event_signing.py
--rw-r--r--   0        0        0    33535 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/crypto/keyring.py
--rw-r--r--   0        0        0    41379 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/event_auth.py
--rw-r--r--   0        0        0    18262 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/events/__init__.py
--rw-r--r--   0        0        0    10075 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/events/builder.py
--rw-r--r--   0        0        0     9044 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/events/presence_router.py
--rw-r--r--   0        0        0    21786 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/events/snapshot.py
--rw-r--r--   0        0        0    28195 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/events/utils.py
--rw-r--r--   0        0        0    11341 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/events/validator.py
--rw-r--r--   0        0        0      739 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/__init__.py
--rw-r--r--   0        0        0    12648 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/federation_base.py
--rw-r--r--   0        0        0    73309 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/federation_client.py
--rw-r--r--   0        0        0    59769 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/federation_server.py
--rw-r--r--   0        0        0     2377 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/persistence.py
--rw-r--r--   0        0        0    17244 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/send_queue.py
--rw-r--r--   0        0        0    41665 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/sender/__init__.py
--rw-r--r--   0        0        0    33785 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/sender/per_destination_queue.py
--rw-r--r--   0        0        0     7013 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/sender/transaction_manager.py
--rw-r--r--   0        0        0     1033 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/transport/__init__.py
--rw-r--r--   0        0        0    36251 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/transport/client.py
--rw-r--r--   0        0        0    10104 2024-01-16 15:31:37.082680 matrix_synapse-1.99.0/synapse/federation/transport/server/__init__.py
--rw-r--r--   0        0        0    14924 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/federation/transport/server/_base.py
--rw-r--r--   0        0        0    26155 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/federation/transport/server/federation.py
--rw-r--r--   0        0        0     3036 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/federation/units.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/__init__.py
--rw-r--r--   0        0        0     5438 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/account.py
--rw-r--r--   0        0        0    13009 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/account_data.py
--rw-r--r--   0        0        0    13827 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/account_validity.py
--rw-r--r--   0        0        0    15959 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/admin.py
--rw-r--r--   0        0        0    39457 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/appservice.py
--rw-r--r--   0        0        0    97956 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/auth.py
--rw-r--r--   0        0        0    14793 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/cas.py
--rw-r--r--   0        0        0    12366 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/deactivate_account.py
--rw-r--r--   0        0        0    61283 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/device.py
--rw-r--r--   0        0        0    15447 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/devicemessage.py
--rw-r--r--   0        0        0    20694 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/directory.py
--rw-r--r--   0        0        0    68460 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/e2e_keys.py
--rw-r--r--   0        0        0    17197 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/e2e_room_keys.py
--rw-r--r--   0        0        0    14257 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/event_auth.py
--rw-r--r--   0        0        0     7045 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/events.py
--rw-r--r--   0        0        0    86451 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/federation.py
--rw-r--r--   0        0        0    98739 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/federation_event.py
--rw-r--r--   0        0        0    30688 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/identity.py
--rw-r--r--   0        0        0    18381 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/initial_sync.py
--rw-r--r--   0        0        0     3934 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/jwt.py
--rw-r--r--   0        0        0    90766 2024-01-16 15:31:37.086680 matrix_synapse-1.99.0/synapse/handlers/message.py
--rw-r--r--   0        0        0    67040 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/oidc.py
--rw-r--r--   0        0        0    29733 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/pagination.py
--rw-r--r--   0        0        0     3393 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/password_policy.py
--rw-r--r--   0        0        0    99963 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/presence.py
--rw-r--r--   0        0        0    18444 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/profile.py
--rw-r--r--   0        0        0     6012 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/push_rules.py
--rw-r--r--   0        0        0     2890 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/read_marker.py
--rw-r--r--   0        0        0    12957 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/receipts.py
--rw-r--r--   0        0        0    42558 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/register.py
--rw-r--r--   0        0        0    23451 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/relations.py
--rw-r--r--   0        0        0    81997 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/room.py
--rw-r--r--   0        0        0    23805 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/room_list.py
--rw-r--r--   0        0        0    89876 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/room_member.py
--rw-r--r--   0        0        0     4774 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/room_member_worker.py
--rw-r--r--   0        0        0    37175 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/room_summary.py
--rw-r--r--   0        0        0    19345 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/saml.py
--rw-r--r--   0        0        0    25673 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/search.py
--rw-r--r--   0        0        0     8228 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/send_email.py
--rw-r--r--   0        0        0     2738 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/set_password.py
--rw-r--r--   0        0        0    47872 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/sso.py
--rw-r--r--   0        0        0     2490 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/state_deltas.py
--rw-r--r--   0        0        0    13052 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/stats.py
--rw-r--r--   0        0        0   118386 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/sync.py
--rw-r--r--   0        0        0    21239 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/typing.py
--rw-r--r--   0        0        0     1715 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/ui_auth/__init__.py
--rw-r--r--   0        0        0    11882 2024-01-16 15:31:37.090680 matrix_synapse-1.99.0/synapse/handlers/ui_auth/checkers.py
--rw-r--r--   0        0        0    31838 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/handlers/user_directory.py
--rw-r--r--   0        0        0    11146 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/handlers/worker_lock.py
--rw-r--r--   0        0        0     3314 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/__init__.py
--rw-r--r--   0        0        0     2092 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/additional_resource.py
--rw-r--r--   0        0        0    40422 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/client.py
--rw-r--r--   0        0        0    10383 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/connectproxyclient.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/federation/__init__.py
--rw-r--r--   0        0        0    16986 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/federation/matrix_federation_agent.py
--rw-r--r--   0        0        0     6069 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/federation/srv_resolver.py
--rw-r--r--   0        0        0    12401 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/federation/well_known_resolver.py
--rw-r--r--   0        0        0    56860 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/matrixfederationclient.py
--rw-r--r--   0        0        0    10144 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/proxy.py
--rw-r--r--   0        0        0    17583 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/proxyagent.py
--rw-r--r--   0        0        0     6799 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/replicationagent.py
--rw-r--r--   0        0        0     8476 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/request_metrics.py
--rw-r--r--   0        0        0    35656 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/server.py
--rw-r--r--   0        0        0    26402 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/servlet.py
--rw-r--r--   0        0        0    26902 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/site.py
--rw-r--r--   0        0        0      975 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/http/types.py
--rw-r--r--   0        0        0     1084 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/__init__.py
--rw-r--r--   0        0        0     8591 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/_remote.py
--rw-r--r--   0        0        0     2571 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/_terse_json.py
--rw-r--r--   0        0        0    32689 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/context.py
--rw-r--r--   0        0        0     1159 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/filter.py
--rw-r--r--   0        0        0     2065 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/formatter.py
--rw-r--r--   0        0        0     2771 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/handlers.py
--rw-r--r--   0        0        0    37077 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/opentracing.py
--rw-r--r--   0        0        0     5867 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/logging/scopecontextmanager.py
--rw-r--r--   0        0        0    15419 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/_base.py
--rw-r--r--   0        0        0    15848 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/filepath.py
--rw-r--r--   0        0        0    46339 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/media_repository.py
--rw-r--r--   0        0        0    14432 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/media_storage.py
--rw-r--r--   0        0        0    10256 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/oembed.py
--rw-r--r--   0        0        0    19117 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/preview_html.py
--rw-r--r--   0        0        0     6709 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/storage_provider.py
--rw-r--r--   0        0        0     8529 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/thumbnailer.py
--rw-r--r--   0        0        0    33456 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/media/url_previewer.py
--rw-r--r--   0        0        0    15059 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/metrics/__init__.py
--rw-r--r--   0        0        0     7238 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/metrics/_gc.py
--rw-r--r--   0        0        0     5544 2024-01-16 15:31:37.094680 matrix_synapse-1.99.0/synapse/metrics/_reactor_metrics.py
--rw-r--r--   0        0        0     1395 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/metrics/_twisted_exposition.py
--rw-r--r--   0        0        0     1146 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/metrics/_types.py
--rw-r--r--   0        0        0    12982 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/metrics/background_process_metrics.py
--rw-r--r--   0        0        0     2734 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/metrics/common_usage_metrics.py
--rw-r--r--   0        0        0     8076 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/metrics/jemalloc.py
--rw-r--r--   0        0        0    72000 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/module_api/__init__.py
--rw-r--r--   0        0        0     1395 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/module_api/callbacks/__init__.py
--rw-r--r--   0        0        0     5072 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/module_api/callbacks/account_validity_callbacks.py
--rw-r--r--   0        0        0    34778 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/module_api/callbacks/spamchecker_callbacks.py
--rw-r--r--   0        0        0    24701 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/module_api/callbacks/third_party_event_rules_callbacks.py
--rw-r--r--   0        0        0     1222 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/module_api/errors.py
--rw-r--r--   0        0        0    31892 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/notifier.py
--rw-r--r--   0        0        0     7279 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/__init__.py
--rw-r--r--   0        0        0    23352 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/bulk_push_rule_evaluator.py
--rw-r--r--   0        0        0     4332 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/clientformat.py
--rw-r--r--   0        0        0    12501 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/emailpusher.py
--rw-r--r--   0        0        0    20366 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/httppusher.py
--rw-r--r--   0        0        0    33725 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/mailer.py
--rw-r--r--   0        0        0     7834 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/presentable_names.py
--rw-r--r--   0        0        0     4250 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/push_tools.py
--rw-r--r--   0        0        0     4882 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/push_types.py
--rw-r--r--   0        0        0     2930 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/pusher.py
--rw-r--r--   0        0        0    17431 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/pusherpool.py
--rw-r--r--   0        0        0      863 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/push/rulekinds.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/py.typed
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/__init__.py
--rw-r--r--   0        0        0     2077 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/__init__.py
--rw-r--r--   0        0        0    18636 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/_base.py
--rw-r--r--   0        0        0     8250 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/account_data.py
--rw-r--r--   0        0        0     5368 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/devices.py
--rw-r--r--   0        0        0    10347 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/federation.py
--rw-r--r--   0        0        0     3622 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/login.py
--rw-r--r--   0        0        0    11444 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/membership.py
--rw-r--r--   0        0        0     3657 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/presence.py
--rw-r--r--   0        0        0     2202 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/push.py
--rw-r--r--   0        0        0     6272 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/register.py
--rw-r--r--   0        0        0     5630 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/send_event.py
--rw-r--r--   0        0        0     6298 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/send_events.py
--rw-r--r--   0        0        0     2484 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/state.py
--rw-r--r--   0        0        0     3196 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/http/streams.py
--rw-r--r--   0        0        0     1874 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/tcp/__init__.py
--rw-r--r--   0        0        0    21607 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/tcp/client.py
--rw-r--r--   0        0        0    15244 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/tcp/commands.py
--rw-r--r--   0        0        0     1513 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/tcp/context.py
--rw-r--r--   0        0        0     4413 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/tcp/external_cache.py
--rw-r--r--   0        0        0    33489 2024-01-16 15:31:37.098680 matrix_synapse-1.99.0/synapse/replication/tcp/handler.py
--rw-r--r--   0        0        0    19184 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/protocol.py
--rw-r--r--   0        0        0    15414 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/redis.py
--rw-r--r--   0        0        0    14466 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/resource.py
--rw-r--r--   0        0        0     2537 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/streams/__init__.py
--rw-r--r--   0        0        0    24081 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/streams/_base.py
--rw-r--r--   0        0        0    10050 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/streams/events.py
--rw-r--r--   0        0        0     3365 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/streams/federation.py
--rw-r--r--   0        0        0     2384 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/replication/tcp/streams/partial_state.py
--rw-r--r--   0        0        0      760 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/providers.json
--rw-r--r--   0        0        0     1035 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/_base.html
--rw-r--r--   0        0        0      240 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/account_previously_renewed.html
--rw-r--r--   0        0        0      308 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/account_renewed.html
--rw-r--r--   0        0        0      413 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/add_threepid.html
--rw-r--r--   0        0        0      230 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/add_threepid.txt
--rw-r--r--   0        0        0      230 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/add_threepid_failure.html
--rw-r--r--   0        0        0      228 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/add_threepid_success.html
--rw-r--r--   0        0        0      490 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/auth_success.html
--rw-r--r--   0        0        0      144 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/invalid_token.html
--rw-r--r--   0        0        0      124 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/mail-Element.css
--rw-r--r--   0        0        0      124 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/mail-Vector.css
--rw-r--r--   0        0        0       63 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/mail-expiry.css
--rw-r--r--   0        0        0     2252 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/mail.css
--rw-r--r--   0        0        0     2044 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/notice_expiry.html
--rw-r--r--   0        0        0      293 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/notice_expiry.txt
--rw-r--r--   0        0        0     2658 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/notif.html
--rw-r--r--   0        0        0      761 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/notif.txt
--rw-r--r--   0        0        0     2674 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/notif_mail.html
--rw-r--r--   0        0        0      191 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/notif_mail.txt
--rw-r--r--   0        0        0      431 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/password_reset.html
--rw-r--r--   0        0        0      269 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/password_reset.txt
--rw-r--r--   0        0        0      740 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/password_reset_confirmation.html
--rw-r--r--   0        0        0      229 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/password_reset_failure.html
--rw-r--r--   0        0        0      240 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/password_reset_success.html
--rw-r--r--   0        0        0     1141 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/recaptcha.html
--rw-r--r--   0        0        0      392 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/registration.html
--rw-r--r--   0        0        0      241 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/registration.txt
--rw-r--r--   0        0        0      185 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/registration_failure.html
--rw-r--r--   0        0        0      228 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/registration_success.html
--rw-r--r--   0        0        0      536 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/registration_token.html
--rw-r--r--   0        0        0     1117 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/room.html
--rw-r--r--   0        0        0      216 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/room.txt
--rw-r--r--   0        0        0     1783 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso.css
--rw-r--r--   0        0        0      671 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_account_deactivated.html
--rw-r--r--   0        0        0     5077 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_auth_account_details.html
--rw-r--r--   0        0        0     3711 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_auth_account_details.js
--rw-r--r--   0        0        0      812 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_auth_bad_user.html
--rw-r--r--   0        0        0      698 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_auth_confirm.html
--rw-r--r--   0        0        0      629 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_auth_success.html
--rw-r--r--   0        0        0     2807 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_error.html
--rw-r--r--   0        0        0     9062 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_footer.html
--rw-r--r--   0        0        0     1258 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_login_idp_picker.html
--rw-r--r--   0        0        0      961 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_new_user_consent.html
--rw-r--r--   0        0        0      873 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_partial_profile.html
--rw-r--r--   0        0        0     1905 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/sso_redirect_confirm.html
--rw-r--r--   0        0        0      641 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/style.css
--rw-r--r--   0        0        0      739 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/res/templates/terms.html
--rw-r--r--   0        0        0     5314 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/__init__.py
--rw-r--r--   0        0        0    13731 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/__init__.py
--rw-r--r--   0        0        0     2201 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/_base.py
--rw-r--r--   0        0        0     5917 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/background_updates.py
--rw-r--r--   0        0        0     7342 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/devices.py
--rw-r--r--   0        0        0     5911 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/event_reports.py
--rw-r--r--   0        0        0     3973 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/experimental_features.py
--rw-r--r--   0        0        0     9269 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/federation.py
--rw-r--r--   0        0        0    17900 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/media.py
--rw-r--r--   0        0        0    11419 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/registration_tokens.py
--rw-r--r--   0        0        0    34939 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/rooms.py
--rw-r--r--   0        0        0     4542 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/server_notice_servlet.py
--rw-r--r--   0        0        0     5370 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/statistics.py
--rw-r--r--   0        0        0     1905 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/username_available.py
--rw-r--r--   0        0        0    47896 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/admin/users.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.102680 matrix_synapse-1.99.0/synapse/rest/client/__init__.py
--rw-r--r--   0        0        0     3584 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/_base.py
--rw-r--r--   0        0        0    35375 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/account.py
--rw-r--r--   0        0        0    12113 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/account_data.py
--rw-r--r--   0        0        0     3608 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/account_validity.py
--rw-r--r--   0        0        0     3926 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/appservice_ping.py
--rw-r--r--   0        0        0     7292 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/auth.py
--rw-r--r--   0        0        0     2209 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/auth_issuer.py
--rw-r--r--   0        0        0     3524 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/capabilities.py
--rw-r--r--   0        0        0    18982 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/devices.py
--rw-r--r--   0        0        0     7513 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/directory.py
--rw-r--r--   0        0        0     4029 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/events.py
--rw-r--r--   0        0        0     3764 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/filter.py
--rw-r--r--   0        0        0     2331 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/initial_sync.py
--rw-r--r--   0        0        0    17255 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/keys.py
--rw-r--r--   0        0        0     3275 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/knock.py
--rw-r--r--   0        0        0    27523 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/login.py
--rw-r--r--   0        0        0     4234 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/login_token_request.py
--rw-r--r--   0        0        0     3331 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/logout.py
--rw-r--r--   0        0        0     3178 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/models.py
--rw-r--r--   0        0        0     3044 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/mutual_rooms.py
--rw-r--r--   0        0        0     3978 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/notifications.py
--rw-r--r--   0        0        0     3402 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/openid.py
--rw-r--r--   0        0        0     1959 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/password_policy.py
--rw-r--r--   0        0        0     3697 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/presence.py
--rw-r--r--   0        0        0     7150 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/profile.py
--rw-r--r--   0        0        0    10511 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/push_rule.py
--rw-r--r--   0        0        0     5807 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/pusher.py
--rw-r--r--   0        0        0     3655 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/read_marker.py
--rw-r--r--   0        0        0     5936 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/receipts.py
--rw-r--r--   0        0        0    40419 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/register.py
--rw-r--r--   0        0        0     4894 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/relations.py
--rw-r--r--   0        0        0     2676 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/rendezvous.py
--rw-r--r--   0        0        0     3194 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/report_event.py
--rw-r--r--   0        0        0    54203 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/room.py
--rw-r--r--   0        0        0    15462 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/room_keys.py
--rw-r--r--   0        0        0     3316 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/room_upgrade_rest_servlet.py
--rw-r--r--   0        0        0     2664 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/sendtodevice.py
--rw-r--r--   0        0        0    21245 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/sync.py
--rw-r--r--   0        0        0     3433 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/tags.py
--rw-r--r--   0        0        0     4185 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/thirdparty.py
--rw-r--r--   0        0        0     1498 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/tokenrefresh.py
--rw-r--r--   0        0        0     5906 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/transactions.py
--rw-r--r--   0        0        0     2911 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/user_directory.py
--rw-r--r--   0        0        0     6938 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/versions.py
--rw-r--r--   0        0        0     2918 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/client/voip.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/consent/__init__.py
--rw-r--r--   0        0        0     7825 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/consent/consent_resource.py
--rw-r--r--   0        0        0     1178 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/health.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/key/__init__.py
--rw-r--r--   0        0        0     1300 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/key/v2/__init__.py
--rw-r--r--   0        0        0     4541 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/key/v2/local_key_resource.py
--rw-r--r--   0        0        0    11248 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/key/v2/remote_key_resource.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/__init__.py
--rw-r--r--   0        0        0     1453 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/config_resource.py
--rw-r--r--   0        0        0     2928 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/create_resource.py
--rw-r--r--   0        0        0     3440 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/download_resource.py
--rw-r--r--   0        0        0     4087 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/media_repository_resource.py
--rw-r--r--   0        0        0     2812 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/preview_url_resource.py
--rw-r--r--   0        0        0    21635 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/thumbnail_resource.py
--rw-r--r--   0        0        0     6285 2024-01-16 15:31:37.106680 matrix_synapse-1.99.0/synapse/rest/media/upload_resource.py
--rw-r--r--   0        0        0     1241 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/media/v1/__init__.py
--rw-r--r--   0        0        0      829 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/media/v1/_base.py
--rw-r--r--   0        0        0      817 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/media/v1/media_storage.py
--rw-r--r--   0        0        0      818 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/media/v1/storage_provider.py
--rw-r--r--   0        0        0     1663 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/models.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/__init__.py
--rw-r--r--   0        0        0     3055 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/__init__.py
--rw-r--r--   0        0        0     2293 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/jwks.py
--rw-r--r--   0        0        0     4515 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/new_user_consent.py
--rw-r--r--   0        0        0     1337 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/oidc/__init__.py
--rw-r--r--   0        0        0     1265 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/oidc/backchannel_logout_resource.py
--rw-r--r--   0        0        0     1583 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/oidc/callback_resource.py
--rw-r--r--   0        0        0     4560 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/password_reset.py
--rw-r--r--   0        0        0     3035 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/pick_idp.py
--rw-r--r--   0        0        0     5633 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/pick_username.py
--rw-r--r--   0        0        0     1308 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/saml2/__init__.py
--rw-r--r--   0        0        0     1403 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/saml2/metadata_resource.py
--rw-r--r--   0        0        0     1860 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/saml2/response_resource.py
--rw-r--r--   0        0        0     1933 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/sso_register.py
--rw-r--r--   0        0        0     2902 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/synapse/client/unsubscribe.py
--rw-r--r--   0        0        0     4650 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/rest/well_known.py
--rw-r--r--   0        0        0    32566 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server_notices/__init__.py
--rw-r--r--   0        0        0     4826 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server_notices/consent_server_notices.py
--rw-r--r--   0        0        0     7971 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server_notices/resource_limits_server_notices.py
--rw-r--r--   0        0        0    14513 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server_notices/server_notices_manager.py
--rw-r--r--   0        0        0     2283 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server_notices/server_notices_sender.py
--rw-r--r--   0        0        0     1388 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/server_notices/worker_server_notices_sender.py
--rw-r--r--   0        0        0      912 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/spam_checker_api/__init__.py
--rw-r--r--   0        0        0    34150 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/state/__init__.py
--rw-r--r--   0        0        0    12402 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/state/v1.py
--rw-r--r--   0        0        0    27610 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/state/v2.py
--rw-r--r--   0        0        0     1703 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/static/client/login/index.html
--rw-r--r--   0        0        0    88145 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/static/client/login/js/jquery-3.4.1.min.js
--rw-r--r--   0        0        0     8277 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/static/client/login/js/login.js
--rw-r--r--   0        0        0     1849 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/static/client/login/spinner.gif
--rw-r--r--   0        0        0     1224 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/static/client/login/style.css
--rw-r--r--   0        0        0    10145 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/static/index.html
--rw-r--r--   0        0        0     1703 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/__init__.py
--rw-r--r--   0        0        0     8791 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/_base.py
--rw-r--r--   0        0        0    42388 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/background_updates.py
--rw-r--r--   0        0        0     1966 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/controllers/__init__.py
--rw-r--r--   0        0        0    45325 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/controllers/persist_events.py
--rw-r--r--   0        0        0     4246 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/controllers/purge_events.py
--rw-r--r--   0        0        0    29791 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/controllers/state.py
--rw-r--r--   0        0        0     4126 2024-01-16 15:31:37.110680 matrix_synapse-1.99.0/synapse/storage/controllers/stats.py
--rw-r--r--   0        0        0    93733 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/database.py
--rw-r--r--   0        0        0     5405 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/__init__.py
--rw-r--r--   0        0        0    13942 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/__init__.py
--rw-r--r--   0        0        0    35853 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/account_data.py
--rw-r--r--   0        0        0    17471 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/appservice.py
--rw-r--r--   0        0        0    31379 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/cache.py
--rw-r--r--   0        0        0     8458 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/censor_events.py
--rw-r--r--   0        0        0    30867 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/client_ips.py
--rw-r--r--   0        0        0    43309 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/deviceinbox.py
--rw-r--r--   0        0        0    86038 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/devices.py
--rw-r--r--   0        0        0     6747 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/directory.py
--rw-r--r--   0        0        0    24499 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/e2e_room_keys.py
--rw-r--r--   0        0        0    64757 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/end_to_end_keys.py
--rw-r--r--   0        0        0    81598 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/event_federation.py
--rw-r--r--   0        0        0    72345 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/event_push_actions.py
--rw-r--r--   0        0        0    97971 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/events.py
--rw-r--r--   0        0        0    57370 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/events_bg_updates.py
--rw-r--r--   0        0        0     4308 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/events_forward_extremities.py
--rw-r--r--   0        0        0    99788 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/events_worker.py
--rw-r--r--   0        0        0     2881 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/experimental_features.py
--rw-r--r--   0        0        0     8252 2024-01-16 15:31:37.114680 matrix_synapse-1.99.0/synapse/storage/databases/main/filtering.py
--rw-r--r--   0        0        0    10679 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/keys.py
--rw-r--r--   0        0        0    16855 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/lock.py
--rw-r--r--   0        0        0    30695 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/media_repository.py
--rw-r--r--   0        0        0    17814 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/metrics.py
--rw-r--r--   0        0        0    17946 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/monthly_active_users.py
--rw-r--r--   0        0        0     1899 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/openid.py
--rw-r--r--   0        0        0    19175 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/presence.py
--rw-r--r--   0        0        0     7630 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/profile.py
--rw-r--r--   0        0        0    18752 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/purge_events.py
--rw-r--r--   0        0        0    33510 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/push_rule.py
--rw-r--r--   0        0        0    28080 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/pusher.py
--rw-r--r--   0        0        0    40364 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/receipts.py
--rw-r--r--   0        0        0   104575 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/registration.py
--rw-r--r--   0        0        0     1163 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/rejections.py
--rw-r--r--   0        0        0    41986 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/relations.py
--rw-r--r--   0        0        0    92730 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/room.py
--rw-r--r--   0        0        0    56179 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/roommember.py
--rw-r--r--   0        0        0    32254 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/search.py
--rw-r--r--   0        0        0     5091 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/session.py
--rw-r--r--   0        0        0     3040 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/signatures.py
--rw-r--r--   0        0        0    26041 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/state.py
--rw-r--r--   0        0        0     5672 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/state_deltas.py
--rw-r--r--   0        0        0    28119 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/stats.py
--rw-r--r--   0        0        0    58386 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/stream.py
--rw-r--r--   0        0        0    10847 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/tags.py
--rw-r--r--   0        0        0     7650 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/task_scheduler.py
--rw-r--r--   0        0        0    21523 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/transactions.py
--rw-r--r--   0        0        0    14628 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/ui_auth.py
--rw-r--r--   0        0        0    49340 2024-01-16 15:31:37.118680 matrix_synapse-1.99.0/synapse/storage/databases/main/user_directory.py
--rw-r--r--   0        0        0     3884 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/databases/main/user_erasure_store.py
--rw-r--r--   0        0        0      758 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/databases/state/__init__.py
--rw-r--r--   0        0        0    21788 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/databases/state/bg_updates.py
--rw-r--r--   0        0        0    32707 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/databases/state/store.py
--rw-r--r--   0        0        0     2295 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/engines/__init__.py
--rw-r--r--   0        0        0     5020 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/engines/_base.py
--rw-r--r--   0        0        0    10256 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/engines/postgres.py
--rw-r--r--   0        0        0     7476 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/engines/sqlite.py
--rw-r--r--   0        0        0     1225 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/keys.py
--rw-r--r--   0        0        0    25679 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/prepare_database.py
--rw-r--r--   0        0        0      779 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/push_rule.py
--rw-r--r--   0        0        0     1778 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/roommember.py
--rw-r--r--   0        0        0      207 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/README.md
--rw-r--r--   0        0        0     6219 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/__init__.py
--rw-r--r--   0        0        0     1559 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/common/delta/25/00background_updates.sql
--rw-r--r--   0        0        0     1347 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/common/delta/35/00background_updates_add_col.sql
--rw-r--r--   0        0        0     1506 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/common/delta/58/00background_update_ordering.sql
--rw-r--r--   0        0        0      269 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/common/full_schemas/72/full.sql.postgres
--rw-r--r--   0        0        0      221 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/common/full_schemas/72/full.sql.sqlite
--rw-r--r--   0        0        0     2207 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/common/schema_version.sql
--rw-r--r--   0        0        0     2587 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/12/v12.sql
--rw-r--r--   0        0        0     1451 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/13/v13.sql
--rw-r--r--   0        0        0     1573 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/14/v14.sql
--rw-r--r--   0        0        0     1690 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/15/appservice_txns.sql
--rw-r--r--   0        0        0       78 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/15/presence_indices.sql
--rw-r--r--   0        0        0      991 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/15/v15.sql
--rw-r--r--   0        0        0      174 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/events_order_index.sql
--rw-r--r--   0        0        0      114 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/remote_media_cache_index.sql
--rw-r--r--   0        0        0      265 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/remove_duplicates.sql
--rw-r--r--   0        0        0      157 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/room_alias_index.sql
--rw-r--r--   0        0        0     2003 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/unique_constraints.sql
--rw-r--r--   0        0        0     1519 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/users.sql
--rw-r--r--   0        0        0     1417 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/17/drop_indexes.sql
--rw-r--r--   0        0        0     1744 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/17/server_keys.sql
--rw-r--r--   0        0        0      310 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/17/user_threepids.sql
--rw-r--r--   0        0        0     2053 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/18/server_keys_bigger_ints.sql
--rw-r--r--   0        0        0     1402 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/19/event_index.sql
--rw-r--r--   0        0        0       10 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/20/dummy.sql
--rw-r--r--   0        0        0     3071 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/20/pushers.py
--rw-r--r--   0        0        0     2247 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/21/end_to_end_keys.sql
--rw-r--r--   0        0        0     1944 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/21/receipts.sql
--rw-r--r--   0        0        0     1637 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/22/receipts_index.sql
--rw-r--r--   0        0        0      546 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/22/user_threepids_unique.sql
--rw-r--r--   0        0        0     1402 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/24/stats_reporting.sql
--rw-r--r--   0        0        0     2525 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/fts.py
--rw-r--r--   0        0        0     1573 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/guest_access.sql
--rw-r--r--   0        0        0     1591 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/history_visibility.sql
--rw-r--r--   0        0        0     2093 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/tags.sql
--rw-r--r--   0        0        0     1376 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/26/account_data.sql
--rw-r--r--   0        0        0     2201 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/27/account_data.sql
--rw-r--r--   0        0        0     1605 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/27/forgotten_memberships.sql
--rw-r--r--   0        0        0     1973 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/27/ts.py
--rw-r--r--   0        0        0     1803 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/event_push_actions.sql
--rw-r--r--   0        0        0     1604 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/events_room_stream.sql
--rw-r--r--   0        0        0     1587 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/public_roms_index.sql
--rw-r--r--   0        0        0     1619 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/receipts_user_id_index.sql
--rw-r--r--   0        0        0     1438 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/upgrade_times.sql
--rw-r--r--   0        0        0     1615 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/users_is_guest.sql
--rw-r--r--   0        0        0     2234 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/29/push_actions.sql
--rw-r--r--   0        0        0     1337 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/alias_creator.sql
--rw-r--r--   0        0        0     2783 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/as_users.py
--rw-r--r--   0        0        0     1640 2024-01-16 15:31:37.122680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/deleted_pushers.sql
--rw-r--r--   0        0        0     1736 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/presence_stream.sql
--rw-r--r--   0        0        0     1648 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/public_rooms.sql
--rw-r--r--   0        0        0     2006 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/push_rule_stream.sql
--rw-r--r--   0        0        0     1770 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/threepid_guest_access_tokens.sql
--rw-r--r--   0        0        0     2127 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/invites.sql
--rw-r--r--   0        0        0     1958 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/local_media_repository_url_cache.sql
--rw-r--r--   0        0        0     2935 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/pushers_0.py
--rw-r--r--   0        0        0     1642 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/pushers_index.sql
--rw-r--r--   0        0        0     2087 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/search_update.py
--rw-r--r--   0        0        0     1337 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/events.sql
--rw-r--r--   0        0        0      241 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/openid.sql
--rw-r--r--   0        0        0     1459 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/pusher_throttle.sql
--rw-r--r--   0        0        0     2275 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/remove_indices.sql
--rw-r--r--   0        0        0     1504 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/reports.sql
--rw-r--r--   0        0        0     1394 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/access_tokens_device_index.sql
--rw-r--r--   0        0        0     1453 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/devices.sql
--rw-r--r--   0        0        0     1488 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/devices_for_e2e_keys.sql
--rw-r--r--   0        0        0     1509 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/devices_for_e2e_keys_clear_unknown_device.sql
--rw-r--r--   0        0        0     1937 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/event_fields.py
--rw-r--r--   0        0        0     1300 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/remote_media_ts.py
--rw-r--r--   0        0        0     1389 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/user_ips_index.sql
--rw-r--r--   0        0        0     1600 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/appservice_stream.sql
--rw-r--r--   0        0        0     1577 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/cache_stream.py
--rw-r--r--   0        0        0     1626 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/device_inbox.sql
--rw-r--r--   0        0        0     1770 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/push_display_name_rename.sql
--rw-r--r--   0        0        0     1203 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/received_txn_purge.py
--rw-r--r--   0        0        0     1396 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/contains_url.sql
--rw-r--r--   0        0        0     2010 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/device_outbox.sql
--rw-r--r--   0        0        0     1460 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/device_stream_id.sql
--rw-r--r--   0        0        0     1391 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/event_push_actions_index.sql
--rw-r--r--   0        0        0     1762 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/public_room_list_change_stream.sql
--rw-r--r--   0        0        0     2001 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/stream_order_to_extrem.sql
--rw-r--r--   0        0        0     1747 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/36/readd_public_rooms.sql
--rw-r--r--   0        0        0     2777 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/37/remove_auth_idx.py
--rw-r--r--   0        0        0     2849 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/37/user_threepids.sql
--rw-r--r--   0        0        0     1467 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/38/postgres_fts_gist.sql
--rw-r--r--   0        0        0     1775 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/appservice_room_list.sql
--rw-r--r--   0        0        0     1368 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/device_federation_stream_idx.sql
--rw-r--r--   0        0        0     1403 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/event_push_index.sql
--rw-r--r--   0        0        0     1599 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/federation_out_position.sql
--rw-r--r--   0        0        0     1517 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/membership_profile.sql
--rw-r--r--   0        0        0     1393 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/current_state_idx.sql
--rw-r--r--   0        0        0     1617 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/device_inbox.sql
--rw-r--r--   0        0        0     2880 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/device_list_streams.sql
--rw-r--r--   0        0        0     2179 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/event_push_summary.sql
--rw-r--r--   0        0        0     1897 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/pushers.sql
--rw-r--r--   0        0        0     1399 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/device_list_stream_idx.sql
--rw-r--r--   0        0        0     1384 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/device_outbound_index.sql
--rw-r--r--   0        0        0     1401 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/event_search_event_id_idx.sql
--rw-r--r--   0        0        0     1488 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/ratelimit.sql
--rw-r--r--   0        0        0     1647 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/current_state_delta.sql
--rw-r--r--   0        0        0     1994 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/device_list_last_id.sql
--rw-r--r--   0        0        0     1395 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/event_auth_state_only.sql
--rw-r--r--   0        0        0     2755 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/user_dir.py
--rw-r--r--   0        0        0     1475 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/blocked_rooms.sql
--rw-r--r--   0        0        0     1423 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/quarantine_media.sql
--rw-r--r--   0        0        0     1355 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/url_cache.sql
--rw-r--r--   0        0        0     2078 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/user_share.sql
--rw-r--r--   0        0        0     2520 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/44/expire_url_cache.sql
--rw-r--r--   0        0        0     5957 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/45/group_server.sql
--rw-r--r--   0        0        0     1767 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/45/profile_cache.sql
--rw-r--r--   0        0        0     1384 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/drop_refresh_tokens.sql
--rw-r--r--   0        0        0     1992 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/drop_unique_deleted_pushers.sql
--rw-r--r--   0        0        0     1850 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/group_server.sql
--rw-r--r--   0        0        0     1764 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/local_media_repository_url_idx.sql
--rw-r--r--   0        0        0     2058 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/user_dir_null_room_ids.sql
--rw-r--r--   0        0        0     1775 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/user_dir_typos.sql
--rw-r--r--   0        0        0     1356 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/47/last_access_media.sql
--rw-r--r--   0        0        0     1395 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/47/postgres_fts_gin.sql
--rw-r--r--   0        0        0     1778 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/47/push_actions_staging.sql
--rw-r--r--   0        0        0     1412 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/add_user_consent.sql
--rw-r--r--   0        0        0     1394 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/add_user_ips_last_seen_index.sql
--rw-r--r--   0        0        0     1643 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/deactivated_users.sql
--rw-r--r--   0        0        0     2237 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/group_unique_indexes.py
--rw-r--r--   0        0        0     1603 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/groups_joinable.sql
--rw-r--r--   0        0        0     1518 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/49/add_user_consent_server_notice_sent.sql
--rw-r--r--   0        0        0     1607 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/49/add_user_daily_visits.sql
--rw-r--r--   0        0        0     1399 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/49/add_user_ips_last_seen_only_index.sql
--rw-r--r--   0        0        0     1389 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/50/add_creation_ts_users_index.sql
--rw-r--r--   0        0        0     1477 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/50/erasure_store.sql
--rw-r--r--   0        0        0     3253 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/50/make_event_content_nullable.py
--rw-r--r--   0        0        0     2037 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/51/e2e_room_keys.sql
--rw-r--r--   0        0        0     1865 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/51/monthly_active_users.sql
--rw-r--r--   0        0        0     1533 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/52/add_event_to_state_group_index.sql
--rw-r--r--   0        0        0     2131 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/52/device_list_streams_unique_idx.sql
--rw-r--r--   0        0        0     2551 2024-01-16 15:31:37.126680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/52/e2e_room_keys.sql
--rw-r--r--   0        0        0     1462 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/add_user_type_to_users.sql
--rw-r--r--   0        0        0     1327 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/drop_sent_transactions.sql
--rw-r--r--   0        0        0     1345 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/event_format_version.sql
--rw-r--r--   0        0        0     2101 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_dir_populate.sql
--rw-r--r--   0        0        0     1983 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_ips_index.sql
--rw-r--r--   0        0        0     2729 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_share.sql
--rw-r--r--   0        0        0     1730 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_threepid_id.sql
--rw-r--r--   0        0        0     1713 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/users_in_public_rooms.sql
--rw-r--r--   0        0        0     1939 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/account_validity_with_renewal.sql
--rw-r--r--   0        0        0     1665 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/add_validity_to_server_keys.sql
--rw-r--r--   0        0        0     1806 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/delete_forward_extremities.sql
--rw-r--r--   0        0        0     1881 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/drop_legacy_tables.sql
--rw-r--r--   0        0        0     1323 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/drop_presence_list.sql
--rw-r--r--   0        0        0     1846 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/relations.sql
--rw-r--r--   0        0        0     3205 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/stats.sql
--rw-r--r--   0        0        0     1895 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/stats2.sql
--rw-r--r--   0        0        0     1472 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/55/access_token_expiry.sql
--rw-r--r--   0        0        0     1804 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/55/track_threepid_validations.sql
--rw-r--r--   0        0        0     1476 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/55/users_alter_deactivated.sql
--rw-r--r--   0        0        0     1559 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/add_spans_to_device_lists.sql
--rw-r--r--   0        0        0     1725 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/current_state_events_membership.sql
--rw-r--r--   0        0        0     1784 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/current_state_events_membership_mk2.sql
--rw-r--r--   0        0        0     1626 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/delete_keys_from_deleted_backups.sql
--rw-r--r--   0        0        0     1635 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/destinations_failure_ts.sql
--rw-r--r--   0        0        0      806 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/destinations_retry_interval_type.sql.postgres
--rw-r--r--   0        0        0     1594 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/device_stream_id_insert.sql
--rw-r--r--   0        0        0     1713 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/devices_last_seen.sql
--rw-r--r--   0        0        0     1475 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/drop_unused_event_tables.sql
--rw-r--r--   0        0        0     1480 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/event_expiry.sql
--rw-r--r--   0        0        0     1961 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/event_labels.sql
--rw-r--r--   0        0        0     1404 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/event_labels_background_update.sql
--rw-r--r--   0        0        0     1503 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/fix_room_keys_index.sql
--rw-r--r--   0        0        0     1460 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/hidden_devices.sql
--rw-r--r--   0        0        0     1449 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/hidden_devices_fix.sql.sqlite
--rw-r--r--   0        0        0     3619 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/nuke_empty_communities_from_db.sql
--rw-r--r--   0        0        0     1415 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/public_room_list_idx.sql
--rw-r--r--   0        0        0     1382 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor.sql
--rw-r--r--   0        0        0     1576 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor2.sql
--rw-r--r--   0        0        0     1093 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor3_fix_update.sql.postgres
--rw-r--r--   0        0        0     1352 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor4.sql
--rw-r--r--   0        0        0     1543 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/remove_tombstoned_rooms_from_directory.sql
--rw-r--r--   0        0        0     1404 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/room_key_etag.sql
--rw-r--r--   0        0        0     1496 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/room_membership_idx.sql
--rw-r--r--   0        0        0     1933 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/room_retention.sql
--rw-r--r--   0        0        0     2783 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/signing_keys.sql
--rw-r--r--   0        0        0     1743 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/signing_keys_nonunique_signatures.sql
--rw-r--r--   0        0        0     5860 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/stats_separated.sql
--rw-r--r--   0        0        0     1620 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/unique_user_filter_index.py
--rw-r--r--   0        0        0     1565 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/user_external_ids.sql
--rw-r--r--   0        0        0     1452 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/users_in_public_rooms_idx.sql
--rw-r--r--   0        0        0     1679 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/delete_old_current_state_events.sql
--rw-r--r--   0        0        0     1787 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/device_list_remote_cache_stale.sql
--rw-r--r--   0        0        0     4397 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/local_current_membership.py
--rw-r--r--   0        0        0     1538 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/remove_sent_outbound_pokes.sql
--rw-r--r--   0        0        0     1634 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column.sql
--rw-r--r--   0        0        0     1713 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.postgres
--rw-r--r--   0        0        0      998 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.sqlite
--rw-r--r--   0        0        0     1920 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.postgres
--rw-r--r--   0        0        0      998 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.sqlite
--rw-r--r--   0        0        0     1594 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/02remove_dup_outbound_pokes.sql
--rw-r--r--   0        0        0     2520 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/03persist_ui_auth.sql
--rw-r--r--   0        0        0     1148 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/05cache_instance.sql.postgres
--rw-r--r--   0        0        0     2784 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/06dlols_unique_idx.py
--rw-r--r--   0        0        0     1552 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.postgres
--rw-r--r--   0        0        0     2349 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.sqlite
--rw-r--r--   0        0        0     1677 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/07persist_ui_auth_ips.sql
--rw-r--r--   0        0        0      823 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.postgres
--rw-r--r--   0        0        0      819 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.sqlite
--rw-r--r--   0        0        0     1458 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/09shadow_ban.sql
--rw-r--r--   0        0        0     1752 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/10_pushrules_enabled_delete_obsolete.sql
--rw-r--r--   0        0        0     1556 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/10drop_local_rejections_stream.sql
--rw-r--r--   0        0        0     1740 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/10federation_pos_instance_name.sql
--rw-r--r--   0        0        0     1488 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/11dehydration.sql
--rw-r--r--   0        0        0     1862 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/11fallback.sql
--rw-r--r--   0        0        0     1261 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/11user_id_seq.py
--rw-r--r--   0        0        0     2255 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/12room_stats.sql
--rw-r--r--   0        0        0     1383 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/13remove_presence_allow_inbound.sql
--rw-r--r--   0        0        0     1355 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/14events_instance_name.sql
--rw-r--r--   0        0        0     1074 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/14events_instance_name.sql.postgres
--rw-r--r--   0        0        0     2821 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/15_catchup_destination_rooms.sql
--rw-r--r--   0        0        0     1886 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/15unread_count.sql
--rw-r--r--   0        0        0     1790 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/16populate_stats_process_rooms_fix.sql
--rw-r--r--   0        0        0     1641 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/17_catchup_last_successful.sql
--rw-r--r--   0        0        0     1524 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/18stream_positions.sql
--rw-r--r--   0        0        0     1001 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/19instance_map.sql.postgres
--rw-r--r--   0        0        0     2353 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/19txn_id.sql
--rw-r--r--   0        0        0     1435 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/20instance_name_event_tables.sql
--rw-r--r--   0        0        0     1427 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/20user_daily_visits.sql
--rw-r--r--   0        0        0     1455 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/21as_device_stream.sql
--rw-r--r--   0        0        0       33 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/21drop_device_max_stream_id.sql
--rw-r--r--   0        0        0     1439 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/22puppet_token.sql
--rw-r--r--   0        0        0      119 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/22users_have_local_media.sql
--rw-r--r--   0        0        0     1427 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/23e2e_cross_signing_keys_idx.sql
--rw-r--r--   0        0        0     1480 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/24drop_event_json_index.sql
--rw-r--r--   0        0        0     1430 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/25user_external_ids_user_id_idx.sql
--rw-r--r--   0        0        0     1484 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/26access_token_last_validated.sql
--rw-r--r--   0        0        0     1376 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/27local_invites.sql
--rw-r--r--   0        0        0      660 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.postgres
--rw-r--r--   0        0        0     2126 2024-01-16 15:31:37.130680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.sqlite
--rw-r--r--   0        0        0     3324 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/01ignored_user.py
--rw-r--r--   0        0        0     1495 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/02shard_send_to_device.sql
--rw-r--r--   0        0        0      999 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/03shard_send_to_device_sequence.sql.postgres
--rw-r--r--   0        0        0     2381 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql
--rw-r--r--   0        0        0      663 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql.postgres
--rw-r--r--   0        0        0     1433 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/04drop_account_data.sql
--rw-r--r--   0        0        0     1432 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/05cache_invalidation.sql
--rw-r--r--   0        0        0     1452 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/06chain_cover_index.sql
--rw-r--r--   0        0        0     1548 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/06shard_account_data.sql
--rw-r--r--   0        0        0     1193 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/06shard_account_data.sql.postgres
--rw-r--r--   0        0        0     1503 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/07shard_account_data_fix.sql
--rw-r--r--   0        0        0     1542 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/08delete_pushers_for_deactivated_accounts.sql
--rw-r--r--   0        0        0     1569 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/08delete_stale_pushers.sql
--rw-r--r--   0        0        0     1975 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/09rejected_events_metadata.sql
--rw-r--r--   0        0        0     1420 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/10delete_purged_chain_cover.sql
--rw-r--r--   0        0        0     1595 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/11add_knock_members_to_stats.sql
--rw-r--r--   0        0        0     1008 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/11drop_thumbnail_constraint.sql.postgres
--rw-r--r--   0        0        0     1520 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/12account_validity_token_used_ts_ms.sql
--rw-r--r--   0        0        0     1503 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/12presence_stream_instance.sql
--rw-r--r--   0        0        0      777 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/12presence_stream_instance_seq.sql.postgres
--rw-r--r--   0        0        0     2268 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/13users_to_send_full_presence_to.sql
--rw-r--r--   0        0        0     1960 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/14refresh_tokens.sql
--rw-r--r--   0        0        0     2352 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/15locks.sql
--rw-r--r--   0        0        0     2020 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/16federation_inbound_staging.sql
--rw-r--r--   0        0        0     2254 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/60/01recreate_stream_ordering.sql.postgres
--rw-r--r--   0        0        0     1480 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/60/02change_stream_ordering_columns.sql.postgres
--rw-r--r--   0        0        0     1083 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/01change_appservices_txns.sql.postgres
--rw-r--r--   0        0        0     2952 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/01insertion_event_lookups.sql
--rw-r--r--   0        0        0     1416 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/02drop_redundant_room_depth_index.sql
--rw-r--r--   0        0        0     2366 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/03recreate_min_depth.py
--rw-r--r--   0        0        0     1718 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/62/01insertion_event_extremities.sql
--rw-r--r--   0        0        0     1845 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/01create_registration_tokens.sql
--rw-r--r--   0        0        0     1570 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/02delete_unlinked_email_pushers.sql
--rw-r--r--   0        0        0     1432 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/02populate-rooms-creator.sql
--rw-r--r--   0        0        0     1697 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/03session_store.sql
--rw-r--r--   0        0        0     1439 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/04add_presence_stream_not_offline_index.sql
--rw-r--r--   0        0        0     1045 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.postgres
--rw-r--r--   0        0        0     1523 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.sqlite
--rw-r--r--   0        0        0     1579 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/01msc2716_insertion_event_edges.sql
--rw-r--r--   0        0        0     1638 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/03remove_hidden_devices_from_device_inbox.sql
--rw-r--r--   0        0        0     1477 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/04_local_group_updates.sql
--rw-r--r--   0        0        0     1531 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/05_remove_room_stats_historical_and_user_stats_historical.sql
--rw-r--r--   0        0        0     2334 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/06remove_deleted_devices_from_device_inbox.sql
--rw-r--r--   0        0        0     1468 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/07_arbitrary_relations.sql
--rw-r--r--   0        0        0     1511 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/08_device_inbox_background_updates.sql
--rw-r--r--   0        0        0     1913 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/10_expirable_refresh_tokens.sql
--rw-r--r--   0        0        0     1753 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/11_devices_auth_provider_session.sql
--rw-r--r--   0        0        0     1384 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/67/01drop_public_room_list_stream.sql
--rw-r--r--   0        0        0     1671 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/01event_columns.sql
--rw-r--r--   0        0        0     1657 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/02_msc2409_add_device_id_appservice_stream_type.sql
--rw-r--r--   0        0        0     1535 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/03_delete_account_data_for_deactivated_accounts.sql
--rw-r--r--   0        0        0     1976 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/04_refresh_tokens_index_next_token_id.sql
--rw-r--r--   0        0        0     2274 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/04partial_state_rooms.sql
--rw-r--r--   0        0        0      968 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/05_delete_non_strings_from_event_search.sql.sqlite
--rw-r--r--   0        0        0     2899 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/05partial_state_rooms_triggers.py
--rw-r--r--   0        0        0     1771 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/06_msc3202_add_device_list_appservice_stream_type.sql
--rw-r--r--   0        0        0     1945 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/69/01as_txn_seq.py
--rw-r--r--   0        0        0     2446 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/69/01device_list_oubound_by_room.sql
--rw-r--r--   0        0        0     1510 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/69/02cache_invalidation_index.sql
--rw-r--r--   0        0        0     1566 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/70/01clean_table_purged_rooms.sql
--rw-r--r--   0        0        0     2096 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.postgres
--rw-r--r--   0        0        0     1800 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.sqlite
--rw-r--r--   0        0        0     3821 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/01remove_noop_background_updates.sql
--rw-r--r--   0        0        0     1478 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/02event_push_summary_unique.sql
--rw-r--r--   0        0        0     1457 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/01add_room_type_to_state_stats.sql
--rw-r--r--   0        0        0     2167 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/01event_push_summary_receipt.sql
--rw-r--r--   0        0        0     1541 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/02event_push_actions_index.sql
--rw-r--r--   0        0        0     2085 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/03bg_populate_events_columns.py
--rw-r--r--   0        0        0     1394 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/03drop_event_reference_hashes.sql
--rw-r--r--   0        0        0     1998 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/03remove_groups.sql
--rw-r--r--   0        0        0      730 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.postgres
--rw-r--r--   0        0        0     1338 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.sqlite
--rw-r--r--   0        0        0     1464 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/05receipts_event_stream_ordering.sql
--rw-r--r--   0        0        0     1583 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/05remove_unstable_private_read_receipts.sql
--rw-r--r--   0        0        0     1345 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/06add_consent_ts_to_users.sql
--rw-r--r--   0        0        0     2052 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/06thread_notifications.sql
--rw-r--r--   0        0        0     2031 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/07force_update_current_state_events_membership.py
--rw-r--r--   0        0        0     1249 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/07thread_receipts.sql.postgres
--rw-r--r--   0        0        0     2741 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/07thread_receipts.sql.sqlite
--rw-r--r--   0        0        0     1007 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/08begin_cache_invalidation_seq_at_2.sql.postgres
--rw-r--r--   0        0        0     1558 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/08thread_receipts.sql
--rw-r--r--   0        0        0     2347 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/09partial_indices.sql.sqlite
--rw-r--r--   0        0        0     1912 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/01event_failed_pull_attempts.sql
--rw-r--r--   0        0        0     1351 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/02add_pusher_enabled.sql
--rw-r--r--   0        0        0     1728 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/02room_id_indexes_for_purging.sql
--rw-r--r--   0        0        0     1704 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/03pusher_device_id.sql
--rw-r--r--   0        0        0     1584 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/03users_approved_column.sql
--rw-r--r--   0        0        0     1879 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/04partial_join_details.sql
--rw-r--r--   0        0        0     1850 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/04pending_device_list_updates.sql
--rw-r--r--   0        0        0     1038 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/05old_push_actions.sql.postgres
--rw-r--r--   0        0        0     1097 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/05old_push_actions.sql.sqlite
--rw-r--r--   0        0        0     1765 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/06thread_notifications_thread_id_idx.sql
--rw-r--r--   0        0        0      881 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.postgres
--rw-r--r--   0        0        0     2896 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.sqlite
--rw-r--r--   0        0        0     1516 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/09partial_joined_via_destination.sql
--rw-r--r--   0        0        0     1893 2024-01-16 15:31:37.134680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/09threads_table.sql
--rw-r--r--   0        0        0     2185 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/10_update_sqlite_fts4_tokenizer.py
--rw-r--r--   0        0        0     1938 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/10login_tokens.sql
--rw-r--r--   0        0        0     1595 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/11event_search_room_id_n_distinct.sql.postgres
--rw-r--r--   0        0        0     3153 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/12refactor_device_list_outbound_pokes.sql
--rw-r--r--   0        0        0     1553 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/13add_device_lists_index.sql
--rw-r--r--   0        0        0     2068 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/20_un_partial_stated_room_stream.sql
--rw-r--r--   0        0        0      819 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/21_un_partial_stated_room_stream_seq.sql.postgres
--rw-r--r--   0        0        0     2240 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/22_rebuild_user_dir_stats.sql
--rw-r--r--   0        0        0     2078 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/22_un_partial_stated_event_stream.sql
--rw-r--r--   0        0        0     2277 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/23_fix_thread_index.sql
--rw-r--r--   0        0        0      822 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/23_un_partial_stated_room_stream_seq.sql.postgres
--rw-r--r--   0        0        0     1426 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/24_events_jump_to_date_index.sql
--rw-r--r--   0        0        0     1349 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/25drop_presence.sql
--rw-r--r--   0        0        0     2420 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/01_user_directory_stale_remote_users.sql
--rw-r--r--   0        0        0     1554 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/02_set_device_id_for_pushers_bg_update.sql
--rw-r--r--   0        0        0     1655 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.postgres
--rw-r--r--   0        0        0     1183 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.sqlite
--rw-r--r--   0        0        0     1537 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/03_room_membership_index.sql
--rw-r--r--   0        0        0     1444 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/04_delete_e2e_backup_keys_for_deactivated_users.sql
--rw-r--r--   0        0        0     3140 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/04_membership_tables_event_stream_ordering_triggers.py
--rw-r--r--   0        0        0     3002 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/05_events_txn_id_device_id.sql
--rw-r--r--   0        0        0     2422 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/90COMMENTS_destinations.sql.postgres
--rw-r--r--   0        0        0     1581 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/01_add_profiles_full_user_id_column.sql
--rw-r--r--   0        0        0     1577 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/02_add_user_filters_full_user_id_column.sql
--rw-r--r--   0        0        0     1798 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/03_per_user_experimental_features.sql
--rw-r--r--   0        0        0     1602 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/04_add_room_forgetter.sql
--rw-r--r--   0        0        0      713 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/01_add_profiles_not_valid_check.sql.postgres
--rw-r--r--   0        0        0      717 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/02_add_user_filters_not_valid_check.sql.postgres
--rw-r--r--   0        0        0     1428 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/03bg_populate_full_user_id_profiles.sql
--rw-r--r--   0        0        0     1432 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/04bg_populate_full_user_id_user_filters.sql
--rw-r--r--   0        0        0     3164 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/05thread_notifications_backfill.sql
--rw-r--r--   0        0        0     4506 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null.sql.sqlite
--rw-r--r--   0        0        0     1347 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions.sql.postgres
--rw-r--r--   0        0        0     1319 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions_staging.sql.postgres
--rw-r--r--   0        0        0     1465 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_summary.sql.postgres
--rw-r--r--   0        0        0     1584 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/14bg_indices_event_stream_ordering.sql
--rw-r--r--   0        0        0     3171 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/01_validate_and_update_profiles.py
--rw-r--r--   0        0        0     3190 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/02_validate_and_update_user_filters.py
--rw-r--r--   0        0        0     2243 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/03_remove_unused_indexes_user_filters.py
--rw-r--r--   0        0        0     2489 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/03event_extremities_constraints.py
--rw-r--r--   0        0        0     1127 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/04_add_full_user_id_index_user_filters.py
--rw-r--r--   0        0        0     5225 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.postgres
--rw-r--r--   0        0        0     3690 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.sqlite
--rw-r--r--   0        0        0     2953 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/04_mitigate_stream_ordering_update_race.py
--rw-r--r--   0        0        0     2763 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.postgres
--rw-r--r--   0        0        0     2853 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.sqlite
--rw-r--r--   0        0        0     1366 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/01_users_alter_locked.sql
--rw-r--r--   0        0        0     1512 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/02_read_write_locks_unlogged.sql.postgres
--rw-r--r--   0        0        0     1670 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/02_scheduled_tasks.sql
--rw-r--r--   0        0        0     1544 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/03_read_write_locks_triggers.sql.postgres
--rw-r--r--   0        0        0     2625 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/04_read_write_locks_deadlock.sql.postgres
--rw-r--r--   0        0        0     1388 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/82/02_scheduled_tasks_index.sql
--rw-r--r--   0        0        0     1561 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/82/04_add_indices_for_purging_rooms.sql
--rw-r--r--   0        0        0     1741 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/82/05gaps.sql
--rw-r--r--   0        0        0     1688 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/01_drop_old_tables.sql
--rw-r--r--   0        0        0      711 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/03_instance_name_receipts.sql.sqlite
--rw-r--r--   0        0        0     1401 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/05_cross_signing_key_update_grant.sql
--rw-r--r--   0        0        0     1435 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/06_event_push_summary_room.sql
--rw-r--r--   0        0        0    53196 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/full_schemas/72/full.sql.postgres
--rw-r--r--   0        0        0    42458 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/main/full_schemas/72/full.sql.sqlite
--rw-r--r--   0        0        0     1340 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/23/drop_state_index.sql
--rw-r--r--   0        0        0     1439 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/32/remove_state_indices.sql
--rw-r--r--   0        0        0     1445 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/35/add_state_index.sql
--rw-r--r--   0        0        0     1543 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/35/state.sql
--rw-r--r--   0        0        0     1401 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/35/state_dedupe.sql
--rw-r--r--   0        0        0     1356 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/47/state_group_seq.py
--rw-r--r--   0        0        0     1412 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/56/state_group_room_idx.sql
--rw-r--r--   0        0        0     1662 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/61/02state_groups_state_n_distinct.sql.postgres
--rw-r--r--   0        0        0     1431 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/delta/70/08_state_group_edges_unique.sql
--rw-r--r--   0        0        0     1128 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/full_schemas/72/full.sql.postgres
--rw-r--r--   0        0        0      741 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/schema/state/full_schemas/72/full.sql.sqlite
--rw-r--r--   0        0        0     6638 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/types.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/util/__init__.py
--rw-r--r--   0        0        0    38595 2024-01-16 15:31:37.138680 matrix_synapse-1.99.0/synapse/storage/util/id_generators.py
--rw-r--r--   0        0        0     7348 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/storage/util/partial_state_events_tracker.py
--rw-r--r--   0        0        0    10025 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/storage/util/sequence.py
--rw-r--r--   0        0        0     1257 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/streams/__init__.py
--rw-r--r--   0        0        0     2984 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/streams/config.py
--rw-r--r--   0        0        0     4802 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/streams/events.py
--rw-r--r--   0        0        0      125 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/synapse_rust/__init__.pyi
--rw-r--r--   0        0        0      828 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/synapse_rust/acl.pyi
--rw-r--r--   0        0        0     4168 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/synapse_rust/events.pyi
--rw-r--r--   0        0        0     2542 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/synapse_rust/push.pyi
--rw-r--r--   0        0        0    41228 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/types/__init__.py
--rw-r--r--   0        0        0    21806 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/types/state.py
--rw-r--r--   0        0        0     7308 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/__init__.py
--rw-r--r--   0        0        0    31245 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/async_helpers.py
--rw-r--r--   0        0        0     6419 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/batching_queue.py
--rw-r--r--   0        0        0     8361 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/__init__.py
--rw-r--r--   0        0        0     5450 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/cached_call.py
--rw-r--r--   0        0        0    18245 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/deferred_cache.py
--rw-r--r--   0        0        0    23181 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/descriptors.py
--rw-r--r--   0        0        0    11916 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/dictionary_cache.py
--rw-r--r--   0        0        0     7400 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/expiringcache.py
--rw-r--r--   0        0        0    30017 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/lrucache.py
--rw-r--r--   0        0        0     9404 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/response_cache.py
--rw-r--r--   0        0        0    11712 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/stream_change_cache.py
--rw-r--r--   0        0        0     5893 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/treecache.py
--rw-r--r--   0        0        0     5301 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/caches/ttlcache.py
--rw-r--r--   0        0        0     2466 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/cancellation.py
--rw-r--r--   0        0        0     8054 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/check_dependencies.py
--rw-r--r--   0        0        0     5048 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/daemonize.py
--rw-r--r--   0        0        0     5016 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/distributor.py
--rw-r--r--   0        0        0     6349 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/file_consumer.py
--rw-r--r--   0        0        0     1380 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/frozenutils.py
--rw-r--r--   0        0        0     5214 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/gai_resolver.py
--rw-r--r--   0        0        0     1106 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/hash.py
--rw-r--r--   0        0        0     4273 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/httpresourcetree.py
--rw-r--r--   0        0        0     5494 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/iterutils.py
--rw-r--r--   0        0        0     5083 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/linked_list.py
--rw-r--r--   0        0        0     1219 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/logcontext.py
--rw-r--r--   0        0        0      845 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/logformatter.py
--rw-r--r--   0        0        0    12051 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/macaroons.py
--rw-r--r--   0        0        0     8317 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/manhole.py
--rw-r--r--   0        0        0     7795 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/metrics.py
--rw-r--r--   0        0        0     4003 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/module_loader.py
--rw-r--r--   0        0        0     1641 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/msisdn.py
--rw-r--r--   0        0        0     9125 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/patch_inline_callbacks.py
--rw-r--r--   0        0        0    13544 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/ratelimitutils.py
--rw-r--r--   0        0        0    12127 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/retryutils.py
--rw-r--r--   0        0        0     1317 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/rlimit.py
--rw-r--r--   0        0        0     2607 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/rust.py
--rw-r--r--   0        0        0     8229 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/stringutils.py
--rw-r--r--   0        0        0    15870 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/task_scheduler.py
--rw-r--r--   0        0        0     4040 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/templates.py
--rw-r--r--   0        0        0     3745 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/threepids.py
--rw-r--r--   0        0        0     3599 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/util/wheel_timer.py
--rw-r--r--   0        0        0    30251 2024-01-16 15:31:37.142680 matrix_synapse-1.99.0/synapse/visibility.py
--rw-r--r--   0        0        0     1354 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/synmark/__init__.py
--rw-r--r--   0        0        0     3657 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/synmark/__main__.py
--rw-r--r--   0        0        0      176 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/synmark/suites/__init__.py
--rw-r--r--   0        0        0     4380 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/synmark/suites/logging.py
--rw-r--r--   0        0        0     1134 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/synmark/suites/lrucache.py
--rw-r--r--   0        0        0     1157 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/synmark/suites/lrucache_evict.py
--rw-r--r--   0        0        0     1610 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/sytest-blacklist
--rw-r--r--   0        0        0      869 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/api/__init__.py
--rw-r--r--   0        0        0    23538 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/api/test_auth.py
--rw-r--r--   0        0        0     1882 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/api/test_errors.py
--rw-r--r--   0        0        0    23756 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/api/test_filtering.py
--rw-r--r--   0        0        0    16009 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/api/test_ratelimiting.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/app/__init__.py
--rw-r--r--   0        0        0     1594 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/app/test_homeserver_start.py
--rw-r--r--   0        0        0     4695 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/app/test_openid_listener.py
--rw-r--r--   0        0        0    10015 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/app/test_phone_stats_home.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/appservice/__init__.py
--rw-r--r--   0        0        0     9001 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/appservice/test_api.py
--rw-r--r--   0        0        0     9396 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/appservice/test_appservice.py
--rw-r--r--   0        0        0    17606 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/appservice/test_scheduler.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/__init__.py
--rw-r--r--   0        0        0     1310 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test___main__.py
--rw-r--r--   0        0        0     4054 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_api.py
--rw-r--r--   0        0        0     1512 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_appservice.py
--rw-r--r--   0        0        0     2588 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_background_update.py
--rw-r--r--   0        0        0     5501 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_base.py
--rw-r--r--   0        0        0     6761 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_cache.py
--rw-r--r--   0        0        0     1212 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_database.py
--rw-r--r--   0        0        0     2244 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_generate.py
--rw-r--r--   0        0        0     5012 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_load.py
--rw-r--r--   0        0        0    11062 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_oauth_delegation.py
--rw-r--r--   0        0        0     2507 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_ratelimiting.py
--rw-r--r--   0        0        0     3739 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_registration_config.py
--rw-r--r--   0        0        0     4922 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_room_directory.py
--rw-r--r--   0        0        0     6474 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_server.py
--rw-r--r--   0        0        0     7846 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_tls.py
--rw-r--r--   0        0        0     1792 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_util.py
--rw-r--r--   0        0        0    12025 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/test_workers.py
--rw-r--r--   0        0        0     2058 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/config/utils.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/crypto/__init__.py
--rw-r--r--   0        0        0     3661 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/crypto/test_event_signing.py
--rw-r--r--   0        0        0    27314 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/crypto/test_keyring.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/events/__init__.py
--rw-r--r--   0        0        0    18867 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/events/test_presence_router.py
--rw-r--r--   0        0        0     4154 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/events/test_snapshot.py
--rw-r--r--   0        0        0    28325 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/events/test_utils.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/__init__.py
--rw-r--r--   0        0        0     9343 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/test_complexity.py
--rw-r--r--   0        0        0    22608 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/test_federation_catch_up.py
--rw-r--r--   0        0        0    11712 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/test_federation_client.py
--rw-r--r--   0        0        0    28083 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/test_federation_sender.py
--rw-r--r--   0        0        0    13571 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/test_federation_server.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/transport/__init__.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/transport/server/__init__.py
--rw-r--r--   0        0        0     5028 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/transport/server/test__base.py
--rw-r--r--   0        0        0     5870 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/transport/test_client.py
--rw-r--r--   0        0        0    12138 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/transport/test_knocking.py
--rw-r--r--   0        0        0     2408 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/federation/transport/test_server.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/handlers/__init__.py
--rw-r--r--   0        0        0      241 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/handlers/oidc_test_key.p8
--rw-r--r--   0        0        0      178 2024-01-16 15:31:37.146679 matrix_synapse-1.99.0/tests/handlers/oidc_test_key.pub.pem
--rw-r--r--   0        0        0    13984 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_admin.py
--rw-r--r--   0        0        0    50710 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_appservice.py
--rw-r--r--   0        0        0     8362 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_auth.py
--rw-r--r--   0        0        0     8214 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_cas.py
--rw-r--r--   0        0        0    11342 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_deactivate_account.py
--rw-r--r--   0        0        0    23221 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_device.py
--rw-r--r--   0        0        0    21741 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_directory.py
--rw-r--r--   0        0        0    63167 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_e2e_keys.py
--rw-r--r--   0        0        0    19558 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_e2e_room_keys.py
--rw-r--r--   0        0        0    30062 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_federation.py
--rw-r--r--   0        0        0    47947 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_federation_event.py
--rw-r--r--   0        0        0    13092 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_message.py
--rw-r--r--   0        0        0    32877 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_oauth_delegation.py
--rw-r--r--   0        0        0    54346 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_oidc.py
--rw-r--r--   0        0        0    38830 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_password_providers.py
--rw-r--r--   0        0        0    71302 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_presence.py
--rw-r--r--   0        0        0    14047 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_profile.py
--rw-r--r--   0        0        0    12352 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_receipts.py
--rw-r--r--   0        0        0    32054 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_register.py
--rw-r--r--   0        0        0     4317 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_room.py
--rw-r--r--   0        0        0     2832 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_room_list.py
--rw-r--r--   0        0        0    16212 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_room_member.py
--rw-r--r--   0        0        0    41655 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_room_summary.py
--rw-r--r--   0        0        0    13234 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_saml.py
--rw-r--r--   0        0        0     8030 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_send_email.py
--rw-r--r--   0        0        0     5689 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_sso.py
--rw-r--r--   0        0        0    19776 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_stats.py
--rw-r--r--   0        0        0    12118 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_sync.py
--rw-r--r--   0        0        0    16574 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_typing.py
--rw-r--r--   0        0        0    52141 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_user_directory.py
--rw-r--r--   0        0        0     2707 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/handlers/test_worker_lock.py
--rw-r--r--   0        0        0     5777 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/http/__init__.py
--rw-r--r--   0        0        0     1115 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/http/ca.crt
--rw-r--r--   0        0        0     1679 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/http/ca.key
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/http/federation/__init__.py
--rw-r--r--   0        0        0    67753 2024-01-16 15:31:37.150680 matrix_synapse-1.99.0/tests/http/federation/test_matrix_federation_agent.py
--rw-r--r--   0        0        0     7864 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/federation/test_srv_resolver.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/server/__init__.py
--rw-r--r--   0        0        0    22077 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/server/_base.py
--rw-r--r--   0        0        0     1679 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/server.key
--rw-r--r--   0        0        0     2578 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_additional_resource.py
--rw-r--r--   0        0        0     9164 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_client.py
--rw-r--r--   0        0        0     2114 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_endpoint.py
--rw-r--r--   0        0        0    34255 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_matrixfederationclient.py
--rw-r--r--   0        0        0     2016 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_proxy.py
--rw-r--r--   0        0        0    34549 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_proxyagent.py
--rw-r--r--   0        0        0     4898 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_servlet.py
--rw-r--r--   0        0        0     6225 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_simple_client.py
--rw-r--r--   0        0        0     3269 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/http/test_site.py
--rw-r--r--   0        0        0     1355 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/logging/__init__.py
--rw-r--r--   0        0        0    10995 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/logging/test_opentracing.py
--rw-r--r--   0        0        0     6430 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/logging/test_remote_handler.py
--rw-r--r--   0        0        0     8219 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/logging/test_terse_json.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/__init__.py
--rw-r--r--   0        0        0     3397 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_base.py
--rw-r--r--   0        0        0    23048 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_filepath.py
--rw-r--r--   0        0        0    20965 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_html_preview.py
--rw-r--r--   0        0        0    11477 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_media_retention.py
--rw-r--r--   0        0        0    30878 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_media_storage.py
--rw-r--r--   0        0        0     6835 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_oembed.py
--rw-r--r--   0        0        0     4477 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/media/test_url_previewer.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/metrics/__init__.py
--rw-r--r--   0        0        0      774 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/metrics/test_background_process_metrics.py
--rw-r--r--   0        0        0     7242 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/metrics/test_metrics.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/module_api/__init__.py
--rw-r--r--   0        0        0     5868 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/module_api/test_account_data_manager.py
--rw-r--r--   0        0        0    39878 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/module_api/test_api.py
--rw-r--r--   0        0        0     2273 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/module_api/test_event_unsigned_addition.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/push/__init__.py
--rw-r--r--   0        0        0    16883 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/push/test_bulk_push_rule_evaluator.py
--rw-r--r--   0        0        0    20451 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/push/test_email.py
--rw-r--r--   0        0        0    39462 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/push/test_http.py
--rw-r--r--   0        0        0     9210 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/push/test_presentable_names.py
--rw-r--r--   0        0        0    32846 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/push/test_push_rule_evaluator.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/__init__.py
--rw-r--r--   0        0        0    22959 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/_base.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/http/__init__.py
--rw-r--r--   0        0        0     3726 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/http/test__base.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/storage/__init__.py
--rw-r--r--   0        0        0     2911 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/storage/_base.py
--rw-r--r--   0        0        0    14928 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/storage/test_events.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/__init__.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/__init__.py
--rw-r--r--   0        0        0     4416 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_account_data.py
--rw-r--r--   0        0        0    20007 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_events.py
--rw-r--r--   0        0        0     3442 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_federation.py
--rw-r--r--   0        0        0     2341 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_partial_state.py
--rw-r--r--   0        0        0     3343 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_receipts.py
--rw-r--r--   0        0        0     3282 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_to_device.py
--rw-r--r--   0        0        0     6290 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/streams/test_typing.py
--rw-r--r--   0        0        0     1784 2024-01-16 15:31:37.154680 matrix_synapse-1.99.0/tests/replication/tcp/test_commands.py
--rw-r--r--   0        0        0     7871 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/tcp/test_handler.py
--rw-r--r--   0        0        0     4240 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_auth.py
--rw-r--r--   0        0        0     3304 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_client_reader_shard.py
--rw-r--r--   0        0        0     3561 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_federation_ack.py
--rw-r--r--   0        0        0     9938 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_federation_sender_shard.py
--rw-r--r--   0        0        0     2728 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_module_cache_invalidation.py
--rw-r--r--   0        0        0     9661 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_multi_media_repo.py
--rw-r--r--   0        0        0     6716 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_pusher_shard.py
--rw-r--r--   0        0        0    12184 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_sharded_event_persister.py
--rw-r--r--   0        0        0     8996 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/replication/test_sharded_receipts.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/__init__.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/__init__.py
--rw-r--r--   0        0        0    16729 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_admin.py
--rw-r--r--   0        0        0    12428 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_background_updates.py
--rw-r--r--   0        0        0    17488 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_device.py
--rw-r--r--   0        0        0    26187 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_event_reports.py
--rw-r--r--   0        0        0    29729 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_federation.py
--rw-r--r--   0        0        0     5528 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_jwks.py
--rw-r--r--   0        0        0    30136 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_media.py
--rw-r--r--   0        0        0    26019 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_registration_tokens.py
--rw-r--r--   0        0        0   106429 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_room.py
--rw-r--r--   0        0        0    27177 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_server_notice.py
--rw-r--r--   0        0        0    18242 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_statistics.py
--rw-r--r--   0        0        0   180599 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_user.py
--rw-r--r--   0        0        0     2902 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/admin/test_username_available.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/__init__.py
--rw-r--r--   0        0        0    51250 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_account.py
--rw-r--r--   0        0        0     2854 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_account_data.py
--rw-r--r--   0        0        0    55112 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_auth.py
--rw-r--r--   0        0        0     2135 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_auth_issuer.py
--rw-r--r--   0        0        0     9198 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_capabilities.py
--rw-r--r--   0        0        0     4639 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_consent.py
--rw-r--r--   0        0        0    22086 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_devices.py
--rw-r--r--   0        0        0     9548 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_directory.py
--rw-r--r--   0        0        0     4212 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_ephemeral_message.py
--rw-r--r--   0        0        0     5725 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_events.py
--rw-r--r--   0        0        0     4298 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_filter.py
--rw-r--r--   0        0        0     2240 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_identity.py
--rw-r--r--   0        0        0    15938 2024-01-16 15:31:37.158680 matrix_synapse-1.99.0/tests/rest/client/test_keys.py
--rw-r--r--   0        0        0    60842 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_login.py
--rw-r--r--   0        0        0     6390 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_login_token_request.py
--rw-r--r--   0        0        0     3025 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_models.py
--rw-r--r--   0        0        0     5833 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_mutual_rooms.py
--rw-r--r--   0        0        0     3444 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_notifications.py
--rw-r--r--   0        0        0     6708 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_password_policy.py
--rw-r--r--   0        0        0     9713 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_power_levels.py
--rw-r--r--   0        0        0     3267 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_presence.py
--rw-r--r--   0        0        0    23618 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_profile.py
--rw-r--r--   0        0        0    16982 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_push_rule_attrs.py
--rw-r--r--   0        0        0     5073 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_read_marker.py
--rw-r--r--   0        0        0    10434 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_receipts.py
--rw-r--r--   0        0        0    25015 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_redactions.py
--rw-r--r--   0        0        0    46981 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_register.py
--rw-r--r--   0        0        0    76170 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_relations.py
--rw-r--r--   0        0        0     1733 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_rendezvous.py
--rw-r--r--   0        0        0     5321 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_report_event.py
--rw-r--r--   0        0        0    15135 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_retention.py
--rw-r--r--   0        0        0   138187 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_rooms.py
--rw-r--r--   0        0        0     9195 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_sendtodevice.py
--rw-r--r--   0        0        0    12034 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_shadow_banned.py
--rw-r--r--   0        0        0    29719 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_sync.py
--rw-r--r--   0        0        0    40200 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_third_party_rules.py
--rw-r--r--   0        0        0     7353 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_transactions.py
--rw-r--r--   0        0        0     3641 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_typing.py
--rw-r--r--   0        0        0    15000 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/test_upgrade_room.py
--rw-r--r--   0        0        0    31031 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/client/utils.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/key/__init__.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/key/v2/__init__.py
--rw-r--r--   0        0        0    10798 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/key/v2/test_remote_key_resource.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/media/__init__.py
--rw-r--r--   0        0        0     5173 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/media/test_domain_blocking.py
--rw-r--r--   0        0        0    50512 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/media/test_url_preview.py
--rw-r--r--   0        0        0     1155 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/test_health.py
--rw-r--r--   0        0        0     4587 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/rest/test_well_known.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/scripts/__init__.py
--rw-r--r--   0        0        0     5336 2024-01-16 15:31:37.162680 matrix_synapse-1.99.0/tests/scripts/test_new_matrix_user.py
--rw-r--r--   0        0        0    37558 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/server.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/server_notices/__init__.py
--rw-r--r--   0        0        0     3788 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/server_notices/test_consent.py
--rw-r--r--   0        0        0    16949 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/server_notices/test_resource_limits_server_notices.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/state/__init__.py
--rw-r--r--   0        0        0    28495 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/state/test_v2.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/__init__.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/__init__.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/__init__.py
--rw-r--r--   0        0        0     4369 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_cache.py
--rw-r--r--   0        0        0     5622 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_deviceinbox.py
--rw-r--r--   0        0        0     4454 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_end_to_end_keys.py
--rw-r--r--   0        0        0    21176 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_events_worker.py
--rw-r--r--   0        0        0    17709 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_lock.py
--rw-r--r--   0        0        0     8197 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_receipts.py
--rw-r--r--   0        0        0     6487 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/databases/main/test_room.py
--rw-r--r--   0        0        0     5037 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test__base.py
--rw-r--r--   0        0        0     6161 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_account_data.py
--rw-r--r--   0        0        0    19190 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_appservice.py
--rw-r--r--   0        0        0    23920 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_background_update.py
--rw-r--r--   0        0        0    28636 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_base.py
--rw-r--r--   0        0        0    14112 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_cleanup_extrems.py
--rw-r--r--   0        0        0    25377 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_client_ips.py
--rw-r--r--   0        0        0    10724 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_database.py
--rw-r--r--   0        0        0    12903 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_devices.py
--rw-r--r--   0        0        0     2509 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_directory.py
--rw-r--r--   0        0        0     2942 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_e2e_room_keys.py
--rw-r--r--   0        0        0     4205 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_end_to_end_keys.py
--rw-r--r--   0        0        0    26823 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_event_chain.py
--rw-r--r--   0        0        0    42747 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_event_federation.py
--rw-r--r--   0        0        0     3537 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_event_metrics.py
--rw-r--r--   0        0        0    26944 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_event_push_actions.py
--rw-r--r--   0        0        0    18601 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_events.py
--rw-r--r--   0        0        0    38215 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_id_generators.py
--rw-r--r--   0        0        0     1752 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_main.py
--rw-r--r--   0        0        0    19617 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_monthly_active_users.py
--rw-r--r--   0        0        0     4507 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_profile.py
--rw-r--r--   0        0        0     5061 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_purge.py
--rw-r--r--   0        0        0    10522 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_receipts.py
--rw-r--r--   0        0        0    15764 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_redaction.py
--rw-r--r--   0        0        0    10381 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_registration.py
--rw-r--r--   0        0        0     4438 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_relations.py
--rw-r--r--   0        0        0     4688 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_rollback_worker.py
--rw-r--r--   0        0        0     2515 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_room.py
--rw-r--r--   0        0        0    14415 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_room_search.py
--rw-r--r--   0        0        0    10196 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_roommember.py
--rw-r--r--   0        0        0    23509 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_state.py
--rw-r--r--   0        0        0     9646 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_stream.py
--rw-r--r--   0        0        0     2669 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_transactions.py
--rw-r--r--   0        0        0     1651 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_txn_limit.py
--rw-r--r--   0        0        0     2076 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_unsafe_locale.py
--rw-r--r--   0        0        0    28251 2024-01-16 15:31:37.166679 matrix_synapse-1.99.0/tests/storage/test_user_directory.py
--rw-r--r--   0        0        0     3402 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/storage/test_user_filters.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/storage/util/__init__.py
--rw-r--r--   0        0        0     6652 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/storage/util/test_partial_state_events_tracker.py
--rw-r--r--   0        0        0     2162 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_distributor.py
--rw-r--r--   0        0        0    32364 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_event_auth.py
--rw-r--r--   0        0        0    14817 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_federation.py
--rw-r--r--   0        0        0    12070 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_mau.py
--rw-r--r--   0        0        0     3546 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_phone_home.py
--rw-r--r--   0        0        0      291 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_rust.py
--rw-r--r--   0        0        0    18805 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_server.py
--rw-r--r--   0        0        0    30235 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_state.py
--rw-r--r--   0        0        0     4963 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_terms_auth.py
--rw-r--r--   0        0        0     1918 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_test_utils.py
--rw-r--r--   0        0        0     4581 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_types.py
--rw-r--r--   0        0        0     4144 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     3982 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_utils/event_injection.py
--rw-r--r--   0        0        0     2013 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_utils/html_parsers.py
--rw-r--r--   0        0        0     2616 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_utils/logging_setup.py
--rw-r--r--   0        0        0    12179 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_utils/oidc.py
--rw-r--r--   0        0        0    12980 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/test_visibility.py
--rw-r--r--   0        0        0        0 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/types/__init__.py
--rw-r--r--   0        0        0    21259 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/types/test_state.py
--rw-r--r--   0        0        0    35404 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/unittest.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/__init__.py
--rw-r--r--   0        0        0      673 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/caches/__init__.py
--rw-r--r--   0        0        0     5314 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/caches/test_cached_call.py
--rw-r--r--   0        0        0     9612 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/caches/test_deferred_cache.py
--rw-r--r--   0        0        0    34232 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/caches/test_descriptors.py
--rw-r--r--   0        0        0     7480 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/caches/test_response_cache.py
--rw-r--r--   0        0        0     3010 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/caches/test_ttlcache.py
--rw-r--r--   0        0        0    20487 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_async_helpers.py
--rw-r--r--   0        0        0     9316 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_batching_queue.py
--rw-r--r--   0        0        0     7228 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_check_dependencies.py
--rw-r--r--   0        0        0     4285 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_dict_cache.py
--rw-r--r--   0        0        0     3091 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_expiring_cache.py
--rw-r--r--   0        0        0     6212 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_file_consumer.py
--rw-r--r--   0        0        0     6342 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_itertools.py
--rw-r--r--   0        0        0     8666 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_linearizer.py
--rw-r--r--   0        0        0     7004 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_logcontext.py
--rw-r--r--   0        0        0     1235 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_logformatter.py
--rw-r--r--   0        0        0    12339 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_lrucache.py
--rw-r--r--   0        0        0     5269 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_macaroons.py
--rw-r--r--   0        0        0     5134 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_ratelimitutils.py
--rw-r--r--   0        0        0     8654 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_retryutils.py
--rw-r--r--   0        0        0    16797 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_rwlock.py
--rw-r--r--   0        0        0     9891 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_stream_change_cache.py
--rw-r--r--   0        0        0     1863 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_stringutils.py
--rw-r--r--   0        0        0     8794 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_task_scheduler.py
--rw-r--r--   0        0        0     1903 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_threepids.py
--rw-r--r--   0        0        0     3158 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_treecache.py
--rw-r--r--   0        0        0     2758 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/util/test_wheel_timer.py
--rw-r--r--   0        0        0    13230 2024-01-16 15:31:37.170679 matrix_synapse-1.99.0/tests/utils.py
--rw-r--r--   0        0        0    20799 1970-01-01 00:00:00.000000 matrix_synapse-1.99.0/setup.py
--rw-r--r--   0        0        0    15125 1970-01-01 00:00:00.000000 matrix_synapse-1.99.0/PKG-INFO
+-rw-r--r--   0        0        0     1611 2024-01-09 15:11:25.366849 matrix_synapse-1.99.0rc1/AUTHORS.rst
+-rw-r--r--   0        0        0   193819 2024-01-09 15:11:25.366849 matrix_synapse-1.99.0rc1/CHANGES.md
+-rw-r--r--   0        0        0      171 2024-01-09 15:11:25.366849 matrix_synapse-1.99.0rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    12715 2024-01-09 15:11:25.366849 matrix_synapse-1.99.0rc1/Cargo.lock
+-rw-r--r--   0        0        0      185 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/Cargo.toml
+-rw-r--r--   0        0        0      283 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/INSTALL.md
+-rw-r--r--   0        0        0    34523 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/LICENSE
+-rw-r--r--   0        0        0    11376 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/README.rst
+-rw-r--r--   0        0        0      257 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/UPGRADE.rst
+-rw-r--r--   0        0        0     1497 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/book.toml
+-rw-r--r--   0        0        0      791 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/build_rust.py
+-rw-r--r--   0        0        0       12 2024-01-09 15:11:25.370849 matrix_synapse-1.99.0rc1/changelog.d/.gitignore
+-rw-r--r--   0        0        0       74 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/demo/.gitignore
+-rwxr-xr-x   0        0        0      350 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/demo/clean.sh
+-rwxr-xr-x   0        0        0     4440 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/demo/start.sh
+-rwxr-xr-x   0        0        0      262 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/demo/stop.sh
+-rw-r--r--   0        0        0      655 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/.sample_config_header.yaml
+-rw-r--r--   0        0        0     1699 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/CAPTCHA_SETUP.md
+-rw-r--r--   0        0        0     3101 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/README.md
+-rw-r--r--   0        0        0     6076 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/SUMMARY.md
+-rw-r--r--   0        0        0      664 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/README.rst
+-rw-r--r--   0        0        0     1273 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/account_validity.md
+-rw-r--r--   0        0        0     6691 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/event_reports.md
+-rw-r--r--   0        0        0     1612 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/experimental_features.md
+-rw-r--r--   0        0        0     7123 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/media_admin_api.md
+-rw-r--r--   0        0        0     2183 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/purge_history_api.md
+-rw-r--r--   0        0        0     2641 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/register_api.md
+-rw-r--r--   0        0        0      832 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/room_membership.md
+-rw-r--r--   0        0        0    35435 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/rooms.md
+-rw-r--r--   0        0        0     1124 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/server_notices.md
+-rw-r--r--   0        0        0     4325 2024-01-09 15:11:25.374849 matrix_synapse-1.99.0rc1/docs/admin_api/statistics.md
+-rw-r--r--   0        0        0    41604 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/admin_api/user_admin_api.md
+-rw-r--r--   0        0        0      480 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/admin_api/version_api.md
+-rw-r--r--   0        0        0     2896 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/ancient_architecture_notes.md
+-rw-r--r--   0        0        0     1250 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/application_services.md
+-rw-r--r--   0        0        0     3583 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/architecture.md
+-rw-r--r--   0        0        0      843 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/auth_chain_diff.dot
+-rw-r--r--   0        0        0    42427 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/auth_chain_diff.dot.png
+-rw-r--r--   0        0        0     7076 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/auth_chain_difference_algorithm.md
+-rw-r--r--   0        0        0    91114 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2019.md
+-rw-r--r--   0        0        0   178146 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2020.md
+-rw-r--r--   0        0        0   220505 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2021.md
+-rw-r--r--   0        0        0   267174 2024-01-09 15:11:25.378849 matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2022.md
+-rw-r--r--   0        0        0   257821 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-pre-1.0.md
+-rw-r--r--   0        0        0       55 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/changelogs/README.md
+-rw-r--r--   0        0        0     4424 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/code_style.md
+-rw-r--r--   0        0        0     7328 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/consent_tracking.md
+-rw-r--r--   0        0        0     4991 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/delegate.md
+-rw-r--r--   0        0        0     2554 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/deprecation_policy.md
+-rw-r--r--   0        0        0     2079 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/cas.md
+-rw-r--r--   0        0        0    23858 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/contributing_guide.md
+-rw-r--r--   0        0        0    17629 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/database_schema.md
+-rw-r--r--   0        0        0     1725 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/demo.md
+-rw-r--r--   0        0        0    10639 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/dependencies.md
+-rw-r--r--   0        0        0     1947 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/experimental_features.md
+-rw-r--r--   0        0        0     7135 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/git.md
+-rw-r--r--   0        0        0    72228 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/img/git/branches.jpg
+-rw-r--r--   0        0        0   110840 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/img/git/clean.png
+-rw-r--r--   0        0        0    29667 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/img/git/squash.png
+-rw-r--r--   0        0        0      594 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/internal_documentation/README.md
+-rw-r--r--   0        0        0     1567 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/releases.md
+-rw-r--r--   0        0        0     2016 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/reviews.md
+-rw-r--r--   0        0        0     4991 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/room-dag-concepts.md
+-rw-r--r--   0        0        0     1839 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/saml.md
+-rw-r--r--   0        0        0    11035 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/synapse_architecture/cancellation.md
+-rw-r--r--   0        0        0    18006 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/synapse_architecture/faster_joins.md
+-rw-r--r--   0        0        0     9698 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/development/synapse_architecture/streams.md
+-rw-r--r--   0        0        0     7908 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/favicon.png
+-rw-r--r--   0        0        0     3946 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/favicon.svg
+-rw-r--r--   0        0        0     3677 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/federate.md
+-rw-r--r--   0        0        0     3844 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/jwt.md
+-rw-r--r--   0        0        0    13642 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/log_contexts.md
+-rw-r--r--   0        0        0     3246 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/manhole.md
+-rw-r--r--   0        0        0     2920 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/media_repository.md
+-rw-r--r--   0        0        0     8429 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/message_retention_policies.md
+-rw-r--r--   0        0        0    19859 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/metrics-howto.md
+-rw-r--r--   0        0        0     3330 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/account_data_callbacks.md
+-rw-r--r--   0        0        0     2192 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/account_validity_callbacks.md
+-rw-r--r--   0        0        0      950 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/add_extra_fields_to_client_events_unsigned.md
+-rw-r--r--   0        0        0     3121 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/background_update_controller_callbacks.md
+-rw-r--r--   0        0        0     2090 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/index.md
+-rw-r--r--   0        0        0    11738 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/password_auth_provider_callbacks.md
+-rw-r--r--   0        0        0     1131 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/porting_legacy_module.md
+-rw-r--r--   0        0        0     4323 2024-01-09 15:11:25.382849 matrix_synapse-1.99.0rc1/docs/modules/presence_router_callbacks.md
+-rw-r--r--   0        0        0    19226 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/modules/spam_checker_callbacks.md
+-rw-r--r--   0        0        0    14496 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/modules/third_party_rules_callbacks.md
+-rw-r--r--   0        0        0     6604 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/modules/writing_a_module.md
+-rw-r--r--   0        0        0    27540 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/openid.md
+-rw-r--r--   0        0        0     4018 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/opentracing.md
+-rw-r--r--   0        0        0     6075 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/other/running_synapse_on_single_board_computers.md
+-rw-r--r--   0        0        0     5268 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/password_auth_providers.md
+-rw-r--r--   0        0        0     9365 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/postgres.md
+-rw-r--r--   0        0        0     9293 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/presence_router_module.md
+-rw-r--r--   0        0        0      724 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/privacy_policy_templates/en/1.0.html
+-rw-r--r--   0        0        0      154 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/privacy_policy_templates/en/success.html
+-rw-r--r--   0        0        0     1540 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/replication.md
+-rw-r--r--   0        0        0     9927 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/reverse_proxy.md
+-rw-r--r--   0        0        0      661 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/room_and_user_statistics.md
+-rw-r--r--   0        0        0     1725 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/sample_config.yaml
+-rw-r--r--   0        0        0     2732 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/sample_log_config.yaml
+-rw-r--r--   0        0        0     2731 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/server_notices.md
+-rw-r--r--   0        0        0     2763 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/setup/forward_proxy.md
+-rw-r--r--   0        0        0    20830 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/setup/installation.md
+-rw-r--r--   0        0        0     6613 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/setup/turn/coturn.md
+-rw-r--r--   0        0        0     7264 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/setup/turn/eturnal.md
+-rw-r--r--   0        0        0     3729 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/spam_checker.md
+-rw-r--r--   0        0        0    11780 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/sso_mapping_providers.md
+-rw-r--r--   0        0        0     2509 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/structured_logging.md
+-rw-r--r--   0        0        0     1131 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/synctl_workers.md
+-rw-r--r--   0        0        0     4240 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/README.md
+-rw-r--r--   0        0        0      887 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/system/matrix-synapse-worker@.service
+-rw-r--r--   0        0        0      813 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/system/matrix-synapse.service
+-rw-r--r--   0        0        0      100 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/system/matrix-synapse.target
+-rw-r--r--   0        0        0      137 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/background_worker.yaml
+-rw-r--r--   0        0        0      544 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/event_persister.yaml
+-rw-r--r--   0        0        0      141 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/federation_sender.yaml
+-rw-r--r--   0        0        0      254 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/generic_worker.yaml
+-rw-r--r--   0        0        0      238 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/media_worker.yaml
+-rw-r--r--   0        0        0      122 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/pusher_worker.yaml
+-rw-r--r--   0        0        0     9614 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/tcp_replication.md
+-rw-r--r--   0        0        0    13804 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/templates.md
+-rw-r--r--   0        0        0     6528 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/turn-howto.md
+-rw-r--r--   0        0        0    98187 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/upgrade.md
+-rw-r--r--   0        0        0      278 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/README.md
+-rw-r--r--   0        0        0     2433 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/README.md
+-rw-r--r--   0        0        0     2468 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/background_updates.md
+-rw-r--r--   0        0        0     7159 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/federation.md
+-rw-r--r--   0        0        0     7442 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/registration_tokens.md
+-rw-r--r--   0        0        0    11809 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/admin_faq.md
+-rw-r--r--   0        0        0     1181 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/database_maintenance_tools.md
+-rw-r--r--   0        0        0    13290 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/monitoring/reporting_homeserver_usage_statistics.md
+-rw-r--r--   0        0        0     4674 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/monthly_active_users.md
+-rw-r--r--   0        0        0     3211 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/request_log.md
+-rw-r--r--   0        0        0     2399 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/state_groups.md
+-rw-r--r--   0        0        0     6420 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/understanding_synapse_through_grafana_graphs.md
+-rw-r--r--   0        0        0     6180 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/administration/useful_sql_for_admins.md
+-rw-r--r--   0        0        0      231 2024-01-09 15:11:25.386849 matrix_synapse-1.99.0rc1/docs/usage/configuration/README.md
+-rw-r--r--   0        0        0   159563 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/config_documentation.md
+-rw-r--r--   0        0        0      715 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/homeserver_sample_config.md
+-rw-r--r--   0        0        0      695 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/logging_sample_config.md
+-rw-r--r--   0        0        0      532 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/README.md
+-rw-r--r--   0        0        0     6992 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/refresh_tokens.md
+-rw-r--r--   0        0        0      207 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/single_sign_on/README.md
+-rw-r--r--   0        0        0      377 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/single_sign_on/cas.md
+-rw-r--r--   0        0        0      338 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/single_sign_on/saml.md
+-rw-r--r--   0        0        0     6558 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/user_directory.md
+-rw-r--r--   0        0        0     1976 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/README.md
+-rw-r--r--   0        0        0      161 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/indent-section-headers.css
+-rw-r--r--   0        0        0      252 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/remove-nav-buttons.css
+-rw-r--r--   0        0        0     1118 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/table-of-contents.css
+-rw-r--r--   0        0        0     4564 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/table-of-contents.js
+-rw-r--r--   0        0        0    15431 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/theme/index.hbs
+-rw-r--r--   0        0        0     1902 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/version-picker.css
+-rw-r--r--   0        0        0     4705 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/version-picker.js
+-rw-r--r--   0        0        0       35 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/website_files/version.js
+-rw-r--r--   0        0        0     2951 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/welcome_and_overview.md
+-rw-r--r--   0        0        0    32956 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/docs/workers.md
+-rw-r--r--   0        0        0     2723 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/mypy.ini
+-rw-r--r--   0        0        0    15760 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1082 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/Cargo.toml
+-rw-r--r--   0        0        0     1300 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/build.rs
+-rw-r--r--   0        0        0     3082 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/acl/mod.rs
+-rw-r--r--   0        0        0    14484 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/events/internal_metadata.rs
+-rw-r--r--   0        0        0     1340 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/events/mod.rs
+-rw-r--r--   0        0        0     1264 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/lib.rs
+-rw-r--r--   0        0        0    29332 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/push/base_rules.rs
+-rw-r--r--   0        0        0    20793 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/push/evaluator.rs
+-rw-r--r--   0        0        0    26288 2024-01-09 15:11:25.390849 matrix_synapse-1.99.0rc1/rust/src/push/mod.rs
+-rw-r--r--   0        0        0     7617 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/rust/src/push/utils.rs
+-rwxr-xr-x   0        0        0     7512 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/build_debian_packages.py
+-rwxr-xr-x   0        0        0     2320 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/check-newsfragment.sh
+-rwxr-xr-x   0        0        0     1009 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/check_line_terminators.sh
+-rwxr-xr-x   0        0        0     1923 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/check_locked_deps_have_sdists.py
+-rwxr-xr-x   0        0        0    16670 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/check_pydantic_models.py
+-rwxr-xr-x   0        0        0     3458 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/check_schema_delta.py
+-rwxr-xr-x   0        0        0    10667 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/complement.sh
+-rwxr-xr-x   0        0        0      538 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/config-lint.sh
+-rwxr-xr-x   0        0        0      362 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/database-save.sh
+-rwxr-xr-x   0        0        0     2848 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/docker_update_debian_changelog.sh
+-rwxr-xr-x   0        0        0      532 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/dump_macaroon.py
+-rwxr-xr-x   0        0        0    11976 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/federation_client.py
+-rwxr-xr-x   0        0        0     1049 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/generate_sample_config.sh
+-rwxr-xr-x   0        0        0     4146 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/lint.sh
+-rwxr-xr-x   0        0        0    11444 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/make_full_schema.sh
+-rw-r--r--   0        0        0    12678 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/mypy_synapse_plugin.py
+-rwxr-xr-x   0        0        0      308 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/next_github_number.sh
+-rwxr-xr-x   0        0        0    30919 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/release.py
+-rwxr-xr-x   0        0        0     6790 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/schema_versions.py
+-rwxr-xr-x   0        0        0     5177 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/scripts-dev/sign_json.py
+-rw-r--r--   0        0        0     3285 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/__init__.py
+-rw-r--r--   0        0        0      982 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/__init__.py
+-rwxr-xr-x   0        0        0     2781 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/export_signing_key.py
+-rwxr-xr-x   0        0        0     2336 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/generate_config.py
+-rwxr-xr-x   0        0        0     1409 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/generate_log_config.py
+-rwxr-xr-x   0        0        0     1491 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/generate_signing_key.py
+-rwxr-xr-x   0        0        0     9751 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/generate_workers_map.py
+-rwxr-xr-x   0        0        0     2076 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/hash_password.py
+-rwxr-xr-x   0        0        0     3780 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/move_remote_media_to_new_store.py
+-rw-r--r--   0        0        0     9110 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/register_new_matrix_user.py
+-rw-r--r--   0        0        0     5987 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/review_recent_signups.py
+-rwxr-xr-x   0        0        0    50656 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/synapse_port_db.py
+-rwxr-xr-x   0        0        0    11921 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/synctl.py
+-rw-r--r--   0        0        0     3746 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/_scripts/update_synapse_database.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/__init__.py
+-rw-r--r--   0        0        0     6131 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/auth/__init__.py
+-rw-r--r--   0        0        0    15587 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/auth/base.py
+-rw-r--r--   0        0        0    10501 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/auth/internal.py
+-rw-r--r--   0        0        0    15240 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/auth/msc3861_delegated.py
+-rw-r--r--   0        0        0     6033 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/auth_blocking.py
+-rw-r--r--   0        0        0     8272 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/constants.py
+-rw-r--r--   0        0        0    28545 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/errors.py
+-rw-r--r--   0        0        0    19926 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/filtering.py
+-rw-r--r--   0        0        0     3164 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/presence.py
+-rw-r--r--   0        0        0    17536 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/ratelimiting.py
+-rw-r--r--   0        0        0    13368 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/room_versions.py
+-rw-r--r--   0        0        0     2307 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/api/urls.py
+-rw-r--r--   0        0        0     1900 2024-01-09 15:11:25.394849 matrix_synapse-1.99.0rc1/synapse/app/__init__.py
+-rw-r--r--   0        0        0    26657 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/_base.py
+-rw-r--r--   0        0        0    12533 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/admin_cmd.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/appservice.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/client_reader.py
+-rw-r--r--   0        0        0     7238 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/complement_fork_starter.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/event_creator.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/federation_reader.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/federation_sender.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/frontend_proxy.py
+-rw-r--r--   0        0        0    13527 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/generic_worker.py
+-rw-r--r--   0        0        0    14883 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/homeserver.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/media_repository.py
+-rw-r--r--   0        0        0     8572 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/phone_stats_home.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/pusher.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/synchrotron.py
+-rw-r--r--   0        0        0      905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/app/user_dir.py
+-rw-r--r--   0        0        0    15399 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/appservice/__init__.py
+-rw-r--r--   0        0        0    19987 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/appservice/api.py
+-rw-r--r--   0        0        0    21253 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/appservice/scheduler.py
+-rw-r--r--   0        0        0      907 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/__init__.py
+-rw-r--r--   0        0        0     1896 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/__main__.py
+-rw-r--r--   0        0        0    36463 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/_base.py
+-rw-r--r--   0        0        0     6184 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/_base.pyi
+-rw-r--r--   0        0        0     3389 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/_util.py
+-rw-r--r--   0        0        0     4577 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/account_validity.py
+-rw-r--r--   0        0        0     4856 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/api.py
+-rw-r--r--   0        0        0     7595 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/appservice.py
+-rw-r--r--   0        0        0     2834 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/auth.py
+-rw-r--r--   0        0        0     1397 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/background_updates.py
+-rw-r--r--   0        0        0     8416 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/cache.py
+-rw-r--r--   0        0        0     1875 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/captcha.py
+-rw-r--r--   0        0        0     3367 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/cas.py
+-rw-r--r--   0        0        0     2669 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/consent.py
+-rw-r--r--   0        0        0     6499 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/database.py
+-rw-r--r--   0        0        0    15124 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/emailconfig.py
+-rw-r--r--   0        0        0    16905 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/experimental.py
+-rw-r--r--   0        0        0     3720 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/federation.py
+-rw-r--r--   0        0        0     3282 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/homeserver.py
+-rw-r--r--   0        0        0     1786 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/jwt.py
+-rw-r--r--   0        0        0    15126 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/key.py
+-rw-r--r--   0        0        0    12101 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/logger.py
+-rw-r--r--   0        0        0     2676 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/metrics.py
+-rw-r--r--   0        0        0     1393 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/modules.py
+-rw-r--r--   0        0        0     6319 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/oembed.py
+-rw-r--r--   0        0        0    16521 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/oidc.py
+-rw-r--r--   0        0        0     2923 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/password_auth_providers.py
+-rw-r--r--   0        0        0     2411 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/push.py
+-rw-r--r--   0        0        0     7527 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/ratelimiting.py
+-rw-r--r--   0        0        0     1799 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/redis.py
+-rw-r--r--   0        0        0    12343 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/registration.py
+-rw-r--r--   0        0        0    10645 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/repository.py
+-rw-r--r--   0        0        0     5945 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/retention.py
+-rw-r--r--   0        0        0     3288 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/room.py
+-rw-r--r--   0        0        0     5529 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/room_directory.py
+-rw-r--r--   0        0        0     9260 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/saml2.py
+-rw-r--r--   0        0        0    39285 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/server.py
+-rw-r--r--   0        0        0     3185 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/server_notices.py
+-rw-r--r--   0        0        0     2680 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/spam_checker.py
+-rw-r--r--   0        0        0     4109 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/sso.py
+-rw-r--r--   0        0        0     1746 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/stats.py
+-rw-r--r--   0        0        0     1217 2024-01-09 15:11:25.398849 matrix_synapse-1.99.0rc1/synapse/config/third_party_event_rules.py
+-rw-r--r--   0        0        0     7551 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/config/tls.py
+-rw-r--r--   0        0        0     2405 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/config/tracer.py
+-rw-r--r--   0        0        0     1501 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/config/user_directory.py
+-rw-r--r--   0        0        0     1299 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/config/voip.py
+-rw-r--r--   0        0        0    24262 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/config/workers.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/crypto/__init__.py
+-rw-r--r--   0        0        0    10738 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/crypto/context_factory.py
+-rw-r--r--   0        0        0     6241 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/crypto/event_signing.py
+-rw-r--r--   0        0        0    33535 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/crypto/keyring.py
+-rw-r--r--   0        0        0    41379 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/event_auth.py
+-rw-r--r--   0        0        0    18262 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/events/__init__.py
+-rw-r--r--   0        0        0    10075 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/events/builder.py
+-rw-r--r--   0        0        0     9044 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/events/presence_router.py
+-rw-r--r--   0        0        0    21786 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/events/snapshot.py
+-rw-r--r--   0        0        0    28195 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/events/utils.py
+-rw-r--r--   0        0        0    11341 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/events/validator.py
+-rw-r--r--   0        0        0      739 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/__init__.py
+-rw-r--r--   0        0        0    12648 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/federation_base.py
+-rw-r--r--   0        0        0    73309 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/federation_client.py
+-rw-r--r--   0        0        0    59769 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/federation_server.py
+-rw-r--r--   0        0        0     2377 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/persistence.py
+-rw-r--r--   0        0        0    17244 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/send_queue.py
+-rw-r--r--   0        0        0    41665 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/sender/__init__.py
+-rw-r--r--   0        0        0    33785 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/sender/per_destination_queue.py
+-rw-r--r--   0        0        0     7013 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/sender/transaction_manager.py
+-rw-r--r--   0        0        0     1033 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/transport/__init__.py
+-rw-r--r--   0        0        0    36251 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/transport/client.py
+-rw-r--r--   0        0        0    10104 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/transport/server/__init__.py
+-rw-r--r--   0        0        0    14924 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/transport/server/_base.py
+-rw-r--r--   0        0        0    26155 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/transport/server/federation.py
+-rw-r--r--   0        0        0     3036 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/federation/units.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/handlers/__init__.py
+-rw-r--r--   0        0        0     5438 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/handlers/account.py
+-rw-r--r--   0        0        0    13009 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/handlers/account_data.py
+-rw-r--r--   0        0        0    13827 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/handlers/account_validity.py
+-rw-r--r--   0        0        0    15959 2024-01-09 15:11:25.402849 matrix_synapse-1.99.0rc1/synapse/handlers/admin.py
+-rw-r--r--   0        0        0    39457 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/appservice.py
+-rw-r--r--   0        0        0    97956 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/auth.py
+-rw-r--r--   0        0        0    14793 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/cas.py
+-rw-r--r--   0        0        0    12366 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/deactivate_account.py
+-rw-r--r--   0        0        0    61283 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/device.py
+-rw-r--r--   0        0        0    15447 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/devicemessage.py
+-rw-r--r--   0        0        0    20694 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/directory.py
+-rw-r--r--   0        0        0    68460 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/e2e_keys.py
+-rw-r--r--   0        0        0    17197 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/e2e_room_keys.py
+-rw-r--r--   0        0        0    14257 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/event_auth.py
+-rw-r--r--   0        0        0     7045 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/events.py
+-rw-r--r--   0        0        0    86451 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/federation.py
+-rw-r--r--   0        0        0    98739 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/federation_event.py
+-rw-r--r--   0        0        0    30688 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/identity.py
+-rw-r--r--   0        0        0    18381 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/initial_sync.py
+-rw-r--r--   0        0        0     3934 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/jwt.py
+-rw-r--r--   0        0        0    90766 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/message.py
+-rw-r--r--   0        0        0    67040 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/oidc.py
+-rw-r--r--   0        0        0    29733 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/pagination.py
+-rw-r--r--   0        0        0     3393 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/password_policy.py
+-rw-r--r--   0        0        0    99963 2024-01-09 15:11:25.406849 matrix_synapse-1.99.0rc1/synapse/handlers/presence.py
+-rw-r--r--   0        0        0    18444 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/profile.py
+-rw-r--r--   0        0        0     6012 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/push_rules.py
+-rw-r--r--   0        0        0     2890 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/read_marker.py
+-rw-r--r--   0        0        0    12957 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/receipts.py
+-rw-r--r--   0        0        0    42558 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/register.py
+-rw-r--r--   0        0        0    23451 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/relations.py
+-rw-r--r--   0        0        0    81997 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/room.py
+-rw-r--r--   0        0        0    23805 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/room_list.py
+-rw-r--r--   0        0        0    89876 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/room_member.py
+-rw-r--r--   0        0        0     4774 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/room_member_worker.py
+-rw-r--r--   0        0        0    37175 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/room_summary.py
+-rw-r--r--   0        0        0    19345 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/saml.py
+-rw-r--r--   0        0        0    25673 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/search.py
+-rw-r--r--   0        0        0     8228 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/send_email.py
+-rw-r--r--   0        0        0     2738 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/set_password.py
+-rw-r--r--   0        0        0    47872 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/sso.py
+-rw-r--r--   0        0        0     2490 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/state_deltas.py
+-rw-r--r--   0        0        0    13052 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/stats.py
+-rw-r--r--   0        0        0   118386 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/sync.py
+-rw-r--r--   0        0        0    21239 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/typing.py
+-rw-r--r--   0        0        0     1715 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/ui_auth/__init__.py
+-rw-r--r--   0        0        0    11882 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/ui_auth/checkers.py
+-rw-r--r--   0        0        0    31838 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/user_directory.py
+-rw-r--r--   0        0        0    11146 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/handlers/worker_lock.py
+-rw-r--r--   0        0        0     3314 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/__init__.py
+-rw-r--r--   0        0        0     2092 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/additional_resource.py
+-rw-r--r--   0        0        0    40422 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/client.py
+-rw-r--r--   0        0        0    10383 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/connectproxyclient.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/federation/__init__.py
+-rw-r--r--   0        0        0    16986 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/federation/matrix_federation_agent.py
+-rw-r--r--   0        0        0     6069 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/federation/srv_resolver.py
+-rw-r--r--   0        0        0    12401 2024-01-09 15:11:25.410849 matrix_synapse-1.99.0rc1/synapse/http/federation/well_known_resolver.py
+-rw-r--r--   0        0        0    56860 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/matrixfederationclient.py
+-rw-r--r--   0        0        0    10144 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/proxy.py
+-rw-r--r--   0        0        0    17583 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/proxyagent.py
+-rw-r--r--   0        0        0     6799 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/replicationagent.py
+-rw-r--r--   0        0        0     8476 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/request_metrics.py
+-rw-r--r--   0        0        0    35656 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/server.py
+-rw-r--r--   0        0        0    26402 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/servlet.py
+-rw-r--r--   0        0        0    26902 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/site.py
+-rw-r--r--   0        0        0      975 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/http/types.py
+-rw-r--r--   0        0        0     1084 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/__init__.py
+-rw-r--r--   0        0        0     8591 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/_remote.py
+-rw-r--r--   0        0        0     2571 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/_terse_json.py
+-rw-r--r--   0        0        0    32689 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/context.py
+-rw-r--r--   0        0        0     1159 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/filter.py
+-rw-r--r--   0        0        0     2065 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/formatter.py
+-rw-r--r--   0        0        0     2771 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/handlers.py
+-rw-r--r--   0        0        0    37077 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/opentracing.py
+-rw-r--r--   0        0        0     5867 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/logging/scopecontextmanager.py
+-rw-r--r--   0        0        0    15419 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/_base.py
+-rw-r--r--   0        0        0    15848 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/filepath.py
+-rw-r--r--   0        0        0    46339 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/media_repository.py
+-rw-r--r--   0        0        0    14432 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/media_storage.py
+-rw-r--r--   0        0        0    10256 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/oembed.py
+-rw-r--r--   0        0        0    19117 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/preview_html.py
+-rw-r--r--   0        0        0     6709 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/storage_provider.py
+-rw-r--r--   0        0        0     8529 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/thumbnailer.py
+-rw-r--r--   0        0        0    33456 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/media/url_previewer.py
+-rw-r--r--   0        0        0    15059 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/__init__.py
+-rw-r--r--   0        0        0     7238 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/_gc.py
+-rw-r--r--   0        0        0     5544 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/_reactor_metrics.py
+-rw-r--r--   0        0        0     1395 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/_twisted_exposition.py
+-rw-r--r--   0        0        0     1146 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/_types.py
+-rw-r--r--   0        0        0    12982 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/background_process_metrics.py
+-rw-r--r--   0        0        0     2734 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/common_usage_metrics.py
+-rw-r--r--   0        0        0     8076 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/metrics/jemalloc.py
+-rw-r--r--   0        0        0    72000 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/module_api/__init__.py
+-rw-r--r--   0        0        0     1395 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/__init__.py
+-rw-r--r--   0        0        0     5072 2024-01-09 15:11:25.414849 matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/account_validity_callbacks.py
+-rw-r--r--   0        0        0    34778 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/spamchecker_callbacks.py
+-rw-r--r--   0        0        0    24701 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/third_party_event_rules_callbacks.py
+-rw-r--r--   0        0        0     1222 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/module_api/errors.py
+-rw-r--r--   0        0        0    31892 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/notifier.py
+-rw-r--r--   0        0        0     7279 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/__init__.py
+-rw-r--r--   0        0        0    23352 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/bulk_push_rule_evaluator.py
+-rw-r--r--   0        0        0     4332 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/clientformat.py
+-rw-r--r--   0        0        0    12501 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/emailpusher.py
+-rw-r--r--   0        0        0    20366 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/httppusher.py
+-rw-r--r--   0        0        0    33725 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/mailer.py
+-rw-r--r--   0        0        0     7834 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/presentable_names.py
+-rw-r--r--   0        0        0     4250 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/push_tools.py
+-rw-r--r--   0        0        0     4882 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/push_types.py
+-rw-r--r--   0        0        0     2930 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/pusher.py
+-rw-r--r--   0        0        0    17431 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/pusherpool.py
+-rw-r--r--   0        0        0      863 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/push/rulekinds.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/py.typed
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/__init__.py
+-rw-r--r--   0        0        0     2077 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/__init__.py
+-rw-r--r--   0        0        0    18636 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/_base.py
+-rw-r--r--   0        0        0     8250 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/account_data.py
+-rw-r--r--   0        0        0     5368 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/devices.py
+-rw-r--r--   0        0        0    10347 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/federation.py
+-rw-r--r--   0        0        0     3622 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/login.py
+-rw-r--r--   0        0        0    11444 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/membership.py
+-rw-r--r--   0        0        0     3657 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/presence.py
+-rw-r--r--   0        0        0     2202 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/push.py
+-rw-r--r--   0        0        0     6272 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/register.py
+-rw-r--r--   0        0        0     5630 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/send_event.py
+-rw-r--r--   0        0        0     6298 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/send_events.py
+-rw-r--r--   0        0        0     2484 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/state.py
+-rw-r--r--   0        0        0     3196 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/http/streams.py
+-rw-r--r--   0        0        0     1874 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/__init__.py
+-rw-r--r--   0        0        0    21607 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/client.py
+-rw-r--r--   0        0        0    15244 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/commands.py
+-rw-r--r--   0        0        0     1513 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/context.py
+-rw-r--r--   0        0        0     4413 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/external_cache.py
+-rw-r--r--   0        0        0    33489 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/handler.py
+-rw-r--r--   0        0        0    19184 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/protocol.py
+-rw-r--r--   0        0        0    15414 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/redis.py
+-rw-r--r--   0        0        0    14466 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/resource.py
+-rw-r--r--   0        0        0     2537 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/__init__.py
+-rw-r--r--   0        0        0    24081 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/_base.py
+-rw-r--r--   0        0        0    10050 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/events.py
+-rw-r--r--   0        0        0     3365 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/federation.py
+-rw-r--r--   0        0        0     2384 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/partial_state.py
+-rw-r--r--   0        0        0      760 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/providers.json
+-rw-r--r--   0        0        0     1035 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/_base.html
+-rw-r--r--   0        0        0      240 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/account_previously_renewed.html
+-rw-r--r--   0        0        0      308 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/account_renewed.html
+-rw-r--r--   0        0        0      413 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/add_threepid.html
+-rw-r--r--   0        0        0      230 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/add_threepid.txt
+-rw-r--r--   0        0        0      230 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/add_threepid_failure.html
+-rw-r--r--   0        0        0      228 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/add_threepid_success.html
+-rw-r--r--   0        0        0      490 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/auth_success.html
+-rw-r--r--   0        0        0      144 2024-01-09 15:11:25.418849 matrix_synapse-1.99.0rc1/synapse/res/templates/invalid_token.html
+-rw-r--r--   0        0        0      124 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/mail-Element.css
+-rw-r--r--   0        0        0      124 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/mail-Vector.css
+-rw-r--r--   0        0        0       63 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/mail-expiry.css
+-rw-r--r--   0        0        0     2252 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/mail.css
+-rw-r--r--   0        0        0     2044 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/notice_expiry.html
+-rw-r--r--   0        0        0      293 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/notice_expiry.txt
+-rw-r--r--   0        0        0     2658 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/notif.html
+-rw-r--r--   0        0        0      761 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/notif.txt
+-rw-r--r--   0        0        0     2674 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/notif_mail.html
+-rw-r--r--   0        0        0      191 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/notif_mail.txt
+-rw-r--r--   0        0        0      431 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/password_reset.html
+-rw-r--r--   0        0        0      269 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/password_reset.txt
+-rw-r--r--   0        0        0      740 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/password_reset_confirmation.html
+-rw-r--r--   0        0        0      229 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/password_reset_failure.html
+-rw-r--r--   0        0        0      240 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/password_reset_success.html
+-rw-r--r--   0        0        0     1141 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/recaptcha.html
+-rw-r--r--   0        0        0      392 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/registration.html
+-rw-r--r--   0        0        0      241 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/registration.txt
+-rw-r--r--   0        0        0      185 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/registration_failure.html
+-rw-r--r--   0        0        0      228 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/registration_success.html
+-rw-r--r--   0        0        0      536 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/registration_token.html
+-rw-r--r--   0        0        0     1117 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/room.html
+-rw-r--r--   0        0        0      216 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/room.txt
+-rw-r--r--   0        0        0     1783 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso.css
+-rw-r--r--   0        0        0      671 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_account_deactivated.html
+-rw-r--r--   0        0        0     5077 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_account_details.html
+-rw-r--r--   0        0        0     3711 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_account_details.js
+-rw-r--r--   0        0        0      812 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_bad_user.html
+-rw-r--r--   0        0        0      698 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_confirm.html
+-rw-r--r--   0        0        0      629 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_success.html
+-rw-r--r--   0        0        0     2807 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_error.html
+-rw-r--r--   0        0        0     9062 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_footer.html
+-rw-r--r--   0        0        0     1258 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_login_idp_picker.html
+-rw-r--r--   0        0        0      961 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_new_user_consent.html
+-rw-r--r--   0        0        0      873 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_partial_profile.html
+-rw-r--r--   0        0        0     1905 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/sso_redirect_confirm.html
+-rw-r--r--   0        0        0      641 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/style.css
+-rw-r--r--   0        0        0      739 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/res/templates/terms.html
+-rw-r--r--   0        0        0     5314 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/__init__.py
+-rw-r--r--   0        0        0    13731 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/__init__.py
+-rw-r--r--   0        0        0     2201 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/_base.py
+-rw-r--r--   0        0        0     5917 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/background_updates.py
+-rw-r--r--   0        0        0     7342 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/devices.py
+-rw-r--r--   0        0        0     5911 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/event_reports.py
+-rw-r--r--   0        0        0     3973 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/experimental_features.py
+-rw-r--r--   0        0        0     9269 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/federation.py
+-rw-r--r--   0        0        0    17900 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/media.py
+-rw-r--r--   0        0        0    11419 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/registration_tokens.py
+-rw-r--r--   0        0        0    34939 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/rooms.py
+-rw-r--r--   0        0        0     4542 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/server_notice_servlet.py
+-rw-r--r--   0        0        0     5370 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/statistics.py
+-rw-r--r--   0        0        0     1905 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/username_available.py
+-rw-r--r--   0        0        0    47896 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/admin/users.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/__init__.py
+-rw-r--r--   0        0        0     3584 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/_base.py
+-rw-r--r--   0        0        0    35375 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/account.py
+-rw-r--r--   0        0        0    12113 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/account_data.py
+-rw-r--r--   0        0        0     3608 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/account_validity.py
+-rw-r--r--   0        0        0     3926 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/appservice_ping.py
+-rw-r--r--   0        0        0     7292 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/auth.py
+-rw-r--r--   0        0        0     2209 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/auth_issuer.py
+-rw-r--r--   0        0        0     3524 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/capabilities.py
+-rw-r--r--   0        0        0    18982 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/devices.py
+-rw-r--r--   0        0        0     7513 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/directory.py
+-rw-r--r--   0        0        0     4029 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/events.py
+-rw-r--r--   0        0        0     3764 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/filter.py
+-rw-r--r--   0        0        0     2331 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/initial_sync.py
+-rw-r--r--   0        0        0    17255 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/keys.py
+-rw-r--r--   0        0        0     3275 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/knock.py
+-rw-r--r--   0        0        0    27523 2024-01-09 15:11:25.422848 matrix_synapse-1.99.0rc1/synapse/rest/client/login.py
+-rw-r--r--   0        0        0     4234 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/login_token_request.py
+-rw-r--r--   0        0        0     3331 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/logout.py
+-rw-r--r--   0        0        0     3178 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/models.py
+-rw-r--r--   0        0        0     3044 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/mutual_rooms.py
+-rw-r--r--   0        0        0     3978 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/notifications.py
+-rw-r--r--   0        0        0     3402 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/openid.py
+-rw-r--r--   0        0        0     1959 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/password_policy.py
+-rw-r--r--   0        0        0     3697 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/presence.py
+-rw-r--r--   0        0        0     7150 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/profile.py
+-rw-r--r--   0        0        0    10511 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/push_rule.py
+-rw-r--r--   0        0        0     5807 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/pusher.py
+-rw-r--r--   0        0        0     3655 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/read_marker.py
+-rw-r--r--   0        0        0     5936 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/receipts.py
+-rw-r--r--   0        0        0    40419 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/register.py
+-rw-r--r--   0        0        0     4894 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/relations.py
+-rw-r--r--   0        0        0     2676 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/rendezvous.py
+-rw-r--r--   0        0        0     3194 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/report_event.py
+-rw-r--r--   0        0        0    54203 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/room.py
+-rw-r--r--   0        0        0    15462 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/room_keys.py
+-rw-r--r--   0        0        0     3316 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/room_upgrade_rest_servlet.py
+-rw-r--r--   0        0        0     2664 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/sendtodevice.py
+-rw-r--r--   0        0        0    21245 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/sync.py
+-rw-r--r--   0        0        0     3433 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/tags.py
+-rw-r--r--   0        0        0     4185 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/thirdparty.py
+-rw-r--r--   0        0        0     1498 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/tokenrefresh.py
+-rw-r--r--   0        0        0     5906 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/transactions.py
+-rw-r--r--   0        0        0     2911 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/user_directory.py
+-rw-r--r--   0        0        0     6938 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/versions.py
+-rw-r--r--   0        0        0     2918 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/client/voip.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/consent/__init__.py
+-rw-r--r--   0        0        0     7825 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/consent/consent_resource.py
+-rw-r--r--   0        0        0     1178 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/health.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/key/__init__.py
+-rw-r--r--   0        0        0     1300 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/key/v2/__init__.py
+-rw-r--r--   0        0        0     4541 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/key/v2/local_key_resource.py
+-rw-r--r--   0        0        0    11248 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/key/v2/remote_key_resource.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/__init__.py
+-rw-r--r--   0        0        0     1453 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/config_resource.py
+-rw-r--r--   0        0        0     2928 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/create_resource.py
+-rw-r--r--   0        0        0     3440 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/download_resource.py
+-rw-r--r--   0        0        0     4087 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/media_repository_resource.py
+-rw-r--r--   0        0        0     2812 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/preview_url_resource.py
+-rw-r--r--   0        0        0    21635 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/thumbnail_resource.py
+-rw-r--r--   0        0        0     6285 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/upload_resource.py
+-rw-r--r--   0        0        0     1241 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/v1/__init__.py
+-rw-r--r--   0        0        0      829 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/v1/_base.py
+-rw-r--r--   0        0        0      817 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/v1/media_storage.py
+-rw-r--r--   0        0        0      818 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/media/v1/storage_provider.py
+-rw-r--r--   0        0        0     1663 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/models.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/__init__.py
+-rw-r--r--   0        0        0     3055 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/__init__.py
+-rw-r--r--   0        0        0     2293 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/jwks.py
+-rw-r--r--   0        0        0     4515 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/new_user_consent.py
+-rw-r--r--   0        0        0     1337 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/oidc/__init__.py
+-rw-r--r--   0        0        0     1265 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/oidc/backchannel_logout_resource.py
+-rw-r--r--   0        0        0     1583 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/oidc/callback_resource.py
+-rw-r--r--   0        0        0     4560 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/password_reset.py
+-rw-r--r--   0        0        0     3035 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/pick_idp.py
+-rw-r--r--   0        0        0     5633 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/pick_username.py
+-rw-r--r--   0        0        0     1308 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/saml2/__init__.py
+-rw-r--r--   0        0        0     1403 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/saml2/metadata_resource.py
+-rw-r--r--   0        0        0     1860 2024-01-09 15:11:25.426848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/saml2/response_resource.py
+-rw-r--r--   0        0        0     1933 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/sso_register.py
+-rw-r--r--   0        0        0     2902 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/unsubscribe.py
+-rw-r--r--   0        0        0     4650 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/rest/well_known.py
+-rw-r--r--   0        0        0    32566 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server_notices/__init__.py
+-rw-r--r--   0        0        0     4826 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server_notices/consent_server_notices.py
+-rw-r--r--   0        0        0     7971 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server_notices/resource_limits_server_notices.py
+-rw-r--r--   0        0        0    14513 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server_notices/server_notices_manager.py
+-rw-r--r--   0        0        0     2283 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server_notices/server_notices_sender.py
+-rw-r--r--   0        0        0     1388 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/server_notices/worker_server_notices_sender.py
+-rw-r--r--   0        0        0      912 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/spam_checker_api/__init__.py
+-rw-r--r--   0        0        0    34150 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/state/__init__.py
+-rw-r--r--   0        0        0    12402 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/state/v1.py
+-rw-r--r--   0        0        0    27610 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/state/v2.py
+-rw-r--r--   0        0        0     1703 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/static/client/login/index.html
+-rw-r--r--   0        0        0    88145 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/static/client/login/js/jquery-3.4.1.min.js
+-rw-r--r--   0        0        0     8277 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/static/client/login/js/login.js
+-rw-r--r--   0        0        0     1849 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/static/client/login/spinner.gif
+-rw-r--r--   0        0        0     1224 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/static/client/login/style.css
+-rw-r--r--   0        0        0    10145 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/static/index.html
+-rw-r--r--   0        0        0     1703 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/__init__.py
+-rw-r--r--   0        0        0     8791 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/_base.py
+-rw-r--r--   0        0        0    42388 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/background_updates.py
+-rw-r--r--   0        0        0     1966 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/controllers/__init__.py
+-rw-r--r--   0        0        0    45325 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/controllers/persist_events.py
+-rw-r--r--   0        0        0     4246 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/controllers/purge_events.py
+-rw-r--r--   0        0        0    29791 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/controllers/state.py
+-rw-r--r--   0        0        0     4126 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/controllers/stats.py
+-rw-r--r--   0        0        0    93733 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/database.py
+-rw-r--r--   0        0        0     5405 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/__init__.py
+-rw-r--r--   0        0        0    13942 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/__init__.py
+-rw-r--r--   0        0        0    35853 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/account_data.py
+-rw-r--r--   0        0        0    17471 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/appservice.py
+-rw-r--r--   0        0        0    31379 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/cache.py
+-rw-r--r--   0        0        0     8458 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/censor_events.py
+-rw-r--r--   0        0        0    30867 2024-01-09 15:11:25.430848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/client_ips.py
+-rw-r--r--   0        0        0    43309 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/deviceinbox.py
+-rw-r--r--   0        0        0    86038 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/devices.py
+-rw-r--r--   0        0        0     6747 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/directory.py
+-rw-r--r--   0        0        0    24499 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/e2e_room_keys.py
+-rw-r--r--   0        0        0    64757 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/end_to_end_keys.py
+-rw-r--r--   0        0        0    81598 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/event_federation.py
+-rw-r--r--   0        0        0    72345 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/event_push_actions.py
+-rw-r--r--   0        0        0    97971 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events.py
+-rw-r--r--   0        0        0    57370 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events_bg_updates.py
+-rw-r--r--   0        0        0     4308 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events_forward_extremities.py
+-rw-r--r--   0        0        0    99788 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events_worker.py
+-rw-r--r--   0        0        0     2881 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/experimental_features.py
+-rw-r--r--   0        0        0     8252 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/filtering.py
+-rw-r--r--   0        0        0    10679 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/keys.py
+-rw-r--r--   0        0        0    16855 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/lock.py
+-rw-r--r--   0        0        0    30695 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/media_repository.py
+-rw-r--r--   0        0        0    17814 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/metrics.py
+-rw-r--r--   0        0        0    17946 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/monthly_active_users.py
+-rw-r--r--   0        0        0     1899 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/openid.py
+-rw-r--r--   0        0        0    19175 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/presence.py
+-rw-r--r--   0        0        0     7630 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/profile.py
+-rw-r--r--   0        0        0    18752 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/purge_events.py
+-rw-r--r--   0        0        0    33510 2024-01-09 15:11:25.434848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/push_rule.py
+-rw-r--r--   0        0        0    28080 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/pusher.py
+-rw-r--r--   0        0        0    40364 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/receipts.py
+-rw-r--r--   0        0        0   104575 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/registration.py
+-rw-r--r--   0        0        0     1163 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/rejections.py
+-rw-r--r--   0        0        0    41986 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/relations.py
+-rw-r--r--   0        0        0    92730 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/room.py
+-rw-r--r--   0        0        0    56179 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/roommember.py
+-rw-r--r--   0        0        0    32254 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/search.py
+-rw-r--r--   0        0        0     5091 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/session.py
+-rw-r--r--   0        0        0     3040 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/signatures.py
+-rw-r--r--   0        0        0    26041 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/state.py
+-rw-r--r--   0        0        0     5672 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/state_deltas.py
+-rw-r--r--   0        0        0    28119 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/stats.py
+-rw-r--r--   0        0        0    58386 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/stream.py
+-rw-r--r--   0        0        0    10847 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/tags.py
+-rw-r--r--   0        0        0     7650 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/task_scheduler.py
+-rw-r--r--   0        0        0    21523 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/transactions.py
+-rw-r--r--   0        0        0    14628 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/ui_auth.py
+-rw-r--r--   0        0        0    49340 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/user_directory.py
+-rw-r--r--   0        0        0     3884 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/main/user_erasure_store.py
+-rw-r--r--   0        0        0      758 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/state/__init__.py
+-rw-r--r--   0        0        0    21788 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/state/bg_updates.py
+-rw-r--r--   0        0        0    32707 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/databases/state/store.py
+-rw-r--r--   0        0        0     2295 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/engines/__init__.py
+-rw-r--r--   0        0        0     5020 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/engines/_base.py
+-rw-r--r--   0        0        0    10256 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/engines/postgres.py
+-rw-r--r--   0        0        0     7476 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/engines/sqlite.py
+-rw-r--r--   0        0        0     1225 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/keys.py
+-rw-r--r--   0        0        0    25679 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/prepare_database.py
+-rw-r--r--   0        0        0      779 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/push_rule.py
+-rw-r--r--   0        0        0     1778 2024-01-09 15:11:25.438848 matrix_synapse-1.99.0rc1/synapse/storage/roommember.py
+-rw-r--r--   0        0        0      207 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/README.md
+-rw-r--r--   0        0        0     6219 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/__init__.py
+-rw-r--r--   0        0        0     1559 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/common/delta/25/00background_updates.sql
+-rw-r--r--   0        0        0     1347 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/common/delta/35/00background_updates_add_col.sql
+-rw-r--r--   0        0        0     1506 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/common/delta/58/00background_update_ordering.sql
+-rw-r--r--   0        0        0      269 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/common/full_schemas/72/full.sql.postgres
+-rw-r--r--   0        0        0      221 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/common/full_schemas/72/full.sql.sqlite
+-rw-r--r--   0        0        0     2207 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/common/schema_version.sql
+-rw-r--r--   0        0        0     2587 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/12/v12.sql
+-rw-r--r--   0        0        0     1451 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/13/v13.sql
+-rw-r--r--   0        0        0     1573 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/14/v14.sql
+-rw-r--r--   0        0        0     1690 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/15/appservice_txns.sql
+-rw-r--r--   0        0        0       78 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/15/presence_indices.sql
+-rw-r--r--   0        0        0      991 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/15/v15.sql
+-rw-r--r--   0        0        0      174 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/events_order_index.sql
+-rw-r--r--   0        0        0      114 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/remote_media_cache_index.sql
+-rw-r--r--   0        0        0      265 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/remove_duplicates.sql
+-rw-r--r--   0        0        0      157 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/room_alias_index.sql
+-rw-r--r--   0        0        0     2003 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/unique_constraints.sql
+-rw-r--r--   0        0        0     1519 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/users.sql
+-rw-r--r--   0        0        0     1417 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/17/drop_indexes.sql
+-rw-r--r--   0        0        0     1744 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/17/server_keys.sql
+-rw-r--r--   0        0        0      310 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/17/user_threepids.sql
+-rw-r--r--   0        0        0     2053 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/18/server_keys_bigger_ints.sql
+-rw-r--r--   0        0        0     1402 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/19/event_index.sql
+-rw-r--r--   0        0        0       10 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/20/dummy.sql
+-rw-r--r--   0        0        0     3071 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/20/pushers.py
+-rw-r--r--   0        0        0     2247 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/21/end_to_end_keys.sql
+-rw-r--r--   0        0        0     1944 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/21/receipts.sql
+-rw-r--r--   0        0        0     1637 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/22/receipts_index.sql
+-rw-r--r--   0        0        0      546 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/22/user_threepids_unique.sql
+-rw-r--r--   0        0        0     1402 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/24/stats_reporting.sql
+-rw-r--r--   0        0        0     2525 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/fts.py
+-rw-r--r--   0        0        0     1573 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/guest_access.sql
+-rw-r--r--   0        0        0     1591 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/history_visibility.sql
+-rw-r--r--   0        0        0     2093 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/tags.sql
+-rw-r--r--   0        0        0     1376 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/26/account_data.sql
+-rw-r--r--   0        0        0     2201 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/27/account_data.sql
+-rw-r--r--   0        0        0     1605 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/27/forgotten_memberships.sql
+-rw-r--r--   0        0        0     1973 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/27/ts.py
+-rw-r--r--   0        0        0     1803 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/event_push_actions.sql
+-rw-r--r--   0        0        0     1604 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/events_room_stream.sql
+-rw-r--r--   0        0        0     1587 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/public_roms_index.sql
+-rw-r--r--   0        0        0     1619 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/receipts_user_id_index.sql
+-rw-r--r--   0        0        0     1438 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/upgrade_times.sql
+-rw-r--r--   0        0        0     1615 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/users_is_guest.sql
+-rw-r--r--   0        0        0     2234 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/29/push_actions.sql
+-rw-r--r--   0        0        0     1337 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/alias_creator.sql
+-rw-r--r--   0        0        0     2783 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/as_users.py
+-rw-r--r--   0        0        0     1640 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/deleted_pushers.sql
+-rw-r--r--   0        0        0     1736 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/presence_stream.sql
+-rw-r--r--   0        0        0     1648 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/public_rooms.sql
+-rw-r--r--   0        0        0     2006 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/push_rule_stream.sql
+-rw-r--r--   0        0        0     1770 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/threepid_guest_access_tokens.sql
+-rw-r--r--   0        0        0     2127 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/invites.sql
+-rw-r--r--   0        0        0     1958 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/local_media_repository_url_cache.sql
+-rw-r--r--   0        0        0     2935 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/pushers_0.py
+-rw-r--r--   0        0        0     1642 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/pushers_index.sql
+-rw-r--r--   0        0        0     2087 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/search_update.py
+-rw-r--r--   0        0        0     1337 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/events.sql
+-rw-r--r--   0        0        0      241 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/openid.sql
+-rw-r--r--   0        0        0     1459 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/pusher_throttle.sql
+-rw-r--r--   0        0        0     2275 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/remove_indices.sql
+-rw-r--r--   0        0        0     1504 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/reports.sql
+-rw-r--r--   0        0        0     1394 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/access_tokens_device_index.sql
+-rw-r--r--   0        0        0     1453 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/devices.sql
+-rw-r--r--   0        0        0     1488 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/devices_for_e2e_keys.sql
+-rw-r--r--   0        0        0     1509 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/devices_for_e2e_keys_clear_unknown_device.sql
+-rw-r--r--   0        0        0     1937 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/event_fields.py
+-rw-r--r--   0        0        0     1300 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/remote_media_ts.py
+-rw-r--r--   0        0        0     1389 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/user_ips_index.sql
+-rw-r--r--   0        0        0     1600 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/appservice_stream.sql
+-rw-r--r--   0        0        0     1577 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/cache_stream.py
+-rw-r--r--   0        0        0     1626 2024-01-09 15:11:25.442848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/device_inbox.sql
+-rw-r--r--   0        0        0     1770 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/push_display_name_rename.sql
+-rw-r--r--   0        0        0     1203 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/received_txn_purge.py
+-rw-r--r--   0        0        0     1396 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/contains_url.sql
+-rw-r--r--   0        0        0     2010 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/device_outbox.sql
+-rw-r--r--   0        0        0     1460 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/device_stream_id.sql
+-rw-r--r--   0        0        0     1391 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/event_push_actions_index.sql
+-rw-r--r--   0        0        0     1762 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/public_room_list_change_stream.sql
+-rw-r--r--   0        0        0     2001 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/stream_order_to_extrem.sql
+-rw-r--r--   0        0        0     1747 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/36/readd_public_rooms.sql
+-rw-r--r--   0        0        0     2777 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/37/remove_auth_idx.py
+-rw-r--r--   0        0        0     2849 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/37/user_threepids.sql
+-rw-r--r--   0        0        0     1467 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/38/postgres_fts_gist.sql
+-rw-r--r--   0        0        0     1775 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/appservice_room_list.sql
+-rw-r--r--   0        0        0     1368 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/device_federation_stream_idx.sql
+-rw-r--r--   0        0        0     1403 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/event_push_index.sql
+-rw-r--r--   0        0        0     1599 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/federation_out_position.sql
+-rw-r--r--   0        0        0     1517 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/membership_profile.sql
+-rw-r--r--   0        0        0     1393 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/current_state_idx.sql
+-rw-r--r--   0        0        0     1617 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/device_inbox.sql
+-rw-r--r--   0        0        0     2880 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/device_list_streams.sql
+-rw-r--r--   0        0        0     2179 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/event_push_summary.sql
+-rw-r--r--   0        0        0     1897 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/pushers.sql
+-rw-r--r--   0        0        0     1399 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/device_list_stream_idx.sql
+-rw-r--r--   0        0        0     1384 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/device_outbound_index.sql
+-rw-r--r--   0        0        0     1401 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/event_search_event_id_idx.sql
+-rw-r--r--   0        0        0     1488 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/ratelimit.sql
+-rw-r--r--   0        0        0     1647 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/current_state_delta.sql
+-rw-r--r--   0        0        0     1994 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/device_list_last_id.sql
+-rw-r--r--   0        0        0     1395 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/event_auth_state_only.sql
+-rw-r--r--   0        0        0     2755 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/user_dir.py
+-rw-r--r--   0        0        0     1475 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/blocked_rooms.sql
+-rw-r--r--   0        0        0     1423 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/quarantine_media.sql
+-rw-r--r--   0        0        0     1355 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/url_cache.sql
+-rw-r--r--   0        0        0     2078 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/user_share.sql
+-rw-r--r--   0        0        0     2520 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/44/expire_url_cache.sql
+-rw-r--r--   0        0        0     5957 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/45/group_server.sql
+-rw-r--r--   0        0        0     1767 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/45/profile_cache.sql
+-rw-r--r--   0        0        0     1384 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/drop_refresh_tokens.sql
+-rw-r--r--   0        0        0     1992 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/drop_unique_deleted_pushers.sql
+-rw-r--r--   0        0        0     1850 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/group_server.sql
+-rw-r--r--   0        0        0     1764 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/local_media_repository_url_idx.sql
+-rw-r--r--   0        0        0     2058 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/user_dir_null_room_ids.sql
+-rw-r--r--   0        0        0     1775 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/user_dir_typos.sql
+-rw-r--r--   0        0        0     1356 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/47/last_access_media.sql
+-rw-r--r--   0        0        0     1395 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/47/postgres_fts_gin.sql
+-rw-r--r--   0        0        0     1778 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/47/push_actions_staging.sql
+-rw-r--r--   0        0        0     1412 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/add_user_consent.sql
+-rw-r--r--   0        0        0     1394 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/add_user_ips_last_seen_index.sql
+-rw-r--r--   0        0        0     1643 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/deactivated_users.sql
+-rw-r--r--   0        0        0     2237 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/group_unique_indexes.py
+-rw-r--r--   0        0        0     1603 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/groups_joinable.sql
+-rw-r--r--   0        0        0     1518 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/49/add_user_consent_server_notice_sent.sql
+-rw-r--r--   0        0        0     1607 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/49/add_user_daily_visits.sql
+-rw-r--r--   0        0        0     1399 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/49/add_user_ips_last_seen_only_index.sql
+-rw-r--r--   0        0        0     1389 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/50/add_creation_ts_users_index.sql
+-rw-r--r--   0        0        0     1477 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/50/erasure_store.sql
+-rw-r--r--   0        0        0     3253 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/50/make_event_content_nullable.py
+-rw-r--r--   0        0        0     2037 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/51/e2e_room_keys.sql
+-rw-r--r--   0        0        0     1865 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/51/monthly_active_users.sql
+-rw-r--r--   0        0        0     1533 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/52/add_event_to_state_group_index.sql
+-rw-r--r--   0        0        0     2131 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/52/device_list_streams_unique_idx.sql
+-rw-r--r--   0        0        0     2551 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/52/e2e_room_keys.sql
+-rw-r--r--   0        0        0     1462 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/add_user_type_to_users.sql
+-rw-r--r--   0        0        0     1327 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/drop_sent_transactions.sql
+-rw-r--r--   0        0        0     1345 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/event_format_version.sql
+-rw-r--r--   0        0        0     2101 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_dir_populate.sql
+-rw-r--r--   0        0        0     1983 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_ips_index.sql
+-rw-r--r--   0        0        0     2729 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_share.sql
+-rw-r--r--   0        0        0     1730 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_threepid_id.sql
+-rw-r--r--   0        0        0     1713 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/users_in_public_rooms.sql
+-rw-r--r--   0        0        0     1939 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/account_validity_with_renewal.sql
+-rw-r--r--   0        0        0     1665 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/add_validity_to_server_keys.sql
+-rw-r--r--   0        0        0     1806 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/delete_forward_extremities.sql
+-rw-r--r--   0        0        0     1881 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/drop_legacy_tables.sql
+-rw-r--r--   0        0        0     1323 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/drop_presence_list.sql
+-rw-r--r--   0        0        0     1846 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/relations.sql
+-rw-r--r--   0        0        0     3205 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/stats.sql
+-rw-r--r--   0        0        0     1895 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/stats2.sql
+-rw-r--r--   0        0        0     1472 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/55/access_token_expiry.sql
+-rw-r--r--   0        0        0     1804 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/55/track_threepid_validations.sql
+-rw-r--r--   0        0        0     1476 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/55/users_alter_deactivated.sql
+-rw-r--r--   0        0        0     1559 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/add_spans_to_device_lists.sql
+-rw-r--r--   0        0        0     1725 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/current_state_events_membership.sql
+-rw-r--r--   0        0        0     1784 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/current_state_events_membership_mk2.sql
+-rw-r--r--   0        0        0     1626 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/delete_keys_from_deleted_backups.sql
+-rw-r--r--   0        0        0     1635 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/destinations_failure_ts.sql
+-rw-r--r--   0        0        0      806 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/destinations_retry_interval_type.sql.postgres
+-rw-r--r--   0        0        0     1594 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/device_stream_id_insert.sql
+-rw-r--r--   0        0        0     1713 2024-01-09 15:11:25.446848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/devices_last_seen.sql
+-rw-r--r--   0        0        0     1475 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/drop_unused_event_tables.sql
+-rw-r--r--   0        0        0     1480 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/event_expiry.sql
+-rw-r--r--   0        0        0     1961 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/event_labels.sql
+-rw-r--r--   0        0        0     1404 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/event_labels_background_update.sql
+-rw-r--r--   0        0        0     1503 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/fix_room_keys_index.sql
+-rw-r--r--   0        0        0     1460 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/hidden_devices.sql
+-rw-r--r--   0        0        0     1449 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/hidden_devices_fix.sql.sqlite
+-rw-r--r--   0        0        0     3619 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/nuke_empty_communities_from_db.sql
+-rw-r--r--   0        0        0     1415 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/public_room_list_idx.sql
+-rw-r--r--   0        0        0     1382 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor.sql
+-rw-r--r--   0        0        0     1576 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor2.sql
+-rw-r--r--   0        0        0     1093 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor3_fix_update.sql.postgres
+-rw-r--r--   0        0        0     1352 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor4.sql
+-rw-r--r--   0        0        0     1543 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/remove_tombstoned_rooms_from_directory.sql
+-rw-r--r--   0        0        0     1404 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/room_key_etag.sql
+-rw-r--r--   0        0        0     1496 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/room_membership_idx.sql
+-rw-r--r--   0        0        0     1933 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/room_retention.sql
+-rw-r--r--   0        0        0     2783 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/signing_keys.sql
+-rw-r--r--   0        0        0     1743 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/signing_keys_nonunique_signatures.sql
+-rw-r--r--   0        0        0     5860 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/stats_separated.sql
+-rw-r--r--   0        0        0     1620 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/unique_user_filter_index.py
+-rw-r--r--   0        0        0     1565 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/user_external_ids.sql
+-rw-r--r--   0        0        0     1452 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/users_in_public_rooms_idx.sql
+-rw-r--r--   0        0        0     1679 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/delete_old_current_state_events.sql
+-rw-r--r--   0        0        0     1787 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/device_list_remote_cache_stale.sql
+-rw-r--r--   0        0        0     4397 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/local_current_membership.py
+-rw-r--r--   0        0        0     1538 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/remove_sent_outbound_pokes.sql
+-rw-r--r--   0        0        0     1634 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column.sql
+-rw-r--r--   0        0        0     1713 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.postgres
+-rw-r--r--   0        0        0      998 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.sqlite
+-rw-r--r--   0        0        0     1920 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.postgres
+-rw-r--r--   0        0        0      998 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.sqlite
+-rw-r--r--   0        0        0     1594 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/02remove_dup_outbound_pokes.sql
+-rw-r--r--   0        0        0     2520 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/03persist_ui_auth.sql
+-rw-r--r--   0        0        0     1148 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/05cache_instance.sql.postgres
+-rw-r--r--   0        0        0     2784 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/06dlols_unique_idx.py
+-rw-r--r--   0        0        0     1552 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.postgres
+-rw-r--r--   0        0        0     2349 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.sqlite
+-rw-r--r--   0        0        0     1677 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/07persist_ui_auth_ips.sql
+-rw-r--r--   0        0        0      823 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.postgres
+-rw-r--r--   0        0        0      819 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.sqlite
+-rw-r--r--   0        0        0     1458 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/09shadow_ban.sql
+-rw-r--r--   0        0        0     1752 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/10_pushrules_enabled_delete_obsolete.sql
+-rw-r--r--   0        0        0     1556 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/10drop_local_rejections_stream.sql
+-rw-r--r--   0        0        0     1740 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/10federation_pos_instance_name.sql
+-rw-r--r--   0        0        0     1488 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/11dehydration.sql
+-rw-r--r--   0        0        0     1862 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/11fallback.sql
+-rw-r--r--   0        0        0     1261 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/11user_id_seq.py
+-rw-r--r--   0        0        0     2255 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/12room_stats.sql
+-rw-r--r--   0        0        0     1383 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/13remove_presence_allow_inbound.sql
+-rw-r--r--   0        0        0     1355 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/14events_instance_name.sql
+-rw-r--r--   0        0        0     1074 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/14events_instance_name.sql.postgres
+-rw-r--r--   0        0        0     2821 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/15_catchup_destination_rooms.sql
+-rw-r--r--   0        0        0     1886 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/15unread_count.sql
+-rw-r--r--   0        0        0     1790 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/16populate_stats_process_rooms_fix.sql
+-rw-r--r--   0        0        0     1641 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/17_catchup_last_successful.sql
+-rw-r--r--   0        0        0     1524 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/18stream_positions.sql
+-rw-r--r--   0        0        0     1001 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/19instance_map.sql.postgres
+-rw-r--r--   0        0        0     2353 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/19txn_id.sql
+-rw-r--r--   0        0        0     1435 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/20instance_name_event_tables.sql
+-rw-r--r--   0        0        0     1427 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/20user_daily_visits.sql
+-rw-r--r--   0        0        0     1455 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/21as_device_stream.sql
+-rw-r--r--   0        0        0       33 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/21drop_device_max_stream_id.sql
+-rw-r--r--   0        0        0     1439 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/22puppet_token.sql
+-rw-r--r--   0        0        0      119 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/22users_have_local_media.sql
+-rw-r--r--   0        0        0     1427 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/23e2e_cross_signing_keys_idx.sql
+-rw-r--r--   0        0        0     1480 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/24drop_event_json_index.sql
+-rw-r--r--   0        0        0     1430 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/25user_external_ids_user_id_idx.sql
+-rw-r--r--   0        0        0     1484 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/26access_token_last_validated.sql
+-rw-r--r--   0        0        0     1376 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/27local_invites.sql
+-rw-r--r--   0        0        0      660 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.postgres
+-rw-r--r--   0        0        0     2126 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.sqlite
+-rw-r--r--   0        0        0     3324 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/01ignored_user.py
+-rw-r--r--   0        0        0     1495 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/02shard_send_to_device.sql
+-rw-r--r--   0        0        0      999 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/03shard_send_to_device_sequence.sql.postgres
+-rw-r--r--   0        0        0     2381 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql
+-rw-r--r--   0        0        0      663 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql.postgres
+-rw-r--r--   0        0        0     1433 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/04drop_account_data.sql
+-rw-r--r--   0        0        0     1432 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/05cache_invalidation.sql
+-rw-r--r--   0        0        0     1452 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/06chain_cover_index.sql
+-rw-r--r--   0        0        0     1548 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/06shard_account_data.sql
+-rw-r--r--   0        0        0     1193 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/06shard_account_data.sql.postgres
+-rw-r--r--   0        0        0     1503 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/07shard_account_data_fix.sql
+-rw-r--r--   0        0        0     1542 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/08delete_pushers_for_deactivated_accounts.sql
+-rw-r--r--   0        0        0     1569 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/08delete_stale_pushers.sql
+-rw-r--r--   0        0        0     1975 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/09rejected_events_metadata.sql
+-rw-r--r--   0        0        0     1420 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/10delete_purged_chain_cover.sql
+-rw-r--r--   0        0        0     1595 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/11add_knock_members_to_stats.sql
+-rw-r--r--   0        0        0     1008 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/11drop_thumbnail_constraint.sql.postgres
+-rw-r--r--   0        0        0     1520 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/12account_validity_token_used_ts_ms.sql
+-rw-r--r--   0        0        0     1503 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/12presence_stream_instance.sql
+-rw-r--r--   0        0        0      777 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/12presence_stream_instance_seq.sql.postgres
+-rw-r--r--   0        0        0     2268 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/13users_to_send_full_presence_to.sql
+-rw-r--r--   0        0        0     1960 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/14refresh_tokens.sql
+-rw-r--r--   0        0        0     2352 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/15locks.sql
+-rw-r--r--   0        0        0     2020 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/16federation_inbound_staging.sql
+-rw-r--r--   0        0        0     2254 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/60/01recreate_stream_ordering.sql.postgres
+-rw-r--r--   0        0        0     1480 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/60/02change_stream_ordering_columns.sql.postgres
+-rw-r--r--   0        0        0     1083 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/01change_appservices_txns.sql.postgres
+-rw-r--r--   0        0        0     2952 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/01insertion_event_lookups.sql
+-rw-r--r--   0        0        0     1416 2024-01-09 15:11:25.450848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/02drop_redundant_room_depth_index.sql
+-rw-r--r--   0        0        0     2366 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/03recreate_min_depth.py
+-rw-r--r--   0        0        0     1718 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/62/01insertion_event_extremities.sql
+-rw-r--r--   0        0        0     1845 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/01create_registration_tokens.sql
+-rw-r--r--   0        0        0     1570 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/02delete_unlinked_email_pushers.sql
+-rw-r--r--   0        0        0     1432 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/02populate-rooms-creator.sql
+-rw-r--r--   0        0        0     1697 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/03session_store.sql
+-rw-r--r--   0        0        0     1439 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/04add_presence_stream_not_offline_index.sql
+-rw-r--r--   0        0        0     1045 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.postgres
+-rw-r--r--   0        0        0     1523 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.sqlite
+-rw-r--r--   0        0        0     1579 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/01msc2716_insertion_event_edges.sql
+-rw-r--r--   0        0        0     1638 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/03remove_hidden_devices_from_device_inbox.sql
+-rw-r--r--   0        0        0     1477 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/04_local_group_updates.sql
+-rw-r--r--   0        0        0     1531 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/05_remove_room_stats_historical_and_user_stats_historical.sql
+-rw-r--r--   0        0        0     2334 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/06remove_deleted_devices_from_device_inbox.sql
+-rw-r--r--   0        0        0     1468 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/07_arbitrary_relations.sql
+-rw-r--r--   0        0        0     1511 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/08_device_inbox_background_updates.sql
+-rw-r--r--   0        0        0     1913 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/10_expirable_refresh_tokens.sql
+-rw-r--r--   0        0        0     1753 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/11_devices_auth_provider_session.sql
+-rw-r--r--   0        0        0     1384 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/67/01drop_public_room_list_stream.sql
+-rw-r--r--   0        0        0     1671 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/01event_columns.sql
+-rw-r--r--   0        0        0     1657 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/02_msc2409_add_device_id_appservice_stream_type.sql
+-rw-r--r--   0        0        0     1535 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/03_delete_account_data_for_deactivated_accounts.sql
+-rw-r--r--   0        0        0     1976 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/04_refresh_tokens_index_next_token_id.sql
+-rw-r--r--   0        0        0     2274 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/04partial_state_rooms.sql
+-rw-r--r--   0        0        0      968 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/05_delete_non_strings_from_event_search.sql.sqlite
+-rw-r--r--   0        0        0     2899 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/05partial_state_rooms_triggers.py
+-rw-r--r--   0        0        0     1771 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/06_msc3202_add_device_list_appservice_stream_type.sql
+-rw-r--r--   0        0        0     1945 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/69/01as_txn_seq.py
+-rw-r--r--   0        0        0     2446 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/69/01device_list_oubound_by_room.sql
+-rw-r--r--   0        0        0     1510 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/69/02cache_invalidation_index.sql
+-rw-r--r--   0        0        0     1566 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/70/01clean_table_purged_rooms.sql
+-rw-r--r--   0        0        0     2096 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.postgres
+-rw-r--r--   0        0        0     1800 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.sqlite
+-rw-r--r--   0        0        0     3821 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/01remove_noop_background_updates.sql
+-rw-r--r--   0        0        0     1478 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/02event_push_summary_unique.sql
+-rw-r--r--   0        0        0     1457 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/01add_room_type_to_state_stats.sql
+-rw-r--r--   0        0        0     2167 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/01event_push_summary_receipt.sql
+-rw-r--r--   0        0        0     1541 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/02event_push_actions_index.sql
+-rw-r--r--   0        0        0     2085 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/03bg_populate_events_columns.py
+-rw-r--r--   0        0        0     1394 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/03drop_event_reference_hashes.sql
+-rw-r--r--   0        0        0     1998 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/03remove_groups.sql
+-rw-r--r--   0        0        0      730 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.postgres
+-rw-r--r--   0        0        0     1338 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.sqlite
+-rw-r--r--   0        0        0     1464 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/05receipts_event_stream_ordering.sql
+-rw-r--r--   0        0        0     1583 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/05remove_unstable_private_read_receipts.sql
+-rw-r--r--   0        0        0     1345 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/06add_consent_ts_to_users.sql
+-rw-r--r--   0        0        0     2052 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/06thread_notifications.sql
+-rw-r--r--   0        0        0     2031 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/07force_update_current_state_events_membership.py
+-rw-r--r--   0        0        0     1249 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/07thread_receipts.sql.postgres
+-rw-r--r--   0        0        0     2741 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/07thread_receipts.sql.sqlite
+-rw-r--r--   0        0        0     1007 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/08begin_cache_invalidation_seq_at_2.sql.postgres
+-rw-r--r--   0        0        0     1558 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/08thread_receipts.sql
+-rw-r--r--   0        0        0     2347 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/09partial_indices.sql.sqlite
+-rw-r--r--   0        0        0     1912 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/01event_failed_pull_attempts.sql
+-rw-r--r--   0        0        0     1351 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/02add_pusher_enabled.sql
+-rw-r--r--   0        0        0     1728 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/02room_id_indexes_for_purging.sql
+-rw-r--r--   0        0        0     1704 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/03pusher_device_id.sql
+-rw-r--r--   0        0        0     1584 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/03users_approved_column.sql
+-rw-r--r--   0        0        0     1879 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/04partial_join_details.sql
+-rw-r--r--   0        0        0     1850 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/04pending_device_list_updates.sql
+-rw-r--r--   0        0        0     1038 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/05old_push_actions.sql.postgres
+-rw-r--r--   0        0        0     1097 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/05old_push_actions.sql.sqlite
+-rw-r--r--   0        0        0     1765 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/06thread_notifications_thread_id_idx.sql
+-rw-r--r--   0        0        0      881 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.postgres
+-rw-r--r--   0        0        0     2896 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.sqlite
+-rw-r--r--   0        0        0     1516 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/09partial_joined_via_destination.sql
+-rw-r--r--   0        0        0     1893 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/09threads_table.sql
+-rw-r--r--   0        0        0     2185 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/10_update_sqlite_fts4_tokenizer.py
+-rw-r--r--   0        0        0     1938 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/10login_tokens.sql
+-rw-r--r--   0        0        0     1595 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/11event_search_room_id_n_distinct.sql.postgres
+-rw-r--r--   0        0        0     3153 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/12refactor_device_list_outbound_pokes.sql
+-rw-r--r--   0        0        0     1553 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/13add_device_lists_index.sql
+-rw-r--r--   0        0        0     2068 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/20_un_partial_stated_room_stream.sql
+-rw-r--r--   0        0        0      819 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/21_un_partial_stated_room_stream_seq.sql.postgres
+-rw-r--r--   0        0        0     2240 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/22_rebuild_user_dir_stats.sql
+-rw-r--r--   0        0        0     2078 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/22_un_partial_stated_event_stream.sql
+-rw-r--r--   0        0        0     2277 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/23_fix_thread_index.sql
+-rw-r--r--   0        0        0      822 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/23_un_partial_stated_room_stream_seq.sql.postgres
+-rw-r--r--   0        0        0     1426 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/24_events_jump_to_date_index.sql
+-rw-r--r--   0        0        0     1349 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/25drop_presence.sql
+-rw-r--r--   0        0        0     2420 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/01_user_directory_stale_remote_users.sql
+-rw-r--r--   0        0        0     1554 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/02_set_device_id_for_pushers_bg_update.sql
+-rw-r--r--   0        0        0     1655 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.postgres
+-rw-r--r--   0        0        0     1183 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.sqlite
+-rw-r--r--   0        0        0     1537 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/03_room_membership_index.sql
+-rw-r--r--   0        0        0     1444 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/04_delete_e2e_backup_keys_for_deactivated_users.sql
+-rw-r--r--   0        0        0     3140 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/04_membership_tables_event_stream_ordering_triggers.py
+-rw-r--r--   0        0        0     3002 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/05_events_txn_id_device_id.sql
+-rw-r--r--   0        0        0     2422 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/90COMMENTS_destinations.sql.postgres
+-rw-r--r--   0        0        0     1581 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/01_add_profiles_full_user_id_column.sql
+-rw-r--r--   0        0        0     1577 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/02_add_user_filters_full_user_id_column.sql
+-rw-r--r--   0        0        0     1798 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/03_per_user_experimental_features.sql
+-rw-r--r--   0        0        0     1602 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/04_add_room_forgetter.sql
+-rw-r--r--   0        0        0      713 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/01_add_profiles_not_valid_check.sql.postgres
+-rw-r--r--   0        0        0      717 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/02_add_user_filters_not_valid_check.sql.postgres
+-rw-r--r--   0        0        0     1428 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/03bg_populate_full_user_id_profiles.sql
+-rw-r--r--   0        0        0     1432 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/04bg_populate_full_user_id_user_filters.sql
+-rw-r--r--   0        0        0     3164 2024-01-09 15:11:25.454848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/05thread_notifications_backfill.sql
+-rw-r--r--   0        0        0     4506 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null.sql.sqlite
+-rw-r--r--   0        0        0     1347 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions.sql.postgres
+-rw-r--r--   0        0        0     1319 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions_staging.sql.postgres
+-rw-r--r--   0        0        0     1465 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_summary.sql.postgres
+-rw-r--r--   0        0        0     1584 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/14bg_indices_event_stream_ordering.sql
+-rw-r--r--   0        0        0     3171 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/01_validate_and_update_profiles.py
+-rw-r--r--   0        0        0     3190 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/02_validate_and_update_user_filters.py
+-rw-r--r--   0        0        0     2243 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/03_remove_unused_indexes_user_filters.py
+-rw-r--r--   0        0        0     2489 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/03event_extremities_constraints.py
+-rw-r--r--   0        0        0     1127 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/04_add_full_user_id_index_user_filters.py
+-rw-r--r--   0        0        0     5225 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.postgres
+-rw-r--r--   0        0        0     3690 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.sqlite
+-rw-r--r--   0        0        0     2953 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/04_mitigate_stream_ordering_update_race.py
+-rw-r--r--   0        0        0     2763 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.postgres
+-rw-r--r--   0        0        0     2853 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.sqlite
+-rw-r--r--   0        0        0     1366 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/01_users_alter_locked.sql
+-rw-r--r--   0        0        0     1512 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/02_read_write_locks_unlogged.sql.postgres
+-rw-r--r--   0        0        0     1670 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/02_scheduled_tasks.sql
+-rw-r--r--   0        0        0     1544 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/03_read_write_locks_triggers.sql.postgres
+-rw-r--r--   0        0        0     2625 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/04_read_write_locks_deadlock.sql.postgres
+-rw-r--r--   0        0        0     1388 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/82/02_scheduled_tasks_index.sql
+-rw-r--r--   0        0        0     1561 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/82/04_add_indices_for_purging_rooms.sql
+-rw-r--r--   0        0        0     1741 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/82/05gaps.sql
+-rw-r--r--   0        0        0     1688 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/01_drop_old_tables.sql
+-rw-r--r--   0        0        0      711 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/03_instance_name_receipts.sql.sqlite
+-rw-r--r--   0        0        0     1401 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/05_cross_signing_key_update_grant.sql
+-rw-r--r--   0        0        0     1435 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/06_event_push_summary_room.sql
+-rw-r--r--   0        0        0    53196 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/full_schemas/72/full.sql.postgres
+-rw-r--r--   0        0        0    42458 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/main/full_schemas/72/full.sql.sqlite
+-rw-r--r--   0        0        0     1340 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/23/drop_state_index.sql
+-rw-r--r--   0        0        0     1439 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/32/remove_state_indices.sql
+-rw-r--r--   0        0        0     1445 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/35/add_state_index.sql
+-rw-r--r--   0        0        0     1543 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/35/state.sql
+-rw-r--r--   0        0        0     1401 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/35/state_dedupe.sql
+-rw-r--r--   0        0        0     1356 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/47/state_group_seq.py
+-rw-r--r--   0        0        0     1412 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/56/state_group_room_idx.sql
+-rw-r--r--   0        0        0     1662 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/61/02state_groups_state_n_distinct.sql.postgres
+-rw-r--r--   0        0        0     1431 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/70/08_state_group_edges_unique.sql
+-rw-r--r--   0        0        0     1128 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/full_schemas/72/full.sql.postgres
+-rw-r--r--   0        0        0      741 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/schema/state/full_schemas/72/full.sql.sqlite
+-rw-r--r--   0        0        0     6638 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/types.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/util/__init__.py
+-rw-r--r--   0        0        0    38595 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/util/id_generators.py
+-rw-r--r--   0        0        0     7348 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/util/partial_state_events_tracker.py
+-rw-r--r--   0        0        0    10025 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/storage/util/sequence.py
+-rw-r--r--   0        0        0     1257 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/streams/__init__.py
+-rw-r--r--   0        0        0     2984 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/streams/config.py
+-rw-r--r--   0        0        0     4802 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/streams/events.py
+-rw-r--r--   0        0        0      125 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/synapse_rust/__init__.pyi
+-rw-r--r--   0        0        0      828 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/synapse_rust/acl.pyi
+-rw-r--r--   0        0        0     4168 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/synapse_rust/events.pyi
+-rw-r--r--   0        0        0     2542 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/synapse_rust/push.pyi
+-rw-r--r--   0        0        0    41228 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/types/__init__.py
+-rw-r--r--   0        0        0    21806 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/types/state.py
+-rw-r--r--   0        0        0     7308 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/util/__init__.py
+-rw-r--r--   0        0        0    31245 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/util/async_helpers.py
+-rw-r--r--   0        0        0     6419 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/util/batching_queue.py
+-rw-r--r--   0        0        0     8361 2024-01-09 15:11:25.458848 matrix_synapse-1.99.0rc1/synapse/util/caches/__init__.py
+-rw-r--r--   0        0        0     5450 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/cached_call.py
+-rw-r--r--   0        0        0    18245 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/deferred_cache.py
+-rw-r--r--   0        0        0    23181 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/descriptors.py
+-rw-r--r--   0        0        0    11916 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/dictionary_cache.py
+-rw-r--r--   0        0        0     7400 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/expiringcache.py
+-rw-r--r--   0        0        0    30017 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/lrucache.py
+-rw-r--r--   0        0        0     9404 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/response_cache.py
+-rw-r--r--   0        0        0    11712 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/stream_change_cache.py
+-rw-r--r--   0        0        0     5893 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/treecache.py
+-rw-r--r--   0        0        0     5301 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/caches/ttlcache.py
+-rw-r--r--   0        0        0     2466 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/cancellation.py
+-rw-r--r--   0        0        0     8054 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/check_dependencies.py
+-rw-r--r--   0        0        0     5048 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/daemonize.py
+-rw-r--r--   0        0        0     5016 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/distributor.py
+-rw-r--r--   0        0        0     6349 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/file_consumer.py
+-rw-r--r--   0        0        0     1380 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/frozenutils.py
+-rw-r--r--   0        0        0     5214 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/gai_resolver.py
+-rw-r--r--   0        0        0     1106 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/hash.py
+-rw-r--r--   0        0        0     4273 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/httpresourcetree.py
+-rw-r--r--   0        0        0     5494 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/iterutils.py
+-rw-r--r--   0        0        0     5083 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/linked_list.py
+-rw-r--r--   0        0        0     1219 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/logcontext.py
+-rw-r--r--   0        0        0      845 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/logformatter.py
+-rw-r--r--   0        0        0    12051 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/macaroons.py
+-rw-r--r--   0        0        0     8317 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/manhole.py
+-rw-r--r--   0        0        0     7795 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/metrics.py
+-rw-r--r--   0        0        0     4003 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/module_loader.py
+-rw-r--r--   0        0        0     1641 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/msisdn.py
+-rw-r--r--   0        0        0     9125 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/patch_inline_callbacks.py
+-rw-r--r--   0        0        0    13544 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/ratelimitutils.py
+-rw-r--r--   0        0        0    12127 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/retryutils.py
+-rw-r--r--   0        0        0     1317 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/rlimit.py
+-rw-r--r--   0        0        0     2607 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/rust.py
+-rw-r--r--   0        0        0     8229 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/stringutils.py
+-rw-r--r--   0        0        0    15870 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/task_scheduler.py
+-rw-r--r--   0        0        0     4040 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/templates.py
+-rw-r--r--   0        0        0     3745 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/threepids.py
+-rw-r--r--   0        0        0     3599 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/util/wheel_timer.py
+-rw-r--r--   0        0        0    30251 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synapse/visibility.py
+-rw-r--r--   0        0        0     1354 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synmark/__init__.py
+-rw-r--r--   0        0        0     3657 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synmark/__main__.py
+-rw-r--r--   0        0        0      176 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synmark/suites/__init__.py
+-rw-r--r--   0        0        0     4380 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synmark/suites/logging.py
+-rw-r--r--   0        0        0     1134 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synmark/suites/lrucache.py
+-rw-r--r--   0        0        0     1157 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/synmark/suites/lrucache_evict.py
+-rw-r--r--   0        0        0     1610 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/sytest-blacklist
+-rw-r--r--   0        0        0      869 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/api/__init__.py
+-rw-r--r--   0        0        0    23538 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/api/test_auth.py
+-rw-r--r--   0        0        0     1882 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/api/test_errors.py
+-rw-r--r--   0        0        0    23756 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/api/test_filtering.py
+-rw-r--r--   0        0        0    16009 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/api/test_ratelimiting.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/app/__init__.py
+-rw-r--r--   0        0        0     1594 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/app/test_homeserver_start.py
+-rw-r--r--   0        0        0     4695 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/app/test_openid_listener.py
+-rw-r--r--   0        0        0    10015 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/app/test_phone_stats_home.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/appservice/__init__.py
+-rw-r--r--   0        0        0     9001 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/appservice/test_api.py
+-rw-r--r--   0        0        0     9396 2024-01-09 15:11:25.462848 matrix_synapse-1.99.0rc1/tests/appservice/test_appservice.py
+-rw-r--r--   0        0        0    17606 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/appservice/test_scheduler.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/__init__.py
+-rw-r--r--   0        0        0     1310 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test___main__.py
+-rw-r--r--   0        0        0     4054 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_api.py
+-rw-r--r--   0        0        0     1512 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_appservice.py
+-rw-r--r--   0        0        0     2588 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_background_update.py
+-rw-r--r--   0        0        0     5501 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_base.py
+-rw-r--r--   0        0        0     6761 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_cache.py
+-rw-r--r--   0        0        0     1212 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_database.py
+-rw-r--r--   0        0        0     2244 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_generate.py
+-rw-r--r--   0        0        0     5012 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_load.py
+-rw-r--r--   0        0        0    11062 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_oauth_delegation.py
+-rw-r--r--   0        0        0     2507 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_ratelimiting.py
+-rw-r--r--   0        0        0     3739 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_registration_config.py
+-rw-r--r--   0        0        0     4922 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_room_directory.py
+-rw-r--r--   0        0        0     6474 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_server.py
+-rw-r--r--   0        0        0     7846 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_tls.py
+-rw-r--r--   0        0        0     1792 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_util.py
+-rw-r--r--   0        0        0    12025 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/test_workers.py
+-rw-r--r--   0        0        0     2058 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/config/utils.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/crypto/__init__.py
+-rw-r--r--   0        0        0     3661 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/crypto/test_event_signing.py
+-rw-r--r--   0        0        0    27314 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/crypto/test_keyring.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/events/__init__.py
+-rw-r--r--   0        0        0    18867 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/events/test_presence_router.py
+-rw-r--r--   0        0        0     4154 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/events/test_snapshot.py
+-rw-r--r--   0        0        0    28325 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/events/test_utils.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/__init__.py
+-rw-r--r--   0        0        0     9343 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/test_complexity.py
+-rw-r--r--   0        0        0    22608 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/test_federation_catch_up.py
+-rw-r--r--   0        0        0    11712 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/test_federation_client.py
+-rw-r--r--   0        0        0    28083 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/test_federation_sender.py
+-rw-r--r--   0        0        0    13571 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/test_federation_server.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/transport/__init__.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/transport/server/__init__.py
+-rw-r--r--   0        0        0     5028 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/transport/server/test__base.py
+-rw-r--r--   0        0        0     5870 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/transport/test_client.py
+-rw-r--r--   0        0        0    12138 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/transport/test_knocking.py
+-rw-r--r--   0        0        0     2408 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/federation/transport/test_server.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/__init__.py
+-rw-r--r--   0        0        0      241 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/oidc_test_key.p8
+-rw-r--r--   0        0        0      178 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/oidc_test_key.pub.pem
+-rw-r--r--   0        0        0    13984 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_admin.py
+-rw-r--r--   0        0        0    50710 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_appservice.py
+-rw-r--r--   0        0        0     8362 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_auth.py
+-rw-r--r--   0        0        0     8214 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_cas.py
+-rw-r--r--   0        0        0    11342 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_deactivate_account.py
+-rw-r--r--   0        0        0    23221 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_device.py
+-rw-r--r--   0        0        0    21741 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_directory.py
+-rw-r--r--   0        0        0    63167 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_e2e_keys.py
+-rw-r--r--   0        0        0    19558 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_e2e_room_keys.py
+-rw-r--r--   0        0        0    30062 2024-01-09 15:11:25.466848 matrix_synapse-1.99.0rc1/tests/handlers/test_federation.py
+-rw-r--r--   0        0        0    47947 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_federation_event.py
+-rw-r--r--   0        0        0    13092 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_message.py
+-rw-r--r--   0        0        0    32877 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_oauth_delegation.py
+-rw-r--r--   0        0        0    54346 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_oidc.py
+-rw-r--r--   0        0        0    38830 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_password_providers.py
+-rw-r--r--   0        0        0    71302 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_presence.py
+-rw-r--r--   0        0        0    14047 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_profile.py
+-rw-r--r--   0        0        0    12352 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_receipts.py
+-rw-r--r--   0        0        0    32054 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_register.py
+-rw-r--r--   0        0        0     4317 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_room.py
+-rw-r--r--   0        0        0     2832 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_room_list.py
+-rw-r--r--   0        0        0    16212 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_room_member.py
+-rw-r--r--   0        0        0    41655 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_room_summary.py
+-rw-r--r--   0        0        0    13234 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_saml.py
+-rw-r--r--   0        0        0     8030 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_send_email.py
+-rw-r--r--   0        0        0     5689 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_sso.py
+-rw-r--r--   0        0        0    19776 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_stats.py
+-rw-r--r--   0        0        0    12118 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_sync.py
+-rw-r--r--   0        0        0    16574 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_typing.py
+-rw-r--r--   0        0        0    52141 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_user_directory.py
+-rw-r--r--   0        0        0     2707 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/handlers/test_worker_lock.py
+-rw-r--r--   0        0        0     5777 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/__init__.py
+-rw-r--r--   0        0        0     1115 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/ca.crt
+-rw-r--r--   0        0        0     1679 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/ca.key
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/federation/__init__.py
+-rw-r--r--   0        0        0    67753 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/federation/test_matrix_federation_agent.py
+-rw-r--r--   0        0        0     7864 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/federation/test_srv_resolver.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/server/__init__.py
+-rw-r--r--   0        0        0    22077 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/server/_base.py
+-rw-r--r--   0        0        0     1679 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/server.key
+-rw-r--r--   0        0        0     2578 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_additional_resource.py
+-rw-r--r--   0        0        0     9164 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_client.py
+-rw-r--r--   0        0        0     2114 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_endpoint.py
+-rw-r--r--   0        0        0    34255 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_matrixfederationclient.py
+-rw-r--r--   0        0        0     2016 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_proxy.py
+-rw-r--r--   0        0        0    34549 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_proxyagent.py
+-rw-r--r--   0        0        0     4898 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_servlet.py
+-rw-r--r--   0        0        0     6225 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_simple_client.py
+-rw-r--r--   0        0        0     3269 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/http/test_site.py
+-rw-r--r--   0        0        0     1355 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/logging/__init__.py
+-rw-r--r--   0        0        0    10995 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/logging/test_opentracing.py
+-rw-r--r--   0        0        0     6430 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/logging/test_remote_handler.py
+-rw-r--r--   0        0        0     8219 2024-01-09 15:11:25.470848 matrix_synapse-1.99.0rc1/tests/logging/test_terse_json.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/__init__.py
+-rw-r--r--   0        0        0     3397 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_base.py
+-rw-r--r--   0        0        0    23048 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_filepath.py
+-rw-r--r--   0        0        0    20965 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_html_preview.py
+-rw-r--r--   0        0        0    11477 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_media_retention.py
+-rw-r--r--   0        0        0    30878 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_media_storage.py
+-rw-r--r--   0        0        0     6835 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_oembed.py
+-rw-r--r--   0        0        0     4477 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/media/test_url_previewer.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/metrics/__init__.py
+-rw-r--r--   0        0        0      774 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/metrics/test_background_process_metrics.py
+-rw-r--r--   0        0        0     7242 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/metrics/test_metrics.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/module_api/__init__.py
+-rw-r--r--   0        0        0     5868 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/module_api/test_account_data_manager.py
+-rw-r--r--   0        0        0    39878 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/module_api/test_api.py
+-rw-r--r--   0        0        0     2273 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/module_api/test_event_unsigned_addition.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/push/__init__.py
+-rw-r--r--   0        0        0    16883 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/push/test_bulk_push_rule_evaluator.py
+-rw-r--r--   0        0        0    20451 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/push/test_email.py
+-rw-r--r--   0        0        0    39462 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/push/test_http.py
+-rw-r--r--   0        0        0     9210 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/push/test_presentable_names.py
+-rw-r--r--   0        0        0    32846 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/push/test_push_rule_evaluator.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/__init__.py
+-rw-r--r--   0        0        0    22959 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/_base.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/http/__init__.py
+-rw-r--r--   0        0        0     3726 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/http/test__base.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/storage/__init__.py
+-rw-r--r--   0        0        0     2911 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/storage/_base.py
+-rw-r--r--   0        0        0    14928 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/storage/test_events.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/__init__.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/__init__.py
+-rw-r--r--   0        0        0     4416 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_account_data.py
+-rw-r--r--   0        0        0    20007 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_events.py
+-rw-r--r--   0        0        0     3442 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_federation.py
+-rw-r--r--   0        0        0     2341 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_partial_state.py
+-rw-r--r--   0        0        0     3343 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_receipts.py
+-rw-r--r--   0        0        0     3282 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_to_device.py
+-rw-r--r--   0        0        0     6290 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_typing.py
+-rw-r--r--   0        0        0     1784 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/test_commands.py
+-rw-r--r--   0        0        0     7871 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/tcp/test_handler.py
+-rw-r--r--   0        0        0     4240 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_auth.py
+-rw-r--r--   0        0        0     3304 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_client_reader_shard.py
+-rw-r--r--   0        0        0     3561 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_federation_ack.py
+-rw-r--r--   0        0        0     9938 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_federation_sender_shard.py
+-rw-r--r--   0        0        0     2728 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_module_cache_invalidation.py
+-rw-r--r--   0        0        0     9661 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_multi_media_repo.py
+-rw-r--r--   0        0        0     6716 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_pusher_shard.py
+-rw-r--r--   0        0        0    12184 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_sharded_event_persister.py
+-rw-r--r--   0        0        0     8996 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/replication/test_sharded_receipts.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/rest/__init__.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.474848 matrix_synapse-1.99.0rc1/tests/rest/admin/__init__.py
+-rw-r--r--   0        0        0    16729 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_admin.py
+-rw-r--r--   0        0        0    12428 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_background_updates.py
+-rw-r--r--   0        0        0    17488 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_device.py
+-rw-r--r--   0        0        0    26187 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_event_reports.py
+-rw-r--r--   0        0        0    29729 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_federation.py
+-rw-r--r--   0        0        0     5528 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_jwks.py
+-rw-r--r--   0        0        0    30136 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_media.py
+-rw-r--r--   0        0        0    26019 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_registration_tokens.py
+-rw-r--r--   0        0        0   106429 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_room.py
+-rw-r--r--   0        0        0    27177 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_server_notice.py
+-rw-r--r--   0        0        0    18242 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_statistics.py
+-rw-r--r--   0        0        0   180599 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_user.py
+-rw-r--r--   0        0        0     2902 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/admin/test_username_available.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/__init__.py
+-rw-r--r--   0        0        0    51250 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_account.py
+-rw-r--r--   0        0        0     2854 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_account_data.py
+-rw-r--r--   0        0        0    55112 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_auth.py
+-rw-r--r--   0        0        0     2135 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_auth_issuer.py
+-rw-r--r--   0        0        0     9198 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_capabilities.py
+-rw-r--r--   0        0        0     4639 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_consent.py
+-rw-r--r--   0        0        0    22086 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_devices.py
+-rw-r--r--   0        0        0     9548 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_directory.py
+-rw-r--r--   0        0        0     4212 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_ephemeral_message.py
+-rw-r--r--   0        0        0     5725 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_events.py
+-rw-r--r--   0        0        0     4298 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_filter.py
+-rw-r--r--   0        0        0     2240 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_identity.py
+-rw-r--r--   0        0        0    15938 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_keys.py
+-rw-r--r--   0        0        0    60842 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_login.py
+-rw-r--r--   0        0        0     6390 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_login_token_request.py
+-rw-r--r--   0        0        0     3025 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_models.py
+-rw-r--r--   0        0        0     5833 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_mutual_rooms.py
+-rw-r--r--   0        0        0     3444 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_notifications.py
+-rw-r--r--   0        0        0     6708 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_password_policy.py
+-rw-r--r--   0        0        0     9713 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_power_levels.py
+-rw-r--r--   0        0        0     3267 2024-01-09 15:11:25.478848 matrix_synapse-1.99.0rc1/tests/rest/client/test_presence.py
+-rw-r--r--   0        0        0    23618 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_profile.py
+-rw-r--r--   0        0        0    16982 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_push_rule_attrs.py
+-rw-r--r--   0        0        0     5073 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_read_marker.py
+-rw-r--r--   0        0        0    10434 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_receipts.py
+-rw-r--r--   0        0        0    25015 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_redactions.py
+-rw-r--r--   0        0        0    46981 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_register.py
+-rw-r--r--   0        0        0    76170 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_relations.py
+-rw-r--r--   0        0        0     1733 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_rendezvous.py
+-rw-r--r--   0        0        0     5321 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_report_event.py
+-rw-r--r--   0        0        0    15135 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_retention.py
+-rw-r--r--   0        0        0   138187 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_rooms.py
+-rw-r--r--   0        0        0     9195 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_sendtodevice.py
+-rw-r--r--   0        0        0    12034 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_shadow_banned.py
+-rw-r--r--   0        0        0    29719 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_sync.py
+-rw-r--r--   0        0        0    40200 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_third_party_rules.py
+-rw-r--r--   0        0        0     7353 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_transactions.py
+-rw-r--r--   0        0        0     3641 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_typing.py
+-rw-r--r--   0        0        0    15000 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/test_upgrade_room.py
+-rw-r--r--   0        0        0    31031 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/client/utils.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/key/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/key/v2/__init__.py
+-rw-r--r--   0        0        0    10798 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/key/v2/test_remote_key_resource.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/media/__init__.py
+-rw-r--r--   0        0        0     5173 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/media/test_domain_blocking.py
+-rw-r--r--   0        0        0    50512 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/media/test_url_preview.py
+-rw-r--r--   0        0        0     1155 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/test_health.py
+-rw-r--r--   0        0        0     4587 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/rest/test_well_known.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     5336 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/scripts/test_new_matrix_user.py
+-rw-r--r--   0        0        0    37558 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/server.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/server_notices/__init__.py
+-rw-r--r--   0        0        0     3788 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/server_notices/test_consent.py
+-rw-r--r--   0        0        0    16949 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/server_notices/test_resource_limits_server_notices.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/state/__init__.py
+-rw-r--r--   0        0        0    28495 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/state/test_v2.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/__init__.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/__init__.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/__init__.py
+-rw-r--r--   0        0        0     4369 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_cache.py
+-rw-r--r--   0        0        0     5622 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_deviceinbox.py
+-rw-r--r--   0        0        0     4454 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_end_to_end_keys.py
+-rw-r--r--   0        0        0    21176 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_events_worker.py
+-rw-r--r--   0        0        0    17709 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_lock.py
+-rw-r--r--   0        0        0     8197 2024-01-09 15:11:25.482848 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_receipts.py
+-rw-r--r--   0        0        0     6487 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_room.py
+-rw-r--r--   0        0        0     5037 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test__base.py
+-rw-r--r--   0        0        0     6161 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_account_data.py
+-rw-r--r--   0        0        0    19190 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_appservice.py
+-rw-r--r--   0        0        0    23920 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_background_update.py
+-rw-r--r--   0        0        0    28636 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_base.py
+-rw-r--r--   0        0        0    14112 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_cleanup_extrems.py
+-rw-r--r--   0        0        0    25377 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_client_ips.py
+-rw-r--r--   0        0        0    10724 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_database.py
+-rw-r--r--   0        0        0    12903 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_devices.py
+-rw-r--r--   0        0        0     2509 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_directory.py
+-rw-r--r--   0        0        0     2942 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_e2e_room_keys.py
+-rw-r--r--   0        0        0     4205 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_end_to_end_keys.py
+-rw-r--r--   0        0        0    26823 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_event_chain.py
+-rw-r--r--   0        0        0    42747 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_event_federation.py
+-rw-r--r--   0        0        0     3537 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_event_metrics.py
+-rw-r--r--   0        0        0    26944 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_event_push_actions.py
+-rw-r--r--   0        0        0    18601 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_events.py
+-rw-r--r--   0        0        0    38215 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_id_generators.py
+-rw-r--r--   0        0        0     1752 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_main.py
+-rw-r--r--   0        0        0    19617 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_monthly_active_users.py
+-rw-r--r--   0        0        0     4507 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_profile.py
+-rw-r--r--   0        0        0     5061 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_purge.py
+-rw-r--r--   0        0        0    10522 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_receipts.py
+-rw-r--r--   0        0        0    15764 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_redaction.py
+-rw-r--r--   0        0        0    10381 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_registration.py
+-rw-r--r--   0        0        0     4438 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_relations.py
+-rw-r--r--   0        0        0     4688 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_rollback_worker.py
+-rw-r--r--   0        0        0     2515 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_room.py
+-rw-r--r--   0        0        0    14415 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_room_search.py
+-rw-r--r--   0        0        0    10196 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_roommember.py
+-rw-r--r--   0        0        0    23509 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_state.py
+-rw-r--r--   0        0        0     9646 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_stream.py
+-rw-r--r--   0        0        0     2669 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_transactions.py
+-rw-r--r--   0        0        0     1651 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_txn_limit.py
+-rw-r--r--   0        0        0     2076 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_unsafe_locale.py
+-rw-r--r--   0        0        0    28251 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_user_directory.py
+-rw-r--r--   0        0        0     3402 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/test_user_filters.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/util/__init__.py
+-rw-r--r--   0        0        0     6652 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/storage/util/test_partial_state_events_tracker.py
+-rw-r--r--   0        0        0     2162 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_distributor.py
+-rw-r--r--   0        0        0    32364 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_event_auth.py
+-rw-r--r--   0        0        0    14817 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_federation.py
+-rw-r--r--   0        0        0    12070 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_mau.py
+-rw-r--r--   0        0        0     3546 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_phone_home.py
+-rw-r--r--   0        0        0      291 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_rust.py
+-rw-r--r--   0        0        0    18805 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_server.py
+-rw-r--r--   0        0        0    30235 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_state.py
+-rw-r--r--   0        0        0     4963 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_terms_auth.py
+-rw-r--r--   0        0        0     1918 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_test_utils.py
+-rw-r--r--   0        0        0     4581 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_types.py
+-rw-r--r--   0        0        0     4144 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     3982 2024-01-09 15:11:25.486847 matrix_synapse-1.99.0rc1/tests/test_utils/event_injection.py
+-rw-r--r--   0        0        0     2013 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/test_utils/html_parsers.py
+-rw-r--r--   0        0        0     2616 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/test_utils/logging_setup.py
+-rw-r--r--   0        0        0    12179 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/test_utils/oidc.py
+-rw-r--r--   0        0        0    12980 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/test_visibility.py
+-rw-r--r--   0        0        0        0 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/types/__init__.py
+-rw-r--r--   0        0        0    21259 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/types/test_state.py
+-rw-r--r--   0        0        0    35404 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/unittest.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/__init__.py
+-rw-r--r--   0        0        0      673 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/caches/__init__.py
+-rw-r--r--   0        0        0     5314 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/caches/test_cached_call.py
+-rw-r--r--   0        0        0     9612 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/caches/test_deferred_cache.py
+-rw-r--r--   0        0        0    34232 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/caches/test_descriptors.py
+-rw-r--r--   0        0        0     7480 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/caches/test_response_cache.py
+-rw-r--r--   0        0        0     3010 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/caches/test_ttlcache.py
+-rw-r--r--   0        0        0    20487 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_async_helpers.py
+-rw-r--r--   0        0        0     9316 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_batching_queue.py
+-rw-r--r--   0        0        0     7228 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_check_dependencies.py
+-rw-r--r--   0        0        0     4285 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_dict_cache.py
+-rw-r--r--   0        0        0     3091 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_expiring_cache.py
+-rw-r--r--   0        0        0     6212 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_file_consumer.py
+-rw-r--r--   0        0        0     6342 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_itertools.py
+-rw-r--r--   0        0        0     8666 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_linearizer.py
+-rw-r--r--   0        0        0     7004 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_logcontext.py
+-rw-r--r--   0        0        0     1235 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_logformatter.py
+-rw-r--r--   0        0        0    12339 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_lrucache.py
+-rw-r--r--   0        0        0     5269 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_macaroons.py
+-rw-r--r--   0        0        0     5134 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_ratelimitutils.py
+-rw-r--r--   0        0        0     8654 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_retryutils.py
+-rw-r--r--   0        0        0    16797 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_rwlock.py
+-rw-r--r--   0        0        0     9891 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_stream_change_cache.py
+-rw-r--r--   0        0        0     1863 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_stringutils.py
+-rw-r--r--   0        0        0     8794 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_task_scheduler.py
+-rw-r--r--   0        0        0     1903 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_threepids.py
+-rw-r--r--   0        0        0     3158 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_treecache.py
+-rw-r--r--   0        0        0     2758 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/util/test_wheel_timer.py
+-rw-r--r--   0        0        0    13230 2024-01-09 15:11:25.490847 matrix_synapse-1.99.0rc1/tests/utils.py
+-rw-r--r--   0        0        0    20802 1970-01-01 00:00:00.000000 matrix_synapse-1.99.0rc1/setup.py
+-rw-r--r--   0        0        0    15128 1970-01-01 00:00:00.000000 matrix_synapse-1.99.0rc1/PKG-INFO
```

### Comparing `matrix_synapse-1.99.0/AUTHORS.rst` & `matrix_synapse-1.99.0rc1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/CHANGES.md` & `matrix_synapse-1.99.0rc1/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-# Synapse 1.99.0 (2024-01-16)
-
-Synapse 1.99.0 is the first Synapse release under an AGPLv3.0 licence (with CLA to enable Element to sell AGPL
-exceptions). You can read more about this here:
-
- - https://matrix.org/blog/2023/11/06/future-of-synapse-dendrite/
- - https://element.io/blog/element-to-adopt-agplv3/
- - https://element.io/blog/synapse-now-lives-at-github-com-element-hq-synapse/
-
-No significant changes since 1.99.0rc1.
-
-
 # Synapse 1.99.0rc1 (2024-01-09)
 
 ### Features
 
 - Add [config options](https://element-hq.github.io/synapse/v1.99/usage/configuration/config_documentation.html#server_notices) to set the avatar and the topic of the server notices room, as well as the avatar of the server notices user. ([\#16679](https://github.com/matrix-org/synapse/issues/16679))
 - Add config option [`email.notif_delay_before_mail`](https://element-hq.github.io/synapse/v1.99/usage/configuration/config_documentation.html#email) to tweak the delay before an email is sent following a notification. ([\#16696](https://github.com/matrix-org/synapse/issues/16696))
 - Add new configuration option [`sentry.environment`](https://element-hq.github.io/synapse/v1.99/usage/configuration/config_documentation.html#sentry) for improved system monitoring. Contributed by @zeeshanrafiqrana. ([\#16738](https://github.com/matrix-org/synapse/issues/16738))
```

### Comparing `matrix_synapse-1.99.0/Cargo.lock` & `matrix_synapse-1.99.0rc1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/LICENSE` & `matrix_synapse-1.99.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/README.rst` & `matrix_synapse-1.99.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/book.toml` & `matrix_synapse-1.99.0rc1/book.toml`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/build_rust.py` & `matrix_synapse-1.99.0rc1/build_rust.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/demo/start.sh` & `matrix_synapse-1.99.0rc1/demo/start.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/.sample_config_header.yaml` & `matrix_synapse-1.99.0rc1/docs/.sample_config_header.yaml`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/CAPTCHA_SETUP.md` & `matrix_synapse-1.99.0rc1/docs/CAPTCHA_SETUP.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/README.md` & `matrix_synapse-1.99.0rc1/docs/README.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/SUMMARY.md` & `matrix_synapse-1.99.0rc1/docs/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/README.rst` & `matrix_synapse-1.99.0rc1/docs/admin_api/README.rst`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/account_validity.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/account_validity.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/event_reports.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/event_reports.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/experimental_features.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/experimental_features.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/media_admin_api.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/media_admin_api.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/purge_history_api.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/purge_history_api.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/register_api.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/register_api.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/room_membership.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/room_membership.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/rooms.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/rooms.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/server_notices.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/server_notices.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/statistics.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/statistics.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/admin_api/user_admin_api.md` & `matrix_synapse-1.99.0rc1/docs/admin_api/user_admin_api.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/ancient_architecture_notes.md` & `matrix_synapse-1.99.0rc1/docs/ancient_architecture_notes.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/application_services.md` & `matrix_synapse-1.99.0rc1/docs/application_services.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/architecture.md` & `matrix_synapse-1.99.0rc1/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/auth_chain_diff.dot` & `matrix_synapse-1.99.0rc1/docs/auth_chain_diff.dot`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/auth_chain_diff.dot.png` & `matrix_synapse-1.99.0rc1/docs/auth_chain_diff.dot.png`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/auth_chain_difference_algorithm.md` & `matrix_synapse-1.99.0rc1/docs/auth_chain_difference_algorithm.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/changelogs/CHANGES-2019.md` & `matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2019.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/changelogs/CHANGES-2020.md` & `matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2020.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/changelogs/CHANGES-2021.md` & `matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2021.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/changelogs/CHANGES-2022.md` & `matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-2022.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/changelogs/CHANGES-pre-1.0.md` & `matrix_synapse-1.99.0rc1/docs/changelogs/CHANGES-pre-1.0.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/code_style.md` & `matrix_synapse-1.99.0rc1/docs/code_style.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/consent_tracking.md` & `matrix_synapse-1.99.0rc1/docs/consent_tracking.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/delegate.md` & `matrix_synapse-1.99.0rc1/docs/delegate.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/deprecation_policy.md` & `matrix_synapse-1.99.0rc1/docs/deprecation_policy.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/cas.md` & `matrix_synapse-1.99.0rc1/docs/development/cas.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/contributing_guide.md` & `matrix_synapse-1.99.0rc1/docs/development/contributing_guide.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/database_schema.md` & `matrix_synapse-1.99.0rc1/docs/development/database_schema.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/demo.md` & `matrix_synapse-1.99.0rc1/docs/development/demo.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/dependencies.md` & `matrix_synapse-1.99.0rc1/docs/development/dependencies.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/experimental_features.md` & `matrix_synapse-1.99.0rc1/docs/development/experimental_features.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/git.md` & `matrix_synapse-1.99.0rc1/docs/development/git.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/img/git/branches.jpg` & `matrix_synapse-1.99.0rc1/docs/development/img/git/branches.jpg`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/img/git/clean.png` & `matrix_synapse-1.99.0rc1/docs/development/img/git/clean.png`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/img/git/squash.png` & `matrix_synapse-1.99.0rc1/docs/development/img/git/squash.png`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/internal_documentation/README.md` & `matrix_synapse-1.99.0rc1/docs/development/internal_documentation/README.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/releases.md` & `matrix_synapse-1.99.0rc1/docs/development/releases.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/reviews.md` & `matrix_synapse-1.99.0rc1/docs/development/reviews.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/room-dag-concepts.md` & `matrix_synapse-1.99.0rc1/docs/development/room-dag-concepts.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/saml.md` & `matrix_synapse-1.99.0rc1/docs/development/saml.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/synapse_architecture/cancellation.md` & `matrix_synapse-1.99.0rc1/docs/development/synapse_architecture/cancellation.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/synapse_architecture/faster_joins.md` & `matrix_synapse-1.99.0rc1/docs/development/synapse_architecture/faster_joins.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/development/synapse_architecture/streams.md` & `matrix_synapse-1.99.0rc1/docs/development/synapse_architecture/streams.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/favicon.png` & `matrix_synapse-1.99.0rc1/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/favicon.svg` & `matrix_synapse-1.99.0rc1/docs/favicon.svg`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/federate.md` & `matrix_synapse-1.99.0rc1/docs/federate.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/jwt.md` & `matrix_synapse-1.99.0rc1/docs/jwt.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/log_contexts.md` & `matrix_synapse-1.99.0rc1/docs/log_contexts.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/manhole.md` & `matrix_synapse-1.99.0rc1/docs/manhole.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/media_repository.md` & `matrix_synapse-1.99.0rc1/docs/media_repository.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/message_retention_policies.md` & `matrix_synapse-1.99.0rc1/docs/message_retention_policies.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/metrics-howto.md` & `matrix_synapse-1.99.0rc1/docs/metrics-howto.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/account_data_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/account_data_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/account_validity_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/account_validity_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/add_extra_fields_to_client_events_unsigned.md` & `matrix_synapse-1.99.0rc1/docs/modules/add_extra_fields_to_client_events_unsigned.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/background_update_controller_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/background_update_controller_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/index.md` & `matrix_synapse-1.99.0rc1/docs/modules/index.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/password_auth_provider_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/password_auth_provider_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/porting_legacy_module.md` & `matrix_synapse-1.99.0rc1/docs/modules/porting_legacy_module.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/presence_router_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/presence_router_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/spam_checker_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/spam_checker_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/third_party_rules_callbacks.md` & `matrix_synapse-1.99.0rc1/docs/modules/third_party_rules_callbacks.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/modules/writing_a_module.md` & `matrix_synapse-1.99.0rc1/docs/modules/writing_a_module.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/openid.md` & `matrix_synapse-1.99.0rc1/docs/openid.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/opentracing.md` & `matrix_synapse-1.99.0rc1/docs/opentracing.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/other/running_synapse_on_single_board_computers.md` & `matrix_synapse-1.99.0rc1/docs/other/running_synapse_on_single_board_computers.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/password_auth_providers.md` & `matrix_synapse-1.99.0rc1/docs/password_auth_providers.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/postgres.md` & `matrix_synapse-1.99.0rc1/docs/postgres.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/presence_router_module.md` & `matrix_synapse-1.99.0rc1/docs/presence_router_module.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/privacy_policy_templates/en/1.0.html` & `matrix_synapse-1.99.0rc1/docs/privacy_policy_templates/en/1.0.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/replication.md` & `matrix_synapse-1.99.0rc1/docs/replication.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/reverse_proxy.md` & `matrix_synapse-1.99.0rc1/docs/reverse_proxy.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/room_and_user_statistics.md` & `matrix_synapse-1.99.0rc1/docs/room_and_user_statistics.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/sample_config.yaml` & `matrix_synapse-1.99.0rc1/docs/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/sample_log_config.yaml` & `matrix_synapse-1.99.0rc1/docs/sample_log_config.yaml`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/server_notices.md` & `matrix_synapse-1.99.0rc1/docs/server_notices.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/setup/forward_proxy.md` & `matrix_synapse-1.99.0rc1/docs/setup/forward_proxy.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/setup/installation.md` & `matrix_synapse-1.99.0rc1/docs/setup/installation.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/setup/turn/coturn.md` & `matrix_synapse-1.99.0rc1/docs/setup/turn/coturn.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/setup/turn/eturnal.md` & `matrix_synapse-1.99.0rc1/docs/setup/turn/eturnal.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/spam_checker.md` & `matrix_synapse-1.99.0rc1/docs/spam_checker.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/sso_mapping_providers.md` & `matrix_synapse-1.99.0rc1/docs/sso_mapping_providers.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/structured_logging.md` & `matrix_synapse-1.99.0rc1/docs/structured_logging.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/synctl_workers.md` & `matrix_synapse-1.99.0rc1/docs/synctl_workers.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/systemd-with-workers/README.md` & `matrix_synapse-1.99.0rc1/docs/systemd-with-workers/README.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/systemd-with-workers/system/matrix-synapse-worker@.service` & `matrix_synapse-1.99.0rc1/docs/systemd-with-workers/system/matrix-synapse-worker@.service`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/systemd-with-workers/system/matrix-synapse.service` & `matrix_synapse-1.99.0rc1/docs/systemd-with-workers/system/matrix-synapse.service`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/systemd-with-workers/workers/event_persister.yaml` & `matrix_synapse-1.99.0rc1/docs/systemd-with-workers/workers/event_persister.yaml`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/tcp_replication.md` & `matrix_synapse-1.99.0rc1/docs/tcp_replication.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/templates.md` & `matrix_synapse-1.99.0rc1/docs/templates.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/turn-howto.md` & `matrix_synapse-1.99.0rc1/docs/turn-howto.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/upgrade.md` & `matrix_synapse-1.99.0rc1/docs/upgrade.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/admin_api/README.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/README.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/admin_api/background_updates.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/background_updates.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/admin_api/federation.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/federation.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/admin_api/registration_tokens.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/admin_api/registration_tokens.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/admin_faq.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/admin_faq.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/database_maintenance_tools.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/database_maintenance_tools.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/monitoring/reporting_homeserver_usage_statistics.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/monitoring/reporting_homeserver_usage_statistics.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/monthly_active_users.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/monthly_active_users.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/request_log.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/request_log.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/state_groups.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/state_groups.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/understanding_synapse_through_grafana_graphs.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/understanding_synapse_through_grafana_graphs.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/administration/useful_sql_for_admins.md` & `matrix_synapse-1.99.0rc1/docs/usage/administration/useful_sql_for_admins.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/configuration/config_documentation.md` & `matrix_synapse-1.99.0rc1/docs/usage/configuration/config_documentation.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/configuration/homeserver_sample_config.md` & `matrix_synapse-1.99.0rc1/docs/usage/configuration/homeserver_sample_config.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/configuration/logging_sample_config.md` & `matrix_synapse-1.99.0rc1/docs/usage/configuration/logging_sample_config.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/README.md` & `matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/README.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/usage/configuration/user_authentication/refresh_tokens.md` & `matrix_synapse-1.99.0rc1/docs/usage/configuration/user_authentication/refresh_tokens.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/user_directory.md` & `matrix_synapse-1.99.0rc1/docs/user_directory.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/website_files/README.md` & `matrix_synapse-1.99.0rc1/docs/website_files/README.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/website_files/table-of-contents.css` & `matrix_synapse-1.99.0rc1/docs/website_files/table-of-contents.css`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/website_files/table-of-contents.js` & `matrix_synapse-1.99.0rc1/docs/website_files/table-of-contents.js`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/website_files/theme/index.hbs` & `matrix_synapse-1.99.0rc1/docs/website_files/theme/index.hbs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/website_files/version-picker.css` & `matrix_synapse-1.99.0rc1/docs/website_files/version-picker.css`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/website_files/version-picker.js` & `matrix_synapse-1.99.0rc1/docs/website_files/version-picker.js`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/welcome_and_overview.md` & `matrix_synapse-1.99.0rc1/docs/welcome_and_overview.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/docs/workers.md` & `matrix_synapse-1.99.0rc1/docs/workers.md`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/mypy.ini` & `matrix_synapse-1.99.0rc1/mypy.ini`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/pyproject.toml` & `matrix_synapse-1.99.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 [tool.maturin]
 manifest-path = "rust/Cargo.toml"
 module-name = "synapse.synapse_rust"
 
 [tool.poetry]
 name = "matrix-synapse"
-version = "1.99.0"
+version = "1.99.0rc1"
 description = "Homeserver for the Matrix decentralised comms protocol"
 authors = ["Matrix.org Team and Contributors <packages@matrix.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/element-hq/synapse"
 packages = [
     { include = "synapse" },
```

### Comparing `matrix_synapse-1.99.0/rust/Cargo.toml` & `matrix_synapse-1.99.0rc1/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/build.rs` & `matrix_synapse-1.99.0rc1/rust/build.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/acl/mod.rs` & `matrix_synapse-1.99.0rc1/rust/src/acl/mod.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/events/internal_metadata.rs` & `matrix_synapse-1.99.0rc1/rust/src/events/internal_metadata.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/events/mod.rs` & `matrix_synapse-1.99.0rc1/rust/src/events/mod.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/lib.rs` & `matrix_synapse-1.99.0rc1/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/push/base_rules.rs` & `matrix_synapse-1.99.0rc1/rust/src/push/base_rules.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/push/evaluator.rs` & `matrix_synapse-1.99.0rc1/rust/src/push/evaluator.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/push/mod.rs` & `matrix_synapse-1.99.0rc1/rust/src/push/mod.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/rust/src/push/utils.rs` & `matrix_synapse-1.99.0rc1/rust/src/push/utils.rs`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/build_debian_packages.py` & `matrix_synapse-1.99.0rc1/scripts-dev/build_debian_packages.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/check-newsfragment.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/check-newsfragment.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/check_line_terminators.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/check_line_terminators.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/check_locked_deps_have_sdists.py` & `matrix_synapse-1.99.0rc1/scripts-dev/check_locked_deps_have_sdists.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/check_pydantic_models.py` & `matrix_synapse-1.99.0rc1/scripts-dev/check_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/check_schema_delta.py` & `matrix_synapse-1.99.0rc1/scripts-dev/check_schema_delta.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/complement.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/complement.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/config-lint.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/config-lint.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/docker_update_debian_changelog.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/docker_update_debian_changelog.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/dump_macaroon.py` & `matrix_synapse-1.99.0rc1/scripts-dev/dump_macaroon.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/federation_client.py` & `matrix_synapse-1.99.0rc1/scripts-dev/federation_client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/generate_sample_config.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/generate_sample_config.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/lint.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/lint.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/make_full_schema.sh` & `matrix_synapse-1.99.0rc1/scripts-dev/make_full_schema.sh`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/mypy_synapse_plugin.py` & `matrix_synapse-1.99.0rc1/scripts-dev/mypy_synapse_plugin.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/release.py` & `matrix_synapse-1.99.0rc1/scripts-dev/release.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/schema_versions.py` & `matrix_synapse-1.99.0rc1/scripts-dev/schema_versions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/scripts-dev/sign_json.py` & `matrix_synapse-1.99.0rc1/scripts-dev/sign_json.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_pydantic_compat.py` & `matrix_synapse-1.99.0rc1/synapse/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/export_signing_key.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/export_signing_key.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/generate_config.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/generate_config.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/generate_log_config.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/generate_log_config.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/generate_signing_key.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/generate_signing_key.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/generate_workers_map.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/generate_workers_map.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/hash_password.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/hash_password.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/move_remote_media_to_new_store.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/move_remote_media_to_new_store.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/register_new_matrix_user.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/register_new_matrix_user.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/review_recent_signups.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/review_recent_signups.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/synapse_port_db.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/synapse_port_db.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/synctl.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/synctl.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/_scripts/update_synapse_database.py` & `matrix_synapse-1.99.0rc1/synapse/_scripts/update_synapse_database.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/auth/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/auth/base.py` & `matrix_synapse-1.99.0rc1/synapse/api/auth/base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/auth/internal.py` & `matrix_synapse-1.99.0rc1/synapse/api/auth/internal.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/auth/msc3861_delegated.py` & `matrix_synapse-1.99.0rc1/synapse/api/auth/msc3861_delegated.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/auth_blocking.py` & `matrix_synapse-1.99.0rc1/synapse/api/auth_blocking.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/constants.py` & `matrix_synapse-1.99.0rc1/synapse/api/constants.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/errors.py` & `matrix_synapse-1.99.0rc1/synapse/api/errors.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/filtering.py` & `matrix_synapse-1.99.0rc1/synapse/api/filtering.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/presence.py` & `matrix_synapse-1.99.0rc1/synapse/api/presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/ratelimiting.py` & `matrix_synapse-1.99.0rc1/synapse/api/ratelimiting.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/room_versions.py` & `matrix_synapse-1.99.0rc1/synapse/api/room_versions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/api/urls.py` & `matrix_synapse-1.99.0rc1/synapse/api/urls.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/app/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/_base.py` & `matrix_synapse-1.99.0rc1/synapse/app/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/admin_cmd.py` & `matrix_synapse-1.99.0rc1/synapse/app/admin_cmd.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/appservice.py` & `matrix_synapse-1.99.0rc1/synapse/app/appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/client_reader.py` & `matrix_synapse-1.99.0rc1/synapse/app/client_reader.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/complement_fork_starter.py` & `matrix_synapse-1.99.0rc1/synapse/app/complement_fork_starter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/event_creator.py` & `matrix_synapse-1.99.0rc1/synapse/app/event_creator.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/federation_reader.py` & `matrix_synapse-1.99.0rc1/synapse/app/federation_reader.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/federation_sender.py` & `matrix_synapse-1.99.0rc1/synapse/app/federation_sender.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/frontend_proxy.py` & `matrix_synapse-1.99.0rc1/synapse/app/frontend_proxy.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/generic_worker.py` & `matrix_synapse-1.99.0rc1/synapse/app/generic_worker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/homeserver.py` & `matrix_synapse-1.99.0rc1/synapse/app/homeserver.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/media_repository.py` & `matrix_synapse-1.99.0rc1/synapse/app/media_repository.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/phone_stats_home.py` & `matrix_synapse-1.99.0rc1/synapse/app/phone_stats_home.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/pusher.py` & `matrix_synapse-1.99.0rc1/synapse/app/pusher.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/synchrotron.py` & `matrix_synapse-1.99.0rc1/synapse/app/synchrotron.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/app/user_dir.py` & `matrix_synapse-1.99.0rc1/synapse/app/user_dir.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/appservice/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/appservice/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/appservice/api.py` & `matrix_synapse-1.99.0rc1/synapse/appservice/api.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/appservice/scheduler.py` & `matrix_synapse-1.99.0rc1/synapse/appservice/scheduler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/config/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/__main__.py` & `matrix_synapse-1.99.0rc1/synapse/config/__main__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/_base.py` & `matrix_synapse-1.99.0rc1/synapse/config/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/_base.pyi` & `matrix_synapse-1.99.0rc1/synapse/config/_base.pyi`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/_util.py` & `matrix_synapse-1.99.0rc1/synapse/config/_util.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/account_validity.py` & `matrix_synapse-1.99.0rc1/synapse/config/account_validity.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/api.py` & `matrix_synapse-1.99.0rc1/synapse/config/api.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/appservice.py` & `matrix_synapse-1.99.0rc1/synapse/config/appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/auth.py` & `matrix_synapse-1.99.0rc1/synapse/config/auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/background_updates.py` & `matrix_synapse-1.99.0rc1/synapse/config/background_updates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/cache.py` & `matrix_synapse-1.99.0rc1/synapse/config/cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/captcha.py` & `matrix_synapse-1.99.0rc1/synapse/config/captcha.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/cas.py` & `matrix_synapse-1.99.0rc1/synapse/config/cas.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/consent.py` & `matrix_synapse-1.99.0rc1/synapse/config/consent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/database.py` & `matrix_synapse-1.99.0rc1/synapse/config/database.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/emailconfig.py` & `matrix_synapse-1.99.0rc1/synapse/config/emailconfig.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/experimental.py` & `matrix_synapse-1.99.0rc1/synapse/config/experimental.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/federation.py` & `matrix_synapse-1.99.0rc1/synapse/config/federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/homeserver.py` & `matrix_synapse-1.99.0rc1/synapse/config/homeserver.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/jwt.py` & `matrix_synapse-1.99.0rc1/synapse/config/jwt.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/key.py` & `matrix_synapse-1.99.0rc1/synapse/config/key.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/logger.py` & `matrix_synapse-1.99.0rc1/synapse/config/logger.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/metrics.py` & `matrix_synapse-1.99.0rc1/synapse/config/metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/modules.py` & `matrix_synapse-1.99.0rc1/synapse/config/modules.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/oembed.py` & `matrix_synapse-1.99.0rc1/synapse/config/oembed.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/oidc.py` & `matrix_synapse-1.99.0rc1/synapse/config/oidc.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/password_auth_providers.py` & `matrix_synapse-1.99.0rc1/synapse/config/password_auth_providers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/push.py` & `matrix_synapse-1.99.0rc1/synapse/config/push.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/ratelimiting.py` & `matrix_synapse-1.99.0rc1/synapse/config/ratelimiting.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/redis.py` & `matrix_synapse-1.99.0rc1/synapse/config/redis.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/registration.py` & `matrix_synapse-1.99.0rc1/synapse/config/registration.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/repository.py` & `matrix_synapse-1.99.0rc1/synapse/config/repository.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/retention.py` & `matrix_synapse-1.99.0rc1/synapse/config/retention.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/room.py` & `matrix_synapse-1.99.0rc1/synapse/config/room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/room_directory.py` & `matrix_synapse-1.99.0rc1/synapse/config/room_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/saml2.py` & `matrix_synapse-1.99.0rc1/synapse/config/saml2.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/server.py` & `matrix_synapse-1.99.0rc1/synapse/config/server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/server_notices.py` & `matrix_synapse-1.99.0rc1/synapse/config/server_notices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/spam_checker.py` & `matrix_synapse-1.99.0rc1/synapse/config/spam_checker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/sso.py` & `matrix_synapse-1.99.0rc1/synapse/config/sso.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/stats.py` & `matrix_synapse-1.99.0rc1/synapse/config/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/third_party_event_rules.py` & `matrix_synapse-1.99.0rc1/synapse/config/third_party_event_rules.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/tls.py` & `matrix_synapse-1.99.0rc1/synapse/config/tls.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/tracer.py` & `matrix_synapse-1.99.0rc1/synapse/config/tracer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/user_directory.py` & `matrix_synapse-1.99.0rc1/synapse/config/user_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/voip.py` & `matrix_synapse-1.99.0rc1/synapse/config/voip.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/config/workers.py` & `matrix_synapse-1.99.0rc1/synapse/config/workers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/crypto/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/crypto/context_factory.py` & `matrix_synapse-1.99.0rc1/synapse/crypto/context_factory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/crypto/event_signing.py` & `matrix_synapse-1.99.0rc1/synapse/crypto/event_signing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/crypto/keyring.py` & `matrix_synapse-1.99.0rc1/synapse/crypto/keyring.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/event_auth.py` & `matrix_synapse-1.99.0rc1/synapse/event_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/events/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/events/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/events/builder.py` & `matrix_synapse-1.99.0rc1/synapse/events/builder.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/events/presence_router.py` & `matrix_synapse-1.99.0rc1/synapse/events/presence_router.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/events/snapshot.py` & `matrix_synapse-1.99.0rc1/synapse/events/snapshot.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/events/utils.py` & `matrix_synapse-1.99.0rc1/synapse/events/utils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/events/validator.py` & `matrix_synapse-1.99.0rc1/synapse/events/validator.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/federation/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/federation_base.py` & `matrix_synapse-1.99.0rc1/synapse/federation/federation_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/federation_client.py` & `matrix_synapse-1.99.0rc1/synapse/federation/federation_client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/federation_server.py` & `matrix_synapse-1.99.0rc1/synapse/federation/federation_server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/persistence.py` & `matrix_synapse-1.99.0rc1/synapse/federation/persistence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/send_queue.py` & `matrix_synapse-1.99.0rc1/synapse/federation/send_queue.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/sender/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/federation/sender/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/sender/per_destination_queue.py` & `matrix_synapse-1.99.0rc1/synapse/federation/sender/per_destination_queue.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/sender/transaction_manager.py` & `matrix_synapse-1.99.0rc1/synapse/federation/sender/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/transport/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/federation/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/transport/client.py` & `matrix_synapse-1.99.0rc1/synapse/federation/transport/client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/transport/server/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/federation/transport/server/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/transport/server/_base.py` & `matrix_synapse-1.99.0rc1/synapse/federation/transport/server/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/transport/server/federation.py` & `matrix_synapse-1.99.0rc1/synapse/federation/transport/server/federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/federation/units.py` & `matrix_synapse-1.99.0rc1/synapse/federation/units.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/account.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/account.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/account_data.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/account_validity.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/account_validity.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/admin.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/admin.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/appservice.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/auth.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/cas.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/cas.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/deactivate_account.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/deactivate_account.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/device.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/device.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/devicemessage.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/devicemessage.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/directory.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/e2e_keys.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/e2e_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/e2e_room_keys.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/e2e_room_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/event_auth.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/event_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/events.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/federation.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/federation_event.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/federation_event.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/identity.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/identity.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/initial_sync.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/initial_sync.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/jwt.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/jwt.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/message.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/message.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/oidc.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/oidc.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/pagination.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/pagination.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/password_policy.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/password_policy.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/presence.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/profile.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/profile.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/push_rules.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/push_rules.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/read_marker.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/read_marker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/receipts.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/register.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/register.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/relations.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/relations.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/room.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/room_list.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/room_list.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/room_member.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/room_member.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/room_member_worker.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/room_member_worker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/room_summary.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/room_summary.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/saml.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/saml.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/search.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/search.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/send_email.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/send_email.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/set_password.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/set_password.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/sso.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/sso.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/state_deltas.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/state_deltas.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/stats.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/sync.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/sync.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/typing.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/typing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/ui_auth/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/ui_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/ui_auth/checkers.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/ui_auth/checkers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/user_directory.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/user_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/handlers/worker_lock.py` & `matrix_synapse-1.99.0rc1/synapse/handlers/worker_lock.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/http/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/additional_resource.py` & `matrix_synapse-1.99.0rc1/synapse/http/additional_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/client.py` & `matrix_synapse-1.99.0rc1/synapse/http/client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/connectproxyclient.py` & `matrix_synapse-1.99.0rc1/synapse/http/connectproxyclient.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/federation/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/http/federation/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/federation/matrix_federation_agent.py` & `matrix_synapse-1.99.0rc1/synapse/http/federation/matrix_federation_agent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/federation/srv_resolver.py` & `matrix_synapse-1.99.0rc1/synapse/http/federation/srv_resolver.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/federation/well_known_resolver.py` & `matrix_synapse-1.99.0rc1/synapse/http/federation/well_known_resolver.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/matrixfederationclient.py` & `matrix_synapse-1.99.0rc1/synapse/http/matrixfederationclient.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/proxy.py` & `matrix_synapse-1.99.0rc1/synapse/http/proxy.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/proxyagent.py` & `matrix_synapse-1.99.0rc1/synapse/http/proxyagent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/replicationagent.py` & `matrix_synapse-1.99.0rc1/synapse/http/replicationagent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/request_metrics.py` & `matrix_synapse-1.99.0rc1/synapse/http/request_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/server.py` & `matrix_synapse-1.99.0rc1/synapse/http/server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/servlet.py` & `matrix_synapse-1.99.0rc1/synapse/http/servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/site.py` & `matrix_synapse-1.99.0rc1/synapse/http/site.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/http/types.py` & `matrix_synapse-1.99.0rc1/synapse/http/types.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/_remote.py` & `matrix_synapse-1.99.0rc1/synapse/logging/_remote.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/_terse_json.py` & `matrix_synapse-1.99.0rc1/synapse/logging/_terse_json.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/context.py` & `matrix_synapse-1.99.0rc1/synapse/logging/context.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/filter.py` & `matrix_synapse-1.99.0rc1/synapse/logging/filter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/formatter.py` & `matrix_synapse-1.99.0rc1/synapse/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/handlers.py` & `matrix_synapse-1.99.0rc1/synapse/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/opentracing.py` & `matrix_synapse-1.99.0rc1/synapse/logging/opentracing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/logging/scopecontextmanager.py` & `matrix_synapse-1.99.0rc1/synapse/logging/scopecontextmanager.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/_base.py` & `matrix_synapse-1.99.0rc1/synapse/media/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/filepath.py` & `matrix_synapse-1.99.0rc1/synapse/media/filepath.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/media_repository.py` & `matrix_synapse-1.99.0rc1/synapse/media/media_repository.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/media_storage.py` & `matrix_synapse-1.99.0rc1/synapse/media/media_storage.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/oembed.py` & `matrix_synapse-1.99.0rc1/synapse/media/oembed.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/preview_html.py` & `matrix_synapse-1.99.0rc1/synapse/media/preview_html.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/storage_provider.py` & `matrix_synapse-1.99.0rc1/synapse/media/storage_provider.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/thumbnailer.py` & `matrix_synapse-1.99.0rc1/synapse/media/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/media/url_previewer.py` & `matrix_synapse-1.99.0rc1/synapse/media/url_previewer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/_gc.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/_gc.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/_reactor_metrics.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/_reactor_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/_twisted_exposition.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/_twisted_exposition.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/_types.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/_types.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/background_process_metrics.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/background_process_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/common_usage_metrics.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/common_usage_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/metrics/jemalloc.py` & `matrix_synapse-1.99.0rc1/synapse/metrics/jemalloc.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/module_api/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/module_api/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/module_api/callbacks/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/module_api/callbacks/account_validity_callbacks.py` & `matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/account_validity_callbacks.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/module_api/callbacks/spamchecker_callbacks.py` & `matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/spamchecker_callbacks.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/module_api/callbacks/third_party_event_rules_callbacks.py` & `matrix_synapse-1.99.0rc1/synapse/module_api/callbacks/third_party_event_rules_callbacks.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/module_api/errors.py` & `matrix_synapse-1.99.0rc1/synapse/module_api/errors.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/notifier.py` & `matrix_synapse-1.99.0rc1/synapse/notifier.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/push/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/bulk_push_rule_evaluator.py` & `matrix_synapse-1.99.0rc1/synapse/push/bulk_push_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/clientformat.py` & `matrix_synapse-1.99.0rc1/synapse/push/clientformat.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/emailpusher.py` & `matrix_synapse-1.99.0rc1/synapse/push/emailpusher.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/httppusher.py` & `matrix_synapse-1.99.0rc1/synapse/push/httppusher.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/mailer.py` & `matrix_synapse-1.99.0rc1/synapse/push/mailer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/presentable_names.py` & `matrix_synapse-1.99.0rc1/synapse/push/presentable_names.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/push_tools.py` & `matrix_synapse-1.99.0rc1/synapse/push/push_tools.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/push_types.py` & `matrix_synapse-1.99.0rc1/synapse/push/push_types.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/pusher.py` & `matrix_synapse-1.99.0rc1/synapse/push/pusher.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/pusherpool.py` & `matrix_synapse-1.99.0rc1/synapse/push/pusherpool.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/push/rulekinds.py` & `matrix_synapse-1.99.0rc1/synapse/push/rulekinds.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/replication/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/_base.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/account_data.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/devices.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/devices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/federation.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/login.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/login.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/membership.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/membership.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/presence.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/push.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/push.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/register.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/register.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/send_event.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/send_event.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/send_events.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/send_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/state.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/http/streams.py` & `matrix_synapse-1.99.0rc1/synapse/replication/http/streams.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/client.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/commands.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/commands.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/context.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/context.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/external_cache.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/external_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/handler.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/handler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/protocol.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/redis.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/redis.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/resource.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/streams/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/streams/_base.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/streams/events.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/streams/federation.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/replication/tcp/streams/partial_state.py` & `matrix_synapse-1.99.0rc1/synapse/replication/tcp/streams/partial_state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/providers.json` & `matrix_synapse-1.99.0rc1/synapse/res/providers.json`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/_base.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/_base.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/mail.css` & `matrix_synapse-1.99.0rc1/synapse/res/templates/mail.css`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/notice_expiry.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/notice_expiry.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/notif.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/notif.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/notif.txt` & `matrix_synapse-1.99.0rc1/synapse/res/templates/notif.txt`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/notif_mail.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/notif_mail.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/password_reset_confirmation.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/password_reset_confirmation.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/recaptcha.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/recaptcha.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/registration_token.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/registration_token.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/room.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/room.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso.css` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso.css`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_account_deactivated.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_account_deactivated.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_auth_account_details.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_account_details.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_auth_account_details.js` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_account_details.js`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_auth_bad_user.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_bad_user.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_auth_confirm.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_confirm.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_auth_success.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_auth_success.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_error.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_error.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_footer.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_footer.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_login_idp_picker.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_login_idp_picker.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_new_user_consent.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_new_user_consent.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_partial_profile.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_partial_profile.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/sso_redirect_confirm.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/sso_redirect_confirm.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/style.css` & `matrix_synapse-1.99.0rc1/synapse/res/templates/style.css`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/res/templates/terms.html` & `matrix_synapse-1.99.0rc1/synapse/res/templates/terms.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/_base.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/background_updates.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/background_updates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/devices.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/devices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/event_reports.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/event_reports.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/experimental_features.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/experimental_features.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/federation.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/media.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/media.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/registration_tokens.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/registration_tokens.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/rooms.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/rooms.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/server_notice_servlet.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/server_notice_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/statistics.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/statistics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/username_available.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/username_available.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/admin/users.py` & `matrix_synapse-1.99.0rc1/synapse/rest/admin/users.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/_base.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/account.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/account.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/account_data.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/account_validity.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/account_validity.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/appservice_ping.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/appservice_ping.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/auth.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/auth_issuer.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/auth_issuer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/capabilities.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/devices.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/devices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/directory.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/events.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/filter.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/filter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/initial_sync.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/initial_sync.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/keys.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/knock.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/knock.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/login.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/login.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/login_token_request.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/login_token_request.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/logout.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/logout.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/models.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/models.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/mutual_rooms.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/mutual_rooms.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/notifications.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/notifications.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/openid.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/openid.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/password_policy.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/password_policy.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/presence.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/profile.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/profile.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/push_rule.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/push_rule.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/pusher.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/pusher.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/read_marker.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/read_marker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/receipts.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/register.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/register.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/relations.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/relations.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/rendezvous.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/rendezvous.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/report_event.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/report_event.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/room.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/room_keys.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/room_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/room_upgrade_rest_servlet.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/room_upgrade_rest_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/sendtodevice.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/sendtodevice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/sync.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/sync.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/tags.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/tags.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/thirdparty.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/thirdparty.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/tokenrefresh.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/tokenrefresh.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/transactions.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/transactions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/user_directory.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/user_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/versions.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/versions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/client/voip.py` & `matrix_synapse-1.99.0rc1/synapse/rest/client/voip.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/consent/consent_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/consent/consent_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/health.py` & `matrix_synapse-1.99.0rc1/synapse/rest/health.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/key/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/key/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/key/v2/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/key/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/key/v2/local_key_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/key/v2/local_key_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/key/v2/remote_key_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/key/v2/remote_key_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/config_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/config_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/create_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/create_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/download_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/download_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/media_repository_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/media_repository_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/preview_url_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/preview_url_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/thumbnail_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/thumbnail_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/upload_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/upload_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/v1/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/v1/_base.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/v1/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/v1/media_storage.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/v1/media_storage.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/media/v1/storage_provider.py` & `matrix_synapse-1.99.0rc1/synapse/rest/media/v1/storage_provider.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/models.py` & `matrix_synapse-1.99.0rc1/synapse/rest/models.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/jwks.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/jwks.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/new_user_consent.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/new_user_consent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/oidc/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/oidc/backchannel_logout_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/oidc/backchannel_logout_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/oidc/callback_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/oidc/callback_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/password_reset.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/password_reset.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/pick_idp.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/pick_idp.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/pick_username.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/pick_username.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/saml2/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/saml2/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/saml2/metadata_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/saml2/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/saml2/response_resource.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/saml2/response_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/sso_register.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/sso_register.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/synapse/client/unsubscribe.py` & `matrix_synapse-1.99.0rc1/synapse/rest/synapse/client/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/rest/well_known.py` & `matrix_synapse-1.99.0rc1/synapse/rest/well_known.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/server.py` & `matrix_synapse-1.99.0rc1/synapse/server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/server_notices/consent_server_notices.py` & `matrix_synapse-1.99.0rc1/synapse/server_notices/consent_server_notices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/server_notices/resource_limits_server_notices.py` & `matrix_synapse-1.99.0rc1/synapse/server_notices/resource_limits_server_notices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/server_notices/server_notices_manager.py` & `matrix_synapse-1.99.0rc1/synapse/server_notices/server_notices_manager.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/server_notices/server_notices_sender.py` & `matrix_synapse-1.99.0rc1/synapse/server_notices/server_notices_sender.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/server_notices/worker_server_notices_sender.py` & `matrix_synapse-1.99.0rc1/synapse/server_notices/worker_server_notices_sender.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/spam_checker_api/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/spam_checker_api/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/state/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/state/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/state/v1.py` & `matrix_synapse-1.99.0rc1/synapse/state/v1.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/state/v2.py` & `matrix_synapse-1.99.0rc1/synapse/state/v2.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/static/client/login/index.html` & `matrix_synapse-1.99.0rc1/synapse/static/client/login/index.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/static/client/login/js/jquery-3.4.1.min.js` & `matrix_synapse-1.99.0rc1/synapse/static/client/login/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/static/client/login/js/login.js` & `matrix_synapse-1.99.0rc1/synapse/static/client/login/js/login.js`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/static/client/login/spinner.gif` & `matrix_synapse-1.99.0rc1/synapse/static/client/login/spinner.gif`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/static/client/login/style.css` & `matrix_synapse-1.99.0rc1/synapse/static/client/login/style.css`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/static/index.html` & `matrix_synapse-1.99.0rc1/synapse/static/index.html`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/_base.py` & `matrix_synapse-1.99.0rc1/synapse/storage/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/background_updates.py` & `matrix_synapse-1.99.0rc1/synapse/storage/background_updates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/controllers/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/controllers/persist_events.py` & `matrix_synapse-1.99.0rc1/synapse/storage/controllers/persist_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/controllers/purge_events.py` & `matrix_synapse-1.99.0rc1/synapse/storage/controllers/purge_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/controllers/state.py` & `matrix_synapse-1.99.0rc1/synapse/storage/controllers/state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/controllers/stats.py` & `matrix_synapse-1.99.0rc1/synapse/storage/controllers/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/database.py` & `matrix_synapse-1.99.0rc1/synapse/storage/database.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/account_data.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/appservice.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/cache.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/censor_events.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/censor_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/client_ips.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/client_ips.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/deviceinbox.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/deviceinbox.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/devices.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/devices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/directory.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/e2e_room_keys.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/e2e_room_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/end_to_end_keys.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/end_to_end_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/event_federation.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/event_federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/event_push_actions.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/event_push_actions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/events.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/events_bg_updates.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events_bg_updates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/events_forward_extremities.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events_forward_extremities.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/events_worker.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/events_worker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/experimental_features.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/experimental_features.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/filtering.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/filtering.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/keys.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/lock.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/lock.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/media_repository.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/media_repository.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/metrics.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/monthly_active_users.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/monthly_active_users.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/openid.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/openid.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/presence.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/profile.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/profile.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/purge_events.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/purge_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/push_rule.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/push_rule.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/pusher.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/pusher.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/receipts.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/registration.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/registration.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/rejections.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/rejections.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/relations.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/relations.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/room.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/roommember.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/roommember.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/search.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/search.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/session.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/session.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/signatures.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/signatures.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/state.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/state_deltas.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/state_deltas.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/stats.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/stream.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/stream.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/tags.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/tags.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/task_scheduler.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/transactions.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/transactions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/ui_auth.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/ui_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/user_directory.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/user_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/main/user_erasure_store.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/main/user_erasure_store.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/state/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/state/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/state/bg_updates.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/state/bg_updates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/databases/state/store.py` & `matrix_synapse-1.99.0rc1/synapse/storage/databases/state/store.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/engines/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/engines/_base.py` & `matrix_synapse-1.99.0rc1/synapse/storage/engines/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/engines/postgres.py` & `matrix_synapse-1.99.0rc1/synapse/storage/engines/postgres.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/engines/sqlite.py` & `matrix_synapse-1.99.0rc1/synapse/storage/engines/sqlite.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/keys.py` & `matrix_synapse-1.99.0rc1/synapse/storage/keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/prepare_database.py` & `matrix_synapse-1.99.0rc1/synapse/storage/prepare_database.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/push_rule.py` & `matrix_synapse-1.99.0rc1/synapse/storage/push_rule.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/roommember.py` & `matrix_synapse-1.99.0rc1/synapse/storage/roommember.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/common/delta/25/00background_updates.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/common/delta/25/00background_updates.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/common/delta/35/00background_updates_add_col.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/common/delta/35/00background_updates_add_col.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/common/delta/58/00background_update_ordering.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/common/delta/58/00background_update_ordering.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/common/schema_version.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/common/schema_version.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/12/v12.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/12/v12.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/13/v13.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/13/v13.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/14/v14.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/14/v14.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/15/appservice_txns.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/15/appservice_txns.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/15/v15.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/15/v15.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/unique_constraints.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/unique_constraints.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/16/users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/16/users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/17/drop_indexes.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/17/drop_indexes.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/17/server_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/17/server_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/18/server_keys_bigger_ints.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/18/server_keys_bigger_ints.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/19/event_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/19/event_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/20/pushers.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/20/pushers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/21/end_to_end_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/21/end_to_end_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/21/receipts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/21/receipts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/22/receipts_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/22/receipts_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/22/user_threepids_unique.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/22/user_threepids_unique.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/24/stats_reporting.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/24/stats_reporting.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/fts.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/fts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/guest_access.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/guest_access.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/history_visibility.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/history_visibility.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/25/tags.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/25/tags.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/26/account_data.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/26/account_data.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/27/account_data.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/27/account_data.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/27/forgotten_memberships.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/27/forgotten_memberships.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/27/ts.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/27/ts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/event_push_actions.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/event_push_actions.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/events_room_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/events_room_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/public_roms_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/public_roms_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/receipts_user_id_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/receipts_user_id_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/upgrade_times.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/upgrade_times.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/28/users_is_guest.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/28/users_is_guest.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/29/push_actions.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/29/push_actions.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/alias_creator.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/alias_creator.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/as_users.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/as_users.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/deleted_pushers.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/deleted_pushers.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/presence_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/presence_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/public_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/public_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/push_rule_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/push_rule_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/30/threepid_guest_access_tokens.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/30/threepid_guest_access_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/invites.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/invites.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/local_media_repository_url_cache.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/local_media_repository_url_cache.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/pushers_0.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/pushers_0.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/pushers_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/pushers_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/31/search_update.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/31/search_update.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/events.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/events.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/pusher_throttle.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/pusher_throttle.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/remove_indices.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/remove_indices.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/32/reports.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/32/reports.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/access_tokens_device_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/access_tokens_device_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/devices.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/devices.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/devices_for_e2e_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/devices_for_e2e_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/devices_for_e2e_keys_clear_unknown_device.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/devices_for_e2e_keys_clear_unknown_device.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/event_fields.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/event_fields.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/remote_media_ts.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/remote_media_ts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/33/user_ips_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/33/user_ips_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/appservice_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/appservice_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/cache_stream.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/cache_stream.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/device_inbox.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/device_inbox.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/push_display_name_rename.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/push_display_name_rename.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/34/received_txn_purge.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/34/received_txn_purge.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/contains_url.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/contains_url.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/device_outbox.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/device_outbox.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/device_stream_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/device_stream_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/event_push_actions_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/event_push_actions_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/public_room_list_change_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/public_room_list_change_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/35/stream_order_to_extrem.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/35/stream_order_to_extrem.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/36/readd_public_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/36/readd_public_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/37/remove_auth_idx.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/37/remove_auth_idx.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/37/user_threepids.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/37/user_threepids.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/38/postgres_fts_gist.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/38/postgres_fts_gist.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/appservice_room_list.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/appservice_room_list.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/device_federation_stream_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/device_federation_stream_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/event_push_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/event_push_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/federation_out_position.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/federation_out_position.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/39/membership_profile.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/39/membership_profile.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/current_state_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/current_state_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/device_inbox.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/device_inbox.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/device_list_streams.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/device_list_streams.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/event_push_summary.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/event_push_summary.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/40/pushers.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/40/pushers.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/device_list_stream_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/device_list_stream_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/device_outbound_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/device_outbound_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/event_search_event_id_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/event_search_event_id_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/41/ratelimit.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/41/ratelimit.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/current_state_delta.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/current_state_delta.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/device_list_last_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/device_list_last_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/event_auth_state_only.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/event_auth_state_only.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/42/user_dir.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/42/user_dir.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/blocked_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/blocked_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/quarantine_media.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/quarantine_media.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/url_cache.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/url_cache.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/43/user_share.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/43/user_share.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/44/expire_url_cache.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/44/expire_url_cache.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/45/group_server.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/45/group_server.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/45/profile_cache.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/45/profile_cache.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/drop_refresh_tokens.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/drop_refresh_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/drop_unique_deleted_pushers.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/drop_unique_deleted_pushers.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/group_server.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/group_server.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/local_media_repository_url_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/local_media_repository_url_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/user_dir_null_room_ids.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/user_dir_null_room_ids.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/46/user_dir_typos.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/46/user_dir_typos.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/47/last_access_media.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/47/last_access_media.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/47/postgres_fts_gin.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/47/postgres_fts_gin.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/47/push_actions_staging.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/47/push_actions_staging.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/add_user_consent.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/add_user_consent.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/add_user_ips_last_seen_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/add_user_ips_last_seen_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/deactivated_users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/deactivated_users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/group_unique_indexes.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/group_unique_indexes.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/48/groups_joinable.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/48/groups_joinable.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/49/add_user_consent_server_notice_sent.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/49/add_user_consent_server_notice_sent.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/49/add_user_daily_visits.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/49/add_user_daily_visits.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/49/add_user_ips_last_seen_only_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/49/add_user_ips_last_seen_only_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/50/add_creation_ts_users_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/50/add_creation_ts_users_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/50/erasure_store.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/50/erasure_store.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/50/make_event_content_nullable.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/50/make_event_content_nullable.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/51/e2e_room_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/51/e2e_room_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/51/monthly_active_users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/51/monthly_active_users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/52/add_event_to_state_group_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/52/add_event_to_state_group_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/52/device_list_streams_unique_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/52/device_list_streams_unique_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/52/e2e_room_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/52/e2e_room_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/add_user_type_to_users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/add_user_type_to_users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/drop_sent_transactions.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/drop_sent_transactions.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/event_format_version.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/event_format_version.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_dir_populate.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_dir_populate.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_ips_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_ips_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_share.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_share.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/user_threepid_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/user_threepid_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/53/users_in_public_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/53/users_in_public_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/account_validity_with_renewal.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/account_validity_with_renewal.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/add_validity_to_server_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/add_validity_to_server_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/delete_forward_extremities.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/delete_forward_extremities.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/drop_legacy_tables.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/drop_legacy_tables.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/drop_presence_list.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/drop_presence_list.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/relations.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/relations.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/stats.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/stats.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/54/stats2.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/54/stats2.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/55/access_token_expiry.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/55/access_token_expiry.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/55/track_threepid_validations.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/55/track_threepid_validations.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/55/users_alter_deactivated.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/55/users_alter_deactivated.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/add_spans_to_device_lists.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/add_spans_to_device_lists.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/current_state_events_membership.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/current_state_events_membership.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/current_state_events_membership_mk2.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/current_state_events_membership_mk2.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/delete_keys_from_deleted_backups.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/delete_keys_from_deleted_backups.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/destinations_failure_ts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/destinations_failure_ts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/destinations_retry_interval_type.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/destinations_retry_interval_type.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/device_stream_id_insert.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/device_stream_id_insert.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/devices_last_seen.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/devices_last_seen.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/drop_unused_event_tables.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/drop_unused_event_tables.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/event_expiry.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/event_expiry.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/event_labels.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/event_labels.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/event_labels_background_update.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/event_labels_background_update.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/fix_room_keys_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/fix_room_keys_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/hidden_devices.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/hidden_devices.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/hidden_devices_fix.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/hidden_devices_fix.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/nuke_empty_communities_from_db.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/nuke_empty_communities_from_db.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/public_room_list_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/public_room_list_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor2.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor2.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor3_fix_update.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor3_fix_update.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/redaction_censor4.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/redaction_censor4.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/remove_tombstoned_rooms_from_directory.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/remove_tombstoned_rooms_from_directory.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/room_key_etag.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/room_key_etag.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/room_membership_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/room_membership_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/room_retention.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/room_retention.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/signing_keys.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/signing_keys.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/signing_keys_nonunique_signatures.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/signing_keys_nonunique_signatures.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/stats_separated.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/stats_separated.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/unique_user_filter_index.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/unique_user_filter_index.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/user_external_ids.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/user_external_ids.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/56/users_in_public_rooms_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/56/users_in_public_rooms_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/delete_old_current_state_events.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/delete_old_current_state_events.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/device_list_remote_cache_stale.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/device_list_remote_cache_stale.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/local_current_membership.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/local_current_membership.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/remove_sent_outbound_pokes.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/remove_sent_outbound_pokes.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_2.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/57/rooms_version_column_3.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/02remove_dup_outbound_pokes.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/02remove_dup_outbound_pokes.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/03persist_ui_auth.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/03persist_ui_auth.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/05cache_instance.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/05cache_instance.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/06dlols_unique_idx.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/06dlols_unique_idx.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/07add_method_to_thumbnail_constraint.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/07persist_ui_auth_ips.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/07persist_ui_auth_ips.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/08_media_safe_from_quarantine.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/09shadow_ban.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/09shadow_ban.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/10_pushrules_enabled_delete_obsolete.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/10_pushrules_enabled_delete_obsolete.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/10drop_local_rejections_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/10drop_local_rejections_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/10federation_pos_instance_name.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/10federation_pos_instance_name.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/11dehydration.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/11dehydration.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/11fallback.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/11fallback.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/11user_id_seq.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/11user_id_seq.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/12room_stats.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/12room_stats.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/13remove_presence_allow_inbound.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/13remove_presence_allow_inbound.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/14events_instance_name.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/14events_instance_name.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/14events_instance_name.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/14events_instance_name.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/15_catchup_destination_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/15_catchup_destination_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/15unread_count.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/15unread_count.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/16populate_stats_process_rooms_fix.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/16populate_stats_process_rooms_fix.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/17_catchup_last_successful.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/17_catchup_last_successful.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/18stream_positions.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/18stream_positions.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/19instance_map.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/19instance_map.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/19txn_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/19txn_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/20instance_name_event_tables.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/20instance_name_event_tables.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/20user_daily_visits.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/20user_daily_visits.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/21as_device_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/21as_device_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/22puppet_token.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/22puppet_token.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/23e2e_cross_signing_keys_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/23e2e_cross_signing_keys_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/24drop_event_json_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/24drop_event_json_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/25user_external_ids_user_id_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/25user_external_ids_user_id_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/26access_token_last_validated.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/26access_token_last_validated.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/27local_invites.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/27local_invites.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/58/28drop_last_used_column.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/01ignored_user.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/01ignored_user.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/02shard_send_to_device.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/02shard_send_to_device.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/03shard_send_to_device_sequence.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/03shard_send_to_device_sequence.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/04_event_auth_chains.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/04drop_account_data.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/04drop_account_data.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/05cache_invalidation.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/05cache_invalidation.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/06chain_cover_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/06chain_cover_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/06shard_account_data.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/06shard_account_data.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/06shard_account_data.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/06shard_account_data.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/07shard_account_data_fix.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/07shard_account_data_fix.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/08delete_pushers_for_deactivated_accounts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/08delete_pushers_for_deactivated_accounts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/08delete_stale_pushers.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/08delete_stale_pushers.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/09rejected_events_metadata.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/09rejected_events_metadata.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/10delete_purged_chain_cover.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/10delete_purged_chain_cover.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/11add_knock_members_to_stats.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/11add_knock_members_to_stats.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/11drop_thumbnail_constraint.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/11drop_thumbnail_constraint.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/12account_validity_token_used_ts_ms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/12account_validity_token_used_ts_ms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/12presence_stream_instance.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/12presence_stream_instance.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/12presence_stream_instance_seq.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/12presence_stream_instance_seq.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/13users_to_send_full_presence_to.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/13users_to_send_full_presence_to.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/14refresh_tokens.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/14refresh_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/15locks.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/15locks.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/59/16federation_inbound_staging.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/59/16federation_inbound_staging.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/60/01recreate_stream_ordering.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/60/01recreate_stream_ordering.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/60/02change_stream_ordering_columns.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/60/02change_stream_ordering_columns.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/01change_appservices_txns.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/01change_appservices_txns.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/01insertion_event_lookups.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/01insertion_event_lookups.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/02drop_redundant_room_depth_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/02drop_redundant_room_depth_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/61/03recreate_min_depth.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/61/03recreate_min_depth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/62/01insertion_event_extremities.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/62/01insertion_event_extremities.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/01create_registration_tokens.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/01create_registration_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/02delete_unlinked_email_pushers.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/02delete_unlinked_email_pushers.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/02populate-rooms-creator.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/02populate-rooms-creator.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/03session_store.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/03session_store.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/63/04add_presence_stream_not_offline_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/63/04add_presence_stream_not_offline_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/64/01msc2716_chunk_to_batch_rename.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/01msc2716_insertion_event_edges.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/01msc2716_insertion_event_edges.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/03remove_hidden_devices_from_device_inbox.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/03remove_hidden_devices_from_device_inbox.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/04_local_group_updates.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/04_local_group_updates.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/05_remove_room_stats_historical_and_user_stats_historical.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/05_remove_room_stats_historical_and_user_stats_historical.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/06remove_deleted_devices_from_device_inbox.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/06remove_deleted_devices_from_device_inbox.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/07_arbitrary_relations.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/07_arbitrary_relations.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/08_device_inbox_background_updates.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/08_device_inbox_background_updates.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/10_expirable_refresh_tokens.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/10_expirable_refresh_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/65/11_devices_auth_provider_session.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/65/11_devices_auth_provider_session.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/67/01drop_public_room_list_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/67/01drop_public_room_list_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/01event_columns.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/01event_columns.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/02_msc2409_add_device_id_appservice_stream_type.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/02_msc2409_add_device_id_appservice_stream_type.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/03_delete_account_data_for_deactivated_accounts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/03_delete_account_data_for_deactivated_accounts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/04_refresh_tokens_index_next_token_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/04_refresh_tokens_index_next_token_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/04partial_state_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/04partial_state_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/05_delete_non_strings_from_event_search.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/05_delete_non_strings_from_event_search.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/05partial_state_rooms_triggers.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/05partial_state_rooms_triggers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/68/06_msc3202_add_device_list_appservice_stream_type.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/68/06_msc3202_add_device_list_appservice_stream_type.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/69/01as_txn_seq.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/69/01as_txn_seq.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/69/01device_list_oubound_by_room.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/69/01device_list_oubound_by_room.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/69/02cache_invalidation_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/69/02cache_invalidation_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/70/01clean_table_purged_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/70/01clean_table_purged_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/01rebuild_event_edges.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/01remove_noop_background_updates.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/01remove_noop_background_updates.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/71/02event_push_summary_unique.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/71/02event_push_summary_unique.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/01add_room_type_to_state_stats.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/01add_room_type_to_state_stats.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/01event_push_summary_receipt.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/01event_push_summary_receipt.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/02event_push_actions_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/02event_push_actions_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/03bg_populate_events_columns.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/03bg_populate_events_columns.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/03drop_event_reference_hashes.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/03drop_event_reference_hashes.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/03remove_groups.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/03remove_groups.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/04drop_column_application_services_state_last_txn.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/05receipts_event_stream_ordering.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/05receipts_event_stream_ordering.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/05remove_unstable_private_read_receipts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/05remove_unstable_private_read_receipts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/06add_consent_ts_to_users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/06add_consent_ts_to_users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/06thread_notifications.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/06thread_notifications.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/07force_update_current_state_events_membership.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/07force_update_current_state_events_membership.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/07thread_receipts.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/07thread_receipts.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/07thread_receipts.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/07thread_receipts.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/08begin_cache_invalidation_seq_at_2.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/08begin_cache_invalidation_seq_at_2.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/08thread_receipts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/08thread_receipts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/72/09partial_indices.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/72/09partial_indices.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/01event_failed_pull_attempts.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/01event_failed_pull_attempts.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/02add_pusher_enabled.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/02add_pusher_enabled.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/02room_id_indexes_for_purging.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/02room_id_indexes_for_purging.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/03pusher_device_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/03pusher_device_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/03users_approved_column.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/03users_approved_column.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/04partial_join_details.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/04partial_join_details.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/04pending_device_list_updates.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/04pending_device_list_updates.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/05old_push_actions.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/05old_push_actions.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/05old_push_actions.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/05old_push_actions.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/06thread_notifications_thread_id_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/06thread_notifications_thread_id_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/08thread_receipts_non_null.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/09partial_joined_via_destination.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/09partial_joined_via_destination.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/09threads_table.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/09threads_table.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/10_update_sqlite_fts4_tokenizer.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/10_update_sqlite_fts4_tokenizer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/10login_tokens.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/10login_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/11event_search_room_id_n_distinct.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/11event_search_room_id_n_distinct.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/12refactor_device_list_outbound_pokes.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/12refactor_device_list_outbound_pokes.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/13add_device_lists_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/13add_device_lists_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/20_un_partial_stated_room_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/20_un_partial_stated_room_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/21_un_partial_stated_room_stream_seq.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/21_un_partial_stated_room_stream_seq.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/22_rebuild_user_dir_stats.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/22_rebuild_user_dir_stats.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/22_un_partial_stated_event_stream.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/22_un_partial_stated_event_stream.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/23_fix_thread_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/23_fix_thread_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/23_un_partial_stated_room_stream_seq.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/23_un_partial_stated_room_stream_seq.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/24_events_jump_to_date_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/24_events_jump_to_date_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/73/25drop_presence.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/73/25drop_presence.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/01_user_directory_stale_remote_users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/01_user_directory_stale_remote_users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/02_set_device_id_for_pushers_bg_update.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/02_set_device_id_for_pushers_bg_update.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/03_membership_tables_event_stream_ordering.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/03_room_membership_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/03_room_membership_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/04_delete_e2e_backup_keys_for_deactivated_users.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/04_delete_e2e_backup_keys_for_deactivated_users.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/04_membership_tables_event_stream_ordering_triggers.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/04_membership_tables_event_stream_ordering_triggers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/05_events_txn_id_device_id.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/05_events_txn_id_device_id.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/74/90COMMENTS_destinations.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/74/90COMMENTS_destinations.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/01_add_profiles_full_user_id_column.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/01_add_profiles_full_user_id_column.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/02_add_user_filters_full_user_id_column.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/02_add_user_filters_full_user_id_column.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/03_per_user_experimental_features.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/03_per_user_experimental_features.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/76/04_add_room_forgetter.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/76/04_add_room_forgetter.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/01_add_profiles_not_valid_check.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/01_add_profiles_not_valid_check.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/02_add_user_filters_not_valid_check.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/02_add_user_filters_not_valid_check.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/03bg_populate_full_user_id_profiles.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/03bg_populate_full_user_id_profiles.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/04bg_populate_full_user_id_user_filters.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/04bg_populate_full_user_id_user_filters.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/05thread_notifications_backfill.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/05thread_notifications_backfill.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions_staging.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_actions_staging.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_summary.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/06thread_notifications_not_null_event_push_summary.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/77/14bg_indices_event_stream_ordering.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/77/14bg_indices_event_stream_ordering.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/01_validate_and_update_profiles.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/01_validate_and_update_profiles.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/02_validate_and_update_user_filters.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/02_validate_and_update_user_filters.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/03_remove_unused_indexes_user_filters.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/03_remove_unused_indexes_user_filters.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/03event_extremities_constraints.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/03event_extremities_constraints.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/78/04_add_full_user_id_index_user_filters.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/78/04_add_full_user_id_index_user_filters.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/03_read_write_locks_triggers.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/04_mitigate_stream_ordering_update_race.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/04_mitigate_stream_ordering_update_race.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/79/05_read_write_locks_triggers.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/01_users_alter_locked.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/01_users_alter_locked.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/02_read_write_locks_unlogged.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/02_read_write_locks_unlogged.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/02_scheduled_tasks.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/02_scheduled_tasks.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/03_read_write_locks_triggers.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/03_read_write_locks_triggers.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/80/04_read_write_locks_deadlock.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/80/04_read_write_locks_deadlock.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/82/02_scheduled_tasks_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/82/02_scheduled_tasks_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/82/04_add_indices_for_purging_rooms.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/82/04_add_indices_for_purging_rooms.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/82/05gaps.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/82/05gaps.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/01_drop_old_tables.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/01_drop_old_tables.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/03_instance_name_receipts.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/03_instance_name_receipts.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/05_cross_signing_key_update_grant.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/05_cross_signing_key_update_grant.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/delta/83/06_event_push_summary_room.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/delta/83/06_event_push_summary_room.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/full_schemas/72/full.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/full_schemas/72/full.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/main/full_schemas/72/full.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/main/full_schemas/72/full.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/23/drop_state_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/23/drop_state_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/32/remove_state_indices.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/32/remove_state_indices.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/35/add_state_index.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/35/add_state_index.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/35/state.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/35/state.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/35/state_dedupe.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/35/state_dedupe.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/47/state_group_seq.py` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/47/state_group_seq.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/56/state_group_room_idx.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/56/state_group_room_idx.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/61/02state_groups_state_n_distinct.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/61/02state_groups_state_n_distinct.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/delta/70/08_state_group_edges_unique.sql` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/delta/70/08_state_group_edges_unique.sql`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/full_schemas/72/full.sql.postgres` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/full_schemas/72/full.sql.postgres`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/schema/state/full_schemas/72/full.sql.sqlite` & `matrix_synapse-1.99.0rc1/synapse/storage/schema/state/full_schemas/72/full.sql.sqlite`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/types.py` & `matrix_synapse-1.99.0rc1/synapse/storage/types.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/util/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/storage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/util/id_generators.py` & `matrix_synapse-1.99.0rc1/synapse/storage/util/id_generators.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/util/partial_state_events_tracker.py` & `matrix_synapse-1.99.0rc1/synapse/storage/util/partial_state_events_tracker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/storage/util/sequence.py` & `matrix_synapse-1.99.0rc1/synapse/storage/util/sequence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/streams/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/streams/config.py` & `matrix_synapse-1.99.0rc1/synapse/streams/config.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/streams/events.py` & `matrix_synapse-1.99.0rc1/synapse/streams/events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/synapse_rust/acl.pyi` & `matrix_synapse-1.99.0rc1/synapse/synapse_rust/acl.pyi`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/synapse_rust/events.pyi` & `matrix_synapse-1.99.0rc1/synapse/synapse_rust/events.pyi`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/synapse_rust/push.pyi` & `matrix_synapse-1.99.0rc1/synapse/synapse_rust/push.pyi`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/types/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/types/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/types/state.py` & `matrix_synapse-1.99.0rc1/synapse/types/state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/async_helpers.py` & `matrix_synapse-1.99.0rc1/synapse/util/async_helpers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/batching_queue.py` & `matrix_synapse-1.99.0rc1/synapse/util/batching_queue.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/__init__.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/cached_call.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/cached_call.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/deferred_cache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/deferred_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/descriptors.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/descriptors.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/dictionary_cache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/dictionary_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/expiringcache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/expiringcache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/lrucache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/lrucache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/response_cache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/response_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/stream_change_cache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/stream_change_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/treecache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/treecache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/caches/ttlcache.py` & `matrix_synapse-1.99.0rc1/synapse/util/caches/ttlcache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/cancellation.py` & `matrix_synapse-1.99.0rc1/synapse/util/cancellation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/check_dependencies.py` & `matrix_synapse-1.99.0rc1/synapse/util/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/daemonize.py` & `matrix_synapse-1.99.0rc1/synapse/util/daemonize.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/distributor.py` & `matrix_synapse-1.99.0rc1/synapse/util/distributor.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/file_consumer.py` & `matrix_synapse-1.99.0rc1/synapse/util/file_consumer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/frozenutils.py` & `matrix_synapse-1.99.0rc1/synapse/util/frozenutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/gai_resolver.py` & `matrix_synapse-1.99.0rc1/synapse/util/gai_resolver.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/hash.py` & `matrix_synapse-1.99.0rc1/synapse/util/hash.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/httpresourcetree.py` & `matrix_synapse-1.99.0rc1/synapse/util/httpresourcetree.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/iterutils.py` & `matrix_synapse-1.99.0rc1/synapse/util/iterutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/linked_list.py` & `matrix_synapse-1.99.0rc1/synapse/util/linked_list.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/logcontext.py` & `matrix_synapse-1.99.0rc1/synapse/util/logcontext.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/logformatter.py` & `matrix_synapse-1.99.0rc1/synapse/util/logformatter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/macaroons.py` & `matrix_synapse-1.99.0rc1/synapse/util/macaroons.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/manhole.py` & `matrix_synapse-1.99.0rc1/synapse/util/manhole.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/metrics.py` & `matrix_synapse-1.99.0rc1/synapse/util/metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/module_loader.py` & `matrix_synapse-1.99.0rc1/synapse/util/module_loader.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/msisdn.py` & `matrix_synapse-1.99.0rc1/synapse/util/msisdn.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/patch_inline_callbacks.py` & `matrix_synapse-1.99.0rc1/synapse/util/patch_inline_callbacks.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/ratelimitutils.py` & `matrix_synapse-1.99.0rc1/synapse/util/ratelimitutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/retryutils.py` & `matrix_synapse-1.99.0rc1/synapse/util/retryutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/rlimit.py` & `matrix_synapse-1.99.0rc1/synapse/util/rlimit.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/rust.py` & `matrix_synapse-1.99.0rc1/synapse/util/rust.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/stringutils.py` & `matrix_synapse-1.99.0rc1/synapse/util/stringutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/task_scheduler.py` & `matrix_synapse-1.99.0rc1/synapse/util/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/templates.py` & `matrix_synapse-1.99.0rc1/synapse/util/templates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/threepids.py` & `matrix_synapse-1.99.0rc1/synapse/util/threepids.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/util/wheel_timer.py` & `matrix_synapse-1.99.0rc1/synapse/util/wheel_timer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synapse/visibility.py` & `matrix_synapse-1.99.0rc1/synapse/visibility.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synmark/__init__.py` & `matrix_synapse-1.99.0rc1/synmark/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synmark/__main__.py` & `matrix_synapse-1.99.0rc1/synmark/__main__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synmark/suites/logging.py` & `matrix_synapse-1.99.0rc1/synmark/suites/logging.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synmark/suites/lrucache.py` & `matrix_synapse-1.99.0rc1/synmark/suites/lrucache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/synmark/suites/lrucache_evict.py` & `matrix_synapse-1.99.0rc1/synmark/suites/lrucache_evict.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/sytest-blacklist` & `matrix_synapse-1.99.0rc1/sytest-blacklist`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/__init__.py` & `matrix_synapse-1.99.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/api/test_auth.py` & `matrix_synapse-1.99.0rc1/tests/api/test_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/api/test_errors.py` & `matrix_synapse-1.99.0rc1/tests/api/test_errors.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/api/test_filtering.py` & `matrix_synapse-1.99.0rc1/tests/api/test_filtering.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/api/test_ratelimiting.py` & `matrix_synapse-1.99.0rc1/tests/api/test_ratelimiting.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/app/test_homeserver_start.py` & `matrix_synapse-1.99.0rc1/tests/app/test_homeserver_start.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/app/test_openid_listener.py` & `matrix_synapse-1.99.0rc1/tests/app/test_openid_listener.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/app/test_phone_stats_home.py` & `matrix_synapse-1.99.0rc1/tests/app/test_phone_stats_home.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/appservice/__init__.py` & `matrix_synapse-1.99.0rc1/tests/appservice/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/appservice/test_api.py` & `matrix_synapse-1.99.0rc1/tests/appservice/test_api.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/appservice/test_appservice.py` & `matrix_synapse-1.99.0rc1/tests/appservice/test_appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/appservice/test_scheduler.py` & `matrix_synapse-1.99.0rc1/tests/appservice/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/__init__.py` & `matrix_synapse-1.99.0rc1/tests/config/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test___main__.py` & `matrix_synapse-1.99.0rc1/tests/config/test___main__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_api.py` & `matrix_synapse-1.99.0rc1/tests/config/test_api.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_appservice.py` & `matrix_synapse-1.99.0rc1/tests/config/test_appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_background_update.py` & `matrix_synapse-1.99.0rc1/tests/config/test_background_update.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_base.py` & `matrix_synapse-1.99.0rc1/tests/config/test_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_cache.py` & `matrix_synapse-1.99.0rc1/tests/config/test_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_database.py` & `matrix_synapse-1.99.0rc1/tests/config/test_database.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_generate.py` & `matrix_synapse-1.99.0rc1/tests/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_load.py` & `matrix_synapse-1.99.0rc1/tests/config/test_load.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_oauth_delegation.py` & `matrix_synapse-1.99.0rc1/tests/config/test_oauth_delegation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_ratelimiting.py` & `matrix_synapse-1.99.0rc1/tests/config/test_ratelimiting.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_registration_config.py` & `matrix_synapse-1.99.0rc1/tests/config/test_registration_config.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_room_directory.py` & `matrix_synapse-1.99.0rc1/tests/config/test_room_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_server.py` & `matrix_synapse-1.99.0rc1/tests/config/test_server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_tls.py` & `matrix_synapse-1.99.0rc1/tests/config/test_tls.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_util.py` & `matrix_synapse-1.99.0rc1/tests/config/test_util.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/test_workers.py` & `matrix_synapse-1.99.0rc1/tests/config/test_workers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/config/utils.py` & `matrix_synapse-1.99.0rc1/tests/config/utils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/crypto/__init__.py` & `matrix_synapse-1.99.0rc1/tests/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/crypto/test_event_signing.py` & `matrix_synapse-1.99.0rc1/tests/crypto/test_event_signing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/crypto/test_keyring.py` & `matrix_synapse-1.99.0rc1/tests/crypto/test_keyring.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/events/test_presence_router.py` & `matrix_synapse-1.99.0rc1/tests/events/test_presence_router.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/events/test_snapshot.py` & `matrix_synapse-1.99.0rc1/tests/events/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/events/test_utils.py` & `matrix_synapse-1.99.0rc1/tests/events/test_utils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/test_complexity.py` & `matrix_synapse-1.99.0rc1/tests/federation/test_complexity.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/test_federation_catch_up.py` & `matrix_synapse-1.99.0rc1/tests/federation/test_federation_catch_up.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/test_federation_client.py` & `matrix_synapse-1.99.0rc1/tests/federation/test_federation_client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/test_federation_sender.py` & `matrix_synapse-1.99.0rc1/tests/federation/test_federation_sender.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/test_federation_server.py` & `matrix_synapse-1.99.0rc1/tests/federation/test_federation_server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/transport/server/__init__.py` & `matrix_synapse-1.99.0rc1/tests/federation/transport/server/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/transport/server/test__base.py` & `matrix_synapse-1.99.0rc1/tests/federation/transport/server/test__base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/transport/test_client.py` & `matrix_synapse-1.99.0rc1/tests/federation/transport/test_client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/transport/test_knocking.py` & `matrix_synapse-1.99.0rc1/tests/federation/transport/test_knocking.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/federation/transport/test_server.py` & `matrix_synapse-1.99.0rc1/tests/federation/transport/test_server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_admin.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_admin.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_appservice.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_auth.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_cas.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_cas.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_deactivate_account.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_deactivate_account.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_device.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_device.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_directory.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_e2e_keys.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_e2e_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_e2e_room_keys.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_e2e_room_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_federation.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_federation_event.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_federation_event.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_message.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_message.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_oauth_delegation.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_oauth_delegation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_oidc.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_oidc.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_password_providers.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_password_providers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_presence.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_profile.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_profile.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_receipts.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_register.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_register.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_room.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_room_list.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_room_list.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_room_member.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_room_member.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_room_summary.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_room_summary.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_saml.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_saml.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_send_email.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_send_email.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_sso.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_sso.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_stats.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_stats.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_sync.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_sync.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_typing.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_typing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_user_directory.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_user_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/handlers/test_worker_lock.py` & `matrix_synapse-1.99.0rc1/tests/handlers/test_worker_lock.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/__init__.py` & `matrix_synapse-1.99.0rc1/tests/http/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/ca.crt` & `matrix_synapse-1.99.0rc1/tests/http/ca.crt`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/ca.key` & `matrix_synapse-1.99.0rc1/tests/http/ca.key`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/federation/__init__.py` & `matrix_synapse-1.99.0rc1/tests/http/federation/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/federation/test_matrix_federation_agent.py` & `matrix_synapse-1.99.0rc1/tests/http/federation/test_matrix_federation_agent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/federation/test_srv_resolver.py` & `matrix_synapse-1.99.0rc1/tests/http/federation/test_srv_resolver.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/server/__init__.py` & `matrix_synapse-1.99.0rc1/tests/http/server/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/server/_base.py` & `matrix_synapse-1.99.0rc1/tests/http/server/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/server.key` & `matrix_synapse-1.99.0rc1/tests/http/server.key`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_additional_resource.py` & `matrix_synapse-1.99.0rc1/tests/http/test_additional_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_client.py` & `matrix_synapse-1.99.0rc1/tests/http/test_client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_endpoint.py` & `matrix_synapse-1.99.0rc1/tests/http/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_matrixfederationclient.py` & `matrix_synapse-1.99.0rc1/tests/http/test_matrixfederationclient.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_proxy.py` & `matrix_synapse-1.99.0rc1/tests/http/test_proxy.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_proxyagent.py` & `matrix_synapse-1.99.0rc1/tests/http/test_proxyagent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_servlet.py` & `matrix_synapse-1.99.0rc1/tests/http/test_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_simple_client.py` & `matrix_synapse-1.99.0rc1/tests/http/test_simple_client.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/http/test_site.py` & `matrix_synapse-1.99.0rc1/tests/http/test_site.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/logging/__init__.py` & `matrix_synapse-1.99.0rc1/tests/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/logging/test_opentracing.py` & `matrix_synapse-1.99.0rc1/tests/logging/test_opentracing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/logging/test_remote_handler.py` & `matrix_synapse-1.99.0rc1/tests/logging/test_remote_handler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/logging/test_terse_json.py` & `matrix_synapse-1.99.0rc1/tests/logging/test_terse_json.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/__init__.py` & `matrix_synapse-1.99.0rc1/tests/media/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_base.py` & `matrix_synapse-1.99.0rc1/tests/media/test_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_filepath.py` & `matrix_synapse-1.99.0rc1/tests/media/test_filepath.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_html_preview.py` & `matrix_synapse-1.99.0rc1/tests/media/test_html_preview.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_media_retention.py` & `matrix_synapse-1.99.0rc1/tests/media/test_media_retention.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_media_storage.py` & `matrix_synapse-1.99.0rc1/tests/media/test_media_storage.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_oembed.py` & `matrix_synapse-1.99.0rc1/tests/media/test_oembed.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/media/test_url_previewer.py` & `matrix_synapse-1.99.0rc1/tests/media/test_url_previewer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/metrics/test_background_process_metrics.py` & `matrix_synapse-1.99.0rc1/tests/metrics/test_background_process_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/metrics/test_metrics.py` & `matrix_synapse-1.99.0rc1/tests/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/module_api/test_account_data_manager.py` & `matrix_synapse-1.99.0rc1/tests/module_api/test_account_data_manager.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/module_api/test_api.py` & `matrix_synapse-1.99.0rc1/tests/module_api/test_api.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/module_api/test_event_unsigned_addition.py` & `matrix_synapse-1.99.0rc1/tests/module_api/test_event_unsigned_addition.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/push/test_bulk_push_rule_evaluator.py` & `matrix_synapse-1.99.0rc1/tests/push/test_bulk_push_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/push/test_email.py` & `matrix_synapse-1.99.0rc1/tests/push/test_email.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/push/test_http.py` & `matrix_synapse-1.99.0rc1/tests/push/test_http.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/push/test_presentable_names.py` & `matrix_synapse-1.99.0rc1/tests/push/test_presentable_names.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/push/test_push_rule_evaluator.py` & `matrix_synapse-1.99.0rc1/tests/push/test_push_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/__init__.py` & `matrix_synapse-1.99.0rc1/tests/replication/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/_base.py` & `matrix_synapse-1.99.0rc1/tests/replication/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/http/__init__.py` & `matrix_synapse-1.99.0rc1/tests/replication/http/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/http/test__base.py` & `matrix_synapse-1.99.0rc1/tests/replication/http/test__base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/storage/__init__.py` & `matrix_synapse-1.99.0rc1/tests/replication/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/storage/_base.py` & `matrix_synapse-1.99.0rc1/tests/replication/storage/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/storage/test_events.py` & `matrix_synapse-1.99.0rc1/tests/replication/storage/test_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/__init__.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/__init__.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_account_data.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_events.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_federation.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_partial_state.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_partial_state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_receipts.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_to_device.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_to_device.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/streams/test_typing.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/streams/test_typing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/test_commands.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/test_commands.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/tcp/test_handler.py` & `matrix_synapse-1.99.0rc1/tests/replication/tcp/test_handler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_auth.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_client_reader_shard.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_client_reader_shard.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_federation_ack.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_federation_ack.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_federation_sender_shard.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_federation_sender_shard.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_module_cache_invalidation.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_module_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_multi_media_repo.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_multi_media_repo.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_pusher_shard.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_pusher_shard.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_sharded_event_persister.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_sharded_event_persister.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/replication/test_sharded_receipts.py` & `matrix_synapse-1.99.0rc1/tests/replication/test_sharded_receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/__init__.py` & `matrix_synapse-1.99.0rc1/tests/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/__init__.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_admin.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_admin.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_background_updates.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_background_updates.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_device.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_device.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_event_reports.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_event_reports.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_federation.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_jwks.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_jwks.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_media.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_media.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_registration_tokens.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_registration_tokens.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_room.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_server_notice.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_server_notice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_statistics.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_statistics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_user.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_user.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/admin/test_username_available.py` & `matrix_synapse-1.99.0rc1/tests/rest/admin/test_username_available.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/__init__.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_account.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_account.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_account_data.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_auth.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_auth_issuer.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_auth_issuer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_capabilities.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_consent.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_consent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_devices.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_devices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_directory.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_ephemeral_message.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_ephemeral_message.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_events.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_filter.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_filter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_identity.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_identity.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_keys.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_login.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_login.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_login_token_request.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_login_token_request.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_models.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_models.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_mutual_rooms.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_mutual_rooms.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_notifications.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_notifications.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_password_policy.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_password_policy.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_power_levels.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_power_levels.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_presence.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_presence.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_profile.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_profile.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_push_rule_attrs.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_push_rule_attrs.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_read_marker.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_read_marker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_receipts.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_redactions.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_redactions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_register.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_register.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_relations.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_relations.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_rendezvous.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_rendezvous.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_report_event.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_report_event.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_retention.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_retention.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_rooms.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_rooms.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_sendtodevice.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_sendtodevice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_shadow_banned.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_shadow_banned.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_sync.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_sync.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_third_party_rules.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_third_party_rules.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_transactions.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_transactions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_typing.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_typing.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/test_upgrade_room.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/test_upgrade_room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/client/utils.py` & `matrix_synapse-1.99.0rc1/tests/rest/client/utils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/key/v2/test_remote_key_resource.py` & `matrix_synapse-1.99.0rc1/tests/rest/key/v2/test_remote_key_resource.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/media/__init__.py` & `matrix_synapse-1.99.0rc1/tests/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/media/test_domain_blocking.py` & `matrix_synapse-1.99.0rc1/tests/rest/media/test_domain_blocking.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/media/test_url_preview.py` & `matrix_synapse-1.99.0rc1/tests/rest/media/test_url_preview.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/test_health.py` & `matrix_synapse-1.99.0rc1/tests/rest/test_health.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/rest/test_well_known.py` & `matrix_synapse-1.99.0rc1/tests/rest/test_well_known.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/scripts/test_new_matrix_user.py` & `matrix_synapse-1.99.0rc1/tests/scripts/test_new_matrix_user.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/server.py` & `matrix_synapse-1.99.0rc1/tests/server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/server_notices/test_consent.py` & `matrix_synapse-1.99.0rc1/tests/server_notices/test_consent.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/server_notices/test_resource_limits_server_notices.py` & `matrix_synapse-1.99.0rc1/tests/server_notices/test_resource_limits_server_notices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/state/test_v2.py` & `matrix_synapse-1.99.0rc1/tests/state/test_v2.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/__init__.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/__init__.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_cache.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_deviceinbox.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_deviceinbox.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_end_to_end_keys.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_end_to_end_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_events_worker.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_events_worker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_lock.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_lock.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_receipts.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/databases/main/test_room.py` & `matrix_synapse-1.99.0rc1/tests/storage/databases/main/test_room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test__base.py` & `matrix_synapse-1.99.0rc1/tests/storage/test__base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_account_data.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_account_data.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_appservice.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_appservice.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_background_update.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_background_update.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_base.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_base.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_cleanup_extrems.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_cleanup_extrems.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_client_ips.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_client_ips.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_database.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_database.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_devices.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_devices.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_directory.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_e2e_room_keys.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_e2e_room_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_end_to_end_keys.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_end_to_end_keys.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_event_chain.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_event_chain.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_event_federation.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_event_federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_event_metrics.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_event_metrics.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_event_push_actions.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_event_push_actions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_events.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_events.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_id_generators.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_id_generators.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_main.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_main.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_monthly_active_users.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_monthly_active_users.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_profile.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_profile.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_purge.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_purge.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_receipts.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_receipts.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_redaction.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_redaction.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_registration.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_registration.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_relations.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_relations.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_rollback_worker.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_rollback_worker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_room.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_room.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_room_search.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_room_search.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_roommember.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_roommember.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_state.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_stream.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_stream.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_transactions.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_transactions.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_txn_limit.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_txn_limit.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_unsafe_locale.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_unsafe_locale.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_user_directory.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_user_directory.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/test_user_filters.py` & `matrix_synapse-1.99.0rc1/tests/storage/test_user_filters.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/util/__init__.py` & `matrix_synapse-1.99.0rc1/tests/storage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/storage/util/test_partial_state_events_tracker.py` & `matrix_synapse-1.99.0rc1/tests/storage/util/test_partial_state_events_tracker.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_distributor.py` & `matrix_synapse-1.99.0rc1/tests/test_distributor.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_event_auth.py` & `matrix_synapse-1.99.0rc1/tests/test_event_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_federation.py` & `matrix_synapse-1.99.0rc1/tests/test_federation.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_mau.py` & `matrix_synapse-1.99.0rc1/tests/test_mau.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_phone_home.py` & `matrix_synapse-1.99.0rc1/tests/test_phone_home.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_server.py` & `matrix_synapse-1.99.0rc1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_state.py` & `matrix_synapse-1.99.0rc1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_terms_auth.py` & `matrix_synapse-1.99.0rc1/tests/test_terms_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_test_utils.py` & `matrix_synapse-1.99.0rc1/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_types.py` & `matrix_synapse-1.99.0rc1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_utils/__init__.py` & `matrix_synapse-1.99.0rc1/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_utils/event_injection.py` & `matrix_synapse-1.99.0rc1/tests/test_utils/event_injection.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_utils/html_parsers.py` & `matrix_synapse-1.99.0rc1/tests/test_utils/html_parsers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_utils/logging_setup.py` & `matrix_synapse-1.99.0rc1/tests/test_utils/logging_setup.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_utils/oidc.py` & `matrix_synapse-1.99.0rc1/tests/test_utils/oidc.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/test_visibility.py` & `matrix_synapse-1.99.0rc1/tests/test_visibility.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/types/test_state.py` & `matrix_synapse-1.99.0rc1/tests/types/test_state.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/unittest.py` & `matrix_synapse-1.99.0rc1/tests/unittest.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/__init__.py` & `matrix_synapse-1.99.0rc1/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/caches/__init__.py` & `matrix_synapse-1.99.0rc1/tests/util/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/caches/test_cached_call.py` & `matrix_synapse-1.99.0rc1/tests/util/caches/test_cached_call.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/caches/test_deferred_cache.py` & `matrix_synapse-1.99.0rc1/tests/util/caches/test_deferred_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/caches/test_descriptors.py` & `matrix_synapse-1.99.0rc1/tests/util/caches/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/caches/test_response_cache.py` & `matrix_synapse-1.99.0rc1/tests/util/caches/test_response_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/caches/test_ttlcache.py` & `matrix_synapse-1.99.0rc1/tests/util/caches/test_ttlcache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_async_helpers.py` & `matrix_synapse-1.99.0rc1/tests/util/test_async_helpers.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_batching_queue.py` & `matrix_synapse-1.99.0rc1/tests/util/test_batching_queue.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_check_dependencies.py` & `matrix_synapse-1.99.0rc1/tests/util/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_dict_cache.py` & `matrix_synapse-1.99.0rc1/tests/util/test_dict_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_expiring_cache.py` & `matrix_synapse-1.99.0rc1/tests/util/test_expiring_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_file_consumer.py` & `matrix_synapse-1.99.0rc1/tests/util/test_file_consumer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_itertools.py` & `matrix_synapse-1.99.0rc1/tests/util/test_itertools.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_linearizer.py` & `matrix_synapse-1.99.0rc1/tests/util/test_linearizer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_logcontext.py` & `matrix_synapse-1.99.0rc1/tests/util/test_logcontext.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_logformatter.py` & `matrix_synapse-1.99.0rc1/tests/util/test_logformatter.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_lrucache.py` & `matrix_synapse-1.99.0rc1/tests/util/test_lrucache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_macaroons.py` & `matrix_synapse-1.99.0rc1/tests/util/test_macaroons.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_ratelimitutils.py` & `matrix_synapse-1.99.0rc1/tests/util/test_ratelimitutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_retryutils.py` & `matrix_synapse-1.99.0rc1/tests/util/test_retryutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_rwlock.py` & `matrix_synapse-1.99.0rc1/tests/util/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_stream_change_cache.py` & `matrix_synapse-1.99.0rc1/tests/util/test_stream_change_cache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_stringutils.py` & `matrix_synapse-1.99.0rc1/tests/util/test_stringutils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_task_scheduler.py` & `matrix_synapse-1.99.0rc1/tests/util/test_task_scheduler.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_threepids.py` & `matrix_synapse-1.99.0rc1/tests/util/test_threepids.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_treecache.py` & `matrix_synapse-1.99.0rc1/tests/util/test_treecache.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/util/test_wheel_timer.py` & `matrix_synapse-1.99.0rc1/tests/util/test_wheel_timer.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/tests/utils.py` & `matrix_synapse-1.99.0rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `matrix_synapse-1.99.0/setup.py` & `matrix_synapse-1.99.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
                      'synapse_worker = synapse.app.generic_worker:main',
                      'synctl = synapse._scripts.synctl:main',
                      'update_synapse_database = '
                      'synapse._scripts.update_synapse_database:main']}
 
 setup_kwargs = {
     'name': 'matrix-synapse',
-    'version': '1.99.0',
+    'version': '1.99.0rc1',
     'description': 'Homeserver for the Matrix decentralised comms protocol',
     'long_description': '=========================================================================\nSynapse |support| |development| |documentation| |license| |pypi| |python|\n=========================================================================\n\nSynapse is an open-source `Matrix <https://matrix.org/>`_ homeserver written and\nmaintained by the Matrix.org Foundation. We began rapid development in 2014,\nreaching v1.0.0 in 2019. Development on Synapse and the Matrix protocol itself continues\nin earnest today.\n\nBriefly, Matrix is an open standard for communications on the internet, supporting\nfederation, encryption and VoIP. Matrix.org has more to say about the `goals of the\nMatrix project <https://matrix.org/docs/guides/introduction>`_, and the `formal specification\n<https://spec.matrix.org/>`_ describes the technical details.\n\n.. contents::\n\nInstalling and configuration\n============================\n\nThe Synapse documentation describes `how to install Synapse <https://element-hq.github.io/synapse/latest/setup/installation.html>`_. We recommend using\n`Docker images <https://element-hq.github.io/synapse/latest/setup/installation.html#docker-images-and-ansible-playbooks>`_ or `Debian packages from Matrix.org\n<https://element-hq.github.io/synapse/latest/setup/installation.html#matrixorg-packages>`_.\n\n.. _federation:\n\nSynapse has a variety of `config options\n<https://element-hq.github.io/synapse/latest/usage/configuration/config_documentation.html>`_\nwhich can be used to customise its behaviour after installation.\nThere are additional details on how to `configure Synapse for federation here\n<https://element-hq.github.io/synapse/latest/federate.html>`_.\n\n.. _reverse-proxy:\n\nUsing a reverse proxy with Synapse\n----------------------------------\n\nIt is recommended to put a reverse proxy such as\n`nginx <https://nginx.org/en/docs/http/ngx_http_proxy_module.html>`_,\n`Apache <https://httpd.apache.org/docs/current/mod/mod_proxy_http.html>`_,\n`Caddy <https://caddyserver.com/docs/quick-starts/reverse-proxy>`_,\n`HAProxy <https://www.haproxy.org/>`_ or\n`relayd <https://man.openbsd.org/relayd.8>`_ in front of Synapse. One advantage of\ndoing so is that it means that you can expose the default https port (443) to\nMatrix clients without needing to run Synapse with root privileges.\nFor information on configuring one, see `the reverse proxy docs\n<https://element-hq.github.io/synapse/latest/reverse_proxy.html>`_.\n\nUpgrading an existing Synapse\n-----------------------------\n\nThe instructions for upgrading Synapse are in `the upgrade notes`_.\nPlease check these instructions as upgrading may require extra steps for some\nversions of Synapse.\n\n.. _the upgrade notes: https://element-hq.github.io/synapse/develop/upgrade.html\n\n\nPlatform dependencies\n---------------------\n\nSynapse uses a number of platform dependencies such as Python and PostgreSQL,\nand aims to follow supported upstream versions. See the\n`deprecation policy <https://element-hq.github.io/synapse/latest/deprecation_policy.html>`_\nfor more details.\n\n\nSecurity note\n-------------\n\nMatrix serves raw, user-supplied data in some APIs -- specifically the `content\nrepository endpoints`_.\n\n.. _content repository endpoints: https://matrix.org/docs/spec/client_server/latest.html#get-matrix-media-r0-download-servername-mediaid\n\nWhilst we make a reasonable effort to mitigate against XSS attacks (for\ninstance, by using `CSP`_), a Matrix homeserver should not be hosted on a\ndomain hosting other web applications. This especially applies to sharing\nthe domain with Matrix web clients and other sensitive applications like\nwebmail. See\nhttps://developer.github.com/changes/2014-04-25-user-content-security for more\ninformation.\n\n.. _CSP: https://github.com/matrix-org/synapse/pull/1021\n\nIdeally, the homeserver should not simply be on a different subdomain, but on\na completely different `registered domain`_ (also known as top-level site or\neTLD+1). This is because `some attacks`_ are still possible as long as the two\napplications share the same registered domain.\n\n.. _registered domain: https://tools.ietf.org/html/draft-ietf-httpbis-rfc6265bis-03#section-2.3\n\n.. _some attacks: https://en.wikipedia.org/wiki/Session_fixation#Attacks_using_cross-subdomain_cookie\n\nTo illustrate this with an example, if your Element Web or other sensitive web\napplication is hosted on ``A.example1.com``, you should ideally host Synapse on\n``example2.com``. Some amount of protection is offered by hosting on\n``B.example1.com`` instead, so this is also acceptable in some scenarios.\nHowever, you should *not* host your Synapse on ``A.example1.com``.\n\nNote that all of the above refers exclusively to the domain used in Synapse\'s\n``public_baseurl`` setting. In particular, it has no bearing on the domain\nmentioned in MXIDs hosted on that server.\n\nFollowing this advice ensures that even if an XSS is found in Synapse, the\nimpact to other applications will be minimal.\n\n\nTesting a new installation\n==========================\n\nThe easiest way to try out your new Synapse installation is by connecting to it\nfrom a web client.\n\nUnless you are running a test instance of Synapse on your local machine, in\ngeneral, you will need to enable TLS support before you can successfully\nconnect from a client: see\n`TLS certificates <https://element-hq.github.io/synapse/latest/setup/installation.html#tls-certificates>`_.\n\nAn easy way to get started is to login or register via Element at\nhttps://app.element.io/#/login or https://app.element.io/#/register respectively.\nYou will need to change the server you are logging into from ``matrix.org``\nand instead specify a Homeserver URL of ``https://<server_name>:8448``\n(or just ``https://<server_name>`` if you are using a reverse proxy).\nIf you prefer to use another client, refer to our\n`client breakdown <https://matrix.org/ecosystem/clients/>`_.\n\nIf all goes well you should at least be able to log in, create a room, and\nstart sending messages.\n\n.. _`client-user-reg`:\n\nRegistering a new user from a client\n------------------------------------\n\nBy default, registration of new users via Matrix clients is disabled. To enable\nit:\n\n1. In the\n   `registration config section <https://element-hq.github.io/synapse/latest/usage/configuration/config_documentation.html#registration>`_\n   set ``enable_registration: true`` in ``homeserver.yaml``.\n2. Then **either**:\n\n   a. set up a `CAPTCHA <https://element-hq.github.io/synapse/latest/CAPTCHA_SETUP.html>`_, or\n   b. set ``enable_registration_without_verification: true`` in ``homeserver.yaml``.\n\nWe **strongly** recommend using a CAPTCHA, particularly if your homeserver is exposed to\nthe public internet. Without it, anyone can freely register accounts on your homeserver.\nThis can be exploited by attackers to create spambots targetting the rest of the Matrix\nfederation.\n\nYour new user name will be formed partly from the ``server_name``, and partly\nfrom a localpart you specify when you create the account. Your name will take\nthe form of::\n\n    @localpart:my.domain.name\n\n(pronounced "at localpart on my dot domain dot name").\n\nAs when logging in, you will need to specify a "Custom server".  Specify your\ndesired ``localpart`` in the \'User name\' box.\n\nTroubleshooting and support\n===========================\n\nThe `Admin FAQ <https://element-hq.github.io/synapse/latest/usage/administration/admin_faq.html>`_\nincludes tips on dealing with some common problems. For more details, see\n`Synapse\'s wider documentation <https://element-hq.github.io/synapse/latest/>`_.\n\nFor additional support installing or managing Synapse, please ask in the community\nsupport room |room|_ (from a matrix.org account if necessary). We do not use GitHub\nissues for support requests, only for bug reports and feature requests.\n\n.. |room| replace:: ``#synapse:matrix.org``\n.. _room: https://matrix.to/#/#synapse:matrix.org\n\n.. |docs| replace:: ``docs``\n.. _docs: docs\n\nIdentity Servers\n================\n\nIdentity servers have the job of mapping email addresses and other 3rd Party\nIDs (3PIDs) to Matrix user IDs, as well as verifying the ownership of 3PIDs\nbefore creating that mapping.\n\n**They are not where accounts or credentials are stored - these live on home\nservers. Identity Servers are just for mapping 3rd party IDs to matrix IDs.**\n\nThis process is very security-sensitive, as there is obvious risk of spam if it\nis too easy to sign up for Matrix accounts or harvest 3PID data. In the longer\nterm, we hope to create a decentralised system to manage it (`matrix-doc #712\n<https://github.com/matrix-org/matrix-doc/issues/712>`_), but in the meantime,\nthe role of managing trusted identity in the Matrix ecosystem is farmed out to\na cluster of known trusted ecosystem partners, who run \'Matrix Identity\nServers\' such as `Sydent <https://github.com/matrix-org/sydent>`_, whose role\nis purely to authenticate and track 3PID logins and publish end-user public\nkeys.\n\nYou can host your own copy of Sydent, but this will prevent you reaching other\nusers in the Matrix ecosystem via their email address, and prevent them finding\nyou. We therefore recommend that you use one of the centralised identity servers\nat ``https://matrix.org`` or ``https://vector.im`` for now.\n\nTo reiterate: the Identity server will only be used if you choose to associate\nan email address with your account, or send an invite to another user via their\nemail address.\n\n\nDevelopment\n===========\n\nWe welcome contributions to Synapse from the community!\nThe best place to get started is our\n`guide for contributors <https://element-hq.github.io/synapse/latest/development/contributing_guide.html>`_.\nThis is part of our larger `documentation <https://element-hq.github.io/synapse/latest>`_, which includes\n\ninformation for Synapse developers as well as Synapse administrators.\nDevelopers might be particularly interested in:\n\n* `Synapse\'s database schema <https://element-hq.github.io/synapse/latest/development/database_schema.html>`_,\n* `notes on Synapse\'s implementation details <https://element-hq.github.io/synapse/latest/development/internal_documentation/index.html>`_, and\n* `how we use git <https://element-hq.github.io/synapse/latest/development/git.html>`_.\n\nAlongside all that, join our developer community on Matrix:\n`#synapse-dev:matrix.org <https://matrix.to/#/#synapse-dev:matrix.org>`_, featuring real humans!\n\n\n.. |support| image:: https://img.shields.io/matrix/synapse:matrix.org?label=support&logo=matrix\n  :alt: (get support on #synapse:matrix.org)\n  :target: https://matrix.to/#/#synapse:matrix.org\n\n.. |development| image:: https://img.shields.io/matrix/synapse-dev:matrix.org?label=development&logo=matrix\n  :alt: (discuss development on #synapse-dev:matrix.org)\n  :target: https://matrix.to/#/#synapse-dev:matrix.org\n\n.. |documentation| image:: https://img.shields.io/badge/documentation-%E2%9C%93-success\n  :alt: (Rendered documentation on GitHub Pages)\n  :target: https://element-hq.github.io/synapse/latest/\n\n.. |license| image:: https://img.shields.io/github/license/element-hq/synapse\n  :alt: (check license in LICENSE file)\n  :target: LICENSE\n\n.. |pypi| image:: https://img.shields.io/pypi/v/matrix-synapse\n  :alt: (latest version released on PyPi)\n  :target: https://pypi.org/project/matrix-synapse\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/matrix-synapse\n  :alt: (supported python versions)\n  :target: https://pypi.org/project/matrix-synapse\n',
     'author': 'Matrix.org Team and Contributors',
     'author_email': 'packages@matrix.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/element-hq/synapse',
```

### Comparing `matrix_synapse-1.99.0/PKG-INFO` & `matrix_synapse-1.99.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-synapse
-Version: 1.99.0
+Version: 1.99.0rc1
 Summary: Homeserver for the Matrix decentralised comms protocol
 Home-page: https://github.com/element-hq/synapse
 License: AGPL-3.0-or-later
 Author: Matrix.org Team and Contributors
 Author-email: packages@matrix.org
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

