# Comparing `tmp/lusid_sdk-2.0.90b0.tar.gz` & `tmp/lusid_sdk-2.0.96b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_sdk-2.0.90b0.tar", max compression
+gzip compressed data, was "lusid_sdk-2.0.96b0.tar", max compression
```

## Comparing `lusid_sdk-2.0.90b0.tar` & `lusid_sdk-2.0.96b0.tar`

### file list

```diff
@@ -1,923 +1,923 @@
--rw-r--r--   0        0        0   161985 2023-11-21 05:31:44.150265 lusid_sdk-2.0.90b0/README.md
--rw-r--r--   0        0        0    66142 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/__init__.py
--rw-r--r--   0        0        0     3571 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/api/__init__.py
--rw-r--r--   0        0        0   134147 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/api/abor_api.py
--rw-r--r--   0        0        0    64035 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/abor_configuration_api.py
--rw-r--r--   0        0        0    31634 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/address_key_definition_api.py
--rw-r--r--   0        0        0    38497 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/aggregation_api.py
--rw-r--r--   0        0        0    45784 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/allocations_api.py
--rw-r--r--   0        0        0    23218 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/application_metadata_api.py
--rw-r--r--   0        0        0    43517 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/blocks_api.py
--rw-r--r--   0        0        0   128345 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/calendars_api.py
--rw-r--r--   0        0        0   275953 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/chart_of_accounts_api.py
--rw-r--r--   0        0        0    48582 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/complex_market_data_api.py
--rw-r--r--   0        0        0   113134 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/compliance_api.py
--rw-r--r--   0        0        0    37723 2023-11-21 05:31:44.098265 lusid_sdk-2.0.90b0/lusid/api/configuration_recipe_api.py
--rw-r--r--   0        0        0   106469 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/conventions_api.py
--rw-r--r--   0        0        0   101978 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/corporate_action_sources_api.py
--rw-r--r--   0        0        0    72533 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/counterparties_api.py
--rw-r--r--   0        0        0   165674 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/custom_entities_api.py
--rw-r--r--   0        0        0    40843 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/custom_entity_definitions_api.py
--rw-r--r--   0        0        0    41497 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/custom_entity_types_api.py
--rw-r--r--   0        0        0    48195 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/cut_label_definitions_api.py
--rw-r--r--   0        0        0    79757 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/data_types_api.py
--rw-r--r--   0        0        0    20221 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/derived_transaction_portfolios_api.py
--rw-r--r--   0        0        0    10437 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/entities_api.py
--rw-r--r--   0        0        0    44423 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/executions_api.py
--rw-r--r--   0        0        0     8595 2023-11-21 05:31:44.099265 lusid_sdk-2.0.90b0/lusid/api/instrument_event_types_api.py
--rw-r--r--   0        0        0    45405 2023-11-21 05:31:44.100265 lusid_sdk-2.0.90b0/lusid/api/instrument_events_api.py
--rw-r--r--   0        0        0   282424 2023-11-21 05:31:44.100265 lusid_sdk-2.0.90b0/lusid/api/instruments_api.py
--rw-r--r--   0        0        0    97260 2023-11-21 05:31:44.100265 lusid_sdk-2.0.90b0/lusid/api/legacy_compliance_api.py
--rw-r--r--   0        0        0   268136 2023-11-21 05:31:44.100265 lusid_sdk-2.0.90b0/lusid/api/legal_entities_api.py
--rw-r--r--   0        0        0    45262 2023-11-21 05:31:44.100265 lusid_sdk-2.0.90b0/lusid/api/order_graph_api.py
--rw-r--r--   0        0        0    46079 2023-11-21 05:31:44.100265 lusid_sdk-2.0.90b0/lusid/api/order_instructions_api.py
--rw-r--r--   0        0        0    19883 2023-11-21 05:31:44.101265 lusid_sdk-2.0.90b0/lusid/api/order_management_api.py
--rw-r--r--   0        0        0    44652 2023-11-21 05:31:44.101265 lusid_sdk-2.0.90b0/lusid/api/orders_api.py
--rw-r--r--   0        0        0    43973 2023-11-21 05:31:44.101265 lusid_sdk-2.0.90b0/lusid/api/packages_api.py
--rw-r--r--   0        0        0    45257 2023-11-21 05:31:44.101265 lusid_sdk-2.0.90b0/lusid/api/participations_api.py
--rw-r--r--   0        0        0   248697 2023-11-21 05:31:44.101265 lusid_sdk-2.0.90b0/lusid/api/persons_api.py
--rw-r--r--   0        0        0    44429 2023-11-21 05:31:44.101265 lusid_sdk-2.0.90b0/lusid/api/placements_api.py
--rw-r--r--   0        0        0   378941 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/portfolio_groups_api.py
--rw-r--r--   0        0        0   369304 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/portfolios_api.py
--rw-r--r--   0        0        0   121270 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/property_definitions_api.py
--rw-r--r--   0        0        0   117875 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/quotes_api.py
--rw-r--r--   0        0        0   249090 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/reconciliations_api.py
--rw-r--r--   0        0        0    39833 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/reference_lists_api.py
--rw-r--r--   0        0        0    47709 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/reference_portfolio_api.py
--rw-r--r--   0        0        0    27615 2023-11-21 05:31:44.102265 lusid_sdk-2.0.90b0/lusid/api/relation_definitions_api.py
--rw-r--r--   0        0        0    22882 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/relations_api.py
--rw-r--r--   0        0        0    54687 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/relationship_definitions_api.py
--rw-r--r--   0        0        0    19980 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/relationships_api.py
--rw-r--r--   0        0        0    31786 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/schemas_api.py
--rw-r--r--   0        0        0     9249 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/scopes_api.py
--rw-r--r--   0        0        0    83307 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/scripted_translation_api.py
--rw-r--r--   0        0        0    58527 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/search_api.py
--rw-r--r--   0        0        0    37454 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/sequences_api.py
--rw-r--r--   0        0        0   112483 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/structured_result_data_api.py
--rw-r--r--   0        0        0    62048 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/system_configuration_api.py
--rw-r--r--   0        0        0    50018 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/tax_rule_sets_api.py
--rw-r--r--   0        0        0   107950 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/transaction_configuration_api.py
--rw-r--r--   0        0        0    64506 2023-11-21 05:31:44.103265 lusid_sdk-2.0.90b0/lusid/api/transaction_fees_api.py
--rw-r--r--   0        0        0   593742 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/api/transaction_portfolios_api.py
--rw-r--r--   0        0        0    20086 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/api/translation_api.py
--rw-r--r--   0        0        0    30447 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/api_client.py
--rw-r--r--   0        0        0      852 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/api_response.py
--rw-r--r--   0        0        0    14404 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/configuration.py
--rw-r--r--   0        0        0     5326 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/exceptions.py
--rw-r--r--   0        0        0      731 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/__init__.py
--rw-r--r--   0        0        0    30391 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/api_client.py
--rw-r--r--   0        0        0     5286 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/api_client_builder.py
--rw-r--r--   0        0        0     4808 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/api_client_factory.py
--rw-r--r--   0        0        0     3974 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/api_configuration.py
--rw-r--r--   0        0        0     6830 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12698 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/rest.py
--rw-r--r--   0        0        0    11564 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/retry.py
--rw-r--r--   0        0        0     1753 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     2417 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0    62162 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/__init__.py
--rw-r--r--   0        0        0     2944 2023-11-21 05:31:44.053265 lusid_sdk-2.0.90b0/lusid/models/a2_b_breakdown.py
--rw-r--r--   0        0        0     2722 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/a2_b_category.py
--rw-r--r--   0        0        0     9734 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/a2_b_data_record.py
--rw-r--r--   0        0        0    10647 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/a2_b_movement_record.py
--rw-r--r--   0        0        0     6468 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/abor.py
--rw-r--r--   0        0        0     7321 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/abor_configuration.py
--rw-r--r--   0        0        0     4370 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/abor_configuration_properties.py
--rw-r--r--   0        0        0     6536 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/abor_configuration_request.py
--rw-r--r--   0        0        0     4239 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/abor_properties.py
--rw-r--r--   0        0        0     5421 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/abor_request.py
--rw-r--r--   0        0        0     3860 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/access_controlled_action.py
--rw-r--r--   0        0        0     4803 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/access_controlled_resource.py
--rw-r--r--   0        0        0     3445 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/access_metadata_operation.py
--rw-r--r--   0        0        0     2393 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/access_metadata_value.py
--rw-r--r--   0        0        0     4947 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/account.py
--rw-r--r--   0        0        0     4269 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/account_properties.py
--rw-r--r--   0        0        0      837 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/accounting_method.py
--rw-r--r--   0        0        0     4117 2023-11-21 05:31:44.054265 lusid_sdk-2.0.90b0/lusid/models/accounts_upsert_response.py
--rw-r--r--   0        0        0     2054 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/action_id.py
--rw-r--r--   0        0        0     2235 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/action_result_of_portfolio.py
--rw-r--r--   0        0        0     2637 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/add_business_days_to_date_request.py
--rw-r--r--   0        0        0     2010 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/add_business_days_to_date_response.py
--rw-r--r--   0        0        0     2531 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/additional_payment.py
--rw-r--r--   0        0        0     4996 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_definition.py
--rw-r--r--   0        0        0     5246 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_key_compliance_parameter.py
--rw-r--r--   0        0        0     3209 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_key_definition.py
--rw-r--r--   0        0        0     2965 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_key_filter.py
--rw-r--r--   0        0        0     3226 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_key_list.py
--rw-r--r--   0        0        0     5160 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_key_list_compliance_parameter.py
--rw-r--r--   0        0        0     3273 2023-11-21 05:31:44.055265 lusid_sdk-2.0.90b0/lusid/models/address_key_option_definition.py
--rw-r--r--   0        0        0     4384 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/adjust_holding.py
--rw-r--r--   0        0        0     5983 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/adjust_holding_for_date_request.py
--rw-r--r--   0        0        0     5694 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/adjust_holding_request.py
--rw-r--r--   0        0        0     3331 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregate_spec.py
--rw-r--r--   0        0        0     5950 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregated_return.py
--rw-r--r--   0        0        0     5493 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregated_returns_dispersion_request.py
--rw-r--r--   0        0        0     7598 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregated_returns_request.py
--rw-r--r--   0        0        0     4095 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregated_returns_response.py
--rw-r--r--   0        0        0     5338 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregated_transactions_request.py
--rw-r--r--   0        0        0     2580 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregation_context.py
--rw-r--r--   0        0        0     3187 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregation_measure_failure_detail.py
--rw-r--r--   0        0        0     1062 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregation_op.py
--rw-r--r--   0        0        0     3125 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregation_options.py
--rw-r--r--   0        0        0     8323 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregation_query.py
--rw-r--r--   0        0        0      892 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/aggregation_type.py
--rw-r--r--   0        0        0    11551 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/allocation.py
--rw-r--r--   0        0        0     9774 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/allocation_request.py
--rw-r--r--   0        0        0     3451 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/allocation_service_run_response.py
--rw-r--r--   0        0        0     2848 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/allocation_set_request.py
--rw-r--r--   0        0        0     4941 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/amortisation_event.py
--rw-r--r--   0        0        0     4344 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/annul_quotes_response.py
--rw-r--r--   0        0        0     3325 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/annul_single_structured_data_response.py
--rw-r--r--   0        0        0     4496 2023-11-21 05:31:44.056265 lusid_sdk-2.0.90b0/lusid/models/annul_structured_data_response.py
--rw-r--r--   0        0        0      793 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/asset_class.py
--rw-r--r--   0        0        0     2432 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/asset_leg.py
--rw-r--r--   0        0        0     2742 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/barrier.py
--rw-r--r--   0        0        0     5785 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/basket.py
--rw-r--r--   0        0        0     2559 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/basket_identifier.py
--rw-r--r--   0        0        0     5684 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/batch_adjust_holdings_response.py
--rw-r--r--   0        0        0     4540 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/batch_upsert_instrument_properties_response.py
--rw-r--r--   0        0        0     5800 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/batch_upsert_portfolio_transactions_response.py
--rw-r--r--   0        0        0     4421 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/batch_upsert_property_definition_properties_response.py
--rw-r--r--   0        0        0     7155 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/block.py
--rw-r--r--   0        0        0     5794 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/block_request.py
--rw-r--r--   0        0        0     2617 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/block_set_request.py
--rw-r--r--   0        0        0    11468 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bond.py
--rw-r--r--   0        0        0     4463 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bond_coupon_event.py
--rw-r--r--   0        0        0     5298 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bond_default_event.py
--rw-r--r--   0        0        0     3534 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/book_transactions_response.py
--rw-r--r--   0        0        0     4823 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bool_compliance_parameter.py
--rw-r--r--   0        0        0     5112 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bool_list_compliance_parameter.py
--rw-r--r--   0        0        0    10442 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bucketed_cash_flow_request.py
--rw-r--r--   0        0        0     5608 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bucketed_cash_flow_response.py
--rw-r--r--   0        0        0     2097 2023-11-21 05:31:44.057265 lusid_sdk-2.0.90b0/lusid/models/bucketing_schedule.py
--rw-r--r--   0        0        0     2477 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/calculation_info.py
--rw-r--r--   0        0        0     3958 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/calendar.py
--rw-r--r--   0        0        0     3685 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/calendar_date.py
--rw-r--r--   0        0        0     3868 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/calendar_dependency.py
--rw-r--r--   0        0        0     5879 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cap_floor.py
--rw-r--r--   0        0        0     4179 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_dependency.py
--rw-r--r--   0        0        0     5752 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_dividend_event.py
--rw-r--r--   0        0        0     3408 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_election.py
--rw-r--r--   0        0        0     4716 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_flow_event.py
--rw-r--r--   0        0        0     4782 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_flow_lineage.py
--rw-r--r--   0        0        0     5096 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_flow_value.py
--rw-r--r--   0        0        0     4421 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_flow_value_set.py
--rw-r--r--   0        0        0     2282 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_ladder_record.py
--rw-r--r--   0        0        0     5082 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cash_perpetual.py
--rw-r--r--   0        0        0     8026 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cds_flow_conventions.py
--rw-r--r--   0        0        0     7486 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cds_index.py
--rw-r--r--   0        0        0     3210 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/cds_protection_detail_specification.py
--rw-r--r--   0        0        0     5073 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/change.py
--rw-r--r--   0        0        0     4248 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/change_history.py
--rw-r--r--   0        0        0      702 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/change_history_action.py
--rw-r--r--   0        0        0     3834 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/change_item.py
--rw-r--r--   0        0        0     5388 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/chart_of_accounts.py
--rw-r--r--   0        0        0     4351 2023-11-21 05:31:44.058265 lusid_sdk-2.0.90b0/lusid/models/chart_of_accounts_properties.py
--rw-r--r--   0        0        0     4546 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/chart_of_accounts_request.py
--rw-r--r--   0        0        0     1977 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/client.py
--rw-r--r--   0        0        0     4143 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/close_event.py
--rw-r--r--   0        0        0     7342 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/complete_portfolio.py
--rw-r--r--   0        0        0     3905 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/complete_relation.py
--rw-r--r--   0        0        0     5165 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/complete_relationship.py
--rw-r--r--   0        0        0     9545 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/complex_bond.py
--rw-r--r--   0        0        0     5657 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/complex_market_data.py
--rw-r--r--   0        0        0     3961 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/complex_market_data_id.py
--rw-r--r--   0        0        0     2967 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_breached_order_info.py
--rw-r--r--   0        0        0     7474 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_parameter.py
--rw-r--r--   0        0        0     1934 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_parameter_type.py
--rw-r--r--   0        0        0     5578 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule.py
--rw-r--r--   0        0        0     3478 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_breakdown.py
--rw-r--r--   0        0        0     3551 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_breakdown_request.py
--rw-r--r--   0        0        0     6983 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_response.py
--rw-r--r--   0        0        0     4088 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_result.py
--rw-r--r--   0        0        0     4934 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_result_detail.py
--rw-r--r--   0        0        0     2317 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_result_portfolio_detail.py
--rw-r--r--   0        0        0     7160 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_upsert_request.py
--rw-r--r--   0        0        0     2500 2023-11-21 05:31:44.059265 lusid_sdk-2.0.90b0/lusid/models/compliance_rule_upsert_response.py
--rw-r--r--   0        0        0     3434 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_run_info.py
--rw-r--r--   0        0        0     2700 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_run_info_v2.py
--rw-r--r--   0        0        0     3175 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_run_summary.py
--rw-r--r--   0        0        0     4893 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_summary_rule_result.py
--rw-r--r--   0        0        0     5012 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_summary_rule_result_request.py
--rw-r--r--   0        0        0     4036 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_template.py
--rw-r--r--   0        0        0     2380 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_template_parameter.py
--rw-r--r--   0        0        0     4336 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compliance_template_variation.py
--rw-r--r--   0        0        0     3347 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/composite_breakdown.py
--rw-r--r--   0        0        0     5312 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/composite_breakdown_request.py
--rw-r--r--   0        0        0     3922 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/composite_breakdown_response.py
--rw-r--r--   0        0        0     5325 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/composite_dispersion.py
--rw-r--r--   0        0        0     4135 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/composite_dispersion_response.py
--rw-r--r--   0        0        0     5316 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/compounding.py
--rw-r--r--   0        0        0     6759 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/configuration_recipe.py
--rw-r--r--   0        0        0     3230 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/constituents_adjustment_header.py
--rw-r--r--   0        0        0     6832 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/contract_for_difference.py
--rw-r--r--   0        0        0     4148 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/corporate_action.py
--rw-r--r--   0        0        0     5008 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/corporate_action_source.py
--rw-r--r--   0        0        0     3505 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition.py
--rw-r--r--   0        0        0     3119 2023-11-21 05:31:44.060265 lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition_component.py
--rw-r--r--   0        0        0     2702 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition_component_request.py
--rw-r--r--   0        0        0     3526 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition_request.py
--rw-r--r--   0        0        0     4155 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/counterparty_agreement.py
--rw-r--r--   0        0        0     4206 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/counterparty_risk_information.py
--rw-r--r--   0        0        0     2823 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/counterparty_signatory.py
--rw-r--r--   0        0        0     2227 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_address_key_definition_request.py
--rw-r--r--   0        0        0     4451 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_calendar_request.py
--rw-r--r--   0        0        0     4731 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_corporate_action_source_request.py
--rw-r--r--   0        0        0     3945 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_custom_entity_type_request.py
--rw-r--r--   0        0        0     3720 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_cut_label_definition_request.py
--rw-r--r--   0        0        0     2475 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_data_map_request.py
--rw-r--r--   0        0        0     8055 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_data_type_request.py
--rw-r--r--   0        0        0     4782 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_date_request.py
--rw-r--r--   0        0        0     5849 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_derived_property_definition_request.py
--rw-r--r--   0        0        0     8927 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_derived_transaction_portfolio_request.py
--rw-r--r--   0        0        0     2361 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_portfolio_details.py
--rw-r--r--   0        0        0     6129 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_portfolio_group_request.py
--rw-r--r--   0        0        0     6840 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_property_definition_request.py
--rw-r--r--   0        0        0     3730 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_recipe_request.py
--rw-r--r--   0        0        0     6388 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_reconciliation_request.py
--rw-r--r--   0        0        0     5015 2023-11-21 05:31:44.061265 lusid_sdk-2.0.90b0/lusid/models/create_reference_portfolio_request.py
--rw-r--r--   0        0        0     4659 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_relation_definition_request.py
--rw-r--r--   0        0        0     2199 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_relation_request.py
--rw-r--r--   0        0        0     6599 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_relationship_definition_request.py
--rw-r--r--   0        0        0     4057 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_relationship_request.py
--rw-r--r--   0        0        0     4882 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_sequence_request.py
--rw-r--r--   0        0        0     3737 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_tax_rule_set_request.py
--rw-r--r--   0        0        0     8979 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_transaction_portfolio_request.py
--rw-r--r--   0        0        0     3415 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/create_unit_definition.py
--rw-r--r--   0        0        0     8080 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/credit_default_swap.py
--rw-r--r--   0        0        0     3085 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/credit_rating.py
--rw-r--r--   0        0        0     6957 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/credit_spread_curve_data.py
--rw-r--r--   0        0        0     5417 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/credit_support_annex.py
--rw-r--r--   0        0        0      772 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/criterion_type.py
--rw-r--r--   0        0        0     2274 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/currency_and_amount.py
--rw-r--r--   0        0        0     5128 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/curve_options.py
--rw-r--r--   0        0        0     5037 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custodian_account.py
--rw-r--r--   0        0        0     4360 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custodian_account_properties.py
--rw-r--r--   0        0        0     6708 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custodian_account_request.py
--rw-r--r--   0        0        0     4379 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custodian_accounts_upsert_response.py
--rw-r--r--   0        0        0     4264 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_definition.py
--rw-r--r--   0        0        0     3945 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_definition_request.py
--rw-r--r--   0        0        0     3393 2023-11-21 05:31:44.062265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_field.py
--rw-r--r--   0        0        0     3576 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_field_definition.py
--rw-r--r--   0        0        0     4566 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_id.py
--rw-r--r--   0        0        0     3673 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_request.py
--rw-r--r--   0        0        0     6025 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_response.py
--rw-r--r--   0        0        0     4222 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/custom_entity_type.py
--rw-r--r--   0        0        0     4902 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/cut_label_definition.py
--rw-r--r--   0        0        0     1892 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/cut_local_time.py
--rw-r--r--   0        0        0     5161 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_definition.py
--rw-r--r--   0        0        0     3404 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_map_key.py
--rw-r--r--   0        0        0     3634 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_mapping.py
--rw-r--r--   0        0        0     2321 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_scope.py
--rw-r--r--   0        0        0     7624 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_type.py
--rw-r--r--   0        0        0     6613 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_type_summary.py
--rw-r--r--   0        0        0      722 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/data_type_value_range.py
--rw-r--r--   0        0        0     5791 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/date_attributes.py
--rw-r--r--   0        0        0     2995 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/date_or_diary_entry.py
--rw-r--r--   0        0        0     2173 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/date_range.py
--rw-r--r--   0        0        0      730 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/date_time_comparison_type.py
--rw-r--r--   0        0        0     4870 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/date_time_compliance_parameter.py
--rw-r--r--   0        0        0     5144 2023-11-21 05:31:44.063265 lusid_sdk-2.0.90b0/lusid/models/date_time_list_compliance_parameter.py
--rw-r--r--   0        0        0      756 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/day_of_week.py
--rw-r--r--   0        0        0     4885 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/decimal_compliance_parameter.py
--rw-r--r--   0        0        0     3253 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/decimal_list.py
--rw-r--r--   0        0        0     5136 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/decimal_list_compliance_parameter.py
--rw-r--r--   0        0        0     2827 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/decorated_compliance_run_summary.py
--rw-r--r--   0        0        0     3324 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_accounts_response.py
--rw-r--r--   0        0        0     3989 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_custodian_accounts_response.py
--rw-r--r--   0        0        0     2789 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_instrument_properties_response.py
--rw-r--r--   0        0        0     3133 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_instrument_response.py
--rw-r--r--   0        0        0     3141 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_instruments_response.py
--rw-r--r--   0        0        0      632 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_modes.py
--rw-r--r--   0        0        0     2259 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_relation_request.py
--rw-r--r--   0        0        0     4131 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/delete_relationship_request.py
--rw-r--r--   0        0        0     3640 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/deleted_entity_response.py
--rw-r--r--   0        0        0     3925 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/dependency_source_filter.py
--rw-r--r--   0        0        0     2674 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/described_address_key.py
--rw-r--r--   0        0        0     2621 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/dialect.py
--rw-r--r--   0        0        0     4331 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/dialect_id.py
--rw-r--r--   0        0        0     2365 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/dialect_schema.py
--rw-r--r--   0        0        0     6714 2023-11-21 05:31:44.064265 lusid_sdk-2.0.90b0/lusid/models/diary_entry.py
--rw-r--r--   0        0        0     4505 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/diary_entry_request.py
--rw-r--r--   0        0        0     5434 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/discount_factor_curve_data.py
--rw-r--r--   0        0        0     4374 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/discounting_dependency.py
--rw-r--r--   0        0        0      734 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/discounting_method.py
--rw-r--r--   0        0        0     6093 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/economic_dependency.py
--rw-r--r--   0        0        0     1290 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/economic_dependency_type.py
--rw-r--r--   0        0        0     3048 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/economic_dependency_with_complex_market_data.py
--rw-r--r--   0        0        0     3355 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/economic_dependency_with_quote.py
--rw-r--r--   0        0        0     2222 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/election_specification.py
--rw-r--r--   0        0        0     3278 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/empty_model_options.py
--rw-r--r--   0        0        0     2624 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/entity_identifier.py
--rw-r--r--   0        0        0     5253 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity.py
--rw-r--r--   0        0        0     3721 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_all_of_identifiers.py
--rw-r--r--   0        0        0     5533 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_curve_by_prices_data.py
--rw-r--r--   0        0        0     5025 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_curve_dependency.py
--rw-r--r--   0        0        0     3780 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_model_options.py
--rw-r--r--   0        0        0     8608 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_option.py
--rw-r--r--   0        0        0     8709 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_swap.py
--rw-r--r--   0        0        0     4906 2023-11-21 05:31:44.065265 lusid_sdk-2.0.90b0/lusid/models/equity_vol_dependency.py
--rw-r--r--   0        0        0     5777 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/equity_vol_surface_data.py
--rw-r--r--   0        0        0     3276 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/error_detail.py
--rw-r--r--   0        0        0     2249 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/event_date_range.py
--rw-r--r--   0        0        0     3508 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/ex_dividend_configuration.py
--rw-r--r--   0        0        0     5899 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/exchange_traded_option.py
--rw-r--r--   0        0        0     5575 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/exchange_traded_option_contract_details.py
--rw-r--r--   0        0        0     8091 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/execution.py
--rw-r--r--   0        0        0     6717 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/execution_request.py
--rw-r--r--   0        0        0     2669 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/execution_set_request.py
--rw-r--r--   0        0        0     4954 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/exercise_event.py
--rw-r--r--   0        0        0     5604 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/exotic_instrument.py
--rw-r--r--   0        0        0     5928 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/expanded_group.py
--rw-r--r--   0        0        0     6067 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/fee_rule.py
--rw-r--r--   0        0        0     6163 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/fee_rule_upsert_request.py
--rw-r--r--   0        0        0     3141 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/fee_rule_upsert_response.py
--rw-r--r--   0        0        0     2379 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/field_definition.py
--rw-r--r--   0        0        0     4029 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/field_schema.py
--rw-r--r--   0        0        0     2207 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/field_value.py
--rw-r--r--   0        0        0     3003 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/file_response.py
--rw-r--r--   0        0        0     4930 2023-11-21 05:31:44.066265 lusid_sdk-2.0.90b0/lusid/models/filter_predicate_compliance_parameter.py
--rw-r--r--   0        0        0     6517 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/fixed_leg.py
--rw-r--r--   0        0        0     2876 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/fixed_leg_all_of_overrides.py
--rw-r--r--   0        0        0     7342 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/fixed_schedule.py
--rw-r--r--   0        0        0     8349 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/float_schedule.py
--rw-r--r--   0        0        0     7457 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/floating_leg.py
--rw-r--r--   0        0        0     2679 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/flow_convention_name.py
--rw-r--r--   0        0        0     9581 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/flow_conventions.py
--rw-r--r--   0        0        0     6488 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/forward_rate_agreement.py
--rw-r--r--   0        0        0     7283 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/funding_leg.py
--rw-r--r--   0        0        0     3597 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/funding_leg_options.py
--rw-r--r--   0        0        0     8912 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/future.py
--rw-r--r--   0        0        0     7333 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/futures_contract_details.py
--rw-r--r--   0        0        0     5211 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/fx_dependency.py
--rw-r--r--   0        0        0     7622 2023-11-21 05:31:44.067265 lusid_sdk-2.0.90b0/lusid/models/fx_forward.py
--rw-r--r--   0        0        0     7647 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forward_curve_by_quote_reference.py
--rw-r--r--   0        0        0     5670 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forward_curve_data.py
--rw-r--r--   0        0        0     4946 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forward_model_options.py
--rw-r--r--   0        0        0     5797 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forward_pips_curve_data.py
--rw-r--r--   0        0        0     7329 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forward_tenor_curve_data.py
--rw-r--r--   0        0        0     7427 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forward_tenor_pips_curve_data.py
--rw-r--r--   0        0        0     5235 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_forwards_dependency.py
--rw-r--r--   0        0        0    11748 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_option.py
--rw-r--r--   0        0        0     5098 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_rate_schedule.py
--rw-r--r--   0        0        0     6142 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_swap.py
--rw-r--r--   0        0        0     2453 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_tenor_convention.py
--rw-r--r--   0        0        0     4945 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_vol_dependency.py
--rw-r--r--   0        0        0     5744 2023-11-21 05:31:44.068265 lusid_sdk-2.0.90b0/lusid/models/fx_vol_surface_data.py
--rw-r--r--   0        0        0     2720 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/general_ledger_profile_mapping.py
--rw-r--r--   0        0        0     4777 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/general_ledger_profile_request.py
--rw-r--r--   0        0        0     6768 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/general_ledger_profile_response.py
--rw-r--r--   0        0        0     4352 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_cds_flow_conventions_response.py
--rw-r--r--   0        0        0     4937 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_complex_market_data_response.py
--rw-r--r--   0        0        0     4383 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_counterparty_agreement_response.py
--rw-r--r--   0        0        0     4356 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_credit_support_annex_response.py
--rw-r--r--   0        0        0     4829 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_data_map_response.py
--rw-r--r--   0        0        0     4315 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_flow_conventions_response.py
--rw-r--r--   0        0        0     4315 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_index_convention_response.py
--rw-r--r--   0        0        0     4939 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_instruments_response.py
--rw-r--r--   0        0        0     5745 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_quotes_response.py
--rw-r--r--   0        0        0     3276 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_recipe_response.py
--rw-r--r--   0        0        0     5655 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_reference_portfolio_constituents_response.py
--rw-r--r--   0        0        0     4973 2023-11-21 05:31:44.069265 lusid_sdk-2.0.90b0/lusid/models/get_structured_result_data_response.py
--rw-r--r--   0        0        0     4909 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/get_virtual_document_response.py
--rw-r--r--   0        0        0     3111 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/grouped_result_of_address_key.py
--rw-r--r--   0        0        0     6448 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/holding_adjustment.py
--rw-r--r--   0        0        0     6723 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/holding_adjustment_with_date.py
--rw-r--r--   0        0        0     2126 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/holding_context.py
--rw-r--r--   0        0        0     2199 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/holding_contributor.py
--rw-r--r--   0        0        0     4751 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/holdings_adjustment.py
--rw-r--r--   0        0        0     4136 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/holdings_adjustment_header.py
--rw-r--r--   0        0        0     3417 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/i_unit_definition_dto.py
--rw-r--r--   0        0        0     3155 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/id_selector_definition.py
--rw-r--r--   0        0        0     3080 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/identifier_part_schema.py
--rw-r--r--   0        0        0     5802 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/index_convention.py
--rw-r--r--   0        0        0     3789 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/index_model_options.py
--rw-r--r--   0        0        0     5040 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/index_projection_dependency.py
--rw-r--r--   0        0        0     2857 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/industry_classifier.py
--rw-r--r--   0        0        0     4256 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/inflation_fixing_dependency.py
--rw-r--r--   0        0        0     4546 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/inflation_index_conventions.py
--rw-r--r--   0        0        0     9718 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/inflation_leg.py
--rw-r--r--   0        0        0    13606 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/inflation_linked_bond.py
--rw-r--r--   0        0        0     6311 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/inflation_swap.py
--rw-r--r--   0        0        0     4288 2023-11-21 05:31:44.070265 lusid_sdk-2.0.90b0/lusid/models/informational_error_event.py
--rw-r--r--   0        0        0     5556 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/informational_event.py
--rw-r--r--   0        0        0    10446 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/inline_valuation_request.py
--rw-r--r--   0        0        0     4746 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/inline_valuations_reconciliation_request.py
--rw-r--r--   0        0        0     2222 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/input_transition.py
--rw-r--r--   0        0        0     8912 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument.py
--rw-r--r--   0        0        0     6374 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_capabilities.py
--rw-r--r--   0        0        0     5435 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_cash_flow.py
--rw-r--r--   0        0        0     4779 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_definition.py
--rw-r--r--   0        0        0     2851 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_definition_format.py
--rw-r--r--   0        0        0      682 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_delete_modes.py
--rw-r--r--   0        0        0     5250 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_event.py
--rw-r--r--   0        0        0     6113 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_event_holder.py
--rw-r--r--   0        0        0     1228 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_event_type.py
--rw-r--r--   0        0        0     2566 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_id_type_descriptor.py
--rw-r--r--   0        0        0     2217 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_id_value.py
--rw-r--r--   0        0        0     5505 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_leg.py
--rw-r--r--   0        0        0     3226 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_list.py
--rw-r--r--   0        0        0     5160 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_list_compliance_parameter.py
--rw-r--r--   0        0        0     3944 2023-11-21 05:31:44.071265 lusid_sdk-2.0.90b0/lusid/models/instrument_match.py
--rw-r--r--   0        0        0     3455 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_models.py
--rw-r--r--   0        0        0     5512 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_payment_diary.py
--rw-r--r--   0        0        0     3084 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_payment_diary_leg.py
--rw-r--r--   0        0        0     7045 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_payment_diary_row.py
--rw-r--r--   0        0        0     4299 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_properties.py
--rw-r--r--   0        0        0     2294 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_search_property.py
--rw-r--r--   0        0        0     1859 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/instrument_type.py
--rw-r--r--   0        0        0     8207 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/interest_rate_swap.py
--rw-r--r--   0        0        0     6138 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/interest_rate_swaption.py
--rw-r--r--   0        0        0     5779 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/ir_vol_cube_data.py
--rw-r--r--   0        0        0     4520 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/ir_vol_dependency.py
--rw-r--r--   0        0        0     2160 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/is_business_day_response.py
--rw-r--r--   0        0        0     3881 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/je_lines_query_parameters.py
--rw-r--r--   0        0        0    11034 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/journal_entry_line.py
--rw-r--r--   0        0        0     4644 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/journal_entry_lines_query_parameters.py
--rw-r--r--   0        0        0     1911 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/label_value_set.py
--rw-r--r--   0        0        0     9843 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/leg_definition.py
--rw-r--r--   0        0        0     8144 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/legal_entity.py
--rw-r--r--   0        0        0     2163 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/level_step.py
--rw-r--r--   0        0        0     3955 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/life_cycle_event_lineage.py
--rw-r--r--   0        0        0     4791 2023-11-21 05:31:44.072265 lusid_sdk-2.0.90b0/lusid/models/life_cycle_event_value.py
--rw-r--r--   0        0        0     2246 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/link.py
--rw-r--r--   0        0        0     3342 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/list_aggregation_reconciliation.py
--rw-r--r--   0        0        0     5409 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/list_aggregation_response.py
--rw-r--r--   0        0        0     3598 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/list_complex_market_data_with_meta_data_response.py
--rw-r--r--   0        0        0     2148 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/loan_period.py
--rw-r--r--   0        0        0     3795 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/look_up_pricing_model_options.py
--rw-r--r--   0        0        0     7221 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/lusid_instrument.py
--rw-r--r--   0        0        0     3841 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/lusid_problem_details.py
--rw-r--r--   0        0        0     9533 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/lusid_trade_ticket.py
--rw-r--r--   0        0        0     2134 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/lusid_unique_id.py
--rw-r--r--   0        0        0     4474 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3010 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/mapped_string.py
--rw-r--r--   0        0        0     4177 2023-11-21 05:31:44.073265 lusid_sdk-2.0.90b0/lusid/models/mapping.py
--rw-r--r--   0        0        0     4962 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/mapping_rule.py
--rw-r--r--   0        0        0     5693 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_context.py
--rw-r--r--   0        0        0     2511 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_context_suppliers.py
--rw-r--r--   0        0        0     9272 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_data_key_rule.py
--rw-r--r--   0        0        0     3563 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_data_options.py
--rw-r--r--   0        0        0      697 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_data_options_type.py
--rw-r--r--   0        0        0     3918 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_data_overrides.py
--rw-r--r--   0        0        0     8277 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_data_specific_rule.py
--rw-r--r--   0        0        0     1523 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_data_type.py
--rw-r--r--   0        0        0      801 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_observable_type.py
--rw-r--r--   0        0        0     6244 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_options.py
--rw-r--r--   0        0        0     3142 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/market_quote.py
--rw-r--r--   0        0        0     3565 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/match_criterion.py
--rw-r--r--   0        0        0     2184 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/metric_value.py
--rw-r--r--   0        0        0     4404 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/model_options.py
--rw-r--r--   0        0        0      991 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/model_options_type.py
--rw-r--r--   0        0        0     3382 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/model_property.py
--rw-r--r--   0        0        0     3858 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/model_schema.py
--rw-r--r--   0        0        0     4010 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/model_selection.py
--rw-r--r--   0        0        0     1181 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/movement_type.py
--rw-r--r--   0        0        0     2715 2023-11-21 05:31:44.074265 lusid_sdk-2.0.90b0/lusid/models/next_value_in_sequence_response.py
--rw-r--r--   0        0        0      772 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/numeric_comparison_type.py
--rw-r--r--   0        0        0     3775 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/opaque_dependency.py
--rw-r--r--   0        0        0     5080 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/opaque_market_data.py
--rw-r--r--   0        0        0     3380 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/opaque_model_options.py
--rw-r--r--   0        0        0     3820 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/open_event.py
--rw-r--r--   0        0        0      648 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/operand_type.py
--rw-r--r--   0        0        0     2543 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/operation.py
--rw-r--r--   0        0        0      622 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/operation_type.py
--rw-r--r--   0        0        0      797 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/operator.py
--rw-r--r--   0        0        0     2133 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/option_entry.py
--rw-r--r--   0        0        0     5340 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/optionality_schedule.py
--rw-r--r--   0        0        0     9656 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order.py
--rw-r--r--   0        0        0     2316 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_by_spec.py
--rw-r--r--   0        0        0     1976 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_flow_configuration.py
--rw-r--r--   0        0        0     4512 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block.py
--rw-r--r--   0        0        0     2175 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_allocation_detail.py
--rw-r--r--   0        0        0     2763 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_allocation_synopsis.py
--rw-r--r--   0        0        0     2167 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_execution_detail.py
--rw-r--r--   0        0        0     2749 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_execution_synopsis.py
--rw-r--r--   0        0        0     3303 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_order_detail.py
--rw-r--r--   0        0        0     2711 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_order_synopsis.py
--rw-r--r--   0        0        0     2167 2023-11-21 05:31:44.075265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_placement_detail.py
--rw-r--r--   0        0        0     2747 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_block_placement_synopsis.py
--rw-r--r--   0        0        0     5287 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement.py
--rw-r--r--   0        0        0     2207 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_allocation_detail.py
--rw-r--r--   0        0        0     2815 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_allocation_synopsis.py
--rw-r--r--   0        0        0     2239 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_child_placement_detail.py
--rw-r--r--   0        0        0     2199 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_execution_detail.py
--rw-r--r--   0        0        0     2811 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_execution_synopsis.py
--rw-r--r--   0        0        0     2167 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_order_detail.py
--rw-r--r--   0        0        0     2552 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_order_synopsis.py
--rw-r--r--   0        0        0     2827 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_placement_synopsis.py
--rw-r--r--   0        0        0     7184 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_instruction.py
--rw-r--r--   0        0        0     5506 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_instruction_request.py
--rw-r--r--   0        0        0     2761 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_instruction_set_request.py
--rw-r--r--   0        0        0     7830 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_request.py
--rw-r--r--   0        0        0     2713 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/order_set_request.py
--rw-r--r--   0        0        0     2416 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/otc_confirmation.py
--rw-r--r--   0        0        0    12843 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/output_transaction.py
--rw-r--r--   0        0        0     3982 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/output_transition.py
--rw-r--r--   0        0        0     5450 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/package.py
--rw-r--r--   0        0        0     4380 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/package_request.py
--rw-r--r--   0        0        0     2643 2023-11-21 05:31:44.076265 lusid_sdk-2.0.90b0/lusid/models/package_set_request.py
--rw-r--r--   0        0        0     4019 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_abor.py
--rw-r--r--   0        0        0     4176 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_abor_configuration.py
--rw-r--r--   0        0        0     4055 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_account.py
--rw-r--r--   0        0        0     4213 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_address_key_definition.py
--rw-r--r--   0        0        0     4091 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_allocation.py
--rw-r--r--   0        0        0     4031 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_block.py
--rw-r--r--   0        0        0     4067 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_calendar.py
--rw-r--r--   0        0        0     4153 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_chart_of_accounts.py
--rw-r--r--   0        0        0     4237 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_compliance_rule_response.py
--rw-r--r--   0        0        0     4202 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_compliance_run_info_v2.py
--rw-r--r--   0        0        0     4188 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_compliance_template.py
--rw-r--r--   0        0        0     4225 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_corporate_action_source.py
--rw-r--r--   0        0        0     4164 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custodian_account.py
--rw-r--r--   0        0        0     4237 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custom_entity_definition.py
--rw-r--r--   0        0        0     4213 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custom_entity_response.py
--rw-r--r--   0        0        0     4165 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custom_entity_type.py
--rw-r--r--   0        0        0     4189 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_cut_label_definition.py
--rw-r--r--   0        0        0     4153 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_data_type_summary.py
--rw-r--r--   0        0        0     4080 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_dialect_id.py
--rw-r--r--   0        0        0     4092 2023-11-21 05:31:44.077265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_diary_entry.py
--rw-r--r--   0        0        0     4079 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_execution.py
--rw-r--r--   0        0        0     4310 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_general_ledger_profile_response.py
--rw-r--r--   0        0        0     4091 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_instrument.py
--rw-r--r--   0        0        0     4225 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_instrument_event_holder.py
--rw-r--r--   0        0        0     4104 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_legal_entity.py
--rw-r--r--   0        0        0     4031 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order.py
--rw-r--r--   0        0        0     4153 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order_graph_block.py
--rw-r--r--   0        0        0     4201 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order_graph_placement.py
--rw-r--r--   0        0        0     4164 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order_instruction.py
--rw-r--r--   0        0        0     4055 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_package.py
--rw-r--r--   0        0        0     4127 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_participation.py
--rw-r--r--   0        0        0     4043 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_person.py
--rw-r--r--   0        0        0     4079 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_placement.py
--rw-r--r--   0        0        0     4140 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_portfolio_group.py
--rw-r--r--   0        0        0     4286 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_portfolio_group_search_result.py
--rw-r--r--   0        0        0     4225 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_portfolio_search_result.py
--rw-r--r--   0        0        0     4225 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_posting_module_response.py
--rw-r--r--   0        0        0     4177 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_posting_module_rule.py
--rw-r--r--   0        0        0     4334 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_property_definition_search_result.py
--rw-r--r--   0        0        0     4139 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reconciliation.py
--rw-r--r--   0        0        0     4176 2023-11-21 05:31:44.078265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reconciliation_run.py
--rw-r--r--   0        0        0     4237 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reconciliation_run_break.py
--rw-r--r--   0        0        0     4225 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reference_list_response.py
--rw-r--r--   0        0        0     4236 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_relationship_definition.py
--rw-r--r--   0        0        0     4188 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_sequence_definition.py
--rw-r--r--   0        0        0     4201 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_translation_script_id.py
--rw-r--r--   0        0        0     4092 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_virtual_row.py
--rw-r--r--   0        0        0     3906 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/participation.py
--rw-r--r--   0        0        0     3226 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/participation_request.py
--rw-r--r--   0        0        0     2721 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/participation_set_request.py
--rw-r--r--   0        0        0     3572 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/performance_return.py
--rw-r--r--   0        0        0     3971 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/performance_returns_metric.py
--rw-r--r--   0        0        0      711 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/period_type.py
--rw-r--r--   0        0        0      713 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/perpetual_entity_state.py
--rw-r--r--   0        0        0     2356 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/perpetual_property.py
--rw-r--r--   0        0        0     6653 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/person.py
--rw-r--r--   0        0        0     9103 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/placement.py
--rw-r--r--   0        0        0     7867 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/placement_request.py
--rw-r--r--   0        0        0     2669 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/placement_set_request.py
--rw-r--r--   0        0        0    10304 2023-11-21 05:31:44.079265 lusid_sdk-2.0.90b0/lusid/models/portfolio.py
--rw-r--r--   0        0        0     8994 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_cash_flow.py
--rw-r--r--   0        0        0     5459 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_cash_ladder.py
--rw-r--r--   0        0        0     7284 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_details.py
--rw-r--r--   0        0        0     3938 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_entity_id.py
--rw-r--r--   0        0        0     7103 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_group.py
--rw-r--r--   0        0        0     5176 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_group_id_compliance_parameter.py
--rw-r--r--   0        0        0     3697 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_group_id_list.py
--rw-r--r--   0        0        0     5208 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_group_id_list_compliance_parameter.py
--rw-r--r--   0        0        0     4340 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_group_properties.py
--rw-r--r--   0        0        0     6283 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_group_search_result.py
--rw-r--r--   0        0        0     8124 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_holding.py
--rw-r--r--   0        0        0     5136 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_id_compliance_parameter.py
--rw-r--r--   0        0        0     3657 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_id_list.py
--rw-r--r--   0        0        0     5168 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_id_list_compliance_parameter.py
--rw-r--r--   0        0        0     4289 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_properties.py
--rw-r--r--   0        0        0     2883 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_reconciliation_request.py
--rw-r--r--   0        0        0     6632 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_result_data_key_rule.py
--rw-r--r--   0        0        0     6680 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_return_breakdown.py
--rw-r--r--   0        0        0     6666 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_search_result.py
--rw-r--r--   0        0        0     2777 2023-11-21 05:31:44.080265 lusid_sdk-2.0.90b0/lusid/models/portfolio_trade_ticket.py
--rw-r--r--   0        0        0      712 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/portfolio_type.py
--rw-r--r--   0        0        0     2998 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/portfolios_reconciliation_request.py
--rw-r--r--   0        0        0     3307 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/posting_module_details.py
--rw-r--r--   0        0        0     4470 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/posting_module_request.py
--rw-r--r--   0        0        0     6101 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/posting_module_response.py
--rw-r--r--   0        0        0     3346 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/posting_module_rule.py
--rw-r--r--   0        0        0     4285 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/posting_module_rules_updated_response.py
--rw-r--r--   0        0        0     2197 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/premium.py
--rw-r--r--   0        0        0     7261 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/pricing_context.py
--rw-r--r--   0        0        0     1395 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/pricing_model.py
--rw-r--r--   0        0        0     7958 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/pricing_options.py
--rw-r--r--   0        0        0     2967 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/processed_command.py
--rw-r--r--   0        0        0    14147 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/property_definition.py
--rw-r--r--   0        0        0    12749 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/property_definition_search_result.py
--rw-r--r--   0        0        0      731 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/property_definition_type.py
--rw-r--r--   0        0        0     1984 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/property_domain.py
--rw-r--r--   0        0        0     3644 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/property_filter.py
--rw-r--r--   0        0        0     3218 2023-11-21 05:31:44.081265 lusid_sdk-2.0.90b0/lusid/models/property_interval.py
--rw-r--r--   0        0        0     4971 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_key_compliance_parameter.py
--rw-r--r--   0        0        0     5168 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_key_list_compliance_parameter.py
--rw-r--r--   0        0        0      681 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_life_time.py
--rw-r--r--   0        0        0     3589 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_schema.py
--rw-r--r--   0        0        0      729 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_type.py
--rw-r--r--   0        0        0     3119 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_value.py
--rw-r--r--   0        0        0     3440 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_value_equals.py
--rw-r--r--   0        0        0     3395 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/property_value_in.py
--rw-r--r--   0        0        0    10335 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/query_bucketed_cash_flows_request.py
--rw-r--r--   0        0        0     3983 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/query_cash_flows_request.py
--rw-r--r--   0        0        0     4966 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/query_instrument_events_request.py
--rw-r--r--   0        0        0     4064 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/query_trade_tickets_request.py
--rw-r--r--   0        0        0     4476 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote.py
--rw-r--r--   0        0        0     3176 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_access_metadata_rule.py
--rw-r--r--   0        0        0     6207 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_access_metadata_rule_id.py
--rw-r--r--   0        0        0     4592 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_dependency.py
--rw-r--r--   0        0        0     2416 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_id.py
--rw-r--r--   0        0        0      886 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_instrument_id_type.py
--rw-r--r--   0        0        0     6131 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_series_id.py
--rw-r--r--   0        0        0      958 2023-11-21 05:31:44.082265 lusid_sdk-2.0.90b0/lusid/models/quote_type.py
--rw-r--r--   0        0        0     4955 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/raw_vendor_event.py
--rw-r--r--   0        0        0     7181 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/realised_gain_loss.py
--rw-r--r--   0        0        0     4570 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconcile_date_time_rule.py
--rw-r--r--   0        0        0     4603 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconcile_numeric_rule.py
--rw-r--r--   0        0        0     5630 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconcile_string_rule.py
--rw-r--r--   0        0        0     3696 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciled_transaction.py
--rw-r--r--   0        0        0     7600 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation.py
--rw-r--r--   0        0        0     5973 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_break.py
--rw-r--r--   0        0        0     3041 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_break_id.py
--rw-r--r--   0        0        0     3033 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_configuration.py
--rw-r--r--   0        0        0     2421 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_id.py
--rw-r--r--   0        0        0     2185 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_left_right_address_key_pair.py
--rw-r--r--   0        0        0     3861 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_line.py
--rw-r--r--   0        0        0     6162 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_request.py
--rw-r--r--   0        0        0     3291 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_response.py
--rw-r--r--   0        0        0     4079 2023-11-21 05:31:44.083265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_rule.py
--rw-r--r--   0        0        0      856 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_rule_type.py
--rw-r--r--   0        0        0     3298 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_run.py
--rw-r--r--   0        0        0     4520 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_run_break.py
--rw-r--r--   0        0        0     2860 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_run_id.py
--rw-r--r--   0        0        0     3349 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_side_configuration.py
--rw-r--r--   0        0        0     2794 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reconciliation_transactions.py
--rw-r--r--   0        0        0     2924 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_data.py
--rw-r--r--   0        0        0     5187 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_instrument.py
--rw-r--r--   0        0        0     3800 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_list.py
--rw-r--r--   0        0        0     3491 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_list_request.py
--rw-r--r--   0        0        0     4556 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_list_response.py
--rw-r--r--   0        0        0      854 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_list_type.py
--rw-r--r--   0        0        0     4705 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_portfolio_constituent.py
--rw-r--r--   0        0        0     3545 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_portfolio_constituent_request.py
--rw-r--r--   0        0        0      759 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/reference_portfolio_weight_type.py
--rw-r--r--   0        0        0     5430 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/related_entity.py
--rw-r--r--   0        0        0     3415 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/relation.py
--rw-r--r--   0        0        0     6911 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/relation_definition.py
--rw-r--r--   0        0        0     4835 2023-11-21 05:31:44.084265 lusid_sdk-2.0.90b0/lusid/models/relationship.py
--rw-r--r--   0        0        0     6147 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/relationship_definition.py
--rw-r--r--   0        0        0    11222 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/repo.py
--rw-r--r--   0        0        0     5290 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/reset_event.py
--rw-r--r--   0        0        0     2061 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_id.py
--rw-r--r--   0        0        0     4221 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4392 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_access_metadata_value_of.py
--rw-r--r--   0        0        0     4173 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_address_key_definition.py
--rw-r--r--   0        0        0     4124 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_aggregated_return.py
--rw-r--r--   0        0        0     4124 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_aggregation_query.py
--rw-r--r--   0        0        0     4051 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_allocation.py
--rw-r--r--   0        0        0     3991 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_block.py
--rw-r--r--   0        0        0     4076 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_calendar_date.py
--rw-r--r--   0        0        0     4003 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_change.py
--rw-r--r--   0        0        0     4088 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_change_history.py
--rw-r--r--   0        0        0     4258 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_breached_order_info.py
--rw-r--r--   0        0        0     4100 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_rule.py
--rw-r--r--   0        0        0     4173 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_rule_result.py
--rw-r--r--   0        0        0     4137 2023-11-21 05:31:44.085265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_run_info.py
--rw-r--r--   0        0        0     4269 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_constituents_adjustment_header.py
--rw-r--r--   0        0        0     4112 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_corporate_action.py
--rw-r--r--   0        0        0     4028 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_data_type.py
--rw-r--r--   0        0        0     4039 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_execution.py
--rw-r--r--   0        0        0     4016 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_fee_rule.py
--rw-r--r--   0        0        0     4283 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_cds_flow_conventions_response.py
--rw-r--r--   0        0        0     4318 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_counterparty_agreement_response.py
--rw-r--r--   0        0        0     4283 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_credit_support_annex_response.py
--rw-r--r--   0        0        0     4246 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_flow_conventions_response.py
--rw-r--r--   0        0        0     4246 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_index_convention_response.py
--rw-r--r--   0        0        0     4137 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_recipe_response.py
--rw-r--r--   0        0        0     4221 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_holdings_adjustment_header.py
--rw-r--r--   0        0        0     4150 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_i_unit_definition_dto.py
--rw-r--r--   0        0        0     4149 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_instrument_cash_flow.py
--rw-r--r--   0        0        0     4185 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_instrument_event_holder.py
--rw-r--r--   0        0        0     4246 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_instrument_id_type_descriptor.py
--rw-r--r--   0        0        0     4064 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_legal_entity.py
--rw-r--r--   0        0        0     4430 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py
--rw-r--r--   0        0        0     4015 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_mapping.py
--rw-r--r--   0        0        0     3991 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_order.py
--rw-r--r--   0        0        0     4124 2023-11-21 05:31:44.086265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_order_instruction.py
--rw-r--r--   0        0        0     4015 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_package.py
--rw-r--r--   0        0        0     4087 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_participation.py
--rw-r--r--   0        0        0     4136 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_performance_return.py
--rw-r--r--   0        0        0     4003 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_person.py
--rw-r--r--   0        0        0     4039 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_placement.py
--rw-r--r--   0        0        0     4039 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio.py
--rw-r--r--   0        0        0     4137 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio_cash_flow.py
--rw-r--r--   0        0        0     4161 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio_cash_ladder.py
--rw-r--r--   0        0        0     4173 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio_trade_ticket.py
--rw-r--r--   0        0        0     4124 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_processed_command.py
--rw-r--r--   0        0        0     4048 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_property.py
--rw-r--r--   0        0        0     4148 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_property_definition.py
--rw-r--r--   0        0        0     4124 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_property_interval.py
--rw-r--r--   0        0        0     3991 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_quote.py
--rw-r--r--   0        0        0     4210 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_quote_access_metadata_rule.py
--rw-r--r--   0        0        0     4160 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_reconciliation_break.py
--rw-r--r--   0        0        0     4027 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_relation.py
--rw-r--r--   0        0        0     4075 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_relationship.py
--rw-r--r--   0        0        0     4112 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_scope_definition.py
--rw-r--r--   0        0        0     4100 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_side_definition.py
--rw-r--r--   0        0        0     3584 2023-11-21 05:31:44.087265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_string.py
--rw-r--r--   0        0        0     4053 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_tax_rule_set.py
--rw-r--r--   0        0        0     4063 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_transaction.py
--rw-r--r--   0        0        0     4112 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_transaction_type.py
--rw-r--r--   0        0        0     3654 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/resource_list_of_value_type.py
--rw-r--r--   0        0        0     3435 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/response_meta_data.py
--rw-r--r--   0        0        0     5431 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_data_key_rule.py
--rw-r--r--   0        0        0     5310 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_data_schema.py
--rw-r--r--   0        0        0     3629 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_key_rule.py
--rw-r--r--   0        0        0      756 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_key_rule_type.py
--rw-r--r--   0        0        0     4895 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value.py
--rw-r--r--   0        0        0     4573 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value0_d.py
--rw-r--r--   0        0        0     3675 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value_bool.py
--rw-r--r--   0        0        0     3890 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value_currency.py
--rw-r--r--   0        0        0     4269 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value_date_time_offset.py
--rw-r--r--   0        0        0     4230 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value_decimal.py
--rw-r--r--   0        0        0     4541 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value_dictionary.py
--rw-r--r--   0        0        0     4170 2023-11-21 05:31:44.088265 lusid_sdk-2.0.90b0/lusid/models/result_value_int.py
--rw-r--r--   0        0        0     3878 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/result_value_string.py
--rw-r--r--   0        0        0     1216 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/result_value_type.py
--rw-r--r--   0        0        0     2294 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/rounding_configuration.py
--rw-r--r--   0        0        0     2108 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/rounding_configuration_component.py
--rw-r--r--   0        0        0     3965 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/rounding_convention.py
--rw-r--r--   0        0        0      699 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/scaling_methodology.py
--rw-r--r--   0        0        0     3831 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/schedule.py
--rw-r--r--   0        0        0      843 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/schedule_type.py
--rw-r--r--   0        0        0     1904 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/scope_definition.py
--rw-r--r--   0        0        0     4436 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/sequence_definition.py
--rw-r--r--   0        0        0     2942 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/set_legal_entity_identifiers_request.py
--rw-r--r--   0        0        0     2980 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/set_legal_entity_properties_request.py
--rw-r--r--   0        0        0     2896 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/set_person_identifiers_request.py
--rw-r--r--   0        0        0     2694 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/set_person_properties_request.py
--rw-r--r--   0        0        0     2933 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/set_transaction_configuration_alias.py
--rw-r--r--   0        0        0     4223 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/set_transaction_configuration_source_request.py
--rw-r--r--   0        0        0     3515 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/side_configuration_data.py
--rw-r--r--   0        0        0     2839 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/side_configuration_data_request.py
--rw-r--r--   0        0        0     4447 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/side_definition.py
--rw-r--r--   0        0        0     3307 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/side_definition_request.py
--rw-r--r--   0        0        0     2744 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/sides_definition_request.py
--rw-r--r--   0        0        0     6171 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/simple_cash_flow_loan.py
--rw-r--r--   0        0        0     6677 2023-11-21 05:31:44.089265 lusid_sdk-2.0.90b0/lusid/models/simple_instrument.py
--rw-r--r--   0        0        0      644 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/sort_order.py
--rw-r--r--   0        0        0     4419 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/step_schedule.py
--rw-r--r--   0        0        0     4514 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/stock_split_event.py
--rw-r--r--   0        0        0     2862 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/stream.py
--rw-r--r--   0        0        0      799 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/string_comparison_type.py
--rw-r--r--   0        0        0     4858 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/string_compliance_parameter.py
--rw-r--r--   0        0        0     3194 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/string_list.py
--rw-r--r--   0        0        0     5128 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/string_list_compliance_parameter.py
--rw-r--r--   0        0        0     3741 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/structured_result_data.py
--rw-r--r--   0        0        0     4408 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/structured_result_data_id.py
--rw-r--r--   0        0        0     3495 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/sub_holding_key_value_equals.py
--rw-r--r--   0        0        0     4293 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/target_tax_lot.py
--rw-r--r--   0        0        0     4287 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/target_tax_lot_request.py
--rw-r--r--   0        0        0     3527 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/tax_rule.py
--rw-r--r--   0        0        0     5004 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/tax_rule_set.py
--rw-r--r--   0        0        0     2336 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/template_field.py
--rw-r--r--   0        0        0     6555 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/term_deposit.py
--rw-r--r--   0        0        0     6523 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/total_return_swap.py
--rw-r--r--   0        0        0     2723 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/touch.py
--rw-r--r--   0        0        0     2317 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/trade_ticket.py
--rw-r--r--   0        0        0      706 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/trade_ticket_type.py
--rw-r--r--   0        0        0    11574 2023-11-21 05:31:44.090265 lusid_sdk-2.0.90b0/lusid/models/transaction.py
--rw-r--r--   0        0        0     4315 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_data.py
--rw-r--r--   0        0        0     4395 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_data_request.py
--rw-r--r--   0        0        0     6931 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_movement_data.py
--rw-r--r--   0        0        0     6570 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_movement_data_request.py
--rw-r--r--   0        0        0     4747 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_type_alias.py
--rw-r--r--   0        0        0     2417 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_price.py
--rw-r--r--   0        0        0      743 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_price_type.py
--rw-r--r--   0        0        0     2819 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_property_mapping.py
--rw-r--r--   0        0        0     2874 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_property_mapping_request.py
--rw-r--r--   0        0        0      699 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_query_mode.py
--rw-r--r--   0        0        0     3362 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_query_parameters.py
--rw-r--r--   0        0        0     4291 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_reconciliation_request.py
--rw-r--r--   0        0        0     5943 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_reconciliation_request_v2.py
--rw-r--r--   0        0        0     9332 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_request.py
--rw-r--r--   0        0        0      839 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_roles.py
--rw-r--r--   0        0        0     4408 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_set_configuration_data.py
--rw-r--r--   0        0        0     3944 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_set_configuration_data_request.py
--rw-r--r--   0        0        0      700 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_status.py
--rw-r--r--   0        0        0     3807 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_template_specification.py
--rw-r--r--   0        0        0     5762 2023-11-21 05:31:44.091265 lusid_sdk-2.0.90b0/lusid/models/transaction_type.py
--rw-r--r--   0        0        0     3819 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transaction_type_alias.py
--rw-r--r--   0        0        0     2448 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transaction_type_calculation.py
--rw-r--r--   0        0        0     7321 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transaction_type_movement.py
--rw-r--r--   0        0        0     3246 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transaction_type_property_mapping.py
--rw-r--r--   0        0        0     5118 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transaction_type_request.py
--rw-r--r--   0        0        0     3080 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transactions_reconciliations_response.py
--rw-r--r--   0        0        0     6045 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/transition_event.py
--rw-r--r--   0        0        0     3573 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_entities_inlined_request.py
--rw-r--r--   0        0        0     3787 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_entities_request.py
--rw-r--r--   0        0        0     4455 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_entities_response.py
--rw-r--r--   0        0        0     3599 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_instrument_definitions_request.py
--rw-r--r--   0        0        0     5060 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_instrument_definitions_response.py
--rw-r--r--   0        0        0     3351 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_trade_ticket_request.py
--rw-r--r--   0        0        0     4981 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translate_trade_tickets_response.py
--rw-r--r--   0        0        0     2032 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translation_input.py
--rw-r--r--   0        0        0     2744 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translation_result.py
--rw-r--r--   0        0        0     2310 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translation_script.py
--rw-r--r--   0        0        0     3276 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/translation_script_id.py
--rw-r--r--   0        0        0     4246 2023-11-21 05:31:44.092265 lusid_sdk-2.0.90b0/lusid/models/trial_balance.py
--rw-r--r--   0        0        0     4019 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/trial_balance_query_parameters.py
--rw-r--r--   0        0        0     4858 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/trigger_event.py
--rw-r--r--   0        0        0     3905 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/typed_resource_id.py
--rw-r--r--   0        0        0      675 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/unit_schema.py
--rw-r--r--   0        0        0      870 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/unmatched_holding_method.py
--rw-r--r--   0        0        0     3315 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_calendar_request.py
--rw-r--r--   0        0        0     3637 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_custom_entity_definition_request.py
--rw-r--r--   0        0        0     3589 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_custom_entity_type_request.py
--rw-r--r--   0        0        0     3631 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_cut_label_definition_request.py
--rw-r--r--   0        0        0     4898 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_data_type_request.py
--rw-r--r--   0        0        0     3320 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_derived_property_definition_request.py
--rw-r--r--   0        0        0     3051 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_instrument_identifier_request.py
--rw-r--r--   0        0        0     2451 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_portfolio_group_request.py
--rw-r--r--   0        0        0     2415 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_portfolio_request.py
--rw-r--r--   0        0        0     2572 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_property_definition_request.py
--rw-r--r--   0        0        0     5898 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_reconciliation_request.py
--rw-r--r--   0        0        0     3594 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_relationship_definition_request.py
--rw-r--r--   0        0        0     3240 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_tax_rule_set_request.py
--rw-r--r--   0        0        0     3886 2023-11-21 05:31:44.093265 lusid_sdk-2.0.90b0/lusid/models/update_unit_request.py
--rw-r--r--   0        0        0     2500 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_cds_flow_conventions_request.py
--rw-r--r--   0        0        0     2827 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_complex_market_data_request.py
--rw-r--r--   0        0        0     5371 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_compliance_rule_request.py
--rw-r--r--   0        0        0     3308 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_compliance_run_summary_request.py
--rw-r--r--   0        0        0     4738 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_corporate_action_request.py
--rw-r--r--   0        0        0     4957 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_corporate_actions_response.py
--rw-r--r--   0        0        0     2545 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_counterparty_agreement_request.py
--rw-r--r--   0        0        0     2528 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_credit_support_annex_request.py
--rw-r--r--   0        0        0     4993 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_custom_entities_response.py
--rw-r--r--   0        0        0     2846 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_custom_entity_access_metadata_request.py
--rw-r--r--   0        0        0     2428 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_flow_conventions_request.py
--rw-r--r--   0        0        0     2428 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_index_convention_request.py
--rw-r--r--   0        0        0     4939 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_event_request.py
--rw-r--r--   0        0        0     4982 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_events_response.py
--rw-r--r--   0        0        0     2822 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_properties_response.py
--rw-r--r--   0        0        0     3344 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_property_request.py
--rw-r--r--   0        0        0     6086 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_instruments_response.py
--rw-r--r--   0        0        0     4946 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_legal_entities_response.py
--rw-r--r--   0        0        0     2838 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_legal_entity_access_metadata_request.py
--rw-r--r--   0        0        0     5625 2023-11-21 05:31:44.094265 lusid_sdk-2.0.90b0/lusid/models/upsert_legal_entity_request.py
--rw-r--r--   0        0        0     2792 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_person_access_metadata_request.py
--rw-r--r--   0        0        0     4275 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_person_request.py
--rw-r--r--   0        0        0     2584 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_portfolio_access_metadata_request.py
--rw-r--r--   0        0        0     2630 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_portfolio_group_access_metadata_request.py
--rw-r--r--   0        0        0     4618 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_portfolio_transactions_response.py
--rw-r--r--   0        0        0     3280 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_quote_access_metadata_rule_request.py
--rw-r--r--   0        0        0     3715 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_quote_request.py
--rw-r--r--   0        0        0     4814 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_quotes_response.py
--rw-r--r--   0        0        0     2438 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_recipe_request.py
--rw-r--r--   0        0        0     3520 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_reconciliation_break_request.py
--rw-r--r--   0        0        0     2175 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_reconciliation_run_request.py
--rw-r--r--   0        0        0     4666 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_reference_portfolio_constituents_request.py
--rw-r--r--   0        0        0     3321 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_reference_portfolio_constituents_response.py
--rw-r--r--   0        0        0     3539 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_result_values_data_request.py
--rw-r--r--   0        0        0     4604 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_returns_response.py
--rw-r--r--   0        0        0     3227 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_single_structured_data_response.py
--rw-r--r--   0        0        0     4409 2023-11-21 05:31:44.095265 lusid_sdk-2.0.90b0/lusid/models/upsert_structured_data_response.py
--rw-r--r--   0        0        0     2693 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/upsert_structured_result_data_request.py
--rw-r--r--   0        0        0     4342 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/upsert_transaction_properties_response.py
--rw-r--r--   0        0        0     2025 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/user.py
--rw-r--r--   0        0        0    10572 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/valuation_request.py
--rw-r--r--   0        0        0     5386 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/valuation_schedule.py
--rw-r--r--   0        0        0     4998 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/valuations_reconciliation_request.py
--rw-r--r--   0        0        0     1241 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/value_type.py
--rw-r--r--   0        0        0     4304 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/vendor_dependency.py
--rw-r--r--   0        0        0      812 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/vendor_library.py
--rw-r--r--   0        0        0     6260 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/vendor_model_rule.py
--rw-r--r--   0        0        0     6004 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/version.py
--rw-r--r--   0        0        0     3581 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/version_summary_dto.py
--rw-r--r--   0        0        0     4519 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_a2_b_data_record.py
--rw-r--r--   0        0        0     4567 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_a2_b_movement_record.py
--rw-r--r--   0        0        0     4577 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_holding_contributor.py
--rw-r--r--   0        0        0     4554 2023-11-21 05:31:44.096265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_journal_entry_line.py
--rw-r--r--   0        0        0     4565 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_output_transaction.py
--rw-r--r--   0        0        0     4553 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_portfolio_holding.py
--rw-r--r--   0        0        0     4492 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_transaction.py
--rw-r--r--   0        0        0     4505 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_trial_balance.py
--rw-r--r--   0        0        0     5576 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py
--rw-r--r--   0        0        0     3253 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/virtual_document.py
--rw-r--r--   0        0        0     2753 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/virtual_document_row.py
--rw-r--r--   0        0        0     3196 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/virtual_row.py
--rw-r--r--   0        0        0     1873 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/warning.py
--rw-r--r--   0        0        0     2312 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/weekend_mask.py
--rw-r--r--   0        0        0     3570 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/weighted_instrument.py
--rw-r--r--   0        0        0     2540 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/weighted_instruments.py
--rw-r--r--   0        0        0     6242 2023-11-21 05:31:44.097265 lusid_sdk-2.0.90b0/lusid/models/yield_curve_data.py
--rw-r--r--   0        0        0        0 2023-11-21 05:31:44.104265 lusid_sdk-2.0.90b0/lusid/py.typed
--rw-r--r--   0        0        0    10007 2023-11-21 05:31:44.105265 lusid_sdk-2.0.90b0/lusid/rest.py
--rw-r--r--   0        0        0      797 2023-11-21 05:31:44.151265 lusid_sdk-2.0.90b0/pyproject.toml
--rw-r--r--   0        0        0   162933 1970-01-01 00:00:00.000000 lusid_sdk-2.0.90b0/PKG-INFO
+-rw-r--r--   0        0        0   161985 2023-11-21 23:48:16.993005 lusid_sdk-2.0.96b0/README.md
+-rw-r--r--   0        0        0    66142 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/__init__.py
+-rw-r--r--   0        0        0     3571 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/__init__.py
+-rw-r--r--   0        0        0   134147 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/api/abor_api.py
+-rw-r--r--   0        0        0    64035 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/api/abor_configuration_api.py
+-rw-r--r--   0        0        0    31634 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/api/address_key_definition_api.py
+-rw-r--r--   0        0        0    38497 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/api/aggregation_api.py
+-rw-r--r--   0        0        0    45784 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/allocations_api.py
+-rw-r--r--   0        0        0    23218 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/application_metadata_api.py
+-rw-r--r--   0        0        0    43517 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/blocks_api.py
+-rw-r--r--   0        0        0   128345 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/calendars_api.py
+-rw-r--r--   0        0        0   275953 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/chart_of_accounts_api.py
+-rw-r--r--   0        0        0    48582 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/complex_market_data_api.py
+-rw-r--r--   0        0        0   113134 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/compliance_api.py
+-rw-r--r--   0        0        0    37723 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/configuration_recipe_api.py
+-rw-r--r--   0        0        0   106469 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/conventions_api.py
+-rw-r--r--   0        0        0   101978 2023-11-21 23:48:16.937005 lusid_sdk-2.0.96b0/lusid/api/corporate_action_sources_api.py
+-rw-r--r--   0        0        0    72533 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/counterparties_api.py
+-rw-r--r--   0        0        0   165674 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/custom_entities_api.py
+-rw-r--r--   0        0        0    40843 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/custom_entity_definitions_api.py
+-rw-r--r--   0        0        0    41497 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/custom_entity_types_api.py
+-rw-r--r--   0        0        0    48195 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/cut_label_definitions_api.py
+-rw-r--r--   0        0        0    79757 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/data_types_api.py
+-rw-r--r--   0        0        0    20221 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/derived_transaction_portfolios_api.py
+-rw-r--r--   0        0        0    10437 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/entities_api.py
+-rw-r--r--   0        0        0    44423 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/executions_api.py
+-rw-r--r--   0        0        0     8595 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/instrument_event_types_api.py
+-rw-r--r--   0        0        0    45405 2023-11-21 23:48:16.938005 lusid_sdk-2.0.96b0/lusid/api/instrument_events_api.py
+-rw-r--r--   0        0        0   282424 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/instruments_api.py
+-rw-r--r--   0        0        0    97260 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/legacy_compliance_api.py
+-rw-r--r--   0        0        0   268136 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/legal_entities_api.py
+-rw-r--r--   0        0        0    45262 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/order_graph_api.py
+-rw-r--r--   0        0        0    46079 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/order_instructions_api.py
+-rw-r--r--   0        0        0    19883 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/order_management_api.py
+-rw-r--r--   0        0        0    44652 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/orders_api.py
+-rw-r--r--   0        0        0    43973 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/packages_api.py
+-rw-r--r--   0        0        0    45257 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/participations_api.py
+-rw-r--r--   0        0        0   248697 2023-11-21 23:48:16.939005 lusid_sdk-2.0.96b0/lusid/api/persons_api.py
+-rw-r--r--   0        0        0    44429 2023-11-21 23:48:16.940005 lusid_sdk-2.0.96b0/lusid/api/placements_api.py
+-rw-r--r--   0        0        0   378941 2023-11-21 23:48:16.940005 lusid_sdk-2.0.96b0/lusid/api/portfolio_groups_api.py
+-rw-r--r--   0        0        0   369304 2023-11-21 23:48:16.940005 lusid_sdk-2.0.96b0/lusid/api/portfolios_api.py
+-rw-r--r--   0        0        0   121270 2023-11-21 23:48:16.940005 lusid_sdk-2.0.96b0/lusid/api/property_definitions_api.py
+-rw-r--r--   0        0        0   117875 2023-11-21 23:48:16.940005 lusid_sdk-2.0.96b0/lusid/api/quotes_api.py
+-rw-r--r--   0        0        0   249090 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/reconciliations_api.py
+-rw-r--r--   0        0        0    39833 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/reference_lists_api.py
+-rw-r--r--   0        0        0    47709 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/reference_portfolio_api.py
+-rw-r--r--   0        0        0    27615 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/relation_definitions_api.py
+-rw-r--r--   0        0        0    22882 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/relations_api.py
+-rw-r--r--   0        0        0    54687 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/relationship_definitions_api.py
+-rw-r--r--   0        0        0    19980 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/relationships_api.py
+-rw-r--r--   0        0        0    31786 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/schemas_api.py
+-rw-r--r--   0        0        0     9249 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/scopes_api.py
+-rw-r--r--   0        0        0    83307 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/scripted_translation_api.py
+-rw-r--r--   0        0        0    58527 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/search_api.py
+-rw-r--r--   0        0        0    37454 2023-11-21 23:48:16.941005 lusid_sdk-2.0.96b0/lusid/api/sequences_api.py
+-rw-r--r--   0        0        0   112483 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/structured_result_data_api.py
+-rw-r--r--   0        0        0    62048 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/system_configuration_api.py
+-rw-r--r--   0        0        0    50018 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/tax_rule_sets_api.py
+-rw-r--r--   0        0        0   107950 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/transaction_configuration_api.py
+-rw-r--r--   0        0        0    64506 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/transaction_fees_api.py
+-rw-r--r--   0        0        0   593742 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/transaction_portfolios_api.py
+-rw-r--r--   0        0        0    20086 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/api/translation_api.py
+-rw-r--r--   0        0        0    30447 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/api_client.py
+-rw-r--r--   0        0        0      852 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/api_response.py
+-rw-r--r--   0        0        0    14404 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/configuration.py
+-rw-r--r--   0        0        0     5326 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/exceptions.py
+-rw-r--r--   0        0        0      731 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/__init__.py
+-rw-r--r--   0        0        0    30391 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/api_client.py
+-rw-r--r--   0        0        0     5286 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/api_client_builder.py
+-rw-r--r--   0        0        0     4808 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     3974 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6830 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2055 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12698 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/rest.py
+-rw-r--r--   0        0        0    11564 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/extensions/retry.py
+-rw-r--r--   0        0        0     1753 2023-11-21 23:48:16.944005 lusid_sdk-2.0.96b0/lusid/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     2417 2023-11-21 23:48:16.944005 lusid_sdk-2.0.96b0/lusid/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0    62162 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/__init__.py
+-rw-r--r--   0        0        0     2944 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/a2_b_breakdown.py
+-rw-r--r--   0        0        0     2722 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/a2_b_category.py
+-rw-r--r--   0        0        0     9734 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/a2_b_data_record.py
+-rw-r--r--   0        0        0    10647 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/a2_b_movement_record.py
+-rw-r--r--   0        0        0     6468 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/abor.py
+-rw-r--r--   0        0        0     7321 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/abor_configuration.py
+-rw-r--r--   0        0        0     4370 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/abor_configuration_properties.py
+-rw-r--r--   0        0        0     6536 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/abor_configuration_request.py
+-rw-r--r--   0        0        0     4239 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/abor_properties.py
+-rw-r--r--   0        0        0     5421 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/abor_request.py
+-rw-r--r--   0        0        0     3860 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4803 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     3445 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/access_metadata_operation.py
+-rw-r--r--   0        0        0     2393 2023-11-21 23:48:16.897005 lusid_sdk-2.0.96b0/lusid/models/access_metadata_value.py
+-rw-r--r--   0        0        0     4947 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/account.py
+-rw-r--r--   0        0        0     4269 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/account_properties.py
+-rw-r--r--   0        0        0      837 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/accounting_method.py
+-rw-r--r--   0        0        0     4117 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/accounts_upsert_response.py
+-rw-r--r--   0        0        0     2054 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/action_id.py
+-rw-r--r--   0        0        0     2235 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/action_result_of_portfolio.py
+-rw-r--r--   0        0        0     2637 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/add_business_days_to_date_request.py
+-rw-r--r--   0        0        0     2010 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/add_business_days_to_date_response.py
+-rw-r--r--   0        0        0     2531 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/additional_payment.py
+-rw-r--r--   0        0        0     4996 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_definition.py
+-rw-r--r--   0        0        0     5246 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_key_compliance_parameter.py
+-rw-r--r--   0        0        0     3209 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_key_definition.py
+-rw-r--r--   0        0        0     2965 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_key_filter.py
+-rw-r--r--   0        0        0     3226 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_key_list.py
+-rw-r--r--   0        0        0     5160 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_key_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3273 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/address_key_option_definition.py
+-rw-r--r--   0        0        0     4384 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/adjust_holding.py
+-rw-r--r--   0        0        0     5983 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/adjust_holding_for_date_request.py
+-rw-r--r--   0        0        0     5694 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/adjust_holding_request.py
+-rw-r--r--   0        0        0     3331 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/aggregate_spec.py
+-rw-r--r--   0        0        0     5950 2023-11-21 23:48:16.898005 lusid_sdk-2.0.96b0/lusid/models/aggregated_return.py
+-rw-r--r--   0        0        0     5493 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregated_returns_dispersion_request.py
+-rw-r--r--   0        0        0     7598 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregated_returns_request.py
+-rw-r--r--   0        0        0     4095 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregated_returns_response.py
+-rw-r--r--   0        0        0     5338 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregated_transactions_request.py
+-rw-r--r--   0        0        0     2580 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregation_context.py
+-rw-r--r--   0        0        0     3187 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregation_measure_failure_detail.py
+-rw-r--r--   0        0        0     1062 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregation_op.py
+-rw-r--r--   0        0        0     3125 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregation_options.py
+-rw-r--r--   0        0        0     8323 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregation_query.py
+-rw-r--r--   0        0        0      892 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/aggregation_type.py
+-rw-r--r--   0        0        0    11551 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/allocation.py
+-rw-r--r--   0        0        0     9774 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/allocation_request.py
+-rw-r--r--   0        0        0     3451 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/allocation_service_run_response.py
+-rw-r--r--   0        0        0     2848 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/allocation_set_request.py
+-rw-r--r--   0        0        0     4941 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/amortisation_event.py
+-rw-r--r--   0        0        0     4344 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/annul_quotes_response.py
+-rw-r--r--   0        0        0     3325 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/annul_single_structured_data_response.py
+-rw-r--r--   0        0        0     4496 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/annul_structured_data_response.py
+-rw-r--r--   0        0        0      793 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/asset_class.py
+-rw-r--r--   0        0        0     2432 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/asset_leg.py
+-rw-r--r--   0        0        0     2742 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/barrier.py
+-rw-r--r--   0        0        0     5785 2023-11-21 23:48:16.899005 lusid_sdk-2.0.96b0/lusid/models/basket.py
+-rw-r--r--   0        0        0     2559 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/basket_identifier.py
+-rw-r--r--   0        0        0     5684 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/batch_adjust_holdings_response.py
+-rw-r--r--   0        0        0     4540 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/batch_upsert_instrument_properties_response.py
+-rw-r--r--   0        0        0     5800 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/batch_upsert_portfolio_transactions_response.py
+-rw-r--r--   0        0        0     4421 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/batch_upsert_property_definition_properties_response.py
+-rw-r--r--   0        0        0     7155 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/block.py
+-rw-r--r--   0        0        0     5794 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/block_request.py
+-rw-r--r--   0        0        0     2617 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/block_set_request.py
+-rw-r--r--   0        0        0    11468 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bond.py
+-rw-r--r--   0        0        0     4463 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bond_coupon_event.py
+-rw-r--r--   0        0        0     5298 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bond_default_event.py
+-rw-r--r--   0        0        0     3534 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/book_transactions_response.py
+-rw-r--r--   0        0        0     4823 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bool_compliance_parameter.py
+-rw-r--r--   0        0        0     5112 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bool_list_compliance_parameter.py
+-rw-r--r--   0        0        0    10442 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bucketed_cash_flow_request.py
+-rw-r--r--   0        0        0     5608 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bucketed_cash_flow_response.py
+-rw-r--r--   0        0        0     2097 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/bucketing_schedule.py
+-rw-r--r--   0        0        0     2477 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/calculation_info.py
+-rw-r--r--   0        0        0     3958 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/calendar.py
+-rw-r--r--   0        0        0     3685 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/calendar_date.py
+-rw-r--r--   0        0        0     3868 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/calendar_dependency.py
+-rw-r--r--   0        0        0     5879 2023-11-21 23:48:16.900005 lusid_sdk-2.0.96b0/lusid/models/cap_floor.py
+-rw-r--r--   0        0        0     4179 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_dependency.py
+-rw-r--r--   0        0        0     5752 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_dividend_event.py
+-rw-r--r--   0        0        0     3408 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_election.py
+-rw-r--r--   0        0        0     4716 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_flow_event.py
+-rw-r--r--   0        0        0     4782 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_flow_lineage.py
+-rw-r--r--   0        0        0     5096 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_flow_value.py
+-rw-r--r--   0        0        0     4421 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_flow_value_set.py
+-rw-r--r--   0        0        0     2282 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_ladder_record.py
+-rw-r--r--   0        0        0     5082 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cash_perpetual.py
+-rw-r--r--   0        0        0     8026 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cds_flow_conventions.py
+-rw-r--r--   0        0        0     7486 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cds_index.py
+-rw-r--r--   0        0        0     3210 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/cds_protection_detail_specification.py
+-rw-r--r--   0        0        0     5073 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/change.py
+-rw-r--r--   0        0        0     4248 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/change_history.py
+-rw-r--r--   0        0        0      702 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/change_history_action.py
+-rw-r--r--   0        0        0     3834 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/change_item.py
+-rw-r--r--   0        0        0     5388 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/chart_of_accounts.py
+-rw-r--r--   0        0        0     4351 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/chart_of_accounts_properties.py
+-rw-r--r--   0        0        0     4546 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/chart_of_accounts_request.py
+-rw-r--r--   0        0        0     1977 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/client.py
+-rw-r--r--   0        0        0     4143 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/close_event.py
+-rw-r--r--   0        0        0     7342 2023-11-21 23:48:16.901005 lusid_sdk-2.0.96b0/lusid/models/complete_portfolio.py
+-rw-r--r--   0        0        0     3905 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/complete_relation.py
+-rw-r--r--   0        0        0     5165 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/complete_relationship.py
+-rw-r--r--   0        0        0     9545 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/complex_bond.py
+-rw-r--r--   0        0        0     5657 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/complex_market_data.py
+-rw-r--r--   0        0        0     3961 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/complex_market_data_id.py
+-rw-r--r--   0        0        0     2967 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_breached_order_info.py
+-rw-r--r--   0        0        0     7474 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_parameter.py
+-rw-r--r--   0        0        0     1934 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_parameter_type.py
+-rw-r--r--   0        0        0     5578 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule.py
+-rw-r--r--   0        0        0     3478 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_breakdown.py
+-rw-r--r--   0        0        0     3551 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_breakdown_request.py
+-rw-r--r--   0        0        0     6983 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_response.py
+-rw-r--r--   0        0        0     4088 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_result.py
+-rw-r--r--   0        0        0     4934 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_result_detail.py
+-rw-r--r--   0        0        0     2317 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_result_portfolio_detail.py
+-rw-r--r--   0        0        0     7160 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_upsert_request.py
+-rw-r--r--   0        0        0     2500 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_rule_upsert_response.py
+-rw-r--r--   0        0        0     3434 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_run_info.py
+-rw-r--r--   0        0        0     2700 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_run_info_v2.py
+-rw-r--r--   0        0        0     3175 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_run_summary.py
+-rw-r--r--   0        0        0     4893 2023-11-21 23:48:16.902005 lusid_sdk-2.0.96b0/lusid/models/compliance_summary_rule_result.py
+-rw-r--r--   0        0        0     5012 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/compliance_summary_rule_result_request.py
+-rw-r--r--   0        0        0     4036 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/compliance_template.py
+-rw-r--r--   0        0        0     2380 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/compliance_template_parameter.py
+-rw-r--r--   0        0        0     4336 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/compliance_template_variation.py
+-rw-r--r--   0        0        0     3347 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/composite_breakdown.py
+-rw-r--r--   0        0        0     5312 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/composite_breakdown_request.py
+-rw-r--r--   0        0        0     3922 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/composite_breakdown_response.py
+-rw-r--r--   0        0        0     5325 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/composite_dispersion.py
+-rw-r--r--   0        0        0     4135 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/composite_dispersion_response.py
+-rw-r--r--   0        0        0     5316 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/compounding.py
+-rw-r--r--   0        0        0     6759 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/configuration_recipe.py
+-rw-r--r--   0        0        0     3230 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/constituents_adjustment_header.py
+-rw-r--r--   0        0        0     6832 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/contract_for_difference.py
+-rw-r--r--   0        0        0     4148 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/corporate_action.py
+-rw-r--r--   0        0        0     5008 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/corporate_action_source.py
+-rw-r--r--   0        0        0     3505 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition.py
+-rw-r--r--   0        0        0     3119 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition_component.py
+-rw-r--r--   0        0        0     2702 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition_component_request.py
+-rw-r--r--   0        0        0     3526 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition_request.py
+-rw-r--r--   0        0        0     4155 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/counterparty_agreement.py
+-rw-r--r--   0        0        0     4206 2023-11-21 23:48:16.903005 lusid_sdk-2.0.96b0/lusid/models/counterparty_risk_information.py
+-rw-r--r--   0        0        0     2823 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/counterparty_signatory.py
+-rw-r--r--   0        0        0     2227 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_address_key_definition_request.py
+-rw-r--r--   0        0        0     4451 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_calendar_request.py
+-rw-r--r--   0        0        0     4731 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_corporate_action_source_request.py
+-rw-r--r--   0        0        0     3945 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_custom_entity_type_request.py
+-rw-r--r--   0        0        0     3720 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_cut_label_definition_request.py
+-rw-r--r--   0        0        0     2475 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_data_map_request.py
+-rw-r--r--   0        0        0     8055 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_data_type_request.py
+-rw-r--r--   0        0        0     4782 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_date_request.py
+-rw-r--r--   0        0        0     5849 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_derived_property_definition_request.py
+-rw-r--r--   0        0        0     8927 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_derived_transaction_portfolio_request.py
+-rw-r--r--   0        0        0     2361 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_portfolio_details.py
+-rw-r--r--   0        0        0     6129 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_portfolio_group_request.py
+-rw-r--r--   0        0        0     6840 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_property_definition_request.py
+-rw-r--r--   0        0        0     3730 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_recipe_request.py
+-rw-r--r--   0        0        0     6388 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_reconciliation_request.py
+-rw-r--r--   0        0        0     5015 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_reference_portfolio_request.py
+-rw-r--r--   0        0        0     4659 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_relation_definition_request.py
+-rw-r--r--   0        0        0     2199 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_relation_request.py
+-rw-r--r--   0        0        0     6599 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_relationship_definition_request.py
+-rw-r--r--   0        0        0     4057 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_relationship_request.py
+-rw-r--r--   0        0        0     4882 2023-11-21 23:48:16.904005 lusid_sdk-2.0.96b0/lusid/models/create_sequence_request.py
+-rw-r--r--   0        0        0     3737 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/create_tax_rule_set_request.py
+-rw-r--r--   0        0        0     8979 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/create_transaction_portfolio_request.py
+-rw-r--r--   0        0        0     3415 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/create_unit_definition.py
+-rw-r--r--   0        0        0     8080 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/credit_default_swap.py
+-rw-r--r--   0        0        0     3085 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/credit_rating.py
+-rw-r--r--   0        0        0     6957 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/credit_spread_curve_data.py
+-rw-r--r--   0        0        0     5417 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/credit_support_annex.py
+-rw-r--r--   0        0        0      772 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/criterion_type.py
+-rw-r--r--   0        0        0     2274 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/currency_and_amount.py
+-rw-r--r--   0        0        0     5128 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/curve_options.py
+-rw-r--r--   0        0        0     5037 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custodian_account.py
+-rw-r--r--   0        0        0     4360 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custodian_account_properties.py
+-rw-r--r--   0        0        0     6708 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custodian_account_request.py
+-rw-r--r--   0        0        0     4379 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custodian_accounts_upsert_response.py
+-rw-r--r--   0        0        0     4264 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_definition.py
+-rw-r--r--   0        0        0     3945 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_definition_request.py
+-rw-r--r--   0        0        0     3393 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_field.py
+-rw-r--r--   0        0        0     3576 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_field_definition.py
+-rw-r--r--   0        0        0     4566 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_id.py
+-rw-r--r--   0        0        0     3673 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_request.py
+-rw-r--r--   0        0        0     6025 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_response.py
+-rw-r--r--   0        0        0     4222 2023-11-21 23:48:16.905005 lusid_sdk-2.0.96b0/lusid/models/custom_entity_type.py
+-rw-r--r--   0        0        0     4902 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/cut_label_definition.py
+-rw-r--r--   0        0        0     1892 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/cut_local_time.py
+-rw-r--r--   0        0        0     5161 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_definition.py
+-rw-r--r--   0        0        0     3404 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_map_key.py
+-rw-r--r--   0        0        0     3634 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_mapping.py
+-rw-r--r--   0        0        0     2321 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_scope.py
+-rw-r--r--   0        0        0     7624 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_type.py
+-rw-r--r--   0        0        0     6613 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_type_summary.py
+-rw-r--r--   0        0        0      722 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/data_type_value_range.py
+-rw-r--r--   0        0        0     5791 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/date_attributes.py
+-rw-r--r--   0        0        0     2995 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/date_or_diary_entry.py
+-rw-r--r--   0        0        0     2173 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/date_range.py
+-rw-r--r--   0        0        0      730 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/date_time_comparison_type.py
+-rw-r--r--   0        0        0     4870 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/date_time_compliance_parameter.py
+-rw-r--r--   0        0        0     5144 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/date_time_list_compliance_parameter.py
+-rw-r--r--   0        0        0      756 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/day_of_week.py
+-rw-r--r--   0        0        0     4885 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/decimal_compliance_parameter.py
+-rw-r--r--   0        0        0     3253 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/decimal_list.py
+-rw-r--r--   0        0        0     5136 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/decimal_list_compliance_parameter.py
+-rw-r--r--   0        0        0     2827 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/decorated_compliance_run_summary.py
+-rw-r--r--   0        0        0     3324 2023-11-21 23:48:16.906005 lusid_sdk-2.0.96b0/lusid/models/delete_accounts_response.py
+-rw-r--r--   0        0        0     3989 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_custodian_accounts_response.py
+-rw-r--r--   0        0        0     2789 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_instrument_properties_response.py
+-rw-r--r--   0        0        0     3133 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_instrument_response.py
+-rw-r--r--   0        0        0     3141 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_instruments_response.py
+-rw-r--r--   0        0        0      632 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_modes.py
+-rw-r--r--   0        0        0     2259 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_relation_request.py
+-rw-r--r--   0        0        0     4131 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/delete_relationship_request.py
+-rw-r--r--   0        0        0     3640 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     3925 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/dependency_source_filter.py
+-rw-r--r--   0        0        0     2674 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/described_address_key.py
+-rw-r--r--   0        0        0     2621 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/dialect.py
+-rw-r--r--   0        0        0     4331 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/dialect_id.py
+-rw-r--r--   0        0        0     2365 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/dialect_schema.py
+-rw-r--r--   0        0        0     6714 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/diary_entry.py
+-rw-r--r--   0        0        0     4505 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/diary_entry_request.py
+-rw-r--r--   0        0        0     5434 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/discount_factor_curve_data.py
+-rw-r--r--   0        0        0     4374 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/discounting_dependency.py
+-rw-r--r--   0        0        0      734 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/discounting_method.py
+-rw-r--r--   0        0        0     6093 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/economic_dependency.py
+-rw-r--r--   0        0        0     1290 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/economic_dependency_type.py
+-rw-r--r--   0        0        0     3048 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/economic_dependency_with_complex_market_data.py
+-rw-r--r--   0        0        0     3355 2023-11-21 23:48:16.907005 lusid_sdk-2.0.96b0/lusid/models/economic_dependency_with_quote.py
+-rw-r--r--   0        0        0     2222 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/election_specification.py
+-rw-r--r--   0        0        0     3278 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/empty_model_options.py
+-rw-r--r--   0        0        0     2624 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/entity_identifier.py
+-rw-r--r--   0        0        0     5253 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity.py
+-rw-r--r--   0        0        0     3721 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_all_of_identifiers.py
+-rw-r--r--   0        0        0     5533 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_curve_by_prices_data.py
+-rw-r--r--   0        0        0     5025 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_curve_dependency.py
+-rw-r--r--   0        0        0     3780 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_model_options.py
+-rw-r--r--   0        0        0     8608 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_option.py
+-rw-r--r--   0        0        0     8709 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_swap.py
+-rw-r--r--   0        0        0     4906 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_vol_dependency.py
+-rw-r--r--   0        0        0     5777 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/equity_vol_surface_data.py
+-rw-r--r--   0        0        0     3276 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/error_detail.py
+-rw-r--r--   0        0        0     2249 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/event_date_range.py
+-rw-r--r--   0        0        0     3508 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/ex_dividend_configuration.py
+-rw-r--r--   0        0        0     5899 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/exchange_traded_option.py
+-rw-r--r--   0        0        0     5575 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/exchange_traded_option_contract_details.py
+-rw-r--r--   0        0        0     8091 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/execution.py
+-rw-r--r--   0        0        0     6717 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/execution_request.py
+-rw-r--r--   0        0        0     2669 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/execution_set_request.py
+-rw-r--r--   0        0        0     4954 2023-11-21 23:48:16.908005 lusid_sdk-2.0.96b0/lusid/models/exercise_event.py
+-rw-r--r--   0        0        0     5604 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/exotic_instrument.py
+-rw-r--r--   0        0        0     5928 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/expanded_group.py
+-rw-r--r--   0        0        0     6067 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/fee_rule.py
+-rw-r--r--   0        0        0     6163 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/fee_rule_upsert_request.py
+-rw-r--r--   0        0        0     3141 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/fee_rule_upsert_response.py
+-rw-r--r--   0        0        0     2379 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/field_definition.py
+-rw-r--r--   0        0        0     4029 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/field_schema.py
+-rw-r--r--   0        0        0     2207 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/field_value.py
+-rw-r--r--   0        0        0     3003 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/file_response.py
+-rw-r--r--   0        0        0     4930 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/filter_predicate_compliance_parameter.py
+-rw-r--r--   0        0        0     6517 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/fixed_leg.py
+-rw-r--r--   0        0        0     2876 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/fixed_leg_all_of_overrides.py
+-rw-r--r--   0        0        0     7342 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/fixed_schedule.py
+-rw-r--r--   0        0        0     8349 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/float_schedule.py
+-rw-r--r--   0        0        0     7457 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/floating_leg.py
+-rw-r--r--   0        0        0     2679 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/flow_convention_name.py
+-rw-r--r--   0        0        0     9581 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/flow_conventions.py
+-rw-r--r--   0        0        0     6488 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/forward_rate_agreement.py
+-rw-r--r--   0        0        0     7283 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/funding_leg.py
+-rw-r--r--   0        0        0     3597 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/funding_leg_options.py
+-rw-r--r--   0        0        0     8912 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/future.py
+-rw-r--r--   0        0        0     7333 2023-11-21 23:48:16.909005 lusid_sdk-2.0.96b0/lusid/models/futures_contract_details.py
+-rw-r--r--   0        0        0     5211 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_dependency.py
+-rw-r--r--   0        0        0     7622 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward.py
+-rw-r--r--   0        0        0     7647 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward_curve_by_quote_reference.py
+-rw-r--r--   0        0        0     5670 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward_curve_data.py
+-rw-r--r--   0        0        0     4946 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward_model_options.py
+-rw-r--r--   0        0        0     5797 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward_pips_curve_data.py
+-rw-r--r--   0        0        0     7329 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward_tenor_curve_data.py
+-rw-r--r--   0        0        0     7427 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forward_tenor_pips_curve_data.py
+-rw-r--r--   0        0        0     5235 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_forwards_dependency.py
+-rw-r--r--   0        0        0    11748 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_option.py
+-rw-r--r--   0        0        0     5098 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_rate_schedule.py
+-rw-r--r--   0        0        0     6142 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_swap.py
+-rw-r--r--   0        0        0     2453 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_tenor_convention.py
+-rw-r--r--   0        0        0     4945 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_vol_dependency.py
+-rw-r--r--   0        0        0     5744 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/fx_vol_surface_data.py
+-rw-r--r--   0        0        0     2720 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/general_ledger_profile_mapping.py
+-rw-r--r--   0        0        0     4777 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/general_ledger_profile_request.py
+-rw-r--r--   0        0        0     6768 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/general_ledger_profile_response.py
+-rw-r--r--   0        0        0     4352 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/get_cds_flow_conventions_response.py
+-rw-r--r--   0        0        0     4937 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/get_complex_market_data_response.py
+-rw-r--r--   0        0        0     4383 2023-11-21 23:48:16.910005 lusid_sdk-2.0.96b0/lusid/models/get_counterparty_agreement_response.py
+-rw-r--r--   0        0        0     4356 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_credit_support_annex_response.py
+-rw-r--r--   0        0        0     4829 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_data_map_response.py
+-rw-r--r--   0        0        0     4315 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_flow_conventions_response.py
+-rw-r--r--   0        0        0     4315 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_index_convention_response.py
+-rw-r--r--   0        0        0     4939 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_instruments_response.py
+-rw-r--r--   0        0        0     5745 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_quotes_response.py
+-rw-r--r--   0        0        0     3276 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_recipe_response.py
+-rw-r--r--   0        0        0     5655 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_reference_portfolio_constituents_response.py
+-rw-r--r--   0        0        0     4973 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_structured_result_data_response.py
+-rw-r--r--   0        0        0     4909 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/get_virtual_document_response.py
+-rw-r--r--   0        0        0     3111 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/grouped_result_of_address_key.py
+-rw-r--r--   0        0        0     6448 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/holding_adjustment.py
+-rw-r--r--   0        0        0     6723 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/holding_adjustment_with_date.py
+-rw-r--r--   0        0        0     2126 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/holding_context.py
+-rw-r--r--   0        0        0     2199 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/holding_contributor.py
+-rw-r--r--   0        0        0     4751 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/holdings_adjustment.py
+-rw-r--r--   0        0        0     4136 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/holdings_adjustment_header.py
+-rw-r--r--   0        0        0     3417 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/i_unit_definition_dto.py
+-rw-r--r--   0        0        0     3155 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3080 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     5802 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/index_convention.py
+-rw-r--r--   0        0        0     3789 2023-11-21 23:48:16.911005 lusid_sdk-2.0.96b0/lusid/models/index_model_options.py
+-rw-r--r--   0        0        0     5040 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/index_projection_dependency.py
+-rw-r--r--   0        0        0     2857 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/industry_classifier.py
+-rw-r--r--   0        0        0     4256 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inflation_fixing_dependency.py
+-rw-r--r--   0        0        0     4546 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inflation_index_conventions.py
+-rw-r--r--   0        0        0     9718 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inflation_leg.py
+-rw-r--r--   0        0        0    13606 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inflation_linked_bond.py
+-rw-r--r--   0        0        0     6311 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inflation_swap.py
+-rw-r--r--   0        0        0     4288 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/informational_error_event.py
+-rw-r--r--   0        0        0     5556 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/informational_event.py
+-rw-r--r--   0        0        0    10446 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inline_valuation_request.py
+-rw-r--r--   0        0        0     4746 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/inline_valuations_reconciliation_request.py
+-rw-r--r--   0        0        0     2222 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/input_transition.py
+-rw-r--r--   0        0        0     8912 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument.py
+-rw-r--r--   0        0        0     6374 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_capabilities.py
+-rw-r--r--   0        0        0     5435 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_cash_flow.py
+-rw-r--r--   0        0        0     4779 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_definition.py
+-rw-r--r--   0        0        0     2851 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_definition_format.py
+-rw-r--r--   0        0        0      682 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_delete_modes.py
+-rw-r--r--   0        0        0     5250 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_event.py
+-rw-r--r--   0        0        0     6113 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_event_holder.py
+-rw-r--r--   0        0        0     1228 2023-11-21 23:48:16.912005 lusid_sdk-2.0.96b0/lusid/models/instrument_event_type.py
+-rw-r--r--   0        0        0     2566 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_id_type_descriptor.py
+-rw-r--r--   0        0        0     2217 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_id_value.py
+-rw-r--r--   0        0        0     5505 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_leg.py
+-rw-r--r--   0        0        0     3226 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_list.py
+-rw-r--r--   0        0        0     5160 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3944 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_match.py
+-rw-r--r--   0        0        0     3455 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_models.py
+-rw-r--r--   0        0        0     5512 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_payment_diary.py
+-rw-r--r--   0        0        0     3084 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_payment_diary_leg.py
+-rw-r--r--   0        0        0     7045 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_payment_diary_row.py
+-rw-r--r--   0        0        0     4299 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_properties.py
+-rw-r--r--   0        0        0     2294 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_search_property.py
+-rw-r--r--   0        0        0     1859 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/instrument_type.py
+-rw-r--r--   0        0        0     8207 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/interest_rate_swap.py
+-rw-r--r--   0        0        0     6138 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/interest_rate_swaption.py
+-rw-r--r--   0        0        0     5779 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/ir_vol_cube_data.py
+-rw-r--r--   0        0        0     4520 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/ir_vol_dependency.py
+-rw-r--r--   0        0        0     2160 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/is_business_day_response.py
+-rw-r--r--   0        0        0     3881 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/je_lines_query_parameters.py
+-rw-r--r--   0        0        0    11034 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/journal_entry_line.py
+-rw-r--r--   0        0        0     4644 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/journal_entry_lines_query_parameters.py
+-rw-r--r--   0        0        0     1911 2023-11-21 23:48:16.913005 lusid_sdk-2.0.96b0/lusid/models/label_value_set.py
+-rw-r--r--   0        0        0     9843 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/leg_definition.py
+-rw-r--r--   0        0        0     8144 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/legal_entity.py
+-rw-r--r--   0        0        0     2163 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/level_step.py
+-rw-r--r--   0        0        0     3955 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/life_cycle_event_lineage.py
+-rw-r--r--   0        0        0     4791 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/life_cycle_event_value.py
+-rw-r--r--   0        0        0     2246 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/link.py
+-rw-r--r--   0        0        0     3342 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/list_aggregation_reconciliation.py
+-rw-r--r--   0        0        0     5409 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/list_aggregation_response.py
+-rw-r--r--   0        0        0     3598 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/list_complex_market_data_with_meta_data_response.py
+-rw-r--r--   0        0        0     2148 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/loan_period.py
+-rw-r--r--   0        0        0     3795 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/look_up_pricing_model_options.py
+-rw-r--r--   0        0        0     7221 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/lusid_instrument.py
+-rw-r--r--   0        0        0     3841 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     9533 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/lusid_trade_ticket.py
+-rw-r--r--   0        0        0     2134 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/lusid_unique_id.py
+-rw-r--r--   0        0        0     4474 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3010 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/mapped_string.py
+-rw-r--r--   0        0        0     4177 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/mapping.py
+-rw-r--r--   0        0        0     4962 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/mapping_rule.py
+-rw-r--r--   0        0        0     5693 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/market_context.py
+-rw-r--r--   0        0        0     2511 2023-11-21 23:48:16.914005 lusid_sdk-2.0.96b0/lusid/models/market_context_suppliers.py
+-rw-r--r--   0        0        0     9272 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_data_key_rule.py
+-rw-r--r--   0        0        0     3563 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_data_options.py
+-rw-r--r--   0        0        0      697 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_data_options_type.py
+-rw-r--r--   0        0        0     3918 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_data_overrides.py
+-rw-r--r--   0        0        0     8277 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_data_specific_rule.py
+-rw-r--r--   0        0        0     1523 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_data_type.py
+-rw-r--r--   0        0        0      801 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_observable_type.py
+-rw-r--r--   0        0        0     6244 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_options.py
+-rw-r--r--   0        0        0     3142 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/market_quote.py
+-rw-r--r--   0        0        0     3565 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/match_criterion.py
+-rw-r--r--   0        0        0     2184 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/metric_value.py
+-rw-r--r--   0        0        0     4404 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/model_options.py
+-rw-r--r--   0        0        0      991 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/model_options_type.py
+-rw-r--r--   0        0        0     3382 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/model_property.py
+-rw-r--r--   0        0        0     3858 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/model_schema.py
+-rw-r--r--   0        0        0     4010 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/model_selection.py
+-rw-r--r--   0        0        0     1181 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/movement_type.py
+-rw-r--r--   0        0        0     2715 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/next_value_in_sequence_response.py
+-rw-r--r--   0        0        0      772 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/numeric_comparison_type.py
+-rw-r--r--   0        0        0     3775 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/opaque_dependency.py
+-rw-r--r--   0        0        0     5080 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/opaque_market_data.py
+-rw-r--r--   0        0        0     3380 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/opaque_model_options.py
+-rw-r--r--   0        0        0     3820 2023-11-21 23:48:16.915005 lusid_sdk-2.0.96b0/lusid/models/open_event.py
+-rw-r--r--   0        0        0      648 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/operand_type.py
+-rw-r--r--   0        0        0     2543 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/operation.py
+-rw-r--r--   0        0        0      622 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/operation_type.py
+-rw-r--r--   0        0        0      797 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/operator.py
+-rw-r--r--   0        0        0     2133 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/option_entry.py
+-rw-r--r--   0        0        0     5340 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/optionality_schedule.py
+-rw-r--r--   0        0        0     9656 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order.py
+-rw-r--r--   0        0        0     2316 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_by_spec.py
+-rw-r--r--   0        0        0     1976 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_flow_configuration.py
+-rw-r--r--   0        0        0     4512 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block.py
+-rw-r--r--   0        0        0     2175 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_allocation_detail.py
+-rw-r--r--   0        0        0     2763 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_allocation_synopsis.py
+-rw-r--r--   0        0        0     2167 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_execution_detail.py
+-rw-r--r--   0        0        0     2749 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_execution_synopsis.py
+-rw-r--r--   0        0        0     3303 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_order_detail.py
+-rw-r--r--   0        0        0     2711 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_order_synopsis.py
+-rw-r--r--   0        0        0     2167 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_placement_detail.py
+-rw-r--r--   0        0        0     2747 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_block_placement_synopsis.py
+-rw-r--r--   0        0        0     5287 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement.py
+-rw-r--r--   0        0        0     2207 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_allocation_detail.py
+-rw-r--r--   0        0        0     2815 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_allocation_synopsis.py
+-rw-r--r--   0        0        0     2239 2023-11-21 23:48:16.916005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_child_placement_detail.py
+-rw-r--r--   0        0        0     2199 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_execution_detail.py
+-rw-r--r--   0        0        0     2811 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_execution_synopsis.py
+-rw-r--r--   0        0        0     2167 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_order_detail.py
+-rw-r--r--   0        0        0     2552 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_order_synopsis.py
+-rw-r--r--   0        0        0     2827 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_placement_synopsis.py
+-rw-r--r--   0        0        0     7184 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_instruction.py
+-rw-r--r--   0        0        0     5506 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_instruction_request.py
+-rw-r--r--   0        0        0     2761 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_instruction_set_request.py
+-rw-r--r--   0        0        0     7830 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_request.py
+-rw-r--r--   0        0        0     2713 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/order_set_request.py
+-rw-r--r--   0        0        0     2416 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/otc_confirmation.py
+-rw-r--r--   0        0        0    12843 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/output_transaction.py
+-rw-r--r--   0        0        0     3982 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/output_transition.py
+-rw-r--r--   0        0        0     5450 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/package.py
+-rw-r--r--   0        0        0     4380 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/package_request.py
+-rw-r--r--   0        0        0     2643 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/package_set_request.py
+-rw-r--r--   0        0        0     4019 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_abor.py
+-rw-r--r--   0        0        0     4176 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_abor_configuration.py
+-rw-r--r--   0        0        0     4055 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_account.py
+-rw-r--r--   0        0        0     4213 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_address_key_definition.py
+-rw-r--r--   0        0        0     4091 2023-11-21 23:48:16.917005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_allocation.py
+-rw-r--r--   0        0        0     4031 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_block.py
+-rw-r--r--   0        0        0     4067 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_calendar.py
+-rw-r--r--   0        0        0     4153 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_chart_of_accounts.py
+-rw-r--r--   0        0        0     4237 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_compliance_rule_response.py
+-rw-r--r--   0        0        0     4202 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_compliance_run_info_v2.py
+-rw-r--r--   0        0        0     4188 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_compliance_template.py
+-rw-r--r--   0        0        0     4225 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_corporate_action_source.py
+-rw-r--r--   0        0        0     4164 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custodian_account.py
+-rw-r--r--   0        0        0     4237 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custom_entity_definition.py
+-rw-r--r--   0        0        0     4213 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custom_entity_response.py
+-rw-r--r--   0        0        0     4165 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custom_entity_type.py
+-rw-r--r--   0        0        0     4189 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_cut_label_definition.py
+-rw-r--r--   0        0        0     4153 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_data_type_summary.py
+-rw-r--r--   0        0        0     4080 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_dialect_id.py
+-rw-r--r--   0        0        0     4092 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_diary_entry.py
+-rw-r--r--   0        0        0     4079 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_execution.py
+-rw-r--r--   0        0        0     4310 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_general_ledger_profile_response.py
+-rw-r--r--   0        0        0     4091 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_instrument.py
+-rw-r--r--   0        0        0     4225 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_instrument_event_holder.py
+-rw-r--r--   0        0        0     4104 2023-11-21 23:48:16.918005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_legal_entity.py
+-rw-r--r--   0        0        0     4031 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order.py
+-rw-r--r--   0        0        0     4153 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order_graph_block.py
+-rw-r--r--   0        0        0     4201 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order_graph_placement.py
+-rw-r--r--   0        0        0     4164 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order_instruction.py
+-rw-r--r--   0        0        0     4055 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_package.py
+-rw-r--r--   0        0        0     4127 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_participation.py
+-rw-r--r--   0        0        0     4043 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_person.py
+-rw-r--r--   0        0        0     4079 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_placement.py
+-rw-r--r--   0        0        0     4140 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_portfolio_group.py
+-rw-r--r--   0        0        0     4286 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_portfolio_group_search_result.py
+-rw-r--r--   0        0        0     4225 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_portfolio_search_result.py
+-rw-r--r--   0        0        0     4225 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_posting_module_response.py
+-rw-r--r--   0        0        0     4177 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_posting_module_rule.py
+-rw-r--r--   0        0        0     4334 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_property_definition_search_result.py
+-rw-r--r--   0        0        0     4139 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reconciliation.py
+-rw-r--r--   0        0        0     4176 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reconciliation_run.py
+-rw-r--r--   0        0        0     4237 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reconciliation_run_break.py
+-rw-r--r--   0        0        0     4225 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reference_list_response.py
+-rw-r--r--   0        0        0     4236 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_relationship_definition.py
+-rw-r--r--   0        0        0     4188 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_sequence_definition.py
+-rw-r--r--   0        0        0     4201 2023-11-21 23:48:16.919005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_translation_script_id.py
+-rw-r--r--   0        0        0     4092 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_virtual_row.py
+-rw-r--r--   0        0        0     3906 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/participation.py
+-rw-r--r--   0        0        0     3226 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/participation_request.py
+-rw-r--r--   0        0        0     2721 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/participation_set_request.py
+-rw-r--r--   0        0        0     3572 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/performance_return.py
+-rw-r--r--   0        0        0     3971 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/performance_returns_metric.py
+-rw-r--r--   0        0        0      711 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/period_type.py
+-rw-r--r--   0        0        0      713 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/perpetual_entity_state.py
+-rw-r--r--   0        0        0     2356 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/perpetual_property.py
+-rw-r--r--   0        0        0     6653 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/person.py
+-rw-r--r--   0        0        0     9103 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/placement.py
+-rw-r--r--   0        0        0     7867 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/placement_request.py
+-rw-r--r--   0        0        0     2669 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/placement_set_request.py
+-rw-r--r--   0        0        0    10304 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio.py
+-rw-r--r--   0        0        0     8994 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_cash_flow.py
+-rw-r--r--   0        0        0     5459 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_cash_ladder.py
+-rw-r--r--   0        0        0     7284 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_details.py
+-rw-r--r--   0        0        0     3938 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_entity_id.py
+-rw-r--r--   0        0        0     7103 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_group.py
+-rw-r--r--   0        0        0     5176 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_group_id_compliance_parameter.py
+-rw-r--r--   0        0        0     3697 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_group_id_list.py
+-rw-r--r--   0        0        0     5208 2023-11-21 23:48:16.920005 lusid_sdk-2.0.96b0/lusid/models/portfolio_group_id_list_compliance_parameter.py
+-rw-r--r--   0        0        0     4340 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_group_properties.py
+-rw-r--r--   0        0        0     6283 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_group_search_result.py
+-rw-r--r--   0        0        0     8124 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_holding.py
+-rw-r--r--   0        0        0     5136 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_id_compliance_parameter.py
+-rw-r--r--   0        0        0     3657 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_id_list.py
+-rw-r--r--   0        0        0     5168 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_id_list_compliance_parameter.py
+-rw-r--r--   0        0        0     4289 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_properties.py
+-rw-r--r--   0        0        0     2883 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_reconciliation_request.py
+-rw-r--r--   0        0        0     6632 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_result_data_key_rule.py
+-rw-r--r--   0        0        0     6680 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_return_breakdown.py
+-rw-r--r--   0        0        0     6666 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_search_result.py
+-rw-r--r--   0        0        0     2777 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_trade_ticket.py
+-rw-r--r--   0        0        0      712 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolio_type.py
+-rw-r--r--   0        0        0     2998 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/portfolios_reconciliation_request.py
+-rw-r--r--   0        0        0     3307 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/posting_module_details.py
+-rw-r--r--   0        0        0     4470 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/posting_module_request.py
+-rw-r--r--   0        0        0     6101 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/posting_module_response.py
+-rw-r--r--   0        0        0     3346 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/posting_module_rule.py
+-rw-r--r--   0        0        0     4285 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/posting_module_rules_updated_response.py
+-rw-r--r--   0        0        0     2197 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/premium.py
+-rw-r--r--   0        0        0     7261 2023-11-21 23:48:16.921005 lusid_sdk-2.0.96b0/lusid/models/pricing_context.py
+-rw-r--r--   0        0        0     1395 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/pricing_model.py
+-rw-r--r--   0        0        0     7958 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/pricing_options.py
+-rw-r--r--   0        0        0     2967 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/processed_command.py
+-rw-r--r--   0        0        0    14147 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_definition.py
+-rw-r--r--   0        0        0    12749 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_definition_search_result.py
+-rw-r--r--   0        0        0      731 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_definition_type.py
+-rw-r--r--   0        0        0     1984 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_domain.py
+-rw-r--r--   0        0        0     3644 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_filter.py
+-rw-r--r--   0        0        0     3218 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_interval.py
+-rw-r--r--   0        0        0     4971 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_key_compliance_parameter.py
+-rw-r--r--   0        0        0     5168 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_key_list_compliance_parameter.py
+-rw-r--r--   0        0        0      681 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_life_time.py
+-rw-r--r--   0        0        0     3589 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_schema.py
+-rw-r--r--   0        0        0      729 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_type.py
+-rw-r--r--   0        0        0     3119 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_value.py
+-rw-r--r--   0        0        0     3440 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_value_equals.py
+-rw-r--r--   0        0        0     3395 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/property_value_in.py
+-rw-r--r--   0        0        0    10335 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/query_bucketed_cash_flows_request.py
+-rw-r--r--   0        0        0     3983 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/query_cash_flows_request.py
+-rw-r--r--   0        0        0     4966 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/query_instrument_events_request.py
+-rw-r--r--   0        0        0     4064 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/query_trade_tickets_request.py
+-rw-r--r--   0        0        0     4476 2023-11-21 23:48:16.922005 lusid_sdk-2.0.96b0/lusid/models/quote.py
+-rw-r--r--   0        0        0     3176 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_access_metadata_rule.py
+-rw-r--r--   0        0        0     6207 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_access_metadata_rule_id.py
+-rw-r--r--   0        0        0     4592 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_dependency.py
+-rw-r--r--   0        0        0     2416 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_id.py
+-rw-r--r--   0        0        0      886 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_instrument_id_type.py
+-rw-r--r--   0        0        0     6131 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_series_id.py
+-rw-r--r--   0        0        0      958 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/quote_type.py
+-rw-r--r--   0        0        0     4955 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/raw_vendor_event.py
+-rw-r--r--   0        0        0     7181 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/realised_gain_loss.py
+-rw-r--r--   0        0        0     4570 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconcile_date_time_rule.py
+-rw-r--r--   0        0        0     4603 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconcile_numeric_rule.py
+-rw-r--r--   0        0        0     5630 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconcile_string_rule.py
+-rw-r--r--   0        0        0     3696 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciled_transaction.py
+-rw-r--r--   0        0        0     7600 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation.py
+-rw-r--r--   0        0        0     5973 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_break.py
+-rw-r--r--   0        0        0     3041 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_break_id.py
+-rw-r--r--   0        0        0     3033 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_configuration.py
+-rw-r--r--   0        0        0     2421 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_id.py
+-rw-r--r--   0        0        0     2185 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_left_right_address_key_pair.py
+-rw-r--r--   0        0        0     3861 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_line.py
+-rw-r--r--   0        0        0     6162 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_request.py
+-rw-r--r--   0        0        0     3291 2023-11-21 23:48:16.923005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_response.py
+-rw-r--r--   0        0        0     4079 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_rule.py
+-rw-r--r--   0        0        0      856 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_rule_type.py
+-rw-r--r--   0        0        0     3298 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_run.py
+-rw-r--r--   0        0        0     4520 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_run_break.py
+-rw-r--r--   0        0        0     2860 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_run_id.py
+-rw-r--r--   0        0        0     3349 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_side_configuration.py
+-rw-r--r--   0        0        0     2794 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reconciliation_transactions.py
+-rw-r--r--   0        0        0     2924 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_data.py
+-rw-r--r--   0        0        0     5187 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_instrument.py
+-rw-r--r--   0        0        0     3800 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_list.py
+-rw-r--r--   0        0        0     3491 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_list_request.py
+-rw-r--r--   0        0        0     4556 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_list_response.py
+-rw-r--r--   0        0        0      854 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_list_type.py
+-rw-r--r--   0        0        0     4705 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_portfolio_constituent.py
+-rw-r--r--   0        0        0     3545 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_portfolio_constituent_request.py
+-rw-r--r--   0        0        0      759 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/reference_portfolio_weight_type.py
+-rw-r--r--   0        0        0     5430 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/related_entity.py
+-rw-r--r--   0        0        0     3415 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/relation.py
+-rw-r--r--   0        0        0     6911 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/relation_definition.py
+-rw-r--r--   0        0        0     4835 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/relationship.py
+-rw-r--r--   0        0        0     6147 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/relationship_definition.py
+-rw-r--r--   0        0        0    11222 2023-11-21 23:48:16.924005 lusid_sdk-2.0.96b0/lusid/models/repo.py
+-rw-r--r--   0        0        0     5290 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/reset_event.py
+-rw-r--r--   0        0        0     2061 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_id.py
+-rw-r--r--   0        0        0     4221 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4392 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_access_metadata_value_of.py
+-rw-r--r--   0        0        0     4173 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_address_key_definition.py
+-rw-r--r--   0        0        0     4124 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_aggregated_return.py
+-rw-r--r--   0        0        0     4124 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_aggregation_query.py
+-rw-r--r--   0        0        0     4051 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_allocation.py
+-rw-r--r--   0        0        0     3991 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_block.py
+-rw-r--r--   0        0        0     4076 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_calendar_date.py
+-rw-r--r--   0        0        0     4003 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_change.py
+-rw-r--r--   0        0        0     4088 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_change_history.py
+-rw-r--r--   0        0        0     4258 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_breached_order_info.py
+-rw-r--r--   0        0        0     4100 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_rule.py
+-rw-r--r--   0        0        0     4173 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_rule_result.py
+-rw-r--r--   0        0        0     4137 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_run_info.py
+-rw-r--r--   0        0        0     4269 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_constituents_adjustment_header.py
+-rw-r--r--   0        0        0     4112 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_corporate_action.py
+-rw-r--r--   0        0        0     4028 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_data_type.py
+-rw-r--r--   0        0        0     4039 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_execution.py
+-rw-r--r--   0        0        0     4016 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_fee_rule.py
+-rw-r--r--   0        0        0     4283 2023-11-21 23:48:16.925005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_cds_flow_conventions_response.py
+-rw-r--r--   0        0        0     4318 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_counterparty_agreement_response.py
+-rw-r--r--   0        0        0     4283 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_credit_support_annex_response.py
+-rw-r--r--   0        0        0     4246 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_flow_conventions_response.py
+-rw-r--r--   0        0        0     4246 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_index_convention_response.py
+-rw-r--r--   0        0        0     4137 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_recipe_response.py
+-rw-r--r--   0        0        0     4221 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_holdings_adjustment_header.py
+-rw-r--r--   0        0        0     4150 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_i_unit_definition_dto.py
+-rw-r--r--   0        0        0     4149 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_instrument_cash_flow.py
+-rw-r--r--   0        0        0     4185 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_instrument_event_holder.py
+-rw-r--r--   0        0        0     4246 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_instrument_id_type_descriptor.py
+-rw-r--r--   0        0        0     4064 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_legal_entity.py
+-rw-r--r--   0        0        0     4430 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py
+-rw-r--r--   0        0        0     4015 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_mapping.py
+-rw-r--r--   0        0        0     3991 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_order.py
+-rw-r--r--   0        0        0     4124 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_order_instruction.py
+-rw-r--r--   0        0        0     4015 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_package.py
+-rw-r--r--   0        0        0     4087 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_participation.py
+-rw-r--r--   0        0        0     4136 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_performance_return.py
+-rw-r--r--   0        0        0     4003 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_person.py
+-rw-r--r--   0        0        0     4039 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_placement.py
+-rw-r--r--   0        0        0     4039 2023-11-21 23:48:16.926005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio.py
+-rw-r--r--   0        0        0     4137 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio_cash_flow.py
+-rw-r--r--   0        0        0     4161 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio_cash_ladder.py
+-rw-r--r--   0        0        0     4173 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio_trade_ticket.py
+-rw-r--r--   0        0        0     4124 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_processed_command.py
+-rw-r--r--   0        0        0     4048 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_property.py
+-rw-r--r--   0        0        0     4148 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_property_definition.py
+-rw-r--r--   0        0        0     4124 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_property_interval.py
+-rw-r--r--   0        0        0     3991 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_quote.py
+-rw-r--r--   0        0        0     4210 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_quote_access_metadata_rule.py
+-rw-r--r--   0        0        0     4160 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_reconciliation_break.py
+-rw-r--r--   0        0        0     4027 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_relation.py
+-rw-r--r--   0        0        0     4075 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_relationship.py
+-rw-r--r--   0        0        0     4112 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_scope_definition.py
+-rw-r--r--   0        0        0     4100 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_side_definition.py
+-rw-r--r--   0        0        0     3584 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_string.py
+-rw-r--r--   0        0        0     4053 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_tax_rule_set.py
+-rw-r--r--   0        0        0     4063 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_transaction.py
+-rw-r--r--   0        0        0     4112 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_transaction_type.py
+-rw-r--r--   0        0        0     3654 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/resource_list_of_value_type.py
+-rw-r--r--   0        0        0     3435 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/response_meta_data.py
+-rw-r--r--   0        0        0     5431 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/result_data_key_rule.py
+-rw-r--r--   0        0        0     5310 2023-11-21 23:48:16.927005 lusid_sdk-2.0.96b0/lusid/models/result_data_schema.py
+-rw-r--r--   0        0        0     3629 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_key_rule.py
+-rw-r--r--   0        0        0      756 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_key_rule_type.py
+-rw-r--r--   0        0        0     4895 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value.py
+-rw-r--r--   0        0        0     4573 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value0_d.py
+-rw-r--r--   0        0        0     3675 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_bool.py
+-rw-r--r--   0        0        0     3890 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_currency.py
+-rw-r--r--   0        0        0     4269 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_date_time_offset.py
+-rw-r--r--   0        0        0     4230 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_decimal.py
+-rw-r--r--   0        0        0     4541 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_dictionary.py
+-rw-r--r--   0        0        0     4170 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_int.py
+-rw-r--r--   0        0        0     3878 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_string.py
+-rw-r--r--   0        0        0     1216 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/result_value_type.py
+-rw-r--r--   0        0        0     2294 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/rounding_configuration.py
+-rw-r--r--   0        0        0     2108 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/rounding_configuration_component.py
+-rw-r--r--   0        0        0     3965 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/rounding_convention.py
+-rw-r--r--   0        0        0      699 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/scaling_methodology.py
+-rw-r--r--   0        0        0     3831 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/schedule.py
+-rw-r--r--   0        0        0      843 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/schedule_type.py
+-rw-r--r--   0        0        0     1904 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/scope_definition.py
+-rw-r--r--   0        0        0     4436 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/sequence_definition.py
+-rw-r--r--   0        0        0     2942 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/set_legal_entity_identifiers_request.py
+-rw-r--r--   0        0        0     2980 2023-11-21 23:48:16.928005 lusid_sdk-2.0.96b0/lusid/models/set_legal_entity_properties_request.py
+-rw-r--r--   0        0        0     2896 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/set_person_identifiers_request.py
+-rw-r--r--   0        0        0     2694 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/set_person_properties_request.py
+-rw-r--r--   0        0        0     2933 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/set_transaction_configuration_alias.py
+-rw-r--r--   0        0        0     4223 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/set_transaction_configuration_source_request.py
+-rw-r--r--   0        0        0     3515 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/side_configuration_data.py
+-rw-r--r--   0        0        0     2839 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/side_configuration_data_request.py
+-rw-r--r--   0        0        0     4447 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/side_definition.py
+-rw-r--r--   0        0        0     3307 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/side_definition_request.py
+-rw-r--r--   0        0        0     2744 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/sides_definition_request.py
+-rw-r--r--   0        0        0     6171 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/simple_cash_flow_loan.py
+-rw-r--r--   0        0        0     6677 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/simple_instrument.py
+-rw-r--r--   0        0        0      644 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/sort_order.py
+-rw-r--r--   0        0        0     4419 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/step_schedule.py
+-rw-r--r--   0        0        0     4514 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/stock_split_event.py
+-rw-r--r--   0        0        0     2862 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/stream.py
+-rw-r--r--   0        0        0      799 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/string_comparison_type.py
+-rw-r--r--   0        0        0     4858 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/string_compliance_parameter.py
+-rw-r--r--   0        0        0     3194 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/string_list.py
+-rw-r--r--   0        0        0     5128 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/string_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3741 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/structured_result_data.py
+-rw-r--r--   0        0        0     4408 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/structured_result_data_id.py
+-rw-r--r--   0        0        0     3495 2023-11-21 23:48:16.929005 lusid_sdk-2.0.96b0/lusid/models/sub_holding_key_value_equals.py
+-rw-r--r--   0        0        0     4293 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/target_tax_lot.py
+-rw-r--r--   0        0        0     4287 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/target_tax_lot_request.py
+-rw-r--r--   0        0        0     3527 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/tax_rule.py
+-rw-r--r--   0        0        0     5004 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/tax_rule_set.py
+-rw-r--r--   0        0        0     2336 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/template_field.py
+-rw-r--r--   0        0        0     6555 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/term_deposit.py
+-rw-r--r--   0        0        0     6523 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/total_return_swap.py
+-rw-r--r--   0        0        0     2723 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/touch.py
+-rw-r--r--   0        0        0     2317 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/trade_ticket.py
+-rw-r--r--   0        0        0      706 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/trade_ticket_type.py
+-rw-r--r--   0        0        0    11574 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction.py
+-rw-r--r--   0        0        0     4315 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_data.py
+-rw-r--r--   0        0        0     4395 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_data_request.py
+-rw-r--r--   0        0        0     6931 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_movement_data.py
+-rw-r--r--   0        0        0     6570 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_movement_data_request.py
+-rw-r--r--   0        0        0     4747 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_type_alias.py
+-rw-r--r--   0        0        0     2417 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_price.py
+-rw-r--r--   0        0        0      743 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_price_type.py
+-rw-r--r--   0        0        0     2819 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_property_mapping.py
+-rw-r--r--   0        0        0     2874 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_property_mapping_request.py
+-rw-r--r--   0        0        0      699 2023-11-21 23:48:16.930005 lusid_sdk-2.0.96b0/lusid/models/transaction_query_mode.py
+-rw-r--r--   0        0        0     3362 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_query_parameters.py
+-rw-r--r--   0        0        0     4291 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_reconciliation_request.py
+-rw-r--r--   0        0        0     5943 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_reconciliation_request_v2.py
+-rw-r--r--   0        0        0     9332 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_request.py
+-rw-r--r--   0        0        0      839 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_roles.py
+-rw-r--r--   0        0        0     4408 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_set_configuration_data.py
+-rw-r--r--   0        0        0     3944 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_set_configuration_data_request.py
+-rw-r--r--   0        0        0      700 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_status.py
+-rw-r--r--   0        0        0     3807 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_template_specification.py
+-rw-r--r--   0        0        0     5762 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_type.py
+-rw-r--r--   0        0        0     3819 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_type_alias.py
+-rw-r--r--   0        0        0     2448 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_type_calculation.py
+-rw-r--r--   0        0        0     7321 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_type_movement.py
+-rw-r--r--   0        0        0     3246 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_type_property_mapping.py
+-rw-r--r--   0        0        0     5118 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transaction_type_request.py
+-rw-r--r--   0        0        0     3080 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transactions_reconciliations_response.py
+-rw-r--r--   0        0        0     6045 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/transition_event.py
+-rw-r--r--   0        0        0     3573 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/translate_entities_inlined_request.py
+-rw-r--r--   0        0        0     3787 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/translate_entities_request.py
+-rw-r--r--   0        0        0     4455 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/translate_entities_response.py
+-rw-r--r--   0        0        0     3599 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/translate_instrument_definitions_request.py
+-rw-r--r--   0        0        0     5060 2023-11-21 23:48:16.931005 lusid_sdk-2.0.96b0/lusid/models/translate_instrument_definitions_response.py
+-rw-r--r--   0        0        0     3351 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/translate_trade_ticket_request.py
+-rw-r--r--   0        0        0     4981 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/translate_trade_tickets_response.py
+-rw-r--r--   0        0        0     2032 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/translation_input.py
+-rw-r--r--   0        0        0     2744 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/translation_result.py
+-rw-r--r--   0        0        0     2310 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/translation_script.py
+-rw-r--r--   0        0        0     3276 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/translation_script_id.py
+-rw-r--r--   0        0        0     4246 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/trial_balance.py
+-rw-r--r--   0        0        0     4019 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/trial_balance_query_parameters.py
+-rw-r--r--   0        0        0     4858 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/trigger_event.py
+-rw-r--r--   0        0        0     3905 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/typed_resource_id.py
+-rw-r--r--   0        0        0      675 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/unit_schema.py
+-rw-r--r--   0        0        0      870 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/unmatched_holding_method.py
+-rw-r--r--   0        0        0     3315 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_calendar_request.py
+-rw-r--r--   0        0        0     3637 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_custom_entity_definition_request.py
+-rw-r--r--   0        0        0     3589 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_custom_entity_type_request.py
+-rw-r--r--   0        0        0     3631 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_cut_label_definition_request.py
+-rw-r--r--   0        0        0     4898 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_data_type_request.py
+-rw-r--r--   0        0        0     3320 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_derived_property_definition_request.py
+-rw-r--r--   0        0        0     3051 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_instrument_identifier_request.py
+-rw-r--r--   0        0        0     2451 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_portfolio_group_request.py
+-rw-r--r--   0        0        0     2415 2023-11-21 23:48:16.932005 lusid_sdk-2.0.96b0/lusid/models/update_portfolio_request.py
+-rw-r--r--   0        0        0     2572 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/update_property_definition_request.py
+-rw-r--r--   0        0        0     5898 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/update_reconciliation_request.py
+-rw-r--r--   0        0        0     3594 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/update_relationship_definition_request.py
+-rw-r--r--   0        0        0     3240 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/update_tax_rule_set_request.py
+-rw-r--r--   0        0        0     3886 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/update_unit_request.py
+-rw-r--r--   0        0        0     2500 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_cds_flow_conventions_request.py
+-rw-r--r--   0        0        0     2827 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_complex_market_data_request.py
+-rw-r--r--   0        0        0     5371 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_compliance_rule_request.py
+-rw-r--r--   0        0        0     3308 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_compliance_run_summary_request.py
+-rw-r--r--   0        0        0     4738 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_corporate_action_request.py
+-rw-r--r--   0        0        0     4957 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_corporate_actions_response.py
+-rw-r--r--   0        0        0     2545 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_counterparty_agreement_request.py
+-rw-r--r--   0        0        0     2528 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_credit_support_annex_request.py
+-rw-r--r--   0        0        0     4993 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_custom_entities_response.py
+-rw-r--r--   0        0        0     2846 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_custom_entity_access_metadata_request.py
+-rw-r--r--   0        0        0     2428 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_flow_conventions_request.py
+-rw-r--r--   0        0        0     2428 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_index_convention_request.py
+-rw-r--r--   0        0        0     4939 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_event_request.py
+-rw-r--r--   0        0        0     4982 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_events_response.py
+-rw-r--r--   0        0        0     2822 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_properties_response.py
+-rw-r--r--   0        0        0     3344 2023-11-21 23:48:16.933005 lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_property_request.py
+-rw-r--r--   0        0        0     6086 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_instruments_response.py
+-rw-r--r--   0        0        0     4946 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_legal_entities_response.py
+-rw-r--r--   0        0        0     2838 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_legal_entity_access_metadata_request.py
+-rw-r--r--   0        0        0     5625 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_legal_entity_request.py
+-rw-r--r--   0        0        0     2792 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_person_access_metadata_request.py
+-rw-r--r--   0        0        0     4275 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_person_request.py
+-rw-r--r--   0        0        0     2584 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_portfolio_access_metadata_request.py
+-rw-r--r--   0        0        0     2630 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_portfolio_group_access_metadata_request.py
+-rw-r--r--   0        0        0     4618 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_portfolio_transactions_response.py
+-rw-r--r--   0        0        0     3280 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_quote_access_metadata_rule_request.py
+-rw-r--r--   0        0        0     3715 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_quote_request.py
+-rw-r--r--   0        0        0     4814 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_quotes_response.py
+-rw-r--r--   0        0        0     2438 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_recipe_request.py
+-rw-r--r--   0        0        0     3520 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_reconciliation_break_request.py
+-rw-r--r--   0        0        0     2175 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_reconciliation_run_request.py
+-rw-r--r--   0        0        0     4666 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_reference_portfolio_constituents_request.py
+-rw-r--r--   0        0        0     3321 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_reference_portfolio_constituents_response.py
+-rw-r--r--   0        0        0     3539 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_result_values_data_request.py
+-rw-r--r--   0        0        0     4604 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_returns_response.py
+-rw-r--r--   0        0        0     3227 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_single_structured_data_response.py
+-rw-r--r--   0        0        0     4409 2023-11-21 23:48:16.934005 lusid_sdk-2.0.96b0/lusid/models/upsert_structured_data_response.py
+-rw-r--r--   0        0        0     2693 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/upsert_structured_result_data_request.py
+-rw-r--r--   0        0        0     4342 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/upsert_transaction_properties_response.py
+-rw-r--r--   0        0        0     2025 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/user.py
+-rw-r--r--   0        0        0    10572 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/valuation_request.py
+-rw-r--r--   0        0        0     5386 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/valuation_schedule.py
+-rw-r--r--   0        0        0     4998 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/valuations_reconciliation_request.py
+-rw-r--r--   0        0        0     1241 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/value_type.py
+-rw-r--r--   0        0        0     4304 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/vendor_dependency.py
+-rw-r--r--   0        0        0      812 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/vendor_library.py
+-rw-r--r--   0        0        0     6260 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/vendor_model_rule.py
+-rw-r--r--   0        0        0     6004 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/version.py
+-rw-r--r--   0        0        0     3581 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/version_summary_dto.py
+-rw-r--r--   0        0        0     4519 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_a2_b_data_record.py
+-rw-r--r--   0        0        0     4567 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_a2_b_movement_record.py
+-rw-r--r--   0        0        0     4577 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_holding_contributor.py
+-rw-r--r--   0        0        0     4554 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_journal_entry_line.py
+-rw-r--r--   0        0        0     4565 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_output_transaction.py
+-rw-r--r--   0        0        0     4553 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_portfolio_holding.py
+-rw-r--r--   0        0        0     4492 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_transaction.py
+-rw-r--r--   0        0        0     4505 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_trial_balance.py
+-rw-r--r--   0        0        0     5576 2023-11-21 23:48:16.935005 lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py
+-rw-r--r--   0        0        0     3253 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/virtual_document.py
+-rw-r--r--   0        0        0     2753 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/virtual_document_row.py
+-rw-r--r--   0        0        0     3196 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/virtual_row.py
+-rw-r--r--   0        0        0     1873 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/warning.py
+-rw-r--r--   0        0        0     2312 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/weekend_mask.py
+-rw-r--r--   0        0        0     3570 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/weighted_instrument.py
+-rw-r--r--   0        0        0     2540 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/weighted_instruments.py
+-rw-r--r--   0        0        0     6242 2023-11-21 23:48:16.936005 lusid_sdk-2.0.96b0/lusid/models/yield_curve_data.py
+-rw-r--r--   0        0        0        0 2023-11-21 23:48:16.942005 lusid_sdk-2.0.96b0/lusid/py.typed
+-rw-r--r--   0        0        0    10007 2023-11-21 23:48:16.943005 lusid_sdk-2.0.96b0/lusid/rest.py
+-rw-r--r--   0        0        0      797 2023-11-21 23:48:16.993005 lusid_sdk-2.0.96b0/pyproject.toml
+-rw-r--r--   0        0        0   162933 1970-01-01 00:00:00.000000 lusid_sdk-2.0.96b0/PKG-INFO
```

### Comparing `lusid_sdk-2.0.90b0/README.md` & `lusid_sdk-2.0.96b0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.11.6039
-- Package version: 2.0.90-beta
+- API version: 0.11.6045
+- Package version: 2.0.96-beta
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_sdk-2.0.90b0/lusid/__init__.py` & `lusid_sdk-2.0.96b0/lusid/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/__init__.py` & `lusid_sdk-2.0.96b0/lusid/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/abor_api.py` & `lusid_sdk-2.0.96b0/lusid/api/abor_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/abor_configuration_api.py` & `lusid_sdk-2.0.96b0/lusid/api/abor_configuration_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/address_key_definition_api.py` & `lusid_sdk-2.0.96b0/lusid/api/address_key_definition_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/aggregation_api.py` & `lusid_sdk-2.0.96b0/lusid/api/aggregation_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/allocations_api.py` & `lusid_sdk-2.0.96b0/lusid/api/allocations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/application_metadata_api.py` & `lusid_sdk-2.0.96b0/lusid/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/blocks_api.py` & `lusid_sdk-2.0.96b0/lusid/api/blocks_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/calendars_api.py` & `lusid_sdk-2.0.96b0/lusid/api/calendars_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/chart_of_accounts_api.py` & `lusid_sdk-2.0.96b0/lusid/api/chart_of_accounts_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/complex_market_data_api.py` & `lusid_sdk-2.0.96b0/lusid/api/complex_market_data_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/compliance_api.py` & `lusid_sdk-2.0.96b0/lusid/api/compliance_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/configuration_recipe_api.py` & `lusid_sdk-2.0.96b0/lusid/api/configuration_recipe_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/conventions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/conventions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/corporate_action_sources_api.py` & `lusid_sdk-2.0.96b0/lusid/api/corporate_action_sources_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/counterparties_api.py` & `lusid_sdk-2.0.96b0/lusid/api/counterparties_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/custom_entities_api.py` & `lusid_sdk-2.0.96b0/lusid/api/custom_entities_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/custom_entity_definitions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/custom_entity_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/custom_entity_types_api.py` & `lusid_sdk-2.0.96b0/lusid/api/custom_entity_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/cut_label_definitions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/cut_label_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/data_types_api.py` & `lusid_sdk-2.0.96b0/lusid/api/data_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/derived_transaction_portfolios_api.py` & `lusid_sdk-2.0.96b0/lusid/api/derived_transaction_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/entities_api.py` & `lusid_sdk-2.0.96b0/lusid/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/executions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/executions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/instrument_event_types_api.py` & `lusid_sdk-2.0.96b0/lusid/api/instrument_event_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/instrument_events_api.py` & `lusid_sdk-2.0.96b0/lusid/api/instrument_events_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/instruments_api.py` & `lusid_sdk-2.0.96b0/lusid/api/instruments_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/legacy_compliance_api.py` & `lusid_sdk-2.0.96b0/lusid/api/legacy_compliance_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/legal_entities_api.py` & `lusid_sdk-2.0.96b0/lusid/api/legal_entities_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/order_graph_api.py` & `lusid_sdk-2.0.96b0/lusid/api/order_graph_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/order_instructions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/order_instructions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/order_management_api.py` & `lusid_sdk-2.0.96b0/lusid/api/order_management_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/orders_api.py` & `lusid_sdk-2.0.96b0/lusid/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/packages_api.py` & `lusid_sdk-2.0.96b0/lusid/api/packages_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/participations_api.py` & `lusid_sdk-2.0.96b0/lusid/api/participations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/persons_api.py` & `lusid_sdk-2.0.96b0/lusid/api/persons_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/placements_api.py` & `lusid_sdk-2.0.96b0/lusid/api/placements_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/portfolio_groups_api.py` & `lusid_sdk-2.0.96b0/lusid/api/portfolio_groups_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/portfolios_api.py` & `lusid_sdk-2.0.96b0/lusid/api/portfolios_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/property_definitions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/property_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/quotes_api.py` & `lusid_sdk-2.0.96b0/lusid/api/quotes_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/reconciliations_api.py` & `lusid_sdk-2.0.96b0/lusid/api/reconciliations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/reference_lists_api.py` & `lusid_sdk-2.0.96b0/lusid/api/reference_lists_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/reference_portfolio_api.py` & `lusid_sdk-2.0.96b0/lusid/api/reference_portfolio_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/relation_definitions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/relation_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/relations_api.py` & `lusid_sdk-2.0.96b0/lusid/api/relations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/relationship_definitions_api.py` & `lusid_sdk-2.0.96b0/lusid/api/relationship_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/relationships_api.py` & `lusid_sdk-2.0.96b0/lusid/api/relationships_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/schemas_api.py` & `lusid_sdk-2.0.96b0/lusid/api/schemas_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/scopes_api.py` & `lusid_sdk-2.0.96b0/lusid/api/scopes_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/scripted_translation_api.py` & `lusid_sdk-2.0.96b0/lusid/api/scripted_translation_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/search_api.py` & `lusid_sdk-2.0.96b0/lusid/api/search_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/sequences_api.py` & `lusid_sdk-2.0.96b0/lusid/api/sequences_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/structured_result_data_api.py` & `lusid_sdk-2.0.96b0/lusid/api/structured_result_data_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/system_configuration_api.py` & `lusid_sdk-2.0.96b0/lusid/api/system_configuration_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/tax_rule_sets_api.py` & `lusid_sdk-2.0.96b0/lusid/api/tax_rule_sets_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/transaction_configuration_api.py` & `lusid_sdk-2.0.96b0/lusid/api/transaction_configuration_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/transaction_fees_api.py` & `lusid_sdk-2.0.96b0/lusid/api/transaction_fees_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/transaction_portfolios_api.py` & `lusid_sdk-2.0.96b0/lusid/api/transaction_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api/translation_api.py` & `lusid_sdk-2.0.96b0/lusid/api/translation_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api_client.py` & `lusid_sdk-2.0.96b0/lusid/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/api_response.py` & `lusid_sdk-2.0.96b0/lusid/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/configuration.py` & `lusid_sdk-2.0.96b0/lusid/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.11.6039\n"\
+               "Version of the API: 0.11.6045\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_sdk-2.0.90b0/lusid/exceptions.py` & `lusid_sdk-2.0.96b0/lusid/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/__init__.py` & `lusid_sdk-2.0.96b0/lusid/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/api_client.py` & `lusid_sdk-2.0.96b0/lusid/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/api_client_builder.py` & `lusid_sdk-2.0.96b0/lusid/extensions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/api_client_factory.py` & `lusid_sdk-2.0.96b0/lusid/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/api_configuration.py` & `lusid_sdk-2.0.96b0/lusid/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/configuration_loaders.py` & `lusid_sdk-2.0.96b0/lusid/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/proxy_config.py` & `lusid_sdk-2.0.96b0/lusid/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/refreshing_token.py` & `lusid_sdk-2.0.96b0/lusid/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/rest.py` & `lusid_sdk-2.0.96b0/lusid/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/retry.py` & `lusid_sdk-2.0.96b0/lusid/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/socket_keep_alive.py` & `lusid_sdk-2.0.96b0/lusid/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/extensions/tcp_keep_alive_connector.py` & `lusid_sdk-2.0.96b0/lusid/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/__init__.py` & `lusid_sdk-2.0.96b0/lusid/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/a2_b_breakdown.py` & `lusid_sdk-2.0.96b0/lusid/models/a2_b_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/a2_b_category.py` & `lusid_sdk-2.0.96b0/lusid/models/a2_b_category.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/a2_b_data_record.py` & `lusid_sdk-2.0.96b0/lusid/models/a2_b_data_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/a2_b_movement_record.py` & `lusid_sdk-2.0.96b0/lusid/models/a2_b_movement_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/abor.py` & `lusid_sdk-2.0.96b0/lusid/models/abor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/abor_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/abor_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/abor_configuration_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/abor_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/abor_configuration_request.py` & `lusid_sdk-2.0.96b0/lusid/models/abor_configuration_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/abor_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/abor_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/abor_request.py` & `lusid_sdk-2.0.96b0/lusid/models/abor_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/access_controlled_action.py` & `lusid_sdk-2.0.96b0/lusid/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/access_controlled_resource.py` & `lusid_sdk-2.0.96b0/lusid/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/access_metadata_operation.py` & `lusid_sdk-2.0.96b0/lusid/models/access_metadata_operation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/access_metadata_value.py` & `lusid_sdk-2.0.96b0/lusid/models/access_metadata_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/account.py` & `lusid_sdk-2.0.96b0/lusid/models/account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/account_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/account_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/accounting_method.py` & `lusid_sdk-2.0.96b0/lusid/models/accounting_method.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/accounts_upsert_response.py` & `lusid_sdk-2.0.96b0/lusid/models/accounts_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/action_id.py` & `lusid_sdk-2.0.96b0/lusid/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/action_result_of_portfolio.py` & `lusid_sdk-2.0.96b0/lusid/models/action_result_of_portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/add_business_days_to_date_request.py` & `lusid_sdk-2.0.96b0/lusid/models/add_business_days_to_date_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/add_business_days_to_date_response.py` & `lusid_sdk-2.0.96b0/lusid/models/add_business_days_to_date_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/additional_payment.py` & `lusid_sdk-2.0.96b0/lusid/models/additional_payment.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/address_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_key_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/address_key_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_key_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/address_key_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_key_filter.py` & `lusid_sdk-2.0.96b0/lusid/models/address_key_filter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_key_list.py` & `lusid_sdk-2.0.96b0/lusid/models/address_key_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_key_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/address_key_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/address_key_option_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/address_key_option_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/adjust_holding.py` & `lusid_sdk-2.0.96b0/lusid/models/adjust_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/adjust_holding_for_date_request.py` & `lusid_sdk-2.0.96b0/lusid/models/adjust_holding_for_date_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/adjust_holding_request.py` & `lusid_sdk-2.0.96b0/lusid/models/adjust_holding_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregate_spec.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregate_spec.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregated_return.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregated_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregated_returns_dispersion_request.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregated_returns_dispersion_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregated_returns_request.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregated_returns_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregated_returns_response.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregated_returns_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregated_transactions_request.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregated_transactions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregation_context.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregation_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregation_measure_failure_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregation_measure_failure_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregation_op.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregation_op.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregation_options.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregation_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregation_query.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregation_query.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/aggregation_type.py` & `lusid_sdk-2.0.96b0/lusid/models/aggregation_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/allocation.py` & `lusid_sdk-2.0.96b0/lusid/models/allocation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/allocation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/allocation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/allocation_service_run_response.py` & `lusid_sdk-2.0.96b0/lusid/models/allocation_service_run_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/allocation_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/allocation_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/amortisation_event.py` & `lusid_sdk-2.0.96b0/lusid/models/amortisation_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/annul_quotes_response.py` & `lusid_sdk-2.0.96b0/lusid/models/annul_quotes_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/annul_single_structured_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/annul_single_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/annul_structured_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/annul_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/asset_class.py` & `lusid_sdk-2.0.96b0/lusid/models/asset_class.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/asset_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/asset_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/barrier.py` & `lusid_sdk-2.0.96b0/lusid/models/barrier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/basket.py` & `lusid_sdk-2.0.96b0/lusid/models/basket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/basket_identifier.py` & `lusid_sdk-2.0.96b0/lusid/models/basket_identifier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/batch_adjust_holdings_response.py` & `lusid_sdk-2.0.96b0/lusid/models/batch_adjust_holdings_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/batch_upsert_instrument_properties_response.py` & `lusid_sdk-2.0.96b0/lusid/models/batch_upsert_instrument_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/batch_upsert_portfolio_transactions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/batch_upsert_portfolio_transactions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/batch_upsert_property_definition_properties_response.py` & `lusid_sdk-2.0.96b0/lusid/models/batch_upsert_property_definition_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/block.py` & `lusid_sdk-2.0.96b0/lusid/models/block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/block_request.py` & `lusid_sdk-2.0.96b0/lusid/models/block_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/block_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/block_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bond.py` & `lusid_sdk-2.0.96b0/lusid/models/bond.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bond_coupon_event.py` & `lusid_sdk-2.0.96b0/lusid/models/bond_coupon_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bond_default_event.py` & `lusid_sdk-2.0.96b0/lusid/models/bond_default_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/book_transactions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/book_transactions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bool_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/bool_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bool_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/bool_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bucketed_cash_flow_request.py` & `lusid_sdk-2.0.96b0/lusid/models/bucketed_cash_flow_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bucketed_cash_flow_response.py` & `lusid_sdk-2.0.96b0/lusid/models/bucketed_cash_flow_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/bucketing_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/bucketing_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/calculation_info.py` & `lusid_sdk-2.0.96b0/lusid/models/calculation_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/calendar.py` & `lusid_sdk-2.0.96b0/lusid/models/calendar.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/calendar_date.py` & `lusid_sdk-2.0.96b0/lusid/models/calendar_date.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/calendar_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/calendar_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cap_floor.py` & `lusid_sdk-2.0.96b0/lusid/models/cap_floor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_dividend_event.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_dividend_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_election.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_election.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_flow_event.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_flow_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_flow_lineage.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_flow_lineage.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_flow_value.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_flow_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_flow_value_set.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_flow_value_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_ladder_record.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_ladder_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cash_perpetual.py` & `lusid_sdk-2.0.96b0/lusid/models/cash_perpetual.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cds_flow_conventions.py` & `lusid_sdk-2.0.96b0/lusid/models/cds_flow_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cds_index.py` & `lusid_sdk-2.0.96b0/lusid/models/cds_index.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cds_protection_detail_specification.py` & `lusid_sdk-2.0.96b0/lusid/models/cds_protection_detail_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/change.py` & `lusid_sdk-2.0.96b0/lusid/models/change.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/change_history.py` & `lusid_sdk-2.0.96b0/lusid/models/change_history.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/change_history_action.py` & `lusid_sdk-2.0.96b0/lusid/models/change_history_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/change_item.py` & `lusid_sdk-2.0.96b0/lusid/models/change_item.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/chart_of_accounts.py` & `lusid_sdk-2.0.96b0/lusid/models/chart_of_accounts.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/chart_of_accounts_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/chart_of_accounts_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/chart_of_accounts_request.py` & `lusid_sdk-2.0.96b0/lusid/models/chart_of_accounts_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/client.py` & `lusid_sdk-2.0.96b0/lusid/models/client.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/close_event.py` & `lusid_sdk-2.0.96b0/lusid/models/close_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/complete_portfolio.py` & `lusid_sdk-2.0.96b0/lusid/models/complete_portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/complete_relation.py` & `lusid_sdk-2.0.96b0/lusid/models/complete_relation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/complete_relationship.py` & `lusid_sdk-2.0.96b0/lusid/models/complete_relationship.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/complex_bond.py` & `lusid_sdk-2.0.96b0/lusid/models/complex_bond.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/complex_market_data.py` & `lusid_sdk-2.0.96b0/lusid/models/complex_market_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/complex_market_data_id.py` & `lusid_sdk-2.0.96b0/lusid/models/complex_market_data_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_breached_order_info.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_breached_order_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_parameter_type.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_parameter_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_breakdown.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_breakdown_request.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_breakdown_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_response.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_result.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_result_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_result_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_result_portfolio_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_result_portfolio_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_upsert_request.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_upsert_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_rule_upsert_response.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_rule_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_run_info.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_run_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_run_info_v2.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_run_info_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_run_summary.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_run_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_summary_rule_result.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_summary_rule_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_summary_rule_result_request.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_summary_rule_result_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_template.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_template.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_template_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_template_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compliance_template_variation.py` & `lusid_sdk-2.0.96b0/lusid/models/compliance_template_variation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/composite_breakdown.py` & `lusid_sdk-2.0.96b0/lusid/models/composite_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/composite_breakdown_request.py` & `lusid_sdk-2.0.96b0/lusid/models/composite_breakdown_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/composite_breakdown_response.py` & `lusid_sdk-2.0.96b0/lusid/models/composite_breakdown_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/composite_dispersion.py` & `lusid_sdk-2.0.96b0/lusid/models/composite_dispersion.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/composite_dispersion_response.py` & `lusid_sdk-2.0.96b0/lusid/models/composite_dispersion_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/compounding.py` & `lusid_sdk-2.0.96b0/lusid/models/compounding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/configuration_recipe.py` & `lusid_sdk-2.0.96b0/lusid/models/configuration_recipe.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/constituents_adjustment_header.py` & `lusid_sdk-2.0.96b0/lusid/models/constituents_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/contract_for_difference.py` & `lusid_sdk-2.0.96b0/lusid/models/contract_for_difference.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/corporate_action.py` & `lusid_sdk-2.0.96b0/lusid/models/corporate_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/corporate_action_source.py` & `lusid_sdk-2.0.96b0/lusid/models/corporate_action_source.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition.py` & `lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition_component.py` & `lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition_component.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition_component_request.py` & `lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition_component_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/corporate_action_transition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/corporate_action_transition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/counterparty_agreement.py` & `lusid_sdk-2.0.96b0/lusid/models/counterparty_agreement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/counterparty_risk_information.py` & `lusid_sdk-2.0.96b0/lusid/models/counterparty_risk_information.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/counterparty_signatory.py` & `lusid_sdk-2.0.96b0/lusid/models/counterparty_signatory.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_address_key_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_address_key_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_calendar_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_calendar_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_corporate_action_source_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_corporate_action_source_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_custom_entity_type_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_custom_entity_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_cut_label_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_cut_label_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_data_map_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_data_map_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_data_type_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_data_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_date_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_date_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_derived_property_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_derived_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_derived_transaction_portfolio_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_derived_transaction_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_portfolio_details.py` & `lusid_sdk-2.0.96b0/lusid/models/create_portfolio_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_portfolio_group_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_portfolio_group_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_property_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_recipe_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_recipe_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_reference_portfolio_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_reference_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_relation_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_relation_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_relation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_relation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_relationship_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_relationship_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_relationship_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_relationship_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_sequence_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_sequence_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_tax_rule_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_tax_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_transaction_portfolio_request.py` & `lusid_sdk-2.0.96b0/lusid/models/create_transaction_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/create_unit_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/create_unit_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/credit_default_swap.py` & `lusid_sdk-2.0.96b0/lusid/models/credit_default_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/credit_rating.py` & `lusid_sdk-2.0.96b0/lusid/models/credit_rating.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/credit_spread_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/credit_spread_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/credit_support_annex.py` & `lusid_sdk-2.0.96b0/lusid/models/credit_support_annex.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/criterion_type.py` & `lusid_sdk-2.0.96b0/lusid/models/criterion_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/currency_and_amount.py` & `lusid_sdk-2.0.96b0/lusid/models/currency_and_amount.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/curve_options.py` & `lusid_sdk-2.0.96b0/lusid/models/curve_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custodian_account.py` & `lusid_sdk-2.0.96b0/lusid/models/custodian_account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custodian_account_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/custodian_account_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custodian_account_request.py` & `lusid_sdk-2.0.96b0/lusid/models/custodian_account_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custodian_accounts_upsert_response.py` & `lusid_sdk-2.0.96b0/lusid/models/custodian_accounts_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_field.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_field.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_field_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_id.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_request.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_response.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/custom_entity_type.py` & `lusid_sdk-2.0.96b0/lusid/models/custom_entity_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cut_label_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/cut_label_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/cut_local_time.py` & `lusid_sdk-2.0.96b0/lusid/models/cut_local_time.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/data_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_map_key.py` & `lusid_sdk-2.0.96b0/lusid/models/data_map_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_mapping.py` & `lusid_sdk-2.0.96b0/lusid/models/data_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_scope.py` & `lusid_sdk-2.0.96b0/lusid/models/data_scope.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_type.py` & `lusid_sdk-2.0.96b0/lusid/models/data_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_type_summary.py` & `lusid_sdk-2.0.96b0/lusid/models/data_type_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/data_type_value_range.py` & `lusid_sdk-2.0.96b0/lusid/models/data_type_value_range.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/date_attributes.py` & `lusid_sdk-2.0.96b0/lusid/models/date_attributes.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/date_or_diary_entry.py` & `lusid_sdk-2.0.96b0/lusid/models/date_or_diary_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/date_range.py` & `lusid_sdk-2.0.96b0/lusid/models/date_range.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/date_time_comparison_type.py` & `lusid_sdk-2.0.96b0/lusid/models/date_time_comparison_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/date_time_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/date_time_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/date_time_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/date_time_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/day_of_week.py` & `lusid_sdk-2.0.96b0/lusid/models/day_of_week.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/decimal_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/decimal_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/decimal_list.py` & `lusid_sdk-2.0.96b0/lusid/models/decimal_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/decimal_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/decimal_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/decorated_compliance_run_summary.py` & `lusid_sdk-2.0.96b0/lusid/models/decorated_compliance_run_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_accounts_response.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_accounts_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_custodian_accounts_response.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_custodian_accounts_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_instrument_properties_response.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_instrument_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_instrument_response.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_instrument_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_instruments_response.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_instruments_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_modes.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_modes.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_relation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_relation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/delete_relationship_request.py` & `lusid_sdk-2.0.96b0/lusid/models/delete_relationship_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/deleted_entity_response.py` & `lusid_sdk-2.0.96b0/lusid/models/deleted_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/dependency_source_filter.py` & `lusid_sdk-2.0.96b0/lusid/models/dependency_source_filter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/described_address_key.py` & `lusid_sdk-2.0.96b0/lusid/models/described_address_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/dialect.py` & `lusid_sdk-2.0.96b0/lusid/models/dialect.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/dialect_id.py` & `lusid_sdk-2.0.96b0/lusid/models/dialect_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/dialect_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/dialect_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/diary_entry.py` & `lusid_sdk-2.0.96b0/lusid/models/diary_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/diary_entry_request.py` & `lusid_sdk-2.0.96b0/lusid/models/diary_entry_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/discount_factor_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/discount_factor_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/discounting_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/discounting_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/discounting_method.py` & `lusid_sdk-2.0.96b0/lusid/models/discounting_method.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/economic_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/economic_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/economic_dependency_type.py` & `lusid_sdk-2.0.96b0/lusid/models/economic_dependency_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/economic_dependency_with_complex_market_data.py` & `lusid_sdk-2.0.96b0/lusid/models/economic_dependency_with_complex_market_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/economic_dependency_with_quote.py` & `lusid_sdk-2.0.96b0/lusid/models/economic_dependency_with_quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/election_specification.py` & `lusid_sdk-2.0.96b0/lusid/models/election_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/empty_model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/empty_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/entity_identifier.py` & `lusid_sdk-2.0.96b0/lusid/models/entity_identifier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity.py` & `lusid_sdk-2.0.96b0/lusid/models/equity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_all_of_identifiers.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_all_of_identifiers.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_curve_by_prices_data.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_curve_by_prices_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_curve_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_curve_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_option.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_option.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_swap.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_vol_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_vol_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/equity_vol_surface_data.py` & `lusid_sdk-2.0.96b0/lusid/models/equity_vol_surface_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/error_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/event_date_range.py` & `lusid_sdk-2.0.96b0/lusid/models/event_date_range.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/ex_dividend_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/ex_dividend_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/exchange_traded_option.py` & `lusid_sdk-2.0.96b0/lusid/models/exchange_traded_option.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/exchange_traded_option_contract_details.py` & `lusid_sdk-2.0.96b0/lusid/models/exchange_traded_option_contract_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/execution.py` & `lusid_sdk-2.0.96b0/lusid/models/execution.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/execution_request.py` & `lusid_sdk-2.0.96b0/lusid/models/execution_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/execution_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/execution_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/exercise_event.py` & `lusid_sdk-2.0.96b0/lusid/models/exercise_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/exotic_instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/exotic_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/expanded_group.py` & `lusid_sdk-2.0.96b0/lusid/models/expanded_group.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fee_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/fee_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fee_rule_upsert_request.py` & `lusid_sdk-2.0.96b0/lusid/models/fee_rule_upsert_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fee_rule_upsert_response.py` & `lusid_sdk-2.0.96b0/lusid/models/fee_rule_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/field_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/field_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/field_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/field_value.py` & `lusid_sdk-2.0.96b0/lusid/models/field_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/file_response.py` & `lusid_sdk-2.0.96b0/lusid/models/file_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/filter_predicate_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/filter_predicate_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fixed_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/fixed_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fixed_leg_all_of_overrides.py` & `lusid_sdk-2.0.96b0/lusid/models/fixed_leg_all_of_overrides.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fixed_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/fixed_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/float_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/float_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/floating_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/floating_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/flow_convention_name.py` & `lusid_sdk-2.0.96b0/lusid/models/flow_convention_name.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/flow_conventions.py` & `lusid_sdk-2.0.96b0/lusid/models/flow_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/forward_rate_agreement.py` & `lusid_sdk-2.0.96b0/lusid/models/forward_rate_agreement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/funding_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/funding_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/funding_leg_options.py` & `lusid_sdk-2.0.96b0/lusid/models/funding_leg_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/future.py` & `lusid_sdk-2.0.96b0/lusid/models/future.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/futures_contract_details.py` & `lusid_sdk-2.0.96b0/lusid/models/futures_contract_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward_curve_by_quote_reference.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward_curve_by_quote_reference.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward_model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward_pips_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward_pips_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward_tenor_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward_tenor_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forward_tenor_pips_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forward_tenor_pips_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_forwards_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_forwards_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_option.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_option.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_rate_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_swap.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_tenor_convention.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_tenor_convention.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_vol_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_vol_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/fx_vol_surface_data.py` & `lusid_sdk-2.0.96b0/lusid/models/fx_vol_surface_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/general_ledger_profile_mapping.py` & `lusid_sdk-2.0.96b0/lusid/models/general_ledger_profile_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/general_ledger_profile_request.py` & `lusid_sdk-2.0.96b0/lusid/models/general_ledger_profile_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/general_ledger_profile_response.py` & `lusid_sdk-2.0.96b0/lusid/models/general_ledger_profile_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_cds_flow_conventions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_cds_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_complex_market_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_complex_market_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_counterparty_agreement_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_counterparty_agreement_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_credit_support_annex_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_credit_support_annex_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_data_map_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_data_map_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_flow_conventions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_index_convention_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_index_convention_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_instruments_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_instruments_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_quotes_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_quotes_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_recipe_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_recipe_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_reference_portfolio_constituents_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_reference_portfolio_constituents_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_structured_result_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_structured_result_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/get_virtual_document_response.py` & `lusid_sdk-2.0.96b0/lusid/models/get_virtual_document_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/grouped_result_of_address_key.py` & `lusid_sdk-2.0.96b0/lusid/models/grouped_result_of_address_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/holding_adjustment.py` & `lusid_sdk-2.0.96b0/lusid/models/holding_adjustment.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/holding_adjustment_with_date.py` & `lusid_sdk-2.0.96b0/lusid/models/holding_adjustment_with_date.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/holding_context.py` & `lusid_sdk-2.0.96b0/lusid/models/holding_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/holding_contributor.py` & `lusid_sdk-2.0.96b0/lusid/models/holding_contributor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/holdings_adjustment.py` & `lusid_sdk-2.0.96b0/lusid/models/holdings_adjustment.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/holdings_adjustment_header.py` & `lusid_sdk-2.0.96b0/lusid/models/holdings_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/i_unit_definition_dto.py` & `lusid_sdk-2.0.96b0/lusid/models/i_unit_definition_dto.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/id_selector_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/identifier_part_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/index_convention.py` & `lusid_sdk-2.0.96b0/lusid/models/index_convention.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/index_model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/index_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/index_projection_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/index_projection_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/industry_classifier.py` & `lusid_sdk-2.0.96b0/lusid/models/industry_classifier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inflation_fixing_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/inflation_fixing_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inflation_index_conventions.py` & `lusid_sdk-2.0.96b0/lusid/models/inflation_index_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inflation_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/inflation_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inflation_linked_bond.py` & `lusid_sdk-2.0.96b0/lusid/models/inflation_linked_bond.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inflation_swap.py` & `lusid_sdk-2.0.96b0/lusid/models/inflation_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/informational_error_event.py` & `lusid_sdk-2.0.96b0/lusid/models/informational_error_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/informational_event.py` & `lusid_sdk-2.0.96b0/lusid/models/informational_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inline_valuation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/inline_valuation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/inline_valuations_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/inline_valuations_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/input_transition.py` & `lusid_sdk-2.0.96b0/lusid/models/input_transition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_capabilities.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_capabilities.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_cash_flow.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_definition_format.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_definition_format.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_delete_modes.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_delete_modes.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_event.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_event_holder.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_event_holder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_event_type.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_event_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_id_type_descriptor.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_id_type_descriptor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_id_value.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_id_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_list.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_match.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_match.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_models.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_models.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_payment_diary.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_payment_diary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_payment_diary_leg.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_payment_diary_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_payment_diary_row.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_payment_diary_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_search_property.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_search_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/instrument_type.py` & `lusid_sdk-2.0.96b0/lusid/models/instrument_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/interest_rate_swap.py` & `lusid_sdk-2.0.96b0/lusid/models/interest_rate_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/interest_rate_swaption.py` & `lusid_sdk-2.0.96b0/lusid/models/interest_rate_swaption.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/ir_vol_cube_data.py` & `lusid_sdk-2.0.96b0/lusid/models/ir_vol_cube_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/ir_vol_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/ir_vol_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/is_business_day_response.py` & `lusid_sdk-2.0.96b0/lusid/models/is_business_day_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/je_lines_query_parameters.py` & `lusid_sdk-2.0.96b0/lusid/models/je_lines_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/journal_entry_line.py` & `lusid_sdk-2.0.96b0/lusid/models/journal_entry_line.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/journal_entry_lines_query_parameters.py` & `lusid_sdk-2.0.96b0/lusid/models/journal_entry_lines_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/label_value_set.py` & `lusid_sdk-2.0.96b0/lusid/models/label_value_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/leg_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/leg_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/legal_entity.py` & `lusid_sdk-2.0.96b0/lusid/models/legal_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/level_step.py` & `lusid_sdk-2.0.96b0/lusid/models/level_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/life_cycle_event_lineage.py` & `lusid_sdk-2.0.96b0/lusid/models/life_cycle_event_lineage.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/life_cycle_event_value.py` & `lusid_sdk-2.0.96b0/lusid/models/life_cycle_event_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/link.py` & `lusid_sdk-2.0.96b0/lusid/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/list_aggregation_reconciliation.py` & `lusid_sdk-2.0.96b0/lusid/models/list_aggregation_reconciliation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/list_aggregation_response.py` & `lusid_sdk-2.0.96b0/lusid/models/list_aggregation_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/list_complex_market_data_with_meta_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/list_complex_market_data_with_meta_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/loan_period.py` & `lusid_sdk-2.0.96b0/lusid/models/loan_period.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/look_up_pricing_model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/look_up_pricing_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/lusid_instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/lusid_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/lusid_problem_details.py` & `lusid_sdk-2.0.96b0/lusid/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/lusid_trade_ticket.py` & `lusid_sdk-2.0.96b0/lusid/models/lusid_trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/lusid_unique_id.py` & `lusid_sdk-2.0.96b0/lusid/models/lusid_unique_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/lusid_validation_problem_details.py` & `lusid_sdk-2.0.96b0/lusid/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/mapped_string.py` & `lusid_sdk-2.0.96b0/lusid/models/mapped_string.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/mapping.py` & `lusid_sdk-2.0.96b0/lusid/models/mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/mapping_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/mapping_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_context.py` & `lusid_sdk-2.0.96b0/lusid/models/market_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_context_suppliers.py` & `lusid_sdk-2.0.96b0/lusid/models/market_context_suppliers.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_data_key_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/market_data_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_data_options.py` & `lusid_sdk-2.0.96b0/lusid/models/market_data_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_data_options_type.py` & `lusid_sdk-2.0.96b0/lusid/models/market_data_options_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_data_overrides.py` & `lusid_sdk-2.0.96b0/lusid/models/market_data_overrides.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_data_specific_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/market_data_specific_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_data_type.py` & `lusid_sdk-2.0.96b0/lusid/models/market_data_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_observable_type.py` & `lusid_sdk-2.0.96b0/lusid/models/market_observable_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_options.py` & `lusid_sdk-2.0.96b0/lusid/models/market_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/market_quote.py` & `lusid_sdk-2.0.96b0/lusid/models/market_quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/match_criterion.py` & `lusid_sdk-2.0.96b0/lusid/models/match_criterion.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/metric_value.py` & `lusid_sdk-2.0.96b0/lusid/models/metric_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/model_options_type.py` & `lusid_sdk-2.0.96b0/lusid/models/model_options_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/model_property.py` & `lusid_sdk-2.0.96b0/lusid/models/model_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/model_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/model_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/model_selection.py` & `lusid_sdk-2.0.96b0/lusid/models/model_selection.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/movement_type.py` & `lusid_sdk-2.0.96b0/lusid/models/movement_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/next_value_in_sequence_response.py` & `lusid_sdk-2.0.96b0/lusid/models/next_value_in_sequence_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/numeric_comparison_type.py` & `lusid_sdk-2.0.96b0/lusid/models/numeric_comparison_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/opaque_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/opaque_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/opaque_market_data.py` & `lusid_sdk-2.0.96b0/lusid/models/opaque_market_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/opaque_model_options.py` & `lusid_sdk-2.0.96b0/lusid/models/opaque_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/open_event.py` & `lusid_sdk-2.0.96b0/lusid/models/open_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/operand_type.py` & `lusid_sdk-2.0.96b0/lusid/models/operand_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/operation.py` & `lusid_sdk-2.0.96b0/lusid/models/operation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/operation_type.py` & `lusid_sdk-2.0.96b0/lusid/models/operation_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/operator.py` & `lusid_sdk-2.0.96b0/lusid/models/operator.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/option_entry.py` & `lusid_sdk-2.0.96b0/lusid/models/option_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/optionality_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/optionality_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order.py` & `lusid_sdk-2.0.96b0/lusid/models/order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_by_spec.py` & `lusid_sdk-2.0.96b0/lusid/models/order_by_spec.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_flow_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/order_flow_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_allocation_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_allocation_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_allocation_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_allocation_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_execution_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_execution_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_execution_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_execution_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_order_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_order_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_order_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_order_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_placement_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_placement_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_block_placement_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_block_placement_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_allocation_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_allocation_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_allocation_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_allocation_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_child_placement_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_child_placement_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_execution_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_execution_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_execution_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_execution_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_order_detail.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_order_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_order_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_order_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_graph_placement_placement_synopsis.py` & `lusid_sdk-2.0.96b0/lusid/models/order_graph_placement_placement_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_instruction.py` & `lusid_sdk-2.0.96b0/lusid/models/order_instruction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_instruction_request.py` & `lusid_sdk-2.0.96b0/lusid/models/order_instruction_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_instruction_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/order_instruction_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_request.py` & `lusid_sdk-2.0.96b0/lusid/models/order_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/order_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/order_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/otc_confirmation.py` & `lusid_sdk-2.0.96b0/lusid/models/otc_confirmation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/output_transaction.py` & `lusid_sdk-2.0.96b0/lusid/models/output_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/output_transition.py` & `lusid_sdk-2.0.96b0/lusid/models/output_transition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/package.py` & `lusid_sdk-2.0.96b0/lusid/models/package.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/package_request.py` & `lusid_sdk-2.0.96b0/lusid/models/package_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/package_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/package_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_abor.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_abor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_abor_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_abor_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_account.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_address_key_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_address_key_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_allocation.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_allocation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_block.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_calendar.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_calendar.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_chart_of_accounts.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_chart_of_accounts.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_compliance_rule_response.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_compliance_rule_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_compliance_run_info_v2.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_compliance_run_info_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_compliance_template.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_compliance_template.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_corporate_action_source.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_corporate_action_source.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custodian_account.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custodian_account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custom_entity_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custom_entity_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custom_entity_response.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custom_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_custom_entity_type.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_custom_entity_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_cut_label_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_cut_label_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_data_type_summary.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_data_type_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_dialect_id.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_dialect_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_diary_entry.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_diary_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_execution.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_execution.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_general_ledger_profile_response.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_general_ledger_profile_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_instrument_event_holder.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_instrument_event_holder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_legal_entity.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_legal_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order_graph_block.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order_graph_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order_graph_placement.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order_graph_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_order_instruction.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_order_instruction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_package.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_package.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_participation.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_participation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_person.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_person.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_placement.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_portfolio_group.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_portfolio_group.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_portfolio_group_search_result.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_portfolio_group_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_portfolio_search_result.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_portfolio_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_posting_module_response.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_posting_module_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_posting_module_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_posting_module_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_property_definition_search_result.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_property_definition_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reconciliation.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reconciliation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reconciliation_run.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reconciliation_run.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reconciliation_run_break.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reconciliation_run_break.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_reference_list_response.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_reference_list_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_relationship_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_relationship_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_sequence_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_sequence_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_translation_script_id.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_translation_script_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/paged_resource_list_of_virtual_row.py` & `lusid_sdk-2.0.96b0/lusid/models/paged_resource_list_of_virtual_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/participation.py` & `lusid_sdk-2.0.96b0/lusid/models/participation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/participation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/participation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/participation_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/participation_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/performance_return.py` & `lusid_sdk-2.0.96b0/lusid/models/performance_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/performance_returns_metric.py` & `lusid_sdk-2.0.96b0/lusid/models/performance_returns_metric.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/period_type.py` & `lusid_sdk-2.0.96b0/lusid/models/period_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/perpetual_entity_state.py` & `lusid_sdk-2.0.96b0/lusid/models/perpetual_entity_state.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/perpetual_property.py` & `lusid_sdk-2.0.96b0/lusid/models/perpetual_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/person.py` & `lusid_sdk-2.0.96b0/lusid/models/person.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/placement.py` & `lusid_sdk-2.0.96b0/lusid/models/placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/placement_request.py` & `lusid_sdk-2.0.96b0/lusid/models/placement_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/placement_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/placement_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_cash_flow.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_cash_ladder.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_cash_ladder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_details.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_entity_id.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_entity_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_group.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_group.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_group_id_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_group_id_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_group_id_list.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_group_id_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_group_id_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_group_id_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_group_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_group_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_group_search_result.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_group_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_holding.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_id_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_id_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_id_list.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_id_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_id_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_id_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_properties.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_result_data_key_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_result_data_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_return_breakdown.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_return_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_search_result.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_trade_ticket.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolio_type.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolio_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/portfolios_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/portfolios_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/posting_module_details.py` & `lusid_sdk-2.0.96b0/lusid/models/posting_module_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/posting_module_request.py` & `lusid_sdk-2.0.96b0/lusid/models/posting_module_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/posting_module_response.py` & `lusid_sdk-2.0.96b0/lusid/models/posting_module_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/posting_module_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/posting_module_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/posting_module_rules_updated_response.py` & `lusid_sdk-2.0.96b0/lusid/models/posting_module_rules_updated_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/premium.py` & `lusid_sdk-2.0.96b0/lusid/models/premium.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/pricing_context.py` & `lusid_sdk-2.0.96b0/lusid/models/pricing_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/pricing_model.py` & `lusid_sdk-2.0.96b0/lusid/models/pricing_model.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/pricing_options.py` & `lusid_sdk-2.0.96b0/lusid/models/pricing_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/processed_command.py` & `lusid_sdk-2.0.96b0/lusid/models/processed_command.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/property_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_definition_search_result.py` & `lusid_sdk-2.0.96b0/lusid/models/property_definition_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_definition_type.py` & `lusid_sdk-2.0.96b0/lusid/models/property_definition_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_domain.py` & `lusid_sdk-2.0.96b0/lusid/models/property_domain.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_filter.py` & `lusid_sdk-2.0.96b0/lusid/models/property_filter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_interval.py` & `lusid_sdk-2.0.96b0/lusid/models/property_interval.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_key_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/property_key_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_key_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/property_key_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_life_time.py` & `lusid_sdk-2.0.96b0/lusid/models/property_life_time.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/property_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_type.py` & `lusid_sdk-2.0.96b0/lusid/models/property_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_value.py` & `lusid_sdk-2.0.96b0/lusid/models/property_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_value_equals.py` & `lusid_sdk-2.0.96b0/lusid/models/property_value_equals.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/property_value_in.py` & `lusid_sdk-2.0.96b0/lusid/models/property_value_in.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/query_bucketed_cash_flows_request.py` & `lusid_sdk-2.0.96b0/lusid/models/query_bucketed_cash_flows_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/query_cash_flows_request.py` & `lusid_sdk-2.0.96b0/lusid/models/query_cash_flows_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/query_instrument_events_request.py` & `lusid_sdk-2.0.96b0/lusid/models/query_instrument_events_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/query_trade_tickets_request.py` & `lusid_sdk-2.0.96b0/lusid/models/query_trade_tickets_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote.py` & `lusid_sdk-2.0.96b0/lusid/models/quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_access_metadata_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_access_metadata_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_access_metadata_rule_id.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_access_metadata_rule_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_id.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_instrument_id_type.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_instrument_id_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_series_id.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_series_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/quote_type.py` & `lusid_sdk-2.0.96b0/lusid/models/quote_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/raw_vendor_event.py` & `lusid_sdk-2.0.96b0/lusid/models/raw_vendor_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/realised_gain_loss.py` & `lusid_sdk-2.0.96b0/lusid/models/realised_gain_loss.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconcile_date_time_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/reconcile_date_time_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconcile_numeric_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/reconcile_numeric_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconcile_string_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/reconcile_string_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciled_transaction.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciled_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_break.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_break.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_break_id.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_break_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_id.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_left_right_address_key_pair.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_left_right_address_key_pair.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_line.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_line.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_response.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_rule_type.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_rule_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_run.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_run.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_run_break.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_run_break.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_run_id.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_run_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_side_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_side_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reconciliation_transactions.py` & `lusid_sdk-2.0.96b0/lusid/models/reconciliation_transactions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_data.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_list.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_list_request.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_list_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_list_response.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_list_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_list_type.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_list_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_portfolio_constituent.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_portfolio_constituent.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_portfolio_constituent_request.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_portfolio_constituent_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reference_portfolio_weight_type.py` & `lusid_sdk-2.0.96b0/lusid/models/reference_portfolio_weight_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/related_entity.py` & `lusid_sdk-2.0.96b0/lusid/models/related_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/relation.py` & `lusid_sdk-2.0.96b0/lusid/models/relation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/relation_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/relation_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/relationship.py` & `lusid_sdk-2.0.96b0/lusid/models/relationship.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/relationship_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/relationship_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/repo.py` & `lusid_sdk-2.0.96b0/lusid/models/repo.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/reset_event.py` & `lusid_sdk-2.0.96b0/lusid/models/reset_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_id.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_access_controlled_resource.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_access_metadata_value_of.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_access_metadata_value_of.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_address_key_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_address_key_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_aggregated_return.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_aggregated_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_aggregation_query.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_aggregation_query.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_allocation.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_allocation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_block.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_calendar_date.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_calendar_date.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_change.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_change.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_change_history.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_change_history.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_breached_order_info.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_breached_order_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_rule_result.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_rule_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_compliance_run_info.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_compliance_run_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_constituents_adjustment_header.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_constituents_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_corporate_action.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_corporate_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_data_type.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_data_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_execution.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_execution.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_fee_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_fee_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_cds_flow_conventions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_cds_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_counterparty_agreement_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_counterparty_agreement_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_credit_support_annex_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_credit_support_annex_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_flow_conventions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_index_convention_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_index_convention_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_get_recipe_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_get_recipe_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_holdings_adjustment_header.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_holdings_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_i_unit_definition_dto.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_i_unit_definition_dto.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_instrument_cash_flow.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_instrument_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_instrument_event_holder.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_instrument_event_holder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_instrument_id_type_descriptor.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_instrument_id_type_descriptor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_legal_entity.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_legal_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_mapping.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_order.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_order_instruction.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_order_instruction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_package.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_package.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_participation.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_participation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_performance_return.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_performance_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_person.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_person.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_placement.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio_cash_flow.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio_cash_ladder.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio_cash_ladder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_portfolio_trade_ticket.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_portfolio_trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_processed_command.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_processed_command.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_property.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_property_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_property_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_property_interval.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_property_interval.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_quote.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_quote_access_metadata_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_quote_access_metadata_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_reconciliation_break.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_reconciliation_break.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_relation.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_relation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_relationship.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_relationship.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_scope_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_scope_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_side_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_side_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_string.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_string.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_tax_rule_set.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_tax_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_transaction.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_transaction_type.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_transaction_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/resource_list_of_value_type.py` & `lusid_sdk-2.0.96b0/lusid/models/resource_list_of_value_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/response_meta_data.py` & `lusid_sdk-2.0.96b0/lusid/models/response_meta_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_data_key_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/result_data_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_data_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/result_data_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_key_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/result_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_key_rule_type.py` & `lusid_sdk-2.0.96b0/lusid/models/result_key_rule_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value0_d.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value0_d.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_bool.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_bool.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_currency.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_currency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_date_time_offset.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_date_time_offset.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_decimal.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_decimal.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_dictionary.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_dictionary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_int.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_int.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_string.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_string.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/result_value_type.py` & `lusid_sdk-2.0.96b0/lusid/models/result_value_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/rounding_configuration.py` & `lusid_sdk-2.0.96b0/lusid/models/rounding_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/rounding_configuration_component.py` & `lusid_sdk-2.0.96b0/lusid/models/rounding_configuration_component.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/rounding_convention.py` & `lusid_sdk-2.0.96b0/lusid/models/rounding_convention.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/scaling_methodology.py` & `lusid_sdk-2.0.96b0/lusid/models/scaling_methodology.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/schedule_type.py` & `lusid_sdk-2.0.96b0/lusid/models/schedule_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/scope_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/scope_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/sequence_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/sequence_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/set_legal_entity_identifiers_request.py` & `lusid_sdk-2.0.96b0/lusid/models/set_legal_entity_identifiers_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/set_legal_entity_properties_request.py` & `lusid_sdk-2.0.96b0/lusid/models/set_legal_entity_properties_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/set_person_identifiers_request.py` & `lusid_sdk-2.0.96b0/lusid/models/set_person_identifiers_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/set_person_properties_request.py` & `lusid_sdk-2.0.96b0/lusid/models/set_person_properties_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/set_transaction_configuration_alias.py` & `lusid_sdk-2.0.96b0/lusid/models/set_transaction_configuration_alias.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/set_transaction_configuration_source_request.py` & `lusid_sdk-2.0.96b0/lusid/models/set_transaction_configuration_source_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/side_configuration_data.py` & `lusid_sdk-2.0.96b0/lusid/models/side_configuration_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/side_configuration_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/side_configuration_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/side_definition.py` & `lusid_sdk-2.0.96b0/lusid/models/side_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/side_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/side_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/sides_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/sides_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/simple_cash_flow_loan.py` & `lusid_sdk-2.0.96b0/lusid/models/simple_cash_flow_loan.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/simple_instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/simple_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/sort_order.py` & `lusid_sdk-2.0.96b0/lusid/models/sort_order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/step_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/step_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/stock_split_event.py` & `lusid_sdk-2.0.96b0/lusid/models/stock_split_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/stream.py` & `lusid_sdk-2.0.96b0/lusid/models/stream.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/string_comparison_type.py` & `lusid_sdk-2.0.96b0/lusid/models/string_comparison_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/string_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/string_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/string_list.py` & `lusid_sdk-2.0.96b0/lusid/models/string_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/string_list_compliance_parameter.py` & `lusid_sdk-2.0.96b0/lusid/models/string_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/structured_result_data.py` & `lusid_sdk-2.0.96b0/lusid/models/structured_result_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/structured_result_data_id.py` & `lusid_sdk-2.0.96b0/lusid/models/structured_result_data_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/sub_holding_key_value_equals.py` & `lusid_sdk-2.0.96b0/lusid/models/sub_holding_key_value_equals.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/target_tax_lot.py` & `lusid_sdk-2.0.96b0/lusid/models/target_tax_lot.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/target_tax_lot_request.py` & `lusid_sdk-2.0.96b0/lusid/models/target_tax_lot_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/tax_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/tax_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/tax_rule_set.py` & `lusid_sdk-2.0.96b0/lusid/models/tax_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/template_field.py` & `lusid_sdk-2.0.96b0/lusid/models/template_field.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/term_deposit.py` & `lusid_sdk-2.0.96b0/lusid/models/term_deposit.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/total_return_swap.py` & `lusid_sdk-2.0.96b0/lusid/models/total_return_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/touch.py` & `lusid_sdk-2.0.96b0/lusid/models/touch.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/trade_ticket.py` & `lusid_sdk-2.0.96b0/lusid/models/trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/trade_ticket_type.py` & `lusid_sdk-2.0.96b0/lusid/models/trade_ticket_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_data.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_movement_data.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_movement_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_movement_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_movement_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_configuration_type_alias.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_configuration_type_alias.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_price.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_price.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_price_type.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_price_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_property_mapping.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_property_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_property_mapping_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_query_mode.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_query_mode.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_query_parameters.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_reconciliation_request_v2.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_reconciliation_request_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_roles.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_roles.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_set_configuration_data.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_set_configuration_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_set_configuration_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_set_configuration_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_status.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_status.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_template_specification.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_template_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_type.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_type_alias.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_type_alias.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_type_calculation.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_type_calculation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_type_movement.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_type_movement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_type_property_mapping.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_type_property_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transaction_type_request.py` & `lusid_sdk-2.0.96b0/lusid/models/transaction_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transactions_reconciliations_response.py` & `lusid_sdk-2.0.96b0/lusid/models/transactions_reconciliations_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/transition_event.py` & `lusid_sdk-2.0.96b0/lusid/models/transition_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_entities_inlined_request.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_entities_inlined_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_entities_request.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_entities_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_entities_response.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_entities_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_instrument_definitions_request.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_instrument_definitions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_instrument_definitions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_instrument_definitions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_trade_ticket_request.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_trade_ticket_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translate_trade_tickets_response.py` & `lusid_sdk-2.0.96b0/lusid/models/translate_trade_tickets_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translation_input.py` & `lusid_sdk-2.0.96b0/lusid/models/translation_input.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translation_result.py` & `lusid_sdk-2.0.96b0/lusid/models/translation_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translation_script.py` & `lusid_sdk-2.0.96b0/lusid/models/translation_script.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/translation_script_id.py` & `lusid_sdk-2.0.96b0/lusid/models/translation_script_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/trial_balance.py` & `lusid_sdk-2.0.96b0/lusid/models/trial_balance.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/trial_balance_query_parameters.py` & `lusid_sdk-2.0.96b0/lusid/models/trial_balance_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/trigger_event.py` & `lusid_sdk-2.0.96b0/lusid/models/trigger_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/typed_resource_id.py` & `lusid_sdk-2.0.96b0/lusid/models/typed_resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/unit_schema.py` & `lusid_sdk-2.0.96b0/lusid/models/unit_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/unmatched_holding_method.py` & `lusid_sdk-2.0.96b0/lusid/models/unmatched_holding_method.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_calendar_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_calendar_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_custom_entity_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_custom_entity_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_custom_entity_type_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_custom_entity_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_cut_label_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_cut_label_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_data_type_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_data_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_derived_property_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_derived_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_instrument_identifier_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_instrument_identifier_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_portfolio_group_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_portfolio_group_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_portfolio_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_property_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_relationship_definition_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_relationship_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_tax_rule_set_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_tax_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/update_unit_request.py` & `lusid_sdk-2.0.96b0/lusid/models/update_unit_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_cds_flow_conventions_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_cds_flow_conventions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_complex_market_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_complex_market_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_compliance_rule_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_compliance_rule_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_compliance_run_summary_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_compliance_run_summary_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_corporate_action_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_corporate_action_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_corporate_actions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_corporate_actions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_counterparty_agreement_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_counterparty_agreement_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_credit_support_annex_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_credit_support_annex_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_custom_entities_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_custom_entities_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_custom_entity_access_metadata_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_custom_entity_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_flow_conventions_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_flow_conventions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_index_convention_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_index_convention_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_event_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_event_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_events_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_events_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_properties_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_instrument_property_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_instrument_property_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_instruments_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_instruments_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_legal_entities_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_legal_entities_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_legal_entity_access_metadata_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_legal_entity_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_legal_entity_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_legal_entity_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_person_access_metadata_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_person_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_person_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_person_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_portfolio_access_metadata_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_portfolio_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_portfolio_group_access_metadata_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_portfolio_group_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_portfolio_transactions_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_portfolio_transactions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_quote_access_metadata_rule_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_quote_access_metadata_rule_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_quote_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_quote_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_quotes_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_quotes_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_recipe_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_recipe_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_reconciliation_break_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_reconciliation_break_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_reconciliation_run_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_reconciliation_run_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_reference_portfolio_constituents_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_reference_portfolio_constituents_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_reference_portfolio_constituents_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_reference_portfolio_constituents_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_result_values_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_result_values_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_returns_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_returns_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_single_structured_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_single_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_structured_data_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_structured_result_data_request.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_structured_result_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/upsert_transaction_properties_response.py` & `lusid_sdk-2.0.96b0/lusid/models/upsert_transaction_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/user.py` & `lusid_sdk-2.0.96b0/lusid/models/user.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/valuation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/valuation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/valuation_schedule.py` & `lusid_sdk-2.0.96b0/lusid/models/valuation_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/valuations_reconciliation_request.py` & `lusid_sdk-2.0.96b0/lusid/models/valuations_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/value_type.py` & `lusid_sdk-2.0.96b0/lusid/models/value_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/vendor_dependency.py` & `lusid_sdk-2.0.96b0/lusid/models/vendor_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/vendor_library.py` & `lusid_sdk-2.0.96b0/lusid/models/vendor_library.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/vendor_model_rule.py` & `lusid_sdk-2.0.96b0/lusid/models/vendor_model_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/version.py` & `lusid_sdk-2.0.96b0/lusid/models/version.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/version_summary_dto.py` & `lusid_sdk-2.0.96b0/lusid/models/version_summary_dto.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_a2_b_data_record.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_a2_b_data_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_a2_b_movement_record.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_a2_b_movement_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_holding_contributor.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_holding_contributor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_journal_entry_line.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_journal_entry_line.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_output_transaction.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_output_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_portfolio_holding.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_portfolio_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_transaction.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_of_trial_balance.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_of_trial_balance.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py` & `lusid_sdk-2.0.96b0/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/virtual_document.py` & `lusid_sdk-2.0.96b0/lusid/models/virtual_document.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/virtual_document_row.py` & `lusid_sdk-2.0.96b0/lusid/models/virtual_document_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/virtual_row.py` & `lusid_sdk-2.0.96b0/lusid/models/virtual_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/warning.py` & `lusid_sdk-2.0.96b0/lusid/models/warning.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/weekend_mask.py` & `lusid_sdk-2.0.96b0/lusid/models/weekend_mask.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/weighted_instrument.py` & `lusid_sdk-2.0.96b0/lusid/models/weighted_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/weighted_instruments.py` & `lusid_sdk-2.0.96b0/lusid/models/weighted_instruments.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/models/yield_curve_data.py` & `lusid_sdk-2.0.96b0/lusid/models/yield_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/lusid/rest.py` & `lusid_sdk-2.0.96b0/lusid/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.0.90b0/pyproject.toml` & `lusid_sdk-2.0.96b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-sdk"
-version = "2.0.90-beta"
+version = "2.0.96-beta"
 description = "LUSID API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/lusid-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "LUSID API", "lusid-sdk"]
 packages = [
```

### Comparing `lusid_sdk-2.0.90b0/PKG-INFO` & `lusid_sdk-2.0.96b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-sdk
-Version: 2.0.90b0
+Version: 2.0.96b0
 Summary: LUSID API
 Home-page: https://github.com/finbourne/lusid-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,LUSID API,lusid-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.11.6039
-- Package version: 2.0.90-beta
+- API version: 0.11.6045
+- Package version: 2.0.96-beta
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

