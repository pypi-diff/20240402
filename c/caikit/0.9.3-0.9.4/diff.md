# Comparing `tmp/caikit-0.9.3.tar.gz` & `tmp/caikit-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.9.3.tar` & `caikit-0.9.4.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0       60 2023-07-06 16:52:07.809360 caikit-0.9.3/.coveragerc
--rw-r--r--   0        0        0      676 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1698 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1117 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      260 2023-07-06 16:52:07.809360 caikit-0.9.3/.gitignore
--rw-r--r--   0        0        0      324 2023-07-06 16:52:07.809360 caikit-0.9.3/.isort.cfg
--rw-r--r--   0        0        0      370 2023-07-06 16:52:07.809360 caikit-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-07-06 16:52:07.809360 caikit-0.9.3/.prettierignore
--rw-r--r--   0        0        0       12 2023-07-06 16:52:07.809360 caikit-0.9.3/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-07-06 16:52:07.809360 caikit-0.9.3/.pylintrc
--rw-r--r--   0        0        0      599 2023-07-06 16:52:07.809360 caikit-0.9.3/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2023-07-06 16:52:07.809360 caikit-0.9.3/.whitesource
--rw-r--r--   0        0        0      368 2023-07-06 16:52:07.809360 caikit-0.9.3/CODEOWNERS
--rw-r--r--   0        0        0     7164 2023-07-06 16:52:07.809360 caikit-0.9.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-07-06 16:52:07.809360 caikit-0.9.3/LICENSE
--rw-r--r--   0        0        0     6317 2023-07-06 16:52:07.809360 caikit-0.9.3/README.md
--rw-r--r--   0        0        0      152 2023-07-06 16:52:07.809360 caikit-0.9.3/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/config/__init__.py
--rw-r--r--   0        0        0     6035 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/config/config.py
--rw-r--r--   0        0        0     6388 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3509 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2817 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2029 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3141 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3243 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2875 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    40051 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2402 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4983 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    17602 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4988 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     5127 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/json_dict.py
--rw-r--r--   0        0        0     1564 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3920 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5446 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4776 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    39907 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3580 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5217 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21179 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2824 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4717 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2880 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5982 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30052 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6145 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/config.py
--rw-r--r--   0        0        0    11011 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4141 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    12931 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3885 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/registries.py
--rw-r--r--   0        0        0      654 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10666 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4688 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8221 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/parsers.py
--rw-r--r--   0        0        0    10542 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/task.py
--rw-r--r--   0        0        0      982 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4704 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21349 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     3240 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/factory.py
--rw-r--r--   0        0        0     4914 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     1648 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    31633 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3356 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     2148 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/sync_to_async.py
--rw-r--r--   0        0        0     5965 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1056 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1169 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      618 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/__init__.py
--rw-r--r--   0        0        0      809 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/data_model/__init__.py
--rw-r--r--   0        0        0      740 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/data_model/package.py
--rw-r--r--   0        0        0     2254 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/data_model/text_generation.py
--rw-r--r--   0        0        0     1383 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/tasks.py
--rw-r--r--   0        0        0      611 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14262 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    15627 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4645 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17083 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2606 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12089 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4310 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1642 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0     9572 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     4229 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12070 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     6146 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/protoable.py
--rw-r--r--   0        0        0    12152 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0     2216 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12641 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    12451 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5440 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6790 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    13825 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0    12228 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/train_executors.py
--rw-r--r--   0        0        0      169 2023-07-06 16:52:07.817361 caikit-0.9.3/code-of-conduct.md
--rw-r--r--   0        0        0      639 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/Makefile
--rw-r--r--   0        0        0     6860 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/001-module.md
--rw-r--r--   0        0        0     1610 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/architecture_club/README.md
--rw-r--r--   0        0        0      805 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/make.bat
--rw-r--r--   0        0        0     3053 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/source/conf.py
--rw-r--r--   0        0        0      225 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/source/index.rst
--rw-r--r--   0        0        0      837 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1475 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       77 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      615 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     2058 2023-07-06 16:52:11.645575 caikit-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2952 2023-07-06 16:52:07.821361 caikit-0.9.3/releases.md
--rwxr-xr-x   0        0        0      639 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/check_deps.sh
--rw-r--r--   0        0        0    13757 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/dsconverter.py
--rwxr-xr-x   0        0        0      720 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/fmt.sh
--rw-r--r--   0        0        0    25639 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/test_dsconverter.py
--rw-r--r--   0        0        0       33 2023-07-06 16:52:07.821361 caikit-0.9.3/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0     5240 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/base.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/config/test_configs.py
--rw-r--r--   0        0        0     4508 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5034 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26951 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16237 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    32651 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     2358 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_json_dict.py
--rw-r--r--   0        0        0     1104 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4378 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6888 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    13033 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4872 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0      521 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_imports.py
--rw-r--r--   0        0        0    21743 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7497 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_task.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/__init__.py
--rw-r--r--   0        0        0     7967 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     2372 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_factory.py
--rw-r--r--   0        0        0     4997 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     3956 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_sync_to_async.py
--rw-r--r--   0        0        0     7824 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/data_model_helpers.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/examples/__init__.py
--rw-r--r--   0        0        0     2537 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/examples/shared.py
--rw-r--r--   0        0        0     2417 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/examples/test_examples.py
--rw-r--r--   0        0        0       39 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      591 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1017 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      508 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_no_id/config.yml
--rw-r--r--   0        0        0      508 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0      326 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_streaming_module/config.yml
--rw-r--r--   0        0        0     3034 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      349 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      396 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0       24 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      296 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      176 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1474 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1946 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      296 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      902 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     3576 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0     1514 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
--rw-r--r--   0        0        0      364 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/__init__.py
--rw-r--r--   0        0        0     1658 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/common/test_producer.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/nlp/__init__.py
--rw-r--r--   0        0        0     2859 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/nlp/test_nlp_tasks.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/__init__.py
--rw-r--r--   0        0        0     6754 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/conftest.py
--rw-r--r--   0        0        0      756 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14101 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2401 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     4035 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    17954 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     3796 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/test_protoable.py
--rw-r--r--   0        0        0     2345 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     8875 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    16401 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     4088 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7776 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    38335 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5072 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    17329 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3819 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2209 2023-07-06 16:52:07.829362 caikit-0.9.3/tox.ini
--rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 caikit-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-07-06 21:35:12.056465 caikit-0.9.4/.coveragerc
+-rw-r--r--   0        0        0      676 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1698 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1117 2023-07-06 21:35:12.056465 caikit-0.9.4/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      260 2023-07-06 21:35:12.056465 caikit-0.9.4/.gitignore
+-rw-r--r--   0        0        0      324 2023-07-06 21:35:12.056465 caikit-0.9.4/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-07-06 21:35:12.056465 caikit-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-07-06 21:35:12.056465 caikit-0.9.4/.prettierignore
+-rw-r--r--   0        0        0       12 2023-07-06 21:35:12.056465 caikit-0.9.4/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-07-06 21:35:12.056465 caikit-0.9.4/.pylintrc
+-rw-r--r--   0        0        0      599 2023-07-06 21:35:12.056465 caikit-0.9.4/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2023-07-06 21:35:12.056465 caikit-0.9.4/.whitesource
+-rw-r--r--   0        0        0      368 2023-07-06 21:35:12.056465 caikit-0.9.4/CODEOWNERS
+-rw-r--r--   0        0        0     7164 2023-07-06 21:35:12.056465 caikit-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-07-06 21:35:12.056465 caikit-0.9.4/LICENSE
+-rw-r--r--   0        0        0     6317 2023-07-06 21:35:12.056465 caikit-0.9.4/README.md
+-rw-r--r--   0        0        0      152 2023-07-06 21:35:12.056465 caikit-0.9.4/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6035 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/config/config.py
+-rw-r--r--   0        0        0     6388 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3509 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2817 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2029 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3141 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3243 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2875 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    40051 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2402 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4983 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    17602 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4988 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     5127 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/json_dict.py
+-rw-r--r--   0        0        0     1564 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3920 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5446 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4776 2023-07-06 21:35:12.056465 caikit-0.9.4/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    39907 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3580 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5217 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21179 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2824 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4717 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2880 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5982 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30633 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6145 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    12087 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4141 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    12931 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3885 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10666 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8221 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0    17565 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/task.py
+-rw-r--r--   0        0        0      982 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4704 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21349 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     3240 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/factory.py
+-rw-r--r--   0        0        0     4914 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     1648 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    31633 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3356 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     2148 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/sync_to_async.py
+-rw-r--r--   0        0        0     5965 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1056 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1169 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      618 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/nlp/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/nlp/data_model/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/nlp/data_model/package.py
+-rw-r--r--   0        0        0     2254 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/nlp/data_model/text_generation.py
+-rw-r--r--   0        0        0     1151 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/nlp/tasks.py
+-rw-r--r--   0        0        0      611 2023-07-06 21:35:12.060465 caikit-0.9.4/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14262 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    15627 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4645 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17083 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2606 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12089 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4310 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1642 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0     9572 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     4229 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12070 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     6146 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/protoable.py
+-rw-r--r--   0        0        0    12237 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2216 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12845 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    12451 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5440 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6790 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    13825 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-07-06 21:35:12.064465 caikit-0.9.4/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0    12228 2023-07-06 21:35:12.068465 caikit-0.9.4/caikit/runtime/work_management/train_executors.py
+-rw-r--r--   0        0        0      169 2023-07-06 21:35:12.068465 caikit-0.9.4/code-of-conduct.md
+-rw-r--r--   0        0        0      639 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/Makefile
+-rw-r--r--   0        0        0     6860 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/adrs/001-module.md
+-rw-r--r--   0        0        0     1610 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      805 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/make.bat
+-rw-r--r--   0        0        0     3053 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2023-07-06 21:35:12.068465 caikit-0.9.4/docs/source/index.rst
+-rw-r--r--   0        0        0      837 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1475 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       77 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      615 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-06 21:35:12.068465 caikit-0.9.4/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     2058 2023-07-06 21:35:17.212487 caikit-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2952 2023-07-06 21:35:12.068465 caikit-0.9.4/releases.md
+-rwxr-xr-x   0        0        0      639 2023-07-06 21:35:12.068465 caikit-0.9.4/scripts/check_deps.sh
+-rw-r--r--   0        0        0    13757 2023-07-06 21:35:12.068465 caikit-0.9.4/scripts/dsconverter.py
+-rwxr-xr-x   0        0        0      720 2023-07-06 21:35:12.068465 caikit-0.9.4/scripts/fmt.sh
+-rw-r--r--   0        0        0    25639 2023-07-06 21:35:12.068465 caikit-0.9.4/scripts/test_dsconverter.py
+-rw-r--r--   0        0        0       33 2023-07-06 21:35:12.068465 caikit-0.9.4/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0     5240 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/base.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/config/test_configs.py
+-rw-r--r--   0        0        0     4508 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5034 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26951 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16237 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    32651 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     2358 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/test_json_dict.py
+-rw-r--r--   0        0        0     1104 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4378 2023-07-06 21:35:12.068465 caikit-0.9.4/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    13033 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21743 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0    11170 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/test_task.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     7967 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     2372 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_factory.py
+-rw-r--r--   0        0        0     4997 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     3956 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_sync_to_async.py
+-rw-r--r--   0        0        0     7824 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/data_model_helpers.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/examples/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/examples/shared.py
+-rw-r--r--   0        0        0     2417 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/examples/test_examples.py
+-rw-r--r--   0        0        0       39 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1017 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      508 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_no_id/config.yml
+-rw-r--r--   0        0        0      508 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0      326 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/dummy_streaming_module/config.yml
+-rw-r--r--   0        0        0     3034 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      349 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      396 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0       24 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      296 2023-07-06 21:35:12.072465 caikit-0.9.4/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1668 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1946 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      296 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      902 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     3576 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     3363 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0     1607 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
+-rw-r--r--   0        0        0      364 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/interfaces/__init__.py
+-rw-r--r--   0        0        0     1658 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/interfaces/common/test_producer.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/interfaces/nlp/__init__.py
+-rw-r--r--   0        0        0     3188 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/interfaces/nlp/test_nlp_tasks.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/__init__.py
+-rw-r--r--   0        0        0     6754 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/conftest.py
+-rw-r--r--   0        0        0      756 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2401 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     4035 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    17954 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     3796 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/service_generation/test_protoable.py
+-rw-r--r--   0        0        0     2345 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     8875 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    16401 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     4088 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7776 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    38335 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5072 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    17329 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3819 2023-07-06 21:35:12.076465 caikit-0.9.4/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2227 2023-07-06 21:35:12.076465 caikit-0.9.4/tox.ini
+-rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 caikit-0.9.4/PKG-INFO
```

### Comparing `caikit-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.9.4/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.github/workflows/build-library.yml` & `caikit-0.9.4/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.github/workflows/lint-code.yml` & `caikit-0.9.4/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.github/workflows/publish-library.yml` & `caikit-0.9.4/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.pylintrc` & `caikit-0.9.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/.readthedocs.yaml` & `caikit-0.9.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/CONTRIBUTING.md` & `caikit-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/LICENSE` & `caikit-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/README.md` & `caikit-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit-overview.png` & `caikit-0.9.4/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/config/__init__.py` & `caikit-0.9.4/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/config/config.py` & `caikit-0.9.4/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/config/config.yml` & `caikit-0.9.4/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/__init__.py` & `caikit-0.9.4/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/__init__.py` & `caikit-0.9.4/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/base.py` & `caikit-0.9.4/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.9.4/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.9.4/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/schemes/base.py` & `caikit-0.9.4/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.9.4/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.9.4/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/__init__.py` & `caikit-0.9.4/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/base.py` & `caikit-0.9.4/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.9.4/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/data_backends/base.py` & `caikit-0.9.4/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.9.4/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/dataobject.py` & `caikit-0.9.4/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/enums.py` & `caikit-0.9.4/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/json_dict.py` & `caikit-0.9.4/caikit/core/data_model/json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/producer.py` & `caikit-0.9.4/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.9.4/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/streams/__init__.py` & `caikit-0.9.4/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/streams/converter.py` & `caikit-0.9.4/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.9.4/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/streams/data_stream.py` & `caikit-0.9.4/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/streams/resolver.py` & `caikit-0.9.4/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/data_model/streams/validator.py` & `caikit-0.9.4/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/model_manager.py` & `caikit-0.9.4/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/module_backends/__init__.py` & `caikit-0.9.4/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/module_backends/backend_types.py` & `caikit-0.9.4/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/module_backends/base.py` & `caikit-0.9.4/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/module_backends/local_backend.py` & `caikit-0.9.4/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/module_backends/module_backend_config.py` & `caikit-0.9.4/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/modules/__init__.py` & `caikit-0.9.4/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/modules/base.py` & `caikit-0.9.4/caikit/core/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # pylint: disable=too-many-lines
 
 # abstract methods may define arguments but not use them
 # pylint: disable=unused-argument
 
 # Standard
 from io import BytesIO
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 import collections
 import os
 import shutil
 import tempfile
 import time
 import types
 
