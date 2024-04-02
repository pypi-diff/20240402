# Comparing `tmp/investing_algorithm_framework-3.2.0.tar.gz` & `tmp/investing_algorithm_framework-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-3.2.0.tar", max compression
+gzip compressed data, was "investing_algorithm_framework-3.3.0.tar", max compression
```

## Comparing `investing_algorithm_framework-3.2.0.tar` & `investing_algorithm_framework-3.3.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
--rw-r--r--   0        0        0    11343 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/LICENSE
--rw-r--r--   0        0        0    19512 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/README.md
--rw-r--r--   0        0        0     2084 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/__init__.py
--rw-r--r--   0        0        0      501 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0        0        0    35307 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0        0        0    30887 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/app.py
--rw-r--r--   0        0        0     1092 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/__init__.py
--rw-r--r--   0        0        0     2362 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0        0        0      154 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0        0        0      451 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0        0        0     1062 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0        0        0     1085 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0        0        0     3750 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0        0        0      963 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/task.py
--rw-r--r--   0        0        0      134 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/__init__.py
--rw-r--r--   0        0        0      587 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0        0        0      693 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0        0        0      727 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0        0        0      617 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0        0        0      506 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0        0        0     2020 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0        0        0      585 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0        0        0      158 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/run_strategies.py
--rw-r--r--   0        0        0      361 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0        0        0      442 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0        0        0      743 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0        0        0      437 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0        0        0       80 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0        0        0      603 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/create_app.py
--rw-r--r--   0        0        0     6206 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/dependency_container.py
--rw-r--r--   0        0        0     3866 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0        0        0     3686 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/config.py
--rw-r--r--   0        0        0     2293 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0        0        0      962 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/data_structures.py
--rw-r--r--   0        0        0      823 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/decimal_parsing.py
--rw-r--r--   0        0        0     1628 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/exceptions.py
--rw-r--r--   0        0        0     1121 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0        0        0      812 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/app_mode.py
--rw-r--r--   0        0        0      253 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
--rw-r--r--   0        0        0     2374 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
--rw-r--r--   0        0        0    13604 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
--rw-r--r--   0        0        0      674 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
--rw-r--r--   0        0        0      659 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/base_model.py
--rw-r--r--   0        0        0       87 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/market/__init__.py
--rw-r--r--   0        0        0      779 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/market/market_credential.py
--rw-r--r--   0        0        0      237 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0        0        0    10301 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0        0        0     1110 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0        0        0      814 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0        0        0      937 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0        0        0      751 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_type.py
--rw-r--r--   0        0        0      230 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0        0        0     2495 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1752 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
--rw-r--r--   0        0        0     3141 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      123 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0        0        0     1251 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0        0        0     1131 2024-03-27 19:54:45.839763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
--rw-r--r--   0        0        0     4598 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/strategy_profile.py
--rw-r--r--   0        0        0     2659 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0        0        0     2798 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0        0        0     2011 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0        0        0       99 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trade/__init__.py
--rw-r--r--   0        0        0     5533 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trade/trade.py
--rw-r--r--   0        0        0      807 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trade/trade_status.py
--rw-r--r--   0        0        0     1119 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0        0        0     6791 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0        0        0      564 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/__init__.py
--rw-r--r--   0        0        0     1047 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/market_credential_service.py
--rw-r--r--   0        0        0     9759 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/market_data_sources.py
--rw-r--r--   0        0        0     3520 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/market_service.py
--rw-r--r--   0        0        0      115 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
--rw-r--r--   0        0        0      320 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0      258 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0        0        0      156 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0        0        0     1805 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/strategy.py
--rw-r--r--   0        0        0      700 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0        0        0    10969 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/backtesting.py
--rw-r--r--   0        0        0     2746 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0        0        0      275 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0        0        0      417 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0        0        0      608 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0        0        0      253 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/synchronized.py
--rw-r--r--   0        0        0     1361 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/__init__.py
--rw-r--r--   0        0        0      176 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0        0        0     1386 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
--rw-r--r--   0        0        0      732 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      327 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
--rw-r--r--   0        0        0      437 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
--rw-r--r--   0        0        0    16664 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
--rw-r--r--   0        0        0     5815 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
--rw-r--r--   0        0        0      142 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/model_extension.py
--rw-r--r--   0        0        0      102 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0        0        0     4877 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0        0        0      847 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py
--rw-r--r--   0        0        0      141 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0        0        0     3226 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1238 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      135 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0        0        0     1898 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0        0        0      842 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
--rw-r--r--   0        0        0      567 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      487 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0        0        0     3352 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0        0        0     1073 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0        0        0     1967 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
--rw-r--r--   0        0        0     1994 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0        0        0      680 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
--rw-r--r--   0        0        0     7661 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0      163 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0        0        0       91 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
--rw-r--r--   0        0        0    14984 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
--rw-r--r--   0        0        0      195 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
--rw-r--r--   0        0        0       43 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
--rw-r--r--   0        0        0    11932 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
--rw-r--r--   0        0        0     1318 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0        0        0      191 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/backtesting/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
--rw-r--r--   0        0        0    14835 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/backtesting/backtest_service.py
--rw-r--r--   0        0        0      624 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/configuration_service.py
--rw-r--r--   0        0        0      820 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_credential_service.py
--rw-r--r--   0        0        0      235 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
--rw-r--r--   0        0        0     5212 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
--rw-r--r--   0        0        0     6267 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
--rw-r--r--   0        0        0      159 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/order_service/__init__.py
--rw-r--r--   0        0        0     7774 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
--rw-r--r--   0        0        0    27733 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/order_service/order_service.py
--rw-r--r--   0        0        0      510 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/__init__.py
--rw-r--r--   0        0        0      825 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
--rw-r--r--   0        0        0     2055 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
--rw-r--r--   0        0        0     4493 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
--rw-r--r--   0        0        0     1984 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
--rw-r--r--   0        0        0    16126 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0     1052 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0        0        0      525 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/position_snapshot_service.py
--rw-r--r--   0        0        0      995 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0        0        0     8075 2024-03-27 19:54:45.843763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0        0        0       68 2024-03-27 19:54:45.847763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/trade_service/__init__.py
--rw-r--r--   0        0        0    14833 2024-03-27 19:54:45.847763 investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/trade_service/trade_service.py
--rw-r--r--   0        0        0      742 2024-03-27 19:54:58.267926 investing_algorithm_framework-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-02 21:01:41.822444 investing_algorithm_framework-3.3.0/LICENSE
+-rw-r--r--   0        0        0    19512 2024-04-02 21:01:41.822444 investing_algorithm_framework-3.3.0/README.md
+-rw-r--r--   0        0        0     2084 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0        0        0    35307 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0        0        0    30887 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/app.py
+-rw-r--r--   0        0        0     1092 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/__init__.py
+-rw-r--r--   0        0        0     2362 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0        0        0      451 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0        0        0     1062 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0        0        0     1085 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0        0        0     3750 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0        0        0      963 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/task.py
+-rw-r--r--   0        0        0      134 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0        0        0      693 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0        0        0      727 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0        0        0      617 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0        0        0      506 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0        0        0     2020 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0        0        0      585 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0        0        0      158 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/run_strategies.py
+-rw-r--r--   0        0        0      361 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0        0        0      743 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0        0        0      437 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0        0        0       80 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0        0        0      603 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/create_app.py
+-rw-r--r--   0        0        0     6206 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/dependency_container.py
+-rw-r--r--   0        0        0     3866 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0        0        0     3686 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0        0        0     2293 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0        0        0      962 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/data_structures.py
+-rw-r--r--   0        0        0      823 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/decimal_parsing.py
+-rw-r--r--   0        0        0     1628 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/exceptions.py
+-rw-r--r--   0        0        0     1121 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/app_mode.py
+-rw-r--r--   0        0        0      253 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
+-rw-r--r--   0        0        0    13604 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
+-rw-r--r--   0        0        0      674 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
+-rw-r--r--   0        0        0      659 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/base_model.py
+-rw-r--r--   0        0        0       87 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/market/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/market/market_credential.py
+-rw-r--r--   0        0        0      237 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0        0        0    10301 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0        0        0     1110 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0        0        0      814 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0        0        0      937 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0        0        0      751 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_type.py
+-rw-r--r--   0        0        0      230 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1752 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+-rw-r--r--   0        0        0     3141 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      123 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0        0        0     1131 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
+-rw-r--r--   0        0        0     4598 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/strategy_profile.py
+-rw-r--r--   0        0        0     2659 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0        0        0     2798 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0        0        0     2011 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0        0        0       99 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/__init__.py
+-rw-r--r--   0        0        0     6819 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade.py
+-rw-r--r--   0        0        0      807 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade_status.py
+-rw-r--r--   0        0        0     1119 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0        0        0     6791 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0        0        0      564 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_credential_service.py
+-rw-r--r--   0        0        0     9759 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_data_sources.py
+-rw-r--r--   0        0        0     3520 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_service.py
+-rw-r--r--   0        0        0      115 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0      258 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0        0        0      156 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0        0        0     1805 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/strategy.py
+-rw-r--r--   0        0        0      700 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0        0        0    10969 2024-04-02 21:01:41.826444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/backtesting.py
+-rw-r--r--   0        0        0     2746 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0        0        0      275 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0        0        0      417 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0        0        0      608 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0        0        0      253 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/synchronized.py
+-rw-r--r--   0        0        0     1361 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+-rw-r--r--   0        0        0      732 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
+-rw-r--r--   0        0        0      437 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
+-rw-r--r--   0        0        0    16664 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
+-rw-r--r--   0        0        0     5472 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
+-rw-r--r--   0        0        0      142 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/model_extension.py
+-rw-r--r--   0        0        0      102 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0        0        0      847 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+-rw-r--r--   0        0        0      141 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     3226 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1238 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      135 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0        0        0      842 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
+-rw-r--r--   0        0        0      567 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      487 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0        0        0     3352 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0        0        0     1073 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0        0        0     1967 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
+-rw-r--r--   0        0        0     1994 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0        0        0      680 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
+-rw-r--r--   0        0        0     7661 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0      163 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
+-rw-r--r--   0        0        0    14984 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
+-rw-r--r--   0        0        0      195 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
+-rw-r--r--   0        0        0    11932 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
+-rw-r--r--   0        0        0     1318 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/__init__.py
+-rw-r--r--   0        0        0     1025 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
+-rw-r--r--   0        0        0    14835 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_service.py
+-rw-r--r--   0        0        0      624 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/configuration_service.py
+-rw-r--r--   0        0        0      820 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_credential_service.py
+-rw-r--r--   0        0        0      235 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
+-rw-r--r--   0        0        0     5212 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
+-rw-r--r--   0        0        0     6267 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
+-rw-r--r--   0        0        0      159 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/__init__.py
+-rw-r--r--   0        0        0     7774 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
+-rw-r--r--   0        0        0    27733 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_service.py
+-rw-r--r--   0        0        0      510 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
+-rw-r--r--   0        0        0     2055 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
+-rw-r--r--   0        0        0     4493 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
+-rw-r--r--   0        0        0     1984 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
+-rw-r--r--   0        0        0    16126 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0     1052 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0        0        0      525 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_snapshot_service.py
+-rw-r--r--   0        0        0      995 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0        0        0     8075 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0        0        0       68 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/trade_service/__init__.py
+-rw-r--r--   0        0        0    14625 2024-04-02 21:01:41.830444 investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/trade_service/trade_service.py
+-rw-r--r--   0        0        0      742 2024-04-02 21:01:53.826645 investing_algorithm_framework-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.3.0/PKG-INFO
```

### Comparing `investing_algorithm_framework-3.2.0/LICENSE` & `investing_algorithm_framework-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/README.md` & `investing_algorithm_framework-3.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -143,50 +143,50 @@
 * Start date: 2023-08-24 00:00:00
 * End date: 2023-12-02 00:00:00
 * Number of days: 100
 * Number of runs: 1201
 ====================Portfolio overview============================
 * Number of orders: 10
 * Initial balance: 400.0000 EUR
