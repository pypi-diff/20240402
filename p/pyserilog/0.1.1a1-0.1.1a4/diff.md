# Comparing `tmp/pyserilog-0.1.1a1.tar.gz` & `tmp/pyserilog-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserilog-0.1.1a1.tar", last modified: Sat Mar 30 06:46:32 2024, max compression
+gzip compressed data, was "pyserilog-0.1.1a4.tar", last modified: Sat Mar 30 07:05:49 2024, max compression
```

## Comparing `pyserilog-0.1.1a1.tar` & `pyserilog-0.1.1a4.tar`

### file list

```diff
@@ -1,132 +1,135 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.606944 pyserilog-0.1.1a1/
--rw-rw-rw-   0        0        0      605 2024-03-30 06:46:32.606944 pyserilog-0.1.1a1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-26 13:30:38.000000 pyserilog-0.1.1a1/README.rst
--rw-rw-rw-   0        0        0      139 2023-03-26 14:18:10.000000 pyserilog-0.1.1a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 06:46:32.607950 pyserilog-0.1.1a1/setup.cfg
--rw-rw-rw-   0        0        0     1585 2024-03-30 06:44:31.000000 pyserilog-0.1.1a1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.506083 pyserilog-0.1.1a1/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.519584 pyserilog-0.1.1a1/src/pyserilog/
--rw-rw-rw-   0        0        0     5466 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/src/pyserilog/ILogger.py
--rw-rw-rw-   0        0        0       97 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.527889 pyserilog-0.1.1a1/src/pyserilog/capturing/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/capturing/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/capturing/depth_limiter.py
--rw-rw-rw-   0        0        0      750 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/capturing/iproperty_value_converter.py
--rw-rw-rw-   0        0        0     1606 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/capturing/message_template_processor.py
--rw-rw-rw-   0        0        0     3672 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/capturing/property_binder.py
--rw-rw-rw-   0        0        0     9550 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/src/pyserilog/capturing/property_value_converter.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.536781 pyserilog-0.1.1a1/src/pyserilog/configuration/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/__init__.py
--rw-rw-rw-   0        0        0      250 2024-03-30 06:04:20.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/ilogger_settings.py
--rw-rw-rw-   0        0        0     1235 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_audit_sink_configuration.py
--rw-rw-rw-   0        0        0     5348 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_destructuring_configuration.py
--rw-rw-rw-   0        0        0     3890 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_enrichment_configuration.py
--rw-rw-rw-   0        0        0     1489 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_filter_configuration.py
--rw-rw-rw-   0        0        0     3621 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_minimum_level_configuration.py
--rw-rw-rw-   0        0        0     1175 2023-03-25 11:29:43.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_settings_configuration.py
--rw-rw-rw-   0        0        0     5520 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/configuration/logger_sink_configuration.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.548960 pyserilog-0.1.1a1/src/pyserilog/core/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/__init__.py
--rw-rw-rw-   0        0        0       70 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.552960 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/__init__.py
--rw-rw-rw-   0        0        0      847 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/conditional_enricher.py
--rw-rw-rw-   0        0        0      345 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/empty_enricher.py
--rw-rw-rw-   0        0        0      641 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/fixed_property_enricher.py
--rw-rw-rw-   0        0        0      905 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/property_enricher.py
--rw-rw-rw-   0        0        0      760 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/enrichers/safe_aggregate_enricher.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.554960 pyserilog-0.1.1a1/src/pyserilog/core/filter/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/filter/__init__.py
--rw-rw-rw-   0        0        0      407 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/filter/delegate_filter.py
--rw-rw-rw-   0        0        0      435 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/idestructuring_policy.py
--rw-rw-rw-   0        0        0      329 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_enricher.py
--rw-rw-rw-   0        0        0      534 2023-03-26 10:16:09.000000 pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_filter.py
--rw-rw-rw-   0        0        0      733 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_property_factory.py
--rw-rw-rw-   0        0        0      305 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_property_value_factory.py
--rw-rw-rw-   0        0        0      198 2023-03-26 07:23:10.000000 pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_sink.py
--rw-rw-rw-   0        0        0      228 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/imessage_template_parser.py
--rw-rw-rw-   0        0        0      250 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/iscalar_conversion_policy.py
--rw-rw-rw-   0        0        0     1876 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/core/level_override_map.py
--rw-rw-rw-   0        0        0     5728 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/src/pyserilog/core/logger.py
--rw-rw-rw-   0        0        0      520 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/logging_level_switch.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.556960 pyserilog-0.1.1a1/src/pyserilog/core/pipeline/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1692 2023-03-25 13:14:23.000000 pyserilog-0.1.1a1/src/pyserilog/core/pipeline/message_template_cache.py
--rw-rw-rw-   0        0        0     2289 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/src/pyserilog/core/pipeline/silet_logger.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.564963 pyserilog-0.1.1a1/src/pyserilog/core/sinks/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/__init__.py
--rw-rw-rw-   0        0        0      852 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/aggregate_sink.py
--rw-rw-rw-   0        0        0      680 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/conditional_sink.py
--rw-rw-rw-   0        0        0      643 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/dispose_delegating_sink.py
--rw-rw-rw-   0        0        0     1193 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/disposing_aggregate_sink.py
--rw-rw-rw-   0        0        0      912 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/filtering_sink.py
--rw-rw-rw-   0        0        0      875 2023-03-27 16:34:12.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/restricted_sink.py
--rw-rw-rw-   0        0        0      621 2023-03-26 07:21:43.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/safe_aggregate_sink.py
--rw-rw-rw-   0        0        0      841 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/src/pyserilog/core/sinks/secondary_logger_sink.py
--rw-rw-rw-   0        0        0      869 2023-03-27 16:18:04.000000 pyserilog-0.1.1a1/src/pyserilog/core/string_writable.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.567960 pyserilog-0.1.1a1/src/pyserilog/data/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/data/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/data/log_event_property_value_rewriter.py
--rw-rw-rw-   0        0        0     1878 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/data/log_event_property_value_visitor.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.568961 pyserilog-0.1.1a1/src/pyserilog/debuging/
--rw-rw-rw-   0        0        0       47 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/debuging/__init__.py
--rw-rw-rw-   0        0        0      802 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/debuging/self_log.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.580942 pyserilog-0.1.1a1/src/pyserilog/events/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/events/__init__.py
--rw-rw-rw-   0        0        0     1039 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/dictionary_value.py
--rw-rw-rw-   0        0        0      740 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/events/event_property.py
--rw-rw-rw-   0        0        0      187 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/events/level_alias.py
--rw-rw-rw-   0        0        0     3491 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/log_event.py
--rw-rw-rw-   0        0        0     1741 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/events/log_event_level.py
--rw-rw-rw-   0        0        0     1049 2023-03-27 16:35:17.000000 pyserilog-0.1.1a1/src/pyserilog/events/log_event_property.py
--rw-rw-rw-   0        0        0      548 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/log_event_property_value.py
--rw-rw-rw-   0        0        0     2746 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/message_template.py
--rw-rw-rw-   0        0        0      294 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/events/property_utils.py
--rw-rw-rw-   0        0        0     1558 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/scalar_value.py
--rw-rw-rw-   0        0        0     1015 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/sequence_value.py
--rw-rw-rw-   0        0        0     1550 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/events/structure_value.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.581942 pyserilog-0.1.1a1/src/pyserilog/filters/
--rw-rw-rw-   0        0        0     1724 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/filters/matching.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.583944 pyserilog-0.1.1a1/src/pyserilog/formatting/
--rw-rw-rw-   0        0        0       65 2023-03-25 10:14:06.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.587943 pyserilog-0.1.1a1/src/pyserilog/formatting/display/
--rw-rw-rw-   0        0        0     3302 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/display/level_output_format.py
--rw-rw-rw-   0        0        0     3639 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/display/message_template_text_formatter.py
--rw-rw-rw-   0        0        0      301 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/display/output_properties.py
--rw-rw-rw-   0        0        0     2240 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/display/properties_output_format.py
--rw-rw-rw-   0        0        0      227 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/itext_formatter.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.590942 pyserilog-0.1.1a1/src/pyserilog/formatting/json/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/json/__init__.py
--rw-rw-rw-   0        0        0     6172 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/json/json_formatter.py
--rw-rw-rw-   0        0        0     7980 2023-03-27 16:35:17.000000 pyserilog-0.1.1a1/src/pyserilog/formatting/json/json_value_formatter.py
--rw-rw-rw-   0        0        0      194 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/guard.py
--rw-rw-rw-   0        0        0     9312 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/logger_configuration.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.596943 pyserilog-0.1.1a1/src/pyserilog/parsing/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/__init__.py
--rw-rw-rw-   0        0        0      879 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/alignment.py
--rw-rw-rw-   0        0        0      529 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/destructuring.py
--rw-rw-rw-   0        0        0     9212 2023-03-27 16:18:03.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/message_template_parser.py
--rw-rw-rw-   0        0        0      477 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/message_template_token.py
--rw-rw-rw-   0        0        0     2310 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/property_token.py
--rw-rw-rw-   0        0        0      802 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/parsing/text_token.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.598942 pyserilog-0.1.1a1/src/pyserilog/policies/
--rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/policies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.600943 pyserilog-0.1.1a1/src/pyserilog/rendering/
--rw-rw-rw-   0        0        0      291 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/rendering/casing.py
--rw-rw-rw-   0        0        0     2910 2023-03-27 16:33:55.000000 pyserilog-0.1.1a1/src/pyserilog/rendering/message_template_renderer.py
--rw-rw-rw-   0        0        0      674 2023-03-27 16:33:54.000000 pyserilog-0.1.1a1/src/pyserilog/rendering/padding.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.513087 pyserilog-0.1.1a1/src/pyserilog/settings/
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.604942 pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/
--rw-rw-rw-   0        0        0     1642 2023-03-26 11:28:32.000000 pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/callable_configuration_method_finder.py
--rw-rw-rw-   0        0        0    13526 2023-03-26 15:34:32.000000 pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/key_value_pair_settings.py
--rw-rw-rw-   0        0        0     1652 2023-03-25 10:33:57.000000 pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/setting_value_conversions.py
--rw-rw-rw-   0        0        0     3661 2023-03-26 11:39:21.000000 pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
--rw-rw-rw-   0        0        0      298 2023-03-25 04:26:11.000000 pyserilog-0.1.1a1/src/pyserilog/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.523217 pyserilog-0.1.1a1/src/pyserilog.egg-info/
--rw-rw-rw-   0        0        0      605 2024-03-30 06:46:32.000000 pyserilog-0.1.1a1/src/pyserilog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4653 2024-03-30 06:46:32.000000 pyserilog-0.1.1a1/src/pyserilog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 06:46:32.000000 pyserilog-0.1.1a1/src/pyserilog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-03-30 06:46:32.000000 pyserilog-0.1.1a1/src/pyserilog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 06:46:32.000000 pyserilog-0.1.1a1/src/pyserilog.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-30 06:46:32.605943 pyserilog-0.1.1a1/test/
--rw-rw-rw-   0        0        0    25947 2024-03-30 05:50:58.000000 pyserilog-0.1.1a1/test/test_logger_configuration.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.949039 pyserilog-0.1.1a4/
+-rw-rw-rw-   0        0        0      605 2024-03-30 07:05:49.948511 pyserilog-0.1.1a4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-26 13:30:38.000000 pyserilog-0.1.1a4/README.rst
+-rw-rw-rw-   0        0        0      139 2023-03-26 14:18:10.000000 pyserilog-0.1.1a4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-30 07:05:49.949039 pyserilog-0.1.1a4/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2024-03-30 07:05:16.000000 pyserilog-0.1.1a4/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.845737 pyserilog-0.1.1a4/src/
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.861731 pyserilog-0.1.1a4/src/pyserilog/
+-rw-rw-rw-   0        0        0       97 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.872093 pyserilog-0.1.1a4/src/pyserilog/capturing/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/capturing/__init__.py
+-rw-rw-rw-   0        0        0     2211 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/capturing/depth_limiter.py
+-rw-rw-rw-   0        0        0      750 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/capturing/iproperty_value_converter.py
+-rw-rw-rw-   0        0        0     1606 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/capturing/message_template_processor.py
+-rw-rw-rw-   0        0        0     3672 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/capturing/property_binder.py
+-rw-rw-rw-   0        0        0     9550 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/capturing/property_value_converter.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.881505 pyserilog-0.1.1a4/src/pyserilog/configuration/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/__init__.py
+-rw-rw-rw-   0        0        0      250 2024-03-30 06:04:20.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/ilogger_settings.py
+-rw-rw-rw-   0        0        0     1235 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_audit_sink_configuration.py
+-rw-rw-rw-   0        0        0     5348 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_destructuring_configuration.py
+-rw-rw-rw-   0        0        0     3890 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_enrichment_configuration.py
+-rw-rw-rw-   0        0        0     1489 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_filter_configuration.py
+-rw-rw-rw-   0        0        0     3621 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_minimum_level_configuration.py
+-rw-rw-rw-   0        0        0     1175 2023-03-25 11:29:43.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_settings_configuration.py
+-rw-rw-rw-   0        0        0     5520 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/configuration/logger_sink_configuration.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.894357 pyserilog-0.1.1a4/src/pyserilog/core/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/constants.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.899534 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/__init__.py
+-rw-rw-rw-   0        0        0      847 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/conditional_enricher.py
+-rw-rw-rw-   0        0        0      345 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/empty_enricher.py
+-rw-rw-rw-   0        0        0      641 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/fixed_property_enricher.py
+-rw-rw-rw-   0        0        0      905 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/property_enricher.py
+-rw-rw-rw-   0        0        0      760 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/enrichers/safe_aggregate_enricher.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.900575 pyserilog-0.1.1a4/src/pyserilog/core/filter/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/filter/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/filter/delegate_filter.py
+-rw-rw-rw-   0        0        0      435 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/idestructuring_policy.py
+-rw-rw-rw-   0        0        0      329 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_enricher.py
+-rw-rw-rw-   0        0        0      534 2023-03-26 10:16:09.000000 pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_filter.py
+-rw-rw-rw-   0        0        0      733 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_property_factory.py
+-rw-rw-rw-   0        0        0      305 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_property_value_factory.py
+-rw-rw-rw-   0        0        0      198 2023-03-26 07:23:10.000000 pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_sink.py
+-rw-rw-rw-   0        0        0      228 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/imessage_template_parser.py
+-rw-rw-rw-   0        0        0      250 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/iscalar_conversion_policy.py
+-rw-rw-rw-   0        0        0     1876 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/core/level_override_map.py
+-rw-rw-rw-   0        0        0     5728 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/core/logger.py
+-rw-rw-rw-   0        0        0      520 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/logging_level_switch.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.902654 pyserilog-0.1.1a4/src/pyserilog/core/pipeline/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-03-25 13:14:23.000000 pyserilog-0.1.1a4/src/pyserilog/core/pipeline/message_template_cache.py
+-rw-rw-rw-   0        0        0     2289 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/core/pipeline/silet_logger.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.909905 pyserilog-0.1.1a4/src/pyserilog/core/sinks/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/__init__.py
+-rw-rw-rw-   0        0        0      852 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/aggregate_sink.py
+-rw-rw-rw-   0        0        0      680 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/conditional_sink.py
+-rw-rw-rw-   0        0        0      643 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/dispose_delegating_sink.py
+-rw-rw-rw-   0        0        0     1193 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/disposing_aggregate_sink.py
+-rw-rw-rw-   0        0        0      912 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/filtering_sink.py
+-rw-rw-rw-   0        0        0      875 2023-03-27 16:34:12.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/restricted_sink.py
+-rw-rw-rw-   0        0        0      621 2023-03-26 07:21:43.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/safe_aggregate_sink.py
+-rw-rw-rw-   0        0        0      841 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/core/sinks/secondary_logger_sink.py
+-rw-rw-rw-   0        0        0      869 2023-03-27 16:18:04.000000 pyserilog-0.1.1a4/src/pyserilog/core/string_writable.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.912006 pyserilog-0.1.1a4/src/pyserilog/data/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/data/__init__.py
+-rw-rw-rw-   0        0        0     3113 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/data/log_event_property_value_rewriter.py
+-rw-rw-rw-   0        0        0     1878 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/data/log_event_property_value_visitor.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.913030 pyserilog-0.1.1a4/src/pyserilog/debuging/
+-rw-rw-rw-   0        0        0       47 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/debuging/__init__.py
+-rw-rw-rw-   0        0        0      802 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/debuging/self_log.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.922321 pyserilog-0.1.1a4/src/pyserilog/events/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/events/__init__.py
+-rw-rw-rw-   0        0        0     1039 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/dictionary_value.py
+-rw-rw-rw-   0        0        0      740 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/events/event_property.py
+-rw-rw-rw-   0        0        0      187 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/events/level_alias.py
+-rw-rw-rw-   0        0        0     3491 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/log_event.py
+-rw-rw-rw-   0        0        0     1741 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/events/log_event_level.py
+-rw-rw-rw-   0        0        0     1049 2023-03-27 16:35:17.000000 pyserilog-0.1.1a4/src/pyserilog/events/log_event_property.py
+-rw-rw-rw-   0        0        0      548 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/log_event_property_value.py
+-rw-rw-rw-   0        0        0     2746 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/message_template.py
+-rw-rw-rw-   0        0        0      294 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/events/property_utils.py
+-rw-rw-rw-   0        0        0     1558 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/scalar_value.py
+-rw-rw-rw-   0        0        0     1015 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/sequence_value.py
+-rw-rw-rw-   0        0        0     1550 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/events/structure_value.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.923352 pyserilog-0.1.1a4/src/pyserilog/filters/
+-rw-rw-rw-   0        0        0     1724 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/filters/matching.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.924379 pyserilog-0.1.1a4/src/pyserilog/formatting/
+-rw-rw-rw-   0        0        0       65 2023-03-25 10:14:06.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.927491 pyserilog-0.1.1a4/src/pyserilog/formatting/display/
+-rw-rw-rw-   0        0        0     3302 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/display/level_output_format.py
+-rw-rw-rw-   0        0        0     3639 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/display/message_template_text_formatter.py
+-rw-rw-rw-   0        0        0      301 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/display/output_properties.py
+-rw-rw-rw-   0        0        0     2240 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/display/properties_output_format.py
+-rw-rw-rw-   0        0        0      227 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/itext_formatter.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.929568 pyserilog-0.1.1a4/src/pyserilog/formatting/json/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/json/__init__.py
+-rw-rw-rw-   0        0        0     6172 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/json/json_formatter.py
+-rw-rw-rw-   0        0        0     7980 2023-03-27 16:35:17.000000 pyserilog-0.1.1a4/src/pyserilog/formatting/json/json_value_formatter.py
+-rw-rw-rw-   0        0        0      194 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/guard.py
+-rw-rw-rw-   0        0        0     5466 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/ilogger.py
+-rw-rw-rw-   0        0        0     9312 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/logger_configuration.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.935755 pyserilog-0.1.1a4/src/pyserilog/parsing/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/__init__.py
+-rw-rw-rw-   0        0        0      879 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/alignment.py
+-rw-rw-rw-   0        0        0      529 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/destructuring.py
+-rw-rw-rw-   0        0        0     9212 2023-03-27 16:18:03.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/message_template_parser.py
+-rw-rw-rw-   0        0        0      477 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/message_template_token.py
+-rw-rw-rw-   0        0        0     2310 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/property_token.py
+-rw-rw-rw-   0        0        0      802 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/parsing/text_token.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.941056 pyserilog-0.1.1a4/src/pyserilog/policies/
+-rw-rw-rw-   0        0        0        0 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/policies/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/policies/byte_array_scalar_conversion_policy.py
+-rw-rw-rw-   0        0        0     1128 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/policies/projected_destruction_policy.py
+-rw-rw-rw-   0        0        0      638 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/policies/reflection_types_scalar_destructuring_policy.py
+-rw-rw-rw-   0        0        0      490 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/policies/simple_scalar_conversion_policy.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.943193 pyserilog-0.1.1a4/src/pyserilog/rendering/
+-rw-rw-rw-   0        0        0      291 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/rendering/casing.py
+-rw-rw-rw-   0        0        0     2910 2023-03-27 16:33:55.000000 pyserilog-0.1.1a4/src/pyserilog/rendering/message_template_renderer.py
+-rw-rw-rw-   0        0        0      674 2023-03-27 16:33:54.000000 pyserilog-0.1.1a4/src/pyserilog/rendering/padding.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.944272 pyserilog-0.1.1a4/src/pyserilog/settings/
+-rw-rw-rw-   0        0        0        0 2024-03-30 05:50:58.000000 pyserilog-0.1.1a4/src/pyserilog/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.947458 pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/
+-rw-rw-rw-   0        0        0     1642 2023-03-26 11:28:32.000000 pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/callable_configuration_method_finder.py
+-rw-rw-rw-   0        0        0    13526 2023-03-26 15:34:32.000000 pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/key_value_pair_settings.py
+-rw-rw-rw-   0        0        0     1652 2023-03-25 10:33:57.000000 pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/setting_value_conversions.py
+-rw-rw-rw-   0        0        0     3661 2023-03-26 11:39:21.000000 pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
+-rw-rw-rw-   0        0        0      298 2023-03-25 04:26:11.000000 pyserilog-0.1.1a4/src/pyserilog/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-30 07:05:49.866917 pyserilog-0.1.1a4/src/pyserilog.egg-info/
+-rw-rw-rw-   0        0        0      605 2024-03-30 07:05:49.000000 pyserilog-0.1.1a4/src/pyserilog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4900 2024-03-30 07:05:49.000000 pyserilog-0.1.1a4/src/pyserilog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-30 07:05:49.000000 pyserilog-0.1.1a4/src/pyserilog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-03-30 07:05:49.000000 pyserilog-0.1.1a4/src/pyserilog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-30 07:05:49.000000 pyserilog-0.1.1a4/src/pyserilog.egg-info/top_level.txt
```

### Comparing `pyserilog-0.1.1a1/PKG-INFO` & `pyserilog-0.1.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserilog
-Version: 0.1.1a1
+Version: 0.1.1a4
 Summary: python version of serilog a structured logging library
 Home-page: UNKNOWN
 Author: Reza Sadeghi
 Author-email: rezasadeghikhas@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyserilog-0.1.1a1/setup.py` & `pyserilog-0.1.1a4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 https://github.com/pypa/sampleproject
 """
 
 # To use a consistent encoding
 from codecs import open
 
 # Always prefer setuptools over distutils
-from setuptools import setup
+from setuptools import setup, find_namespace_packages
 
 # Get the long description from the README file
 with open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
+packages = find_namespace_packages(where="./src", include=["pyserilog" , "pyserilog.*"], exclude=["tests", "tests.*"])
 setup(
     name="pyserilog",
 
-    version="0.1.1a1",
+    version="0.1.1a4",
 
     description="python version of serilog a structured logging library",
     long_description=long_description,
     author='Reza Sadeghi',
     author_email='rezasadeghikhas@gmail.com',
     license="Apache2",
 
@@ -45,10 +46,11 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3.11',
     ],
 
     package_dir={"": "src"},
     install_requires=[
         "multipledispatch==0.6.0"
-    ]
+    ],
+    packages=packages
 
 )
```

### Comparing `pyserilog-0.1.1a1/src/pyserilog/ILogger.py` & `pyserilog-0.1.1a4/src/pyserilog/ilogger.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/capturing/depth_limiter.py` & `pyserilog-0.1.1a4/src/pyserilog/capturing/depth_limiter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/capturing/iproperty_value_converter.py` & `pyserilog-0.1.1a4/src/pyserilog/capturing/iproperty_value_converter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/capturing/message_template_processor.py` & `pyserilog-0.1.1a4/src/pyserilog/capturing/message_template_processor.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/capturing/property_binder.py` & `pyserilog-0.1.1a4/src/pyserilog/capturing/property_binder.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/capturing/property_value_converter.py` & `pyserilog-0.1.1a4/src/pyserilog/capturing/property_value_converter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_audit_sink_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_audit_sink_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_destructuring_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_destructuring_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_enrichment_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_enrichment_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_filter_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_filter_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_minimum_level_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_minimum_level_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_settings_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_settings_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/configuration/logger_sink_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/configuration/logger_sink_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/enrichers/conditional_enricher.py` & `pyserilog-0.1.1a4/src/pyserilog/core/enrichers/conditional_enricher.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/enrichers/fixed_property_enricher.py` & `pyserilog-0.1.1a4/src/pyserilog/core/enrichers/fixed_property_enricher.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/enrichers/property_enricher.py` & `pyserilog-0.1.1a4/src/pyserilog/core/enrichers/property_enricher.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/enrichers/safe_aggregate_enricher.py` & `pyserilog-0.1.1a4/src/pyserilog/core/enrichers/safe_aggregate_enricher.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_filter.py` & `pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/ilog_event_property_factory.py` & `pyserilog-0.1.1a4/src/pyserilog/core/ilog_event_property_factory.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/level_override_map.py` & `pyserilog-0.1.1a4/src/pyserilog/core/level_override_map.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/logger.py` & `pyserilog-0.1.1a4/src/pyserilog/core/logger.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/logging_level_switch.py` & `pyserilog-0.1.1a4/src/pyserilog/core/logging_level_switch.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/pipeline/message_template_cache.py` & `pyserilog-0.1.1a4/src/pyserilog/core/pipeline/message_template_cache.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/pipeline/silet_logger.py` & `pyserilog-0.1.1a4/src/pyserilog/core/pipeline/silet_logger.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/aggregate_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/aggregate_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/conditional_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/conditional_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/dispose_delegating_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/dispose_delegating_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/disposing_aggregate_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/disposing_aggregate_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/filtering_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/filtering_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/restricted_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/restricted_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/safe_aggregate_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/safe_aggregate_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/sinks/secondary_logger_sink.py` & `pyserilog-0.1.1a4/src/pyserilog/core/sinks/secondary_logger_sink.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/core/string_writable.py` & `pyserilog-0.1.1a4/src/pyserilog/core/string_writable.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/data/log_event_property_value_rewriter.py` & `pyserilog-0.1.1a4/src/pyserilog/data/log_event_property_value_rewriter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/data/log_event_property_value_visitor.py` & `pyserilog-0.1.1a4/src/pyserilog/data/log_event_property_value_visitor.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/debuging/self_log.py` & `pyserilog-0.1.1a4/src/pyserilog/debuging/self_log.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/dictionary_value.py` & `pyserilog-0.1.1a4/src/pyserilog/events/dictionary_value.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/event_property.py` & `pyserilog-0.1.1a4/src/pyserilog/events/event_property.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/log_event.py` & `pyserilog-0.1.1a4/src/pyserilog/events/log_event.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/log_event_level.py` & `pyserilog-0.1.1a4/src/pyserilog/events/log_event_level.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/log_event_property.py` & `pyserilog-0.1.1a4/src/pyserilog/events/log_event_property.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/log_event_property_value.py` & `pyserilog-0.1.1a4/src/pyserilog/events/log_event_property_value.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/message_template.py` & `pyserilog-0.1.1a4/src/pyserilog/events/message_template.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/scalar_value.py` & `pyserilog-0.1.1a4/src/pyserilog/events/scalar_value.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/sequence_value.py` & `pyserilog-0.1.1a4/src/pyserilog/events/sequence_value.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/events/structure_value.py` & `pyserilog-0.1.1a4/src/pyserilog/events/structure_value.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/filters/matching.py` & `pyserilog-0.1.1a4/src/pyserilog/filters/matching.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/formatting/display/level_output_format.py` & `pyserilog-0.1.1a4/src/pyserilog/formatting/display/level_output_format.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/formatting/display/message_template_text_formatter.py` & `pyserilog-0.1.1a4/src/pyserilog/formatting/display/message_template_text_formatter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/formatting/display/properties_output_format.py` & `pyserilog-0.1.1a4/src/pyserilog/formatting/display/properties_output_format.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/formatting/json/json_formatter.py` & `pyserilog-0.1.1a4/src/pyserilog/formatting/json/json_formatter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/formatting/json/json_value_formatter.py` & `pyserilog-0.1.1a4/src/pyserilog/formatting/json/json_value_formatter.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/logger_configuration.py` & `pyserilog-0.1.1a4/src/pyserilog/logger_configuration.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/parsing/alignment.py` & `pyserilog-0.1.1a4/src/pyserilog/parsing/alignment.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/parsing/destructuring.py` & `pyserilog-0.1.1a4/src/pyserilog/parsing/destructuring.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/parsing/message_template_parser.py` & `pyserilog-0.1.1a4/src/pyserilog/parsing/message_template_parser.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/parsing/property_token.py` & `pyserilog-0.1.1a4/src/pyserilog/parsing/property_token.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/parsing/text_token.py` & `pyserilog-0.1.1a4/src/pyserilog/parsing/text_token.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/rendering/message_template_renderer.py` & `pyserilog-0.1.1a4/src/pyserilog/rendering/message_template_renderer.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/rendering/padding.py` & `pyserilog-0.1.1a4/src/pyserilog/rendering/padding.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/callable_configuration_method_finder.py` & `pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/callable_configuration_method_finder.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/key_value_pair_settings.py` & `pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/key_value_pair_settings.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/setting_value_conversions.py` & `pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/setting_value_conversions.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog/settings/key_value_paies/surrogate_configuration_methods.py` & `pyserilog-0.1.1a4/src/pyserilog/settings/key_value_paies/surrogate_configuration_methods.py`

 * *Files identical despite different names*

### Comparing `pyserilog-0.1.1a1/src/pyserilog.egg-info/PKG-INFO` & `pyserilog-0.1.1a4/src/pyserilog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserilog
-Version: 0.1.1a1
+Version: 0.1.1a4
 Summary: python version of serilog a structured logging library
 Home-page: UNKNOWN
 Author: Reza Sadeghi
 Author-email: rezasadeghikhas@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyserilog-0.1.1a1/src/pyserilog.egg-info/SOURCES.txt` & `pyserilog-0.1.1a4/src/pyserilog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 README.rst
 pyproject.toml
 setup.py
-src/pyserilog/ILogger.py
 src/pyserilog/__init__.py
 src/pyserilog/guard.py
+src/pyserilog/ilogger.py
 src/pyserilog/logger_configuration.py
 src/pyserilog/utils.py
 src/pyserilog.egg-info/PKG-INFO
 src/pyserilog.egg-info/SOURCES.txt
 src/pyserilog.egg-info/dependency_links.txt
 src/pyserilog.egg-info/requires.txt
 src/pyserilog.egg-info/top_level.txt
@@ -92,15 +92,19 @@
 src/pyserilog/parsing/alignment.py
 src/pyserilog/parsing/destructuring.py
 src/pyserilog/parsing/message_template_parser.py
 src/pyserilog/parsing/message_template_token.py
 src/pyserilog/parsing/property_token.py
 src/pyserilog/parsing/text_token.py
 src/pyserilog/policies/__init__.py
+src/pyserilog/policies/byte_array_scalar_conversion_policy.py
+src/pyserilog/policies/projected_destruction_policy.py
+src/pyserilog/policies/reflection_types_scalar_destructuring_policy.py
+src/pyserilog/policies/simple_scalar_conversion_policy.py
 src/pyserilog/rendering/casing.py
 src/pyserilog/rendering/message_template_renderer.py
 src/pyserilog/rendering/padding.py
+src/pyserilog/settings/__init__.py
 src/pyserilog/settings/key_value_paies/callable_configuration_method_finder.py
 src/pyserilog/settings/key_value_paies/key_value_pair_settings.py
 src/pyserilog/settings/key_value_paies/setting_value_conversions.py
-src/pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
-test/test_logger_configuration.py
+src/pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
```