@@ -78,14 +78,26 @@
 
     def set_load_backend(self, load_backend):
         """Method used by the model manager to indicate the load backend that
         was used to load this module
         """
         self._load_backend = load_backend
 
+    @classmethod
+    def get_inference_signature(
+        cls, input_streaming: bool, output_streaming: bool
+    ) -> Optional["caikit.core.signature_parsing.CaikitMethodSignature"]:
+        """Returns the inference method signature that is capable of running the module's task
+        for the given flavors of input and output streaming
+        """
+        for in_streaming, out_streaming, signature in cls._INFERENCE_SIGNATURES:
+            if in_streaming == input_streaming and out_streaming == output_streaming:
+                return signature
+        return None
+
     @property
     def load_backend(self):
         """Get the backend instance used to load this module. This can be used
         in module implementations that require use of a specific backend at
         inference time.
         """
         return self._load_backend
```

### Comparing `caikit-0.9.3/caikit/core/modules/config.py` & `caikit-0.9.4/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/modules/decorator.py` & `caikit-0.9.4/caikit/core/modules/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,18 +187,42 @@
             cls_.TASK_CLASS = parent_task
         else:
             cls_.TASK_CLASS = task
 
         # Parse the `train` and `run` signatures
         cls_.RUN_SIGNATURE = CaikitMethodSignature(cls_, "run")
         cls_.TRAIN_SIGNATURE = CaikitMethodSignature(cls_, "train")