-* Final balance: 426.7818 EUR
-* Total net gain: 23.4238 EUR
-* Total net gain percentage: 5.8560%
-* Growth rate: 6.6955%
-* Growth 26.7818 EUR
+* Final balance: 431.8837 EUR
+* Total net gain: 28.4171 EUR
+* Total net gain percentage: 7.1043%
+* Growth rate: 7.9709%
+* Growth 31.8837 EUR
 ====================Positions overview========================
 ╭────────────┬──────────┬──────────────────────┬───────────────────────┬──────────────┬───────────────┬───────────────────────────┬────────────────┬───────────────╮
 │ Position   │   Amount │   Pending buy amount │   Pending sell amount │   Cost (EUR) │   Value (EUR) │ Percentage of portfolio   │   Growth (EUR) │ Growth_rate   │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ EUR        │ 213.928  │                    0 │                     0 │      213.928 │       213.928 │ 50.1259%                  │         0      │ 0.0000%       │
+│ EUR        │ 214.219  │                    0 │                     0 │      214.219 │       214.219 │ 49.6010%                  │         0      │ 0.0000%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ BTC        │   0.003  │                    0 │                     0 │      103.64  │       106.84  │ 25.0338%                  │         3.1999 │ 3.0875%       │
+│ BTC        │   0.0031 │                    0 │                     0 │      107.095 │       110.401 │ 25.5627%                  │         3.3066 │ 3.0875%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ DOT        │  21.0805 │                    0 │                     0 │      105.856 │       106.014 │ 24.8403%                  │         0.1581 │ 0.1494%       │
+│ DOT        │  21.3291 │                    0 │                     0 │      107.104 │       107.264 │ 24.8363%                  │         0.16   │ 0.1494%       │
 ╰────────────┴──────────┴──────────────────────┴───────────────────────┴──────────────┴───────────────┴───────────────────────────┴────────────────┴───────────────╯
 ====================Trades overview===========================
 * Number of trades closed: 4
 * Number of trades open: 2
 * Percentage of positive trades: 60.0%
 * Percentage of negative trades: 20.0%
 * Average trade size: 98.8728 EUR