+        cls_._INFERENCE_SIGNATURES = []
 
         # If the module has a task, validate it:
         if cls_.TASK_CLASS:
-            cls_.TASK_CLASS.validate_run_signature(cls_.RUN_SIGNATURE)
+            if not cls_.TASK_CLASS.has_inference_method_decorators(module_class=cls_):
+                # Hackity hack hack - make sure at least one flavor is supported
+                validated = False
+                validation_errs = []
+                for input_streaming, output_streaming in [
+                    [False, False],
+                    [True, True],
+                    [False, True],
+                ]:
+                    try:
+                        cls_.TASK_CLASS.validate_run_signature(
+                            cls_.RUN_SIGNATURE, input_streaming, output_streaming
+                        )
+                        validated = True
+                        cls_._INFERENCE_SIGNATURES.append(
+                            (input_streaming, output_streaming, cls_.RUN_SIGNATURE)
+                        )
+                        break
+                    except (ValueError, TypeError) as e:
+                        validation_errs.append(e)
+                if not validated:
+                    raise validation_errs[0]
+
+            cls_.TASK_CLASS.deferred_method_decoration(cls_)
 
         # If no backend support described in the class, add current backend
         # as the only backend that can load models trained by this module
         cls_.SUPPORTED_LOAD_BACKENDS = getattr(
             cls_, SUPPORTED_LOAD_BACKENDS_VAR_NAME, [backend_type]
         )