-* Average trade duration: 191.0 hours
+* Average trade duration: 183.5 hours
 ╭─────────┬─────────────────────┬─────────────────────┬────────────────────┬──────────────┬──────────────────┬───────────────────────┬────────────────────┬─────────────────────╮
 │ Pair    │ Open date           │ Close date          │   Duration (hours) │   Size (EUR) │   Net gain (EUR) │ Net gain percentage   │   Open price (EUR) │   Close price (EUR) │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-11-30 20:00:00 │                     │            2802.99 │     105.856  │           0      │ 0.0000%               │             5.0215 │                     │
+│ DOT-EUR │ 2023-11-30 20:00:00 │                     │            2976.65 │     107.104  │           0      │ 0.0000%               │             5.0215 │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-29 14:00:00 │                     │            2832.99 │     103.64   │           0      │ 0.0000%               │         34546.6    │                     │
+│ BTC-EUR │ 2023-11-29 14:00:00 │                     │            3006.65 │     107.095  │           0      │ 0.0000%               │         34546.6    │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-08 00:00:00 │ 2023-11-14 16:00:00 │             160    │      99.2265 │           1.3352 │ 1.3456%               │         33075.5    │           33520.6   │
+│ BTC-EUR │ 2023-11-08 00:00:00 │ 2023-11-14 16:00:00 │             160    │      99.2265 │           1.3352 │ 1.3456%               │         33075.5    │          33520.6    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-06 16:00:00 │ 2023-11-06 20:00:00 │               4    │      97.8607 │          -0.0026 │ -0.0026%              │         32620.2    │           32619.4   │
+│ BTC-EUR │ 2023-11-06 16:00:00 │ 2023-11-06 20:00:00 │               4    │      97.8607 │          -0.0026 │ -0.0026%              │         32620.2    │          32619.4    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-10-30 06:00:00 │ 2023-11-15 06:00:00 │             384    │     100.551  │          19.8861 │ 19.7771%              │             4.0375 │               4.836 │
+│ DOT-EUR │ 2023-10-30 06:00:00 │ 2023-11-14 00:00:00 │             354    │     100.551  │          24.8794 │ 24.7430%              │             4.0375 │              5.0365 │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-09-13 16:00:00 │ 2023-09-22 16:00:00 │             216    │      97.8529 │           2.2051 │ 2.2534%               │         24463.2    │           25014.5   │
+│ BTC-EUR │ 2023-09-13 16:00:00 │ 2023-09-22 16:00:00 │             216    │      97.8529 │           2.2051 │ 2.2534%               │         24463.2    │          25014.5    │
 ╰─────────┴─────────────────────┴─────────────────────┴────────────────────┴──────────────┴──────────────────┴───────────────────────┴────────────────────┴─────────────────────╯
 ==================================================================
 ```
 
 ### Backtest experiments
 The framework also supports backtest experiments. Backtest experiments allows you to 
 compare multiple algorithms and evaluate their performance. Ideally,
```

#### html2text {}