```

### Comparing `caikit-0.9.3/caikit/core/modules/loader.py` & `caikit-0.9.4/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/modules/meta.py` & `caikit-0.9.4/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/modules/saver.py` & `caikit-0.9.4/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/registries.py` & `caikit-0.9.4/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/signature_parsing/__init__.py` & `caikit-0.9.4/caikit/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/signature_parsing/docstrings.py` & `caikit-0.9.4/caikit/core/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/signature_parsing/module_signature.py` & `caikit-0.9.4/caikit/core/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/signature_parsing/parsers.py` & `caikit-0.9.4/caikit/core/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/__init__.py` & `caikit-0.9.4/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/compatibility.py` & `caikit-0.9.4/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/errors/__init__.py` & `caikit-0.9.4/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.9.4/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.9.4/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/factory.py` & `caikit-0.9.4/caikit/core/toolkit/factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/fileio.py` & `caikit-0.9.4/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/logging.py` & `caikit-0.9.4/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.9.4/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/serializers.py` & `caikit-0.9.4/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/sync_to_async.py` & `caikit-0.9.4/caikit/core/toolkit/sync_to_async.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/core/toolkit/wip_decorator.py` & `caikit-0.9.4/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/__init__.py` & `caikit-0.9.4/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/common/__init__.py` & `caikit-0.9.4/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.9.4/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/common/data_model/producer.py` & `caikit-0.9.4/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/nlp/__init__.py` & `caikit-0.9.4/caikit/interfaces/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/nlp/data_model/__init__.py` & `caikit-0.9.4/caikit/interfaces/nlp/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/nlp/data_model/package.py` & `caikit-0.9.4/caikit/interfaces/nlp/data_model/package.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/nlp/data_model/text_generation.py` & `caikit-0.9.4/caikit/interfaces/nlp/data_model/text_generation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/nlp/tasks.py` & `caikit-0.9.4/caikit/interfaces/nlp/tasks.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,24 +20,15 @@
 
 # Local
 from ...core import TaskBase, task
 from .data_model.text_generation import GeneratedTextResult, GeneratedTextStreamResult
 
 
 @task(
-    required_parameters={"inputs": str},
-    output_type=GeneratedTextResult,
+    unary_parameters={"inputs": str},
+    unary_output_type=GeneratedTextResult,
+    streaming_output_type=Iterable[GeneratedTextStreamResult],
 )
 class TextGenerationTask(TaskBase):
     """The Text Generation Task is responsible for taking input prompting text
     and generating additional text from that prompt.
     """