```diff
@@ -71,55 +71,55 @@
 ```pretty_print_backtest``` function to print a backtest report. For example if
 you run the [moving average example trading bot](./examples/
 crossover_moving_average_trading_bot) you will get the following backtesting
 report: ```bash ====================Backtest
 report=============================== * Start date: 2023-08-24 00:00:00 * End
 date: 2023-12-02 00:00:00 * Number of days: 100 * Number of runs: 1201
 ====================Portfolio overview============================ * Number of
-orders: 10 * Initial balance: 400.0000 EUR * Final balance: 426.7818 EUR *
-Total net gain: 23.4238 EUR * Total net gain percentage: 5.8560% * Growth rate:
-6.6955% * Growth 26.7818 EUR ====================Positions
+orders: 10 * Initial balance: 400.0000 EUR * Final balance: 431.8837 EUR *
+Total net gain: 28.4171 EUR * Total net gain percentage: 7.1043% * Growth rate:
+7.9709% * Growth 31.8837 EUR ====================Positions
 overview========================
 â­âââââââââââââ¬âââââââââââ¬âââââââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââ¬ââââââââââââââââ¬ââââââââââââââââââââââââââââ¬âââââââââââââââââ¬ââââââââââââââââ®
 â Position â Amount â Pending buy amount â Pending sell amount â Cost
 (EUR) â Value (EUR) â Percentage of portfolio â Growth (EUR) â
 Growth_rate â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â EUR â 213.928 â 0 â 0 â 213.928 â 213.928 â 50.1259% â 0 â
+â EUR â 214.219 â 0 â 0 â 214.219 â 214.219 â 49.6010% â 0 â
 0.0000% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â BTC â 0.003 â 0 â 0 â 103.64 â 106.84 â 25.0338% â 3.1999 â
-3.0875% â
+â BTC â 0.0031 â 0 â 0 â 107.095 â 110.401 â 25.5627% â 3.3066
+â 3.0875% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â DOT â 21.0805 â 0 â 0 â 105.856 â 106.014 â 24.8403% â 0.1581
+â DOT â 21.3291 â 0 â 0 â 107.104 â 107.264 â 24.8363% â 0.16
 â 0.1494% â
 â°âââââââââââââ´âââââââââââ´âââââââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââ´ââââââââââââââââ´ââââââââââââââââââââââââââââ´âââââââââââââââââ´ââââââââââââââââ¯
 ====================Trades overview=========================== * Number of
 trades closed: 4 * Number of trades open: 2 * Percentage of positive trades:
 60.0% * Percentage of negative trades: 20.0% * Average trade size: 98.8728 EUR
-* Average trade duration: 191.0 hours
+* Average trade duration: 183.5 hours
 â­ââââââââââ¬ââââââââââââââââââââââ¬ââââââââââââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââ¬âââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââââââââ¬ââââââââââââââââââââââ®
 â Pair â Open date â Close date â Duration (hours) â Size (EUR) â
 Net gain (EUR) â Net gain percentage â Open price (EUR) â Close price
 (EUR) â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-11-30 20:00:00 â â 2802.99 â 105.856 â 0 â
+â DOT-EUR â 2023-11-30 20:00:00 â â 2976.65 â 107.104 â 0 â
 0.0000% â 5.0215 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-29 14:00:00 â â 2832.99 â 103.64 â 0 â
+â BTC-EUR â 2023-11-29 14:00:00 â â 3006.65 â 107.095 â 0 â
 0.0000% â 34546.6 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
 â BTC-EUR â 2023-11-08 00:00:00 â 2023-11-14 16:00:00 â 160 â 99.2265
 â 1.3352 â 1.3456% â 33075.5 â 33520.6 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
 â BTC-EUR â 2023-11-06 16:00:00 â 2023-11-06 20:00:00 â 4 â 97.8607
 â -0.0026 â -0.0026% â 32620.2 â 32619.4 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-10-30 06:00:00 â 2023-11-15 06:00:00 â 384 â 100.551
-â 19.8861 â 19.7771% â 4.0375 â 4.836 â
+â DOT-EUR â 2023-10-30 06:00:00 â 2023-11-14 00:00:00 â 354 â 100.551
+â 24.8794 â 24.7430% â 4.0375 â 5.0365 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
 â BTC-EUR â 2023-09-13 16:00:00 â 2023-09-22 16:00:00 â 216 â 97.8529
 â 2.2051 â 2.2534% â 24463.2 â 25014.5 â
 â°ââââââââââ´ââââââââââââââââââââââ´ââââââââââââââââââââââ´âââââââââââââââââââââ´âââââââââââââââ´âââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââââââââ´ââââââââââââââââââââââ¯
 ================================================================== ``` ###
 Backtest experiments The framework also supports backtest experiments. Backtest
 experiments allows you to compare multiple algorithms and evaluate their
```

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/algorithm.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/create_app.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/dependency_container.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/data_structures.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/data_structures.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/decimal_parsing.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/decimal_parsing.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/app_mode.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/app_mode.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/market/market_credential.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/market/market_credential.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/position/position_snapshot.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/strategy_profile.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/strategy_profile.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trade/trade.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+from typing import List
+from polars import DataFrame
+import polars as pl
 from datetime import datetime
 from investing_algorithm_framework.domain.models.base_model import BaseModel
+from investing_algorithm_framework.domain.exceptions import \
+    OperationalException
+from investing_algorithm_framework.domain.constants import DATETIME_FORMAT
 
 
 class Trade(BaseModel):
     """
     Trade model
 
     A trade is a combination of a buy and sell order that has been opened or
@@ -160,30 +166,59 @@
         value = self.value
         return value - self.size
 
     def get_absolute_change(self):
         return self.absolute_change
 
     def is_manual_stop_loss_trigger(
-        self, current_price, prices, stop_loss_percentage
+        self,
+        current_price,
+        stop_loss_percentage,
+        prices: List[float] = None,
+        ohlcv_df: DataFrame = None
     ):
-        # Stop loss is triggered when the current price is lower than the
-        # calculated stop loss price. The stop loss price is calculated by
-        # taking the highest price of the given range. If the highest price
-        # is lower than the open price, the stop loss price is calculated by
-        # taking the open price and subtracting the stop loss percentage.
-        # If the highest price is higher than the open price, the stop loss
-        # price is calculated by taking the open price and adding the stop
-        # loss percentage.
+        """
+        Function to check if the stop loss is triggered for a given trade.
+
+        You can use either the prices list or the ohlcv_df DataFrame to
+        calculate the stop loss. The dataframe needs to be a Polars
+        DataFrame with the following columns: "Datetime" and "Close".
+
+        You can use the default CCXTOHLCVMarketDataSource to get the ohlcv_df
+        DataFrame.
+
+        Stop loss is triggered when the current price is lower than the
+        calculated stop loss price. The stop loss price is calculated by
+        taking the highest price of the given range. If the highest price
+        is lower than the open price, the stop loss price is calculated by
+        taking the open price and subtracting the stop loss percentage.
+        If the highest price is higher than the open price, the stop loss
+        price is calculated by taking the open price and adding the stop
+        loss percentage.
+        """
+
+        if prices is None and ohlcv_df is None:
+            raise OperationalException(
+                "Either prices or a polars ohlcv dataframe must be provided"
+            )
 
         if current_price < self.open_price:
             stop_loss_price = self.open_price * \
                               (1 - stop_loss_percentage / 100)
             return current_price <= stop_loss_price
         else:
+            # If dataframes are provided, we use the dataframe to calculate
+            # the stop loss price
+            if ohlcv_df is not None:
+                filtered_df = ohlcv_df.filter(
+                    pl.col('Datetime') >= self.opened_at.strftime(
+                        DATETIME_FORMAT
+                    )
+                )
+                prices = filtered_df['Close'].to_numpy()
             highest_price = max(prices)
             stop_loss_price = highest_price * (1 - stop_loss_percentage / 100)
             return current_price <= stop_loss_price
 
     def __repr__(self):
         return self.repr(
             target_symbol=self.target_symbol,
```

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trade/trade_status.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trade/trade_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/market_credential_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/market_data_sources.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_data_sources.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/services/market_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/backtesting.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/backtesting.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from datetime import datetime
+import polars
+import logging
 
-import pandas as pd
 from dateutil.parser import parse
 
 from investing_algorithm_framework.domain import OHLCVMarketDataSource, \
-    BacktestMarketDataSource, OperationalException, TickerMarketDataSource
+    BacktestMarketDataSource, OperationalException, TickerMarketDataSource, \
+    DATETIME_FORMAT
+
+logger = logging.getLogger(__name__)
 
 
 class CSVOHLCVMarketDataSource(OHLCVMarketDataSource):
 
     def empty(self):
         data = self.get_data(
             from_time_stamp=self.start_date,
@@ -40,71 +44,57 @@
             end_date_func=end_date_func,
             window_size=window_size,
         )
         self._csv_file_path = csv_file_path
         self._columns = [
             "Datetime", "Open", "High", "Low", "Close", "Volume"
         ]
-        df = pd.read_csv(self._csv_file_path)
+        df = polars.read_csv(csv_file_path)
 
+        # Check if all column names are in the csv file
         if not all(column in df.columns for column in self._columns):
             # Identify missing columns
             missing_columns = [column for column in self._columns if
                                column not in df.columns]
             raise OperationalException(
                 f"Csv file {self._csv_file_path} does not contain "
                 f"all required ohlcv columns. "
                 f"Missing columns: {missing_columns}"
             )
 
-        first_row = df.iloc[0]
-        last_row = df.iloc[-1]
-        self._start_date = parse(first_row[0])
-        self._end_date = parse(last_row[0])
+        first_row = df.head(1)
+        last_row = df.tail(1)
+        self._start_date = parse(first_row["Datetime"][0])
+        self._end_date = parse(last_row["Datetime"][0])
 
     @property
     def csv_file_path(self):
         return self._csv_file_path
 
     def get_data(
         self,
-        from_time_stamp=None,
-        to_time_stamp=None,
+        from_timestamp=None,
+        to_timestamp=None,
         **kwargs
     ):
 
-        if from_time_stamp is None:
-            from_time_stamp = self.start_date
-
-        if to_time_stamp is None:
-            to_time_stamp = self.end_date
-
-        df = pd.read_csv(self._csv_file_path)
+        if from_timestamp is None:
+            from_timestamp = self.start_date
 
-        # Convert the 'Datetime' column to datetime type if
-        # it's not already
-        if 'Datetime' in df.columns and pd.api.types.is_string_dtype(
-                df['Datetime']):
-            df['Datetime'] = pd.to_datetime(df['Datetime'], utc=True)
-
-        # Filter rows based on the start and end dates
-        filtered_df = df[
-            (df['Datetime'] >= from_time_stamp)
-            & (df['Datetime'] <= to_time_stamp)
-        ]
-
-        # Specify the columns you want in the inner lists
-        selected_columns = ["Datetime", "Open", "High", "Low", "Close",
-                            "Volume"]
-
-        # Convert DataFrame to a list of lists with selected columns
-        filtered_list_of_lists = \
-            self.dataframe_to_list_of_lists(filtered_df, selected_columns)
+        if to_timestamp is None:
+            to_timestamp = self.end_date
 
-        return filtered_list_of_lists
+        df = polars.read_csv(
+            self.csv_file_path, columns=self._columns, separator=","
+        )
+        df = df.filter(
+            (df['Datetime'] >= from_timestamp.strftime(DATETIME_FORMAT))
+            & (df['Datetime'] <= to_timestamp.strftime(DATETIME_FORMAT))
+        )
+        return df
 
     def dataframe_to_list_of_lists(self, dataframe, columns):
         # Extract selected columns from DataFrame and convert
         # to a list of lists
         data_list_of_lists = dataframe[columns].values.tolist()
         return data_list_of_lists
 
@@ -126,15 +116,15 @@
             market=market,
             symbol=symbol,
         )
         self._csv_file_path = csv_file_path
         self._columns = [
             "Datetime", "Open", "High", "Low", "Close", "Volume"
         ]
-        df = pd.read_csv(self._csv_file_path)
+        df = polars.read_csv(self._csv_file_path)
 
         if not all(column in df.columns for column in self._columns):
             # Identify missing columns
             missing_columns = [column for column in self._columns if
                                column not in df.columns]
             raise OperationalException(
                 f"Csv file {self._csv_file_path} does not contain "
@@ -147,35 +137,38 @@
         return self._csv_file_path
 
     def get_data(self, index_datetime=None, **kwargs):
 
         if index_datetime is None:
             index_datetime = datetime.utcnow()
 
-        index_datetime = pd.to_datetime(index_datetime, utc=True)
-        df = pd.read_csv(self._csv_file_path)
-
-        # Convert the 'Datetime' column to datetime type if
-        # it's not already
-        if 'Datetime' in df.columns and pd.api.types.is_string_dtype(
-                df['Datetime']):
-            df['Datetime'] = pd.to_datetime(df['Datetime'], utc=True)
+        # Filter the data based on the backtest index date and the end date
+        df = polars.read_csv(self._csv_file_path)
+        df = df.filter(
+            (df['Datetime'] >= index_datetime
+             .strftime(DATETIME_FORMAT))
+        )
 
-        # Filter rows based on the start and end dates
-        filtered_df = df[(df['Datetime'] <= index_datetime)]
+        # Check if the dataframe is empty
+        if df.shape[0] == 0:
+            raise OperationalException(
+                f"No ticker data found for {self.symbol} "
+                f"at {index_datetime}"
+            )
 
-        if len(filtered_df) == 0:
-            return None
+        first_row = df.head(1)[0]
 
-        last_row = filtered_df.iloc[-1]
+        # Calculate the bid and ask price based on the high and low price
         return {
             "symbol": self.symbol,
-            "bid": (float(last_row[3]) + float(last_row[2])) / 2,
-            "ask": (float(last_row[3]) + float(last_row[2])) / 2,
-            "datetime": last_row[0],
+            "bid": float((first_row["Low"][0])
+                         + float(first_row["High"][0])) / 2,
+            "ask": float((first_row["Low"][0])
+                         + float(first_row["High"][0])) / 2,
+            "datetime": first_row["Datetime"][0],
         }
 
     def dataframe_to_list_of_lists(self, dataframe, columns):
         # Extract selected columns from DataFrame and convert
         # to a list of lists
         data_list_of_lists = dataframe[columns].values.tolist()
         return data_list_of_lists
```

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/backtesting/backtest_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/backtesting/backtest_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/configuration_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_credential_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/order_service/order_backtest_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_backtest_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/order_service/order_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/position_snapshot_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/position_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.2.0/investing_algorithm_framework/services/trade_service/trade_service.py` & `investing_algorithm_framework-3.3.0/investing_algorithm_framework/services/trade_service/trade_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,30 +94,22 @@
                     first_buy_order.set_filled(remaining)
                 else:
                     sell_amount = sell_amount - available
                     buy_orders_queue.dequeue()
 
             for buy_order in buy_orders_queue:
                 symbol = buy_order.get_symbol()
-
+                current_price = buy_order.get_price()
                 try:
                     ticker = self.market_data_source_service.get_ticker(
                         symbol=symbol, market=market
                     )
+                    current_price = ticker["bid"]
                 except Exception as e:
                     logger.error(e)
-                    raise OperationalException(
-                        f"Error getting ticker data for "
-                        f"trade {buy_order.get_target_symbol()}"
-                        f"-{buy_order.get_trading_symbol()}. Make sure you "
-                        f"have registered a ticker market data source for "
-                        f"{buy_order.get_target_symbol()}"
-                        f"-{buy_order.get_trading_symbol()} "
-                        f"for market {portfolio.market}"
-                    )
 
                 amount = buy_order.get_filled()
                 closed_amount = buy_order.get_trade_closed_amount()
 
                 if closed_amount is not None:
                     amount = amount - closed_amount
 
@@ -125,15 +117,15 @@
                     Trade(
                         buy_order_id=buy_order.id,
                         target_symbol=buy_order.get_target_symbol(),
                         trading_symbol=buy_order.get_trading_symbol(),
                         amount=amount,
                         open_price=buy_order.get_price(),
                         opened_at=buy_order.get_created_at(),
-                        current_price=ticker["bid"]
+                        current_price=current_price
                     )
                 )
 
         return trades
 
     def get_trades(self, market=None) -> List[Trade]:
         """