-
-
-@task(
-    required_parameters={"inputs": str},
-    output_type=Iterable[GeneratedTextStreamResult],
-)
-class TextGenerationStreamTask(TaskBase):
-    """The Text Generation Stream Task is responsible for taking input prompting
-    text and iteratively producing output tokens in a stream.
-    """
```

### Comparing `caikit-0.9.3/caikit/interfaces/runtime/__init__.py` & `caikit-0.9.4/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.9.4/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.9.4/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/__init__.py` & `caikit-0.9.4/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/dump_services.py` & `caikit-0.9.4/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/grpc_server.py` & `caikit-0.9.4/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/interceptors/__init__.py` & `caikit-0.9.4/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.9.4/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/metrics/__init__.py` & `caikit-0.9.4/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.9.4/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/__init__.py` & `caikit-0.9.4/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/batcher.py` & `caikit-0.9.4/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/loaded_model.py` & `caikit-0.9.4/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/model_loader.py` & `caikit-0.9.4/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/model_manager.py` & `caikit-0.9.4/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/model_sizer.py` & `caikit-0.9.4/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/model_management/training_manager.py` & `caikit-0.9.4/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/__init__.py` & `caikit-0.9.4/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.9.4/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.9.4/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.9.4/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.9.4/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.9.4/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.9.4/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.9.4/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.9.4/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.9.4/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/service_factory.py` & `caikit-0.9.4/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.9.4/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/service_generation/create_service.py` & `caikit-0.9.4/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.9.4/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/service_generation/protoable.py` & `caikit-0.9.4/caikit/runtime/service_generation/protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/service_generation/rpcs.py` & `caikit-0.9.4/caikit/runtime/service_generation/rpcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             name=self.request.name,
             attrs=attrs,
             annotations={**properties, **optional_properties},
         )
 
     def create_rpc_json(self, package_name: str) -> Dict:
         """Return json snippet for the service definition of this RPC"""
-        if self.module_list[0].TASK_CLASS.is_output_streaming_task():
+        if self.module_list[0].TASK_CLASS._is_iterable_type(self.return_type):
+            # if self.module_list[0].TASK_CLASS.is_output_streaming_task():
             output_type_name = (
                 typing.get_args(self.return_type)[0]
                 .get_proto_class()
                 .DESCRIPTOR.full_name
             )
             server_streaming = True
         else:
```

### Comparing `caikit-0.9.3/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.9.4/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/servicers/__init__.py` & `caikit-0.9.4/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.9.4/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,18 @@
                     **caikit_library_request,
                 )
 
                 # Marshall the response to the necessary return type
                 with PREDICT_TO_PROTO_SUMMARY.labels(
                     grpc_request=request_name, model_id=model_id
                 ).time():
-                    if model.TASK_CLASS.is_output_streaming_task():
+                    # if model.TASK_CLASS.is_output_streaming_task():
+                    # hackity hack: We need to check the actual RPC def to see if this is streaming
+                    # out or not
+                    if model.TASK_CLASS._is_iterable_type(response):
                         response_proto = build_proto_stream(response)
                     else:
                         response_proto = build_proto_response(response)
                 return response_proto
 
     def predict_model(
         self,
```

### Comparing `caikit-0.9.3/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.9.4/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.9.4/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.9.4/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.9.4/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/types/__init__.py` & `caikit-0.9.4/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/types/aborted_exception.py` & `caikit-0.9.4/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.9.4/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.9.4/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/utils/__init__.py` & `caikit-0.9.4/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/utils/import_util.py` & `caikit-0.9.4/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/utils/servicer_util.py` & `caikit-0.9.4/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/work_management/__init__.py` & `caikit-0.9.4/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/work_management/abortable_action.py` & `caikit-0.9.4/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/work_management/call_aborter.py` & `caikit-0.9.4/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.9.4/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/caikit/runtime/work_management/train_executors.py` & `caikit-0.9.4/caikit/runtime/work_management/train_executors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/Makefile` & `caikit-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/adrs/001-module.md` & `caikit-0.9.4/docs/adrs/001-module.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/adrs/010-data-model-definition.md` & `caikit-0.9.4/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/adrs/015-runtime-service-generation.md` & `caikit-0.9.4/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/adrs/018-shared-backends.md` & `caikit-0.9.4/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/adrs/019-loader-stack.md` & `caikit-0.9.4/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/architecture_club/04-25-23.md` & `caikit-0.9.4/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/make.bat` & `caikit-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/docs/source/conf.py` & `caikit-0.9.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/start_runtime_with_sample_lib.py` & `caikit-0.9.4/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/README.md` & `caikit-0.9.4/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/client.py` & `caikit-0.9.4/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.9.4/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/start_runtime.py` & `caikit-0.9.4/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.9.4/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.9.4/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.9.4/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.9.4/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.9.4/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.9.4/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/pyproject.toml` & `caikit-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.9.3"
+version = "0.9.4"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.9.3/releases.md` & `caikit-0.9.4/releases.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/scripts/check_deps.sh` & `caikit-0.9.4/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/scripts/dsconverter.py` & `caikit-0.9.4/scripts/dsconverter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/scripts/fmt.sh` & `caikit-0.9.4/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/scripts/test_dsconverter.py` & `caikit-0.9.4/scripts/test_dsconverter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/__init__.py` & `caikit-0.9.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/base.py` & `caikit-0.9.4/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/config/test_configs.py` & `caikit-0.9.4/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/conftest.py` & `caikit-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.9.4/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.9.4/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.9.4/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/streams/test_converter.py` & `caikit-0.9.4/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.9.4/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.9.4/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/streams/test_resolver.py` & `caikit-0.9.4/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/streams/test_validator.py` & `caikit-0.9.4/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/test_base.py` & `caikit-0.9.4/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/test_dataobject.py` & `caikit-0.9.4/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/test_enums.py` & `caikit-0.9.4/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/test_json_dict.py` & `caikit-0.9.4/tests/core/data_model/test_json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/data_model/test_producer.py` & `caikit-0.9.4/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/helpers.py` & `caikit-0.9.4/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/module_backends/test_backend_types.py` & `caikit-0.9.4/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.9.4/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/modules/test_module.py` & `caikit-0.9.4/tests/core/modules/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/modules/test_module_metadata.py` & `caikit-0.9.4/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/signature_parsing/__init__.py` & `caikit-0.9.4/tests/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/signature_parsing/test_docstrings.py` & `caikit-0.9.4/tests/core/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/signature_parsing/test_parsers.py` & `caikit-0.9.4/tests/core/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/test_imports.py` & `caikit-0.9.4/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/test_model_manager.py` & `caikit-0.9.4/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/test_no_write_permissions.py` & `caikit-0.9.4/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_compatibility.py` & `caikit-0.9.4/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_error_handler.py` & `caikit-0.9.4/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_factory.py` & `caikit-0.9.4/tests/core/toolkit/test_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_fileio.py` & `caikit-0.9.4/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.9.4/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_serializers.py` & `caikit-0.9.4/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_sync_to_async.py` & `caikit-0.9.4/tests/core/toolkit/test_sync_to_async.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.9.4/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/data_model_helpers.py` & `caikit-0.9.4/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/examples/shared.py` & `caikit-0.9.4/tests/examples/shared.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/examples/test_examples.py` & `caikit-0.9.4/tests/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/config/config.yml` & `caikit-0.9.4/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.9.4/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/dummy_module.zip` & `caikit-0.9.4/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/dummy_module/config.yml` & `caikit-0.9.4/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.9.4/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/fixtures.py` & `caikit-0.9.4/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/invalid.zip` & `caikit-0.9.4/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/linux.txt` & `caikit-0.9.4/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.9.4/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Dummy data model object for testing
 """
 # Standard
+from typing import Iterable
 import typing
 
 # Local
 from caikit.core import DataObjectBase, TaskBase, dataobject, task
 
 
 @dataobject(package="caikit_data_model.sample_lib")
@@ -34,28 +35,31 @@
 class SampleTrainingType(DataObjectBase):
     """A sample `training data` type for the `sample_task` task."""
 
     number: int
 
 
 @task(
-    required_parameters={"sample_input": SampleInputType},
-    output_type=SampleOutputType,
+    unary_parameters={"sample_input": SampleInputType},
+    streaming_parameters={"sample_inputs": Iterable[SampleInputType]},
+    unary_output_type=SampleOutputType,
+    streaming_output_type=Iterable[SampleOutputType],
 )
 class SampleTask(TaskBase):
     """A sample `task` for our test models"""
 
 
 @task(
-    required_parameters={"sample_input": SampleInputType},
-    output_type=typing.Iterable[SampleOutputType],
+    unary_parameters={"sample_input": SampleInputType},
+    unary_output_type=OtherOutputType,
 )
-class StreamingTask(TaskBase):
-    """A streaming version of a task"""
+class OtherTask(TaskBase):
+    """Another sample `task` for our test models"""
 
 
+# NB: Backwards compatibility test
 @task(
     required_parameters={"sample_input": SampleInputType},
-    output_type=OtherOutputType,
+    output_type=typing.Iterable[SampleOutputType],
 )
-class OtherTask(TaskBase):
-    """Another sample `task` for our test models"""
+class StreamingTask(TaskBase):
+    """A streaming version of a task"""
```

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.9.4/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.9.4/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     @classmethod
     def load(cls, model_path, **kwargs):
         loader = ModuleLoader(model_path)
         config = loader.config
         return cls(config["train"]["batch_size"], config["train"]["learning_rate"])
 
+    @SampleTask.taskmethod()
     def run(
         self, sample_input: SampleInputType, throw: bool = False
     ) -> SampleOutputType:
         """
         Args:
             sample_input (sample_lib.data_model.SampleInputType): the input
 
@@ -46,14 +47,33 @@
         """
         if throw:
             raise RuntimeError("barf!")
         if sample_input.name == self.POISON_PILL_NAME:
             raise ValueError(f"{self.POISON_PILL_NAME} is not allowed!")
         return SampleOutputType(f"Hello {sample_input.name}")
 
+    @SampleTask.taskmethod(output_streaming=True)
+    def run_stream_out(
+        self, sample_input: SampleInputType
+    ) -> DataStream[SampleOutputType]:
+        """
+        Args:
+            sample_input (sample_lib.data_model.SampleInputType): the input
+
+        Returns:
+            caikit.core.data_model.DataStream[sample_lib.data_model.SampleOutputType]: The output
+                stream
+        """
+        list_ = [
+            SampleOutputType(f"Hello {sample_input.name}")
+            for x in range(self.stream_size)
+        ]
+        stream = DataStream.from_iterable(list_)
+        return stream
+
     def save(self, model_path):
         module_saver = ModuleSaver(
             self,
             model_path=model_path,
         )
         with module_saver:
             config_options = {
```

### Comparing `caikit-0.9.3/tests/interfaces/__init__.py` & `caikit-0.9.4/tests/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/interfaces/common/test_producer.py` & `caikit-0.9.4/tests/interfaces/common/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/interfaces/nlp/__init__.py` & `caikit-0.9.4/tests/interfaces/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/interfaces/nlp/test_nlp_tasks.py` & `caikit-0.9.4/tests/interfaces/nlp/test_nlp_tasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for the NLP task definitions"""
 # Standard
-from typing import Type
+from typing import Dict, Type
 
 # Third Party
 import pytest
 
 # Local
 from caikit.core import ModuleBase, TaskBase, module
 from caikit.interfaces.nlp import tasks as nlp_tasks
@@ -30,22 +30,29 @@
 
 
 class InvalidType:
     pass
 
 
 @pytest.mark.parametrize(
-    "task", (nlp_tasks.TextGenerationTask, nlp_tasks.TextGenerationStreamTask)
+    "flavor",
+    (
+        {"input_streaming": False, "output_streaming": False},
+        {"input_streaming": False, "output_streaming": True},
+    ),
 )
-def test_tasks(reset_globals, task: Type[TaskBase]):
+def test_tasks(reset_globals, flavor: Dict[str, bool]):
     """Common tests for all tasks"""
     # Only support single required param named "inputs"
-    assert set(task.get_required_parameters().keys()) == {"inputs"}
-    input_type = task.get_required_parameters()["inputs"]
-    output_type = task.get_output_type()
+    task = nlp_tasks.TextGenerationTask
+    assert set(task.get_required_parameters(flavor["input_streaming"]).keys()) == {
+        "inputs"
+    }
+    input_type = task.get_required_parameters(flavor["input_streaming"])["inputs"]
+    output_type = task.get_output_type(flavor["output_streaming"])
 
     # Version with the right signature and nothing else
     @module(id="foo1", name="Foo", version="0.0.0", task=task)
     class Foo1(ModuleBase):
         def run(self, inputs: input_type) -> output_type:
             return output_type()
 
@@ -62,25 +69,28 @@
             return output_type()
 
     # Version with missing required argument
     with pytest.raises(TypeError):
 
         @module(id="foo3", name="Foo", version="0.0.0", task=task)
         class Foo3(ModuleBase):
+            @task.taskmethod(**flavor)
             def run(self, other_name: str) -> output_type:
                 return output_type()
 
     # Version with bad required argument type
     with pytest.raises(TypeError):
 
         @module(id="foo4", name="Foo", version="0.0.0", task=task)
         class Foo4(ModuleBase):
+            @task.taskmethod(**flavor)
             def run(self, inputs: InvalidType) -> output_type:
                 return output_type()
 
     # Version with bad return type
     with pytest.raises(TypeError):
 
         @module(id="foo", name="Foo", version="0.0.0", task=task)
         class Foo(ModuleBase):
+            @task.taskmethod(**flavor)
             def run(self, inputs: input_type) -> InvalidType:
                 return "hi there"
```

### Comparing `caikit-0.9.3/tests/runtime/conftest.py` & `caikit-0.9.4/tests/runtime/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/generated/__init__.py` & `caikit-0.9.4/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/metrics/__init__.py` & `caikit-0.9.4/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.9.4/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/model_management/__init__.py` & `caikit-0.9.4/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/model_management/test_batcher.py` & `caikit-0.9.4/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/model_management/test_model_loader.py` & `caikit-0.9.4/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/model_management/test_model_manager.py` & `caikit-0.9.4/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.9.4/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/model_management/test_training_manager.py` & `caikit-0.9.4/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/service_generation/test_create_service.py` & `caikit-0.9.4/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.9.4/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/service_generation/test_protoable.py` & `caikit-0.9.4/tests/runtime/service_generation/test_protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.9.4/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.9.4/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/servicers/__init__.py` & `caikit-0.9.4/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.9.4/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.9.4/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.9.4/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.9.4/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.9.4/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/test_grpc_server.py` & `caikit-0.9.4/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/test_service_factory.py` & `caikit-0.9.4/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/utils/__init__.py` & `caikit-0.9.4/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/utils/test_import_util.py` & `caikit-0.9.4/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/utils/test_servicer_util.py` & `caikit-0.9.4/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/work_management/__init__.py` & `caikit-0.9.4/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.9.4/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.9.4/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.9.4/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.3/tox.ini` & `caikit-0.9.4/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 # Ensure compatibility is maintained with protobuf 3.X
 [testenv:proto3]
 description = run tests with pytest with coverage
 commands =
     pip uninstall grpcio-health-checking grpcio-reflection -y
     pip install protobuf==3.19.0 grpcio-health-checking grpcio-reflection --upgrade
-    pytest --cov=caikit --cov-report=html {posargs:tests}
+    pytest --cov=caikit --cov-report=html {posargs:tests -m "not examples"}
 
 # Ensure tests targeting caikit.core can be run with no optional dependencies
 [testenv:core]
 description = run tests against caikit.core without any extras
 base = ""
 extras = dev-test
 commands =
```

### Comparing `caikit-0.9.3/PKG-INFO` & `caikit-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.9.3
+Version: 0.9.4
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
```