@@ -152,28 +144,34 @@
                 "status": OrderStatus.CLOSED.value,
                 "order_side": OrderSide.BUY.value,
                 "portfolio_id": portfolio.id
             })
 
             for buy_order in buy_orders:
                 symbol = buy_order.get_symbol()
-                ticker = self.market_data_source_service.get_ticker(
-                    symbol=symbol, market=market
-                )
+                current_price = buy_order.get_price()
+                try:
+                    ticker = self.market_data_source_service.get_ticker(
+                        symbol=symbol, market=market
+                    )
+                    current_price = ticker["bid"]
+                except Exception as e:
+                    logger.error(e)
+
                 trades.append(
                     Trade(
                         buy_order_id=buy_order.id,
                         target_symbol=buy_order.get_target_symbol(),
                         trading_symbol=buy_order.get_trading_symbol(),
                         amount=buy_order.get_amount(),
                         open_price=buy_order.get_price(),
                         closed_price=buy_order.get_trade_closed_price(),
                         closed_at=buy_order.get_trade_closed_at(),
                         opened_at=buy_order.get_created_at(),
-                        current_price=ticker["bid"]
+                        current_price=current_price
                     )
                 )
 
         return trades
 
     def get_closed_trades(self, portfolio_id=None) -> List[Trade]:
         """
```

### Comparing `investing_algorithm_framework-3.2.0/pyproject.toml` & `investing_algorithm_framework-3.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investing-algorithm-framework"
-version = "v3.2.0"
+version = "v3.3.0"
 description = "A framework for creating trading bots"
 authors = ["MDUYN"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 wrapt = "^1.16.0"
```

### Comparing `investing_algorithm_framework-3.2.0/PKG-INFO` & `investing_algorithm_framework-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 3.2.0
+Version: 3.3.0
 Summary: A framework for creating trading bots
 Author: MDUYN
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -170,50 +170,50 @@
 * Start date: 2023-08-24 00:00:00
 * End date: 2023-12-02 00:00:00
 * Number of days: 100
 * Number of runs: 1201
 ====================Portfolio overview============================
 * Number of orders: 10
 * Initial balance: 400.0000 EUR
-* Final balance: 426.7818 EUR
-* Total net gain: 23.4238 EUR
-* Total net gain percentage: 5.8560%
-* Growth rate: 6.6955%
-* Growth 26.7818 EUR
+* Final balance: 431.8837 EUR
+* Total net gain: 28.4171 EUR
+* Total net gain percentage: 7.1043%
+* Growth rate: 7.9709%
+* Growth 31.8837 EUR
 ====================Positions overview========================
 ╭────────────┬──────────┬──────────────────────┬───────────────────────┬──────────────┬───────────────┬───────────────────────────┬────────────────┬───────────────╮
 │ Position   │   Amount │   Pending buy amount │   Pending sell amount │   Cost (EUR) │   Value (EUR) │ Percentage of portfolio   │   Growth (EUR) │ Growth_rate   │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ EUR        │ 213.928  │                    0 │                     0 │      213.928 │       213.928 │ 50.1259%                  │         0      │ 0.0000%       │
+│ EUR        │ 214.219  │                    0 │                     0 │      214.219 │       214.219 │ 49.6010%                  │         0      │ 0.0000%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ BTC        │   0.003  │                    0 │                     0 │      103.64  │       106.84  │ 25.0338%                  │         3.1999 │ 3.0875%       │
+│ BTC        │   0.0031 │                    0 │                     0 │      107.095 │       110.401 │ 25.5627%                  │         3.3066 │ 3.0875%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ DOT        │  21.0805 │                    0 │                     0 │      105.856 │       106.014 │ 24.8403%                  │         0.1581 │ 0.1494%       │
+│ DOT        │  21.3291 │                    0 │                     0 │      107.104 │       107.264 │ 24.8363%                  │         0.16   │ 0.1494%       │
 ╰────────────┴──────────┴──────────────────────┴───────────────────────┴──────────────┴───────────────┴───────────────────────────┴────────────────┴───────────────╯
 ====================Trades overview===========================
 * Number of trades closed: 4
 * Number of trades open: 2
 * Percentage of positive trades: 60.0%
 * Percentage of negative trades: 20.0%
 * Average trade size: 98.8728 EUR
-* Average trade duration: 191.0 hours
+* Average trade duration: 183.5 hours
 ╭─────────┬─────────────────────┬─────────────────────┬────────────────────┬──────────────┬──────────────────┬───────────────────────┬────────────────────┬─────────────────────╮
 │ Pair    │ Open date           │ Close date          │   Duration (hours) │   Size (EUR) │   Net gain (EUR) │ Net gain percentage   │   Open price (EUR) │   Close price (EUR) │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-11-30 20:00:00 │                     │            2802.99 │     105.856  │           0      │ 0.0000%               │             5.0215 │                     │
+│ DOT-EUR │ 2023-11-30 20:00:00 │                     │            2976.65 │     107.104  │           0      │ 0.0000%               │             5.0215 │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-29 14:00:00 │                     │            2832.99 │     103.64   │           0      │ 0.0000%               │         34546.6    │                     │
+│ BTC-EUR │ 2023-11-29 14:00:00 │                     │            3006.65 │     107.095  │           0      │ 0.0000%               │         34546.6    │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-08 00:00:00 │ 2023-11-14 16:00:00 │             160    │      99.2265 │           1.3352 │ 1.3456%               │         33075.5    │           33520.6   │
+│ BTC-EUR │ 2023-11-08 00:00:00 │ 2023-11-14 16:00:00 │             160    │      99.2265 │           1.3352 │ 1.3456%               │         33075.5    │          33520.6    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-06 16:00:00 │ 2023-11-06 20:00:00 │               4    │      97.8607 │          -0.0026 │ -0.0026%              │         32620.2    │           32619.4   │
+│ BTC-EUR │ 2023-11-06 16:00:00 │ 2023-11-06 20:00:00 │               4    │      97.8607 │          -0.0026 │ -0.0026%              │         32620.2    │          32619.4    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-10-30 06:00:00 │ 2023-11-15 06:00:00 │             384    │     100.551  │          19.8861 │ 19.7771%              │             4.0375 │               4.836 │
+│ DOT-EUR │ 2023-10-30 06:00:00 │ 2023-11-14 00:00:00 │             354    │     100.551  │          24.8794 │ 24.7430%              │             4.0375 │              5.0365 │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-09-13 16:00:00 │ 2023-09-22 16:00:00 │             216    │      97.8529 │           2.2051 │ 2.2534%               │         24463.2    │           25014.5   │
+│ BTC-EUR │ 2023-09-13 16:00:00 │ 2023-09-22 16:00:00 │             216    │      97.8529 │           2.2051 │ 2.2534%               │         24463.2    │          25014.5    │
 ╰─────────┴─────────────────────┴─────────────────────┴────────────────────┴──────────────┴──────────────────┴───────────────────────┴────────────────────┴─────────────────────╯
 ==================================================================
 ```
 
 ### Backtest experiments
 The framework also supports backtest experiments. Backtest experiments allows you to 
 compare multiple algorithms and evaluate their performance. Ideally,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.2.0
+Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.3.0
 Summary: A framework for creating trading bots Author: MDUYN Requires-Python:
 >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.9,<4.0.0) Requires-Dist: Flask-Migrate
 (>=2.6.0,<3.0.0) Requires-Dist: MarkupSafe (>=2.1.2,<3.0.0) Requires-Dist:
@@ -85,55 +85,55 @@
 ```pretty_print_backtest``` function to print a backtest report. For example if
 you run the [moving average example trading bot](./examples/
 crossover_moving_average_trading_bot) you will get the following backtesting
 report: ```bash ====================Backtest
 report=============================== * Start date: 2023-08-24 00:00:00 * End
 date: 2023-12-02 00:00:00 * Number of days: 100 * Number of runs: 1201
 ====================Portfolio overview============================ * Number of
-orders: 10 * Initial balance: 400.0000 EUR * Final balance: 426.7818 EUR *
-Total net gain: 23.4238 EUR * Total net gain percentage: 5.8560% * Growth rate:
-6.6955% * Growth 26.7818 EUR ====================Positions
+orders: 10 * Initial balance: 400.0000 EUR * Final balance: 431.8837 EUR *
+Total net gain: 28.4171 EUR * Total net gain percentage: 7.1043% * Growth rate:
+7.9709% * Growth 31.8837 EUR ====================Positions
 overview========================
 â­âââââââââââââ¬âââââââââââ¬âââââââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââ¬ââââââââââââââââ¬ââââââââââââââââââââââââââââ¬âââââââââââââââââ¬ââââââââââââââââ®
 â Position â Amount â Pending buy amount â Pending sell amount â Cost
 (EUR) â Value (EUR) â Percentage of portfolio â Growth (EUR) â
 Growth_rate â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â EUR â 213.928 â 0 â 0 â 213.928 â 213.928 â 50.1259% â 0 â
+â EUR â 214.219 â 0 â 0 â 214.219 â 214.219 â 49.6010% â 0 â
 0.0000% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â BTC â 0.003 â 0 â 0 â 103.64 â 106.84 â 25.0338% â 3.1999 â
-3.0875% â
+â BTC â 0.0031 â 0 â 0 â 107.095 â 110.401 â 25.5627% â 3.3066
+â 3.0875% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â DOT â 21.0805 â 0 â 0 â 105.856 â 106.014 â 24.8403% â 0.1581
+â DOT â 21.3291 â 0 â 0 â 107.104 â 107.264 â 24.8363% â 0.16
 â 0.1494% â
 â°âââââââââââââ´âââââââââââ´âââââââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââ´ââââââââââââââââ´ââââââââââââââââââââââââââââ´âââââââââââââââââ´ââââââââââââââââ¯
 ====================Trades overview=========================== * Number of
 trades closed: 4 * Number of trades open: 2 * Percentage of positive trades:
 60.0% * Percentage of negative trades: 20.0% * Average trade size: 98.8728 EUR
-* Average trade duration: 191.0 hours
+* Average trade duration: 183.5 hours
 â­ââââââââââ¬ââââââââââââââââââââââ¬ââââââââââââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââ¬âââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââââââââ¬ââââââââââââââââââââââ®
 â Pair â Open date â Close date â Duration (hours) â Size (EUR) â
 Net gain (EUR) â Net gain percentage â Open price (EUR) â Close price
 (EUR) â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-11-30 20:00:00 â â 2802.99 â 105.856 â 0 â
+â DOT-EUR â 2023-11-30 20:00:00 â â 2976.65 â 107.104 â 0 â
 0.0000% â 5.0215 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-29 14:00:00 â â 2832.99 â 103.64 â 0 â
+â BTC-EUR â 2023-11-29 14:00:00 â â 3006.65 â 107.095 â 0 â
 0.0000% â 34546.6 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
 â BTC-EUR â 2023-11-08 00:00:00 â 2023-11-14 16:00:00 â 160 â 99.2265
 â 1.3352 â 1.3456% â 33075.5 â 33520.6 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
 â BTC-EUR â 2023-11-06 16:00:00 â 2023-11-06 20:00:00 â 4 â 97.8607
 â -0.0026 â -0.0026% â 32620.2 â 32619.4 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-10-30 06:00:00 â 2023-11-15 06:00:00 â 384 â 100.551
-â 19.8861 â 19.7771% â 4.0375 â 4.836 â
+â DOT-EUR â 2023-10-30 06:00:00 â 2023-11-14 00:00:00 â 354 â 100.551
+â 24.8794 â 24.7430% â 4.0375 â 5.0365 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
 â BTC-EUR â 2023-09-13 16:00:00 â 2023-09-22 16:00:00 â 216 â 97.8529
 â 2.2051 â 2.2534% â 24463.2 â 25014.5 â
 â°ââââââââââ´ââââââââââââââââââââââ´ââââââââââââââââââââââ´âââââââââââââââââââââ´âââââââââââââââ´âââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââââââââ´ââââââââââââââââââââââ¯
 ================================================================== ``` ###
 Backtest experiments The framework also supports backtest experiments. Backtest
 experiments allows you to compare multiple algorithms and evaluate their
```

