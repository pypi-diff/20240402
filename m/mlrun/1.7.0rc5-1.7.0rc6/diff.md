# Comparing `tmp/mlrun-1.7.0rc5-py3-none-any.whl.zip` & `tmp/mlrun-1.7.0rc6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,325 +1,328 @@
-Zip file size: 1042940 bytes, number of entries: 323
--rw-r--r--  2.0 unx     7248 b- defN 24-Mar-13 15:32 mlrun/__init__.py
--rw-r--r--  2.0 unx    49229 b- defN 24-Mar-13 15:32 mlrun/__main__.py
--rw-r--r--  2.0 unx    62563 b- defN 24-Mar-13 15:32 mlrun/config.py
--rw-r--r--  2.0 unx     7080 b- defN 24-Mar-13 15:32 mlrun/errors.py
--rw-r--r--  2.0 unx    40866 b- defN 24-Mar-13 15:32 mlrun/execution.py
--rw-r--r--  2.0 unx    15569 b- defN 24-Mar-13 15:32 mlrun/features.py
--rw-r--r--  2.0 unx     7023 b- defN 24-Mar-13 15:32 mlrun/k8s_utils.py
--rw-r--r--  2.0 unx    30481 b- defN 24-Mar-13 15:32 mlrun/kfpops.py
--rw-r--r--  2.0 unx     8286 b- defN 24-Mar-13 15:32 mlrun/lists.py
--rw-r--r--  2.0 unx    70583 b- defN 24-Mar-13 15:32 mlrun/model.py
--rw-r--r--  2.0 unx    13009 b- defN 24-Mar-13 15:32 mlrun/render.py
--rw-r--r--  2.0 unx    42400 b- defN 24-Mar-13 15:32 mlrun/run.py
--rw-r--r--  2.0 unx     7776 b- defN 24-Mar-13 15:32 mlrun/secrets.py
--rw-r--r--  2.0 unx    14211 b- defN 24-Mar-13 15:32 mlrun/api/schemas/__init__.py
--rw-r--r--  2.0 unx     1187 b- defN 24-Mar-13 15:32 mlrun/artifacts/__init__.py
--rw-r--r--  2.0 unx    34970 b- defN 24-Mar-13 15:32 mlrun/artifacts/base.py
--rw-r--r--  2.0 unx    22360 b- defN 24-Mar-13 15:32 mlrun/artifacts/dataset.py
--rw-r--r--  2.0 unx    14425 b- defN 24-Mar-13 15:32 mlrun/artifacts/manager.py
--rw-r--r--  2.0 unx    25205 b- defN 24-Mar-13 15:32 mlrun/artifacts/model.py
--rw-r--r--  2.0 unx    15701 b- defN 24-Mar-13 15:32 mlrun/artifacts/plots.py
--rw-r--r--  2.0 unx      571 b- defN 24-Mar-13 15:32 mlrun/common/__init__.py
--rw-r--r--  2.0 unx      745 b- defN 24-Mar-13 15:32 mlrun/common/constants.py
--rw-r--r--  2.0 unx     1087 b- defN 24-Mar-13 15:32 mlrun/common/helpers.py
--rw-r--r--  2.0 unx     5181 b- defN 24-Mar-13 15:32 mlrun/common/secrets.py
--rw-r--r--  2.0 unx      790 b- defN 24-Mar-13 15:32 mlrun/common/types.py
--rw-r--r--  2.0 unx      571 b- defN 24-Mar-13 15:32 mlrun/common/db/__init__.py
--rw-r--r--  2.0 unx     2659 b- defN 24-Mar-13 15:32 mlrun/common/db/sql_session.py
--rw-r--r--  2.0 unx      721 b- defN 24-Mar-13 15:32 mlrun/common/model_monitoring/__init__.py
--rw-r--r--  2.0 unx     4405 b- defN 24-Mar-13 15:32 mlrun/common/model_monitoring/helpers.py
--rw-r--r--  2.0 unx     4935 b- defN 24-Mar-13 15:32 mlrun/common/schemas/__init__.py
--rw-r--r--  2.0 unx     2344 b- defN 24-Mar-13 15:32 mlrun/common/schemas/api_gateway.py
--rw-r--r--  2.0 unx     2796 b- defN 24-Mar-13 15:32 mlrun/common/schemas/artifact.py
--rw-r--r--  2.0 unx     5970 b- defN 24-Mar-13 15:32 mlrun/common/schemas/auth.py
--rw-r--r--  2.0 unx     1707 b- defN 24-Mar-13 15:32 mlrun/common/schemas/background_task.py
--rw-r--r--  2.0 unx     2858 b- defN 24-Mar-13 15:32 mlrun/common/schemas/client_spec.py
--rw-r--r--  2.0 unx      888 b- defN 24-Mar-13 15:32 mlrun/common/schemas/clusterization_spec.py
--rw-r--r--  2.0 unx     1557 b- defN 24-Mar-13 15:32 mlrun/common/schemas/common.py
--rw-r--r--  2.0 unx     6476 b- defN 24-Mar-13 15:32 mlrun/common/schemas/constants.py
--rw-r--r--  2.0 unx      750 b- defN 24-Mar-13 15:32 mlrun/common/schemas/datastore_profile.py
--rw-r--r--  2.0 unx     1026 b- defN 24-Mar-13 15:32 mlrun/common/schemas/events.py
--rw-r--r--  2.0 unx     3717 b- defN 24-Mar-13 15:32 mlrun/common/schemas/feature_store.py
--rw-r--r--  2.0 unx     2418 b- defN 24-Mar-13 15:32 mlrun/common/schemas/frontend_spec.py
--rw-r--r--  2.0 unx     4577 b- defN 24-Mar-13 15:32 mlrun/common/schemas/function.py
--rw-r--r--  2.0 unx      705 b- defN 24-Mar-13 15:32 mlrun/common/schemas/http.py
--rw-r--r--  2.0 unx     4203 b- defN 24-Mar-13 15:32 mlrun/common/schemas/hub.py
--rw-r--r--  2.0 unx     1395 b- defN 24-Mar-13 15:32 mlrun/common/schemas/k8s.py
--rw-r--r--  2.0 unx      892 b- defN 24-Mar-13 15:32 mlrun/common/schemas/memory_reports.py
--rw-r--r--  2.0 unx     1768 b- defN 24-Mar-13 15:32 mlrun/common/schemas/notification.py
--rw-r--r--  2.0 unx     1980 b- defN 24-Mar-13 15:32 mlrun/common/schemas/object.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Mar-13 15:32 mlrun/common/schemas/pipeline.py
--rw-r--r--  2.0 unx     4277 b- defN 24-Mar-13 15:32 mlrun/common/schemas/project.py
--rw-r--r--  2.0 unx      776 b- defN 24-Mar-13 15:32 mlrun/common/schemas/regex.py
--rw-r--r--  2.0 unx      745 b- defN 24-Mar-13 15:32 mlrun/common/schemas/runs.py
--rw-r--r--  2.0 unx     1554 b- defN 24-Mar-13 15:32 mlrun/common/schemas/runtime_resource.py
--rw-r--r--  2.0 unx     4287 b- defN 24-Mar-13 15:32 mlrun/common/schemas/schedule.py
--rw-r--r--  2.0 unx     1484 b- defN 24-Mar-13 15:32 mlrun/common/schemas/secret.py
--rw-r--r--  2.0 unx      884 b- defN 24-Mar-13 15:32 mlrun/common/schemas/tag.py
--rw-r--r--  2.0 unx     1823 b- defN 24-Mar-13 15:32 mlrun/common/schemas/workflow.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Mar-13 15:32 mlrun/common/schemas/model_monitoring/__init__.py
--rw-r--r--  2.0 unx     7822 b- defN 24-Mar-13 15:32 mlrun/common/schemas/model_monitoring/constants.py
--rw-r--r--  2.0 unx     1431 b- defN 24-Mar-13 15:32 mlrun/common/schemas/model_monitoring/grafana.py
--rw-r--r--  2.0 unx    12000 b- defN 24-Mar-13 15:32 mlrun/common/schemas/model_monitoring/model_endpoints.py
--rw-r--r--  2.0 unx     1087 b- defN 24-Mar-13 15:32 mlrun/data_types/__init__.py
--rw-r--r--  2.0 unx     4647 b- defN 24-Mar-13 15:32 mlrun/data_types/data_types.py
--rw-r--r--  2.0 unx     6134 b- defN 24-Mar-13 15:32 mlrun/data_types/infer.py
--rw-r--r--  2.0 unx     9457 b- defN 24-Mar-13 15:32 mlrun/data_types/spark.py
--rw-r--r--  2.0 unx     9945 b- defN 24-Mar-13 15:32 mlrun/data_types/to_pandas.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Mar-13 15:32 mlrun/datastore/__init__.py
--rw-r--r--  2.0 unx     9168 b- defN 24-Mar-13 15:32 mlrun/datastore/azure_blob.py
--rw-r--r--  2.0 unx    24175 b- defN 24-Mar-13 15:32 mlrun/datastore/base.py
--rw-r--r--  2.0 unx     9018 b- defN 24-Mar-13 15:32 mlrun/datastore/datastore.py
--rw-r--r--  2.0 unx    15985 b- defN 24-Mar-13 15:32 mlrun/datastore/datastore_profile.py
--rw-r--r--  2.0 unx     6634 b- defN 24-Mar-13 15:32 mlrun/datastore/dbfs_store.py
--rw-r--r--  2.0 unx     3767 b- defN 24-Mar-13 15:32 mlrun/datastore/filestore.py
--rw-r--r--  2.0 unx     6112 b- defN 24-Mar-13 15:32 mlrun/datastore/google_cloud_storage.py
--rw-r--r--  2.0 unx     1674 b- defN 24-Mar-13 15:32 mlrun/datastore/hdfs.py
--rw-r--r--  2.0 unx      622 b- defN 24-Mar-13 15:32 mlrun/datastore/helpers.py
--rw-r--r--  2.0 unx     2779 b- defN 24-Mar-13 15:32 mlrun/datastore/inmem.py
--rw-r--r--  2.0 unx     5575 b- defN 24-Mar-13 15:32 mlrun/datastore/redis.py
--rw-r--r--  2.0 unx     8110 b- defN 24-Mar-13 15:32 mlrun/datastore/s3.py
--rw-r--r--  2.0 unx    40060 b- defN 24-Mar-13 15:32 mlrun/datastore/sources.py
--rw-r--r--  2.0 unx     1498 b- defN 24-Mar-13 15:32 mlrun/datastore/spark_udf.py
--rw-r--r--  2.0 unx     1611 b- defN 24-Mar-13 15:32 mlrun/datastore/spark_utils.py
--rw-r--r--  2.0 unx     6839 b- defN 24-Mar-13 15:32 mlrun/datastore/store_resources.py
--rw-r--r--  2.0 unx    70714 b- defN 24-Mar-13 15:32 mlrun/datastore/targets.py
--rw-r--r--  2.0 unx     5227 b- defN 24-Mar-13 15:32 mlrun/datastore/utils.py
--rw-r--r--  2.0 unx     9252 b- defN 24-Mar-13 15:32 mlrun/datastore/v3io.py
--rw-r--r--  2.0 unx     1343 b- defN 24-Mar-13 15:32 mlrun/datastore/wasbfs/__init__.py
--rw-r--r--  2.0 unx     6151 b- defN 24-Mar-13 15:32 mlrun/datastore/wasbfs/fs.py
--rw-r--r--  2.0 unx     1163 b- defN 24-Mar-13 15:32 mlrun/db/__init__.py
--rw-r--r--  2.0 unx    18906 b- defN 24-Mar-13 15:32 mlrun/db/base.py
--rw-r--r--  2.0 unx     2403 b- defN 24-Mar-13 15:32 mlrun/db/factory.py
--rw-r--r--  2.0 unx   158600 b- defN 24-Mar-13 15:32 mlrun/db/httpdb.py
--rw-r--r--  2.0 unx    14814 b- defN 24-Mar-13 15:32 mlrun/db/nopdb.py
--rw-r--r--  2.0 unx     1584 b- defN 24-Mar-13 15:32 mlrun/feature_store/__init__.py
--rw-r--r--  2.0 unx    49480 b- defN 24-Mar-13 15:32 mlrun/feature_store/api.py
--rw-r--r--  2.0 unx    12853 b- defN 24-Mar-13 15:32 mlrun/feature_store/common.py
--rw-r--r--  2.0 unx    55295 b- defN 24-Mar-13 15:32 mlrun/feature_store/feature_set.py
--rw-r--r--  2.0 unx    43560 b- defN 24-Mar-13 15:32 mlrun/feature_store/feature_vector.py
--rw-r--r--  2.0 unx    11210 b- defN 24-Mar-13 15:32 mlrun/feature_store/ingestion.py
--rw-r--r--  2.0 unx    28882 b- defN 24-Mar-13 15:32 mlrun/feature_store/steps.py
--rw-r--r--  2.0 unx     1282 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/__init__.py
--rw-r--r--  2.0 unx    30004 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/base.py
--rw-r--r--  2.0 unx    11654 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/conversion.py
--rw-r--r--  2.0 unx     5491 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/dask_merger.py
--rw-r--r--  2.0 unx     8261 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/job.py
--rw-r--r--  2.0 unx     4429 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/local_merger.py
--rw-r--r--  2.0 unx    11165 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/spark_merger.py
--rw-r--r--  2.0 unx     6314 b- defN 24-Mar-13 15:32 mlrun/feature_store/retrieval/storey_merger.py
--rw-r--r--  2.0 unx      743 b- defN 24-Mar-13 15:32 mlrun/frameworks/__init__.py
--rw-r--r--  2.0 unx    11487 b- defN 24-Mar-13 15:32 mlrun/frameworks/parallel_coordinates.py
--rw-r--r--  2.0 unx      962 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/__init__.py
--rw-r--r--  2.0 unx     8497 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/artifacts_library.py
--rw-r--r--  2.0 unx    20999 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/mlrun_interface.py
--rw-r--r--  2.0 unx    55312 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/model_handler.py
--rw-r--r--  2.0 unx     3445 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/plan.py
--rw-r--r--  2.0 unx     5727 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/producer.py
--rw-r--r--  2.0 unx     9131 b- defN 24-Mar-13 15:32 mlrun/frameworks/_common/utils.py
--rw-r--r--  2.0 unx      750 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/__init__.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/model_handler.py
--rw-r--r--  2.0 unx      996 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/utils.py
--rw-r--r--  2.0 unx      787 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/loggers/__init__.py
--rw-r--r--  2.0 unx    11477 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/loggers/logger.py
--rw-r--r--  2.0 unx    14748 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/loggers/mlrun_logger.py
--rw-r--r--  2.0 unx    27936 b- defN 24-Mar-13 15:32 mlrun/frameworks/_dl_common/loggers/tensorboard_logger.py
--rw-r--r--  2.0 unx      956 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/__init__.py
--rw-r--r--  2.0 unx     3145 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/artifacts_library.py
--rw-r--r--  2.0 unx    16885 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/model_handler.py
--rw-r--r--  2.0 unx     2717 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/pkl_model_server.py
--rw-r--r--  2.0 unx     4869 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plan.py
--rw-r--r--  2.0 unx     4061 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/producer.py
--rw-r--r--  2.0 unx    10477 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/utils.py
--rw-r--r--  2.0 unx      737 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/loggers/__init__.py
--rw-r--r--  2.0 unx     5630 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/loggers/logger.py
--rw-r--r--  2.0 unx     6406 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/loggers/mlrun_logger.py
--rw-r--r--  2.0 unx      922 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plans/__init__.py
--rw-r--r--  2.0 unx     4894 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plans/calibration_curve_plan.py
--rw-r--r--  2.0 unx     6030 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plans/confusion_matrix_plan.py
--rw-r--r--  2.0 unx     6611 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plans/dataset_plan.py
--rw-r--r--  2.0 unx     5285 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plans/feature_importance_plan.py
--rw-r--r--  2.0 unx     6963 b- defN 24-Mar-13 15:32 mlrun/frameworks/_ml_common/plans/roc_curve_plan.py
--rw-r--r--  2.0 unx      706 b- defN 24-Mar-13 15:32 mlrun/frameworks/auto_mlrun/__init__.py
--rw-r--r--  2.0 unx    24074 b- defN 24-Mar-13 15:32 mlrun/frameworks/auto_mlrun/auto_mlrun.py
--rw-r--r--  2.0 unx      721 b- defN 24-Mar-13 15:32 mlrun/frameworks/huggingface/__init__.py
--rw-r--r--  2.0 unx     6043 b- defN 24-Mar-13 15:32 mlrun/frameworks/huggingface/model_server.py
--rw-r--r--  2.0 unx    15873 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/__init__.py
--rw-r--r--  2.0 unx    13791 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/model_handler.py
--rw-r--r--  2.0 unx     9156 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/model_server.py
--rw-r--r--  2.0 unx     8265 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/utils.py
--rw-r--r--  2.0 unx      857 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/callbacks/__init__.py
--rw-r--r--  2.0 unx     4081 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/callbacks/callback.py
--rw-r--r--  2.0 unx     5111 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/callbacks/logging_callback.py
--rw-r--r--  2.0 unx     4061 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/callbacks/mlrun_logging_callback.py
--rw-r--r--  2.0 unx      842 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/mlrun_interfaces/__init__.py
--rw-r--r--  2.0 unx     1531 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/mlrun_interfaces/booster_mlrun_interface.py
--rw-r--r--  2.0 unx    14221 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/mlrun_interfaces/mlrun_interface.py
--rw-r--r--  2.0 unx     1333 b- defN 24-Mar-13 15:32 mlrun/frameworks/lgbm/mlrun_interfaces/model_mlrun_interface.py
--rw-r--r--  2.0 unx      791 b- defN 24-Mar-13 15:32 mlrun/frameworks/onnx/__init__.py
--rw-r--r--  2.0 unx     6085 b- defN 24-Mar-13 15:32 mlrun/frameworks/onnx/dataset.py
--rw-r--r--  2.0 unx     2399 b- defN 24-Mar-13 15:32 mlrun/frameworks/onnx/mlrun_interface.py
--rw-r--r--  2.0 unx     6125 b- defN 24-Mar-13 15:32 mlrun/frameworks/onnx/model_handler.py
--rw-r--r--  2.0 unx     7021 b- defN 24-Mar-13 15:32 mlrun/frameworks/onnx/model_server.py
--rw-r--r--  2.0 unx    22037 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/__init__.py
--rw-r--r--  2.0 unx    27885 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/callbacks_handler.py
--rw-r--r--  2.0 unx    44621 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/mlrun_interface.py
--rw-r--r--  2.0 unx    22290 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/model_handler.py
--rw-r--r--  2.0 unx    10094 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/model_server.py
--rw-r--r--  2.0 unx     4515 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/utils.py
--rw-r--r--  2.0 unx      896 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/callbacks/__init__.py
--rw-r--r--  2.0 unx    11500 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/callbacks/callback.py
--rw-r--r--  2.0 unx    23126 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/callbacks/logging_callback.py
--rw-r--r--  2.0 unx     9239 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/callbacks/mlrun_logging_callback.py
--rw-r--r--  2.0 unx    26299 b- defN 24-Mar-13 15:32 mlrun/frameworks/pytorch/callbacks/tensorboard_logging_callback.py
--rw-r--r--  2.0 unx    10880 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/__init__.py
--rw-r--r--  2.0 unx     5840 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/estimator.py
--rw-r--r--  2.0 unx     7089 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/metric.py
--rw-r--r--  2.0 unx    12203 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/metrics_library.py
--rw-r--r--  2.0 unx    14054 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/mlrun_interface.py
--rw-r--r--  2.0 unx     4695 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/model_handler.py
--rw-r--r--  2.0 unx     1209 b- defN 24-Mar-13 15:32 mlrun/frameworks/sklearn/utils.py
--rw-r--r--  2.0 unx    10447 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/__init__.py
--rw-r--r--  2.0 unx    16610 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/mlrun_interface.py
--rw-r--r--  2.0 unx    28102 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/model_handler.py
--rw-r--r--  2.0 unx     9529 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/model_server.py
--rw-r--r--  2.0 unx     4284 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/utils.py
--rw-r--r--  2.0 unx      844 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/callbacks/__init__.py
--rw-r--r--  2.0 unx    21855 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/callbacks/logging_callback.py
--rw-r--r--  2.0 unx     8701 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/callbacks/mlrun_logging_callback.py
--rw-r--r--  2.0 unx    28419 b- defN 24-Mar-13 15:32 mlrun/frameworks/tf_keras/callbacks/tensorboard_logging_callback.py
--rw-r--r--  2.0 unx    10276 b- defN 24-Mar-13 15:32 mlrun/frameworks/xgboost/__init__.py
--rw-r--r--  2.0 unx      878 b- defN 24-Mar-13 15:32 mlrun/frameworks/xgboost/mlrun_interface.py
--rw-r--r--  2.0 unx    11530 b- defN 24-Mar-13 15:32 mlrun/frameworks/xgboost/model_handler.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Mar-13 15:32 mlrun/frameworks/xgboost/utils.py
--rw-r--r--  2.0 unx      577 b- defN 24-Mar-13 15:32 mlrun/launcher/__init__.py
--rw-r--r--  2.0 unx    16438 b- defN 24-Mar-13 15:32 mlrun/launcher/base.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Mar-13 15:32 mlrun/launcher/client.py
--rw-r--r--  2.0 unx     2344 b- defN 24-Mar-13 15:32 mlrun/launcher/factory.py
--rw-r--r--  2.0 unx    10915 b- defN 24-Mar-13 15:32 mlrun/launcher/local.py
--rw-r--r--  2.0 unx     7475 b- defN 24-Mar-13 15:32 mlrun/launcher/remote.py
--rw-r--r--  2.0 unx      915 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/__init__.py
--rw-r--r--  2.0 unx    36626 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/api.py
--rw-r--r--  2.0 unx    12282 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/application.py
--rw-r--r--  2.0 unx    39836 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/batch.py
--rw-r--r--  2.0 unx    28342 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/controller.py
--rw-r--r--  2.0 unx     1336 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/controller_handler.py
--rw-r--r--  2.0 unx     4824 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/evidently_application.py
--rw-r--r--  2.0 unx    24866 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/features_drift_table.py
--rw-r--r--  2.0 unx     7302 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/helpers.py
--rw-r--r--  2.0 unx     3938 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/model_endpoint.py
--rw-r--r--  2.0 unx     7578 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/prometheus.py
--rw-r--r--  2.0 unx    48113 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stream_processing.py
--rw-r--r--  2.0 unx     5283 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/tracking_policy.py
--rw-r--r--  2.0 unx     8669 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/writer.py
--rw-r--r--  2.0 unx      569 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/applications/__init__.py
--rw-r--r--  2.0 unx     8005 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/applications/histogram_data_drift.py
--rw-r--r--  2.0 unx      569 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/metrics/__init__.py
--rw-r--r--  2.0 unx     4724 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/metrics/histogram_distance.py
--rw-r--r--  2.0 unx     4525 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/__init__.py
--rw-r--r--  2.0 unx    22222 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/kv_model_endpoint_store.py
--rw-r--r--  2.0 unx     5590 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/model_endpoint_store.py
--rw-r--r--  2.0 unx    16139 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/sql_model_endpoint_store.py
--rw-r--r--  2.0 unx     1111 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/models/__init__.py
--rw-r--r--  2.0 unx     2801 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/models/base.py
--rw-r--r--  2.0 unx     1131 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/models/mysql.py
--rw-r--r--  2.0 unx      765 b- defN 24-Mar-13 15:32 mlrun/model_monitoring/stores/models/sqlite.py
--rw-r--r--  2.0 unx     7082 b- defN 24-Mar-13 15:32 mlrun/package/__init__.py
--rw-r--r--  2.0 unx    14589 b- defN 24-Mar-13 15:32 mlrun/package/context_handler.py
--rw-r--r--  2.0 unx     1204 b- defN 24-Mar-13 15:32 mlrun/package/errors.py
--rw-r--r--  2.0 unx    15064 b- defN 24-Mar-13 15:32 mlrun/package/packager.py
--rw-r--r--  2.0 unx    37160 b- defN 24-Mar-13 15:32 mlrun/package/packagers_manager.py
--rw-r--r--  2.0 unx      769 b- defN 24-Mar-13 15:32 mlrun/package/packagers/__init__.py
--rw-r--r--  2.0 unx    26625 b- defN 24-Mar-13 15:32 mlrun/package/packagers/default_packager.py
--rw-r--r--  2.0 unx    25602 b- defN 24-Mar-13 15:32 mlrun/package/packagers/numpy_packagers.py
--rw-r--r--  2.0 unx    35761 b- defN 24-Mar-13 15:32 mlrun/package/packagers/pandas_packagers.py
--rw-r--r--  2.0 unx    22322 b- defN 24-Mar-13 15:32 mlrun/package/packagers/python_standard_library_packagers.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Mar-13 15:32 mlrun/package/utils/__init__.py
--rw-r--r--  2.0 unx     7951 b- defN 24-Mar-13 15:32 mlrun/package/utils/_archiver.py
--rw-r--r--  2.0 unx     6373 b- defN 24-Mar-13 15:32 mlrun/package/utils/_formatter.py
--rw-r--r--  2.0 unx    10341 b- defN 24-Mar-13 15:32 mlrun/package/utils/_pickler.py
--rw-r--r--  2.0 unx     2357 b- defN 24-Mar-13 15:32 mlrun/package/utils/_supported_format.py
--rw-r--r--  2.0 unx     3696 b- defN 24-Mar-13 15:32 mlrun/package/utils/log_hint_utils.py
--rw-r--r--  2.0 unx    14695 b- defN 24-Mar-13 15:32 mlrun/package/utils/type_hint_utils.py
--rw-r--r--  2.0 unx     2352 b- defN 24-Mar-13 15:32 mlrun/platforms/__init__.py
--rw-r--r--  2.0 unx    19434 b- defN 24-Mar-13 15:32 mlrun/platforms/iguazio.py
--rw-r--r--  2.0 unx    11828 b- defN 24-Mar-13 15:32 mlrun/platforms/other.py
--rw-r--r--  2.0 unx     1153 b- defN 24-Mar-13 15:32 mlrun/projects/__init__.py
--rw-r--r--  2.0 unx    18538 b- defN 24-Mar-13 15:32 mlrun/projects/operations.py
--rw-r--r--  2.0 unx    40124 b- defN 24-Mar-13 15:32 mlrun/projects/pipelines.py
--rw-r--r--  2.0 unx   158052 b- defN 24-Mar-13 15:32 mlrun/projects/project.py
--rw-r--r--  2.0 unx     7034 b- defN 24-Mar-13 15:32 mlrun/runtimes/__init__.py
--rw-r--r--  2.0 unx    36562 b- defN 24-Mar-13 15:32 mlrun/runtimes/base.py
--rw-r--r--  2.0 unx     9513 b- defN 24-Mar-13 15:32 mlrun/runtimes/constants.py
--rw-r--r--  2.0 unx    19149 b- defN 24-Mar-13 15:32 mlrun/runtimes/daskjob.py
--rw-r--r--  2.0 unx    10508 b- defN 24-Mar-13 15:32 mlrun/runtimes/funcdoc.py
--rw-r--r--  2.0 unx     4918 b- defN 24-Mar-13 15:32 mlrun/runtimes/function_reference.py
--rw-r--r--  2.0 unx     7241 b- defN 24-Mar-13 15:32 mlrun/runtimes/generators.py
--rw-r--r--  2.0 unx    12500 b- defN 24-Mar-13 15:32 mlrun/runtimes/kubejob.py
--rw-r--r--  2.0 unx    21783 b- defN 24-Mar-13 15:32 mlrun/runtimes/local.py
--rw-r--r--  2.0 unx    58650 b- defN 24-Mar-13 15:32 mlrun/runtimes/pod.py
--rw-r--r--  2.0 unx     7326 b- defN 24-Mar-13 15:32 mlrun/runtimes/remotesparkjob.py
--rw-r--r--  2.0 unx    16004 b- defN 24-Mar-13 15:32 mlrun/runtimes/utils.py
--rw-r--r--  2.0 unx      569 b- defN 24-Mar-13 15:32 mlrun/runtimes/databricks_job/__init__.py
--rw-r--r--  2.0 unx     2245 b- defN 24-Mar-13 15:32 mlrun/runtimes/databricks_job/databricks_cancel_task.py
--rw-r--r--  2.0 unx    12749 b- defN 24-Mar-13 15:32 mlrun/runtimes/databricks_job/databricks_runtime.py
--rw-r--r--  2.0 unx     8679 b- defN 24-Mar-13 15:32 mlrun/runtimes/databricks_job/databricks_wrapper.py
--rw-r--r--  2.0 unx     1583 b- defN 24-Mar-13 15:32 mlrun/runtimes/mpijob/__init__.py
--rw-r--r--  2.0 unx     9161 b- defN 24-Mar-13 15:32 mlrun/runtimes/mpijob/abstract.py
--rw-r--r--  2.0 unx     3206 b- defN 24-Mar-13 15:32 mlrun/runtimes/mpijob/v1.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Mar-13 15:32 mlrun/runtimes/mpijob/v1alpha1.py
--rw-r--r--  2.0 unx      794 b- defN 24-Mar-13 15:32 mlrun/runtimes/nuclio/__init__.py
--rw-r--r--  2.0 unx    10277 b- defN 24-Mar-13 15:32 mlrun/runtimes/nuclio/api_gateway.py
--rw-r--r--  2.0 unx    47402 b- defN 24-Mar-13 15:32 mlrun/runtimes/nuclio/function.py
--rw-r--r--  2.0 unx     2942 b- defN 24-Mar-13 15:32 mlrun/runtimes/nuclio/nuclio.py
--rw-r--r--  2.0 unx    30363 b- defN 24-Mar-13 15:32 mlrun/runtimes/nuclio/serving.py
--rw-r--r--  2.0 unx      709 b- defN 24-Mar-13 15:32 mlrun/runtimes/sparkjob/__init__.py
--rw-r--r--  2.0 unx    41189 b- defN 24-Mar-13 15:32 mlrun/runtimes/sparkjob/spark3job.py
--rw-r--r--  2.0 unx     1078 b- defN 24-Mar-13 15:32 mlrun/serving/__init__.py
--rw-r--r--  2.0 unx     6116 b- defN 24-Mar-13 15:32 mlrun/serving/merger.py
--rw-r--r--  2.0 unx    18010 b- defN 24-Mar-13 15:32 mlrun/serving/remote.py
--rw-r--r--  2.0 unx    54976 b- defN 24-Mar-13 15:32 mlrun/serving/routers.py
--rw-r--r--  2.0 unx    21161 b- defN 24-Mar-13 15:32 mlrun/serving/server.py
--rw-r--r--  2.0 unx      836 b- defN 24-Mar-13 15:32 mlrun/serving/serving_wrapper.py
--rw-r--r--  2.0 unx    56175 b- defN 24-Mar-13 15:32 mlrun/serving/states.py
--rw-r--r--  2.0 unx     3871 b- defN 24-Mar-13 15:32 mlrun/serving/utils.py
--rw-r--r--  2.0 unx    11805 b- defN 24-Mar-13 15:32 mlrun/serving/v1_serving.py
--rw-r--r--  2.0 unx    23559 b- defN 24-Mar-13 15:32 mlrun/serving/v2_serving.py
--rw-r--r--  2.0 unx      765 b- defN 24-Mar-13 15:32 mlrun/track/__init__.py
--rw-r--r--  2.0 unx     3541 b- defN 24-Mar-13 15:32 mlrun/track/tracker.py
--rw-r--r--  2.0 unx     5726 b- defN 24-Mar-13 15:32 mlrun/track/tracker_manager.py
--rw-r--r--  2.0 unx      569 b- defN 24-Mar-13 15:32 mlrun/track/trackers/__init__.py
--rw-r--r--  2.0 unx    23258 b- defN 24-Mar-13 15:32 mlrun/track/trackers/mlflow_tracker.py
--rw-r--r--  2.0 unx      826 b- defN 24-Mar-13 15:32 mlrun/utils/__init__.py
--rw-r--r--  2.0 unx    11092 b- defN 24-Mar-13 15:32 mlrun/utils/async_http.py
--rw-r--r--  2.0 unx     3450 b- defN 24-Mar-13 15:32 mlrun/utils/azure_vault.py
--rw-r--r--  2.0 unx     7361 b- defN 24-Mar-13 15:32 mlrun/utils/clones.py
--rw-r--r--  2.0 unx     1897 b- defN 24-Mar-13 15:32 mlrun/utils/condition_evaluator.py
--rw-r--r--  2.0 unx     1713 b- defN 24-Mar-13 15:32 mlrun/utils/db.py
--rw-r--r--  2.0 unx    51162 b- defN 24-Mar-13 15:32 mlrun/utils/helpers.py
--rw-r--r--  2.0 unx     8700 b- defN 24-Mar-13 15:32 mlrun/utils/http.py
--rw-r--r--  2.0 unx     8133 b- defN 24-Mar-13 15:32 mlrun/utils/logger.py
--rw-r--r--  2.0 unx     4581 b- defN 24-Mar-13 15:32 mlrun/utils/regex.py
--rw-r--r--  2.0 unx     7522 b- defN 24-Mar-13 15:32 mlrun/utils/retryer.py
--rw-r--r--  2.0 unx      869 b- defN 24-Mar-13 15:32 mlrun/utils/singleton.py
--rw-r--r--  2.0 unx     1284 b- defN 24-Mar-13 15:32 mlrun/utils/v3io_clients.py
--rw-r--r--  2.0 unx    10447 b- defN 24-Mar-13 15:32 mlrun/utils/vault.py
--rw-r--r--  2.0 unx      990 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/__init__.py
--rw-r--r--  2.0 unx    21679 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification_pusher.py
--rw-r--r--  2.0 unx     2092 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/__init__.py
--rw-r--r--  2.0 unx     2279 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/base.py
--rw-r--r--  2.0 unx     2532 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/console.py
--rw-r--r--  2.0 unx     5221 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/git.py
--rw-r--r--  2.0 unx     1955 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/ipython.py
--rw-r--r--  2.0 unx     3898 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/slack.py
--rw-r--r--  2.0 unx     2390 b- defN 24-Mar-13 15:32 mlrun/utils/notifications/notification/webhook.py
--rw-r--r--  2.0 unx      614 b- defN 24-Mar-13 15:32 mlrun/utils/version/__init__.py
--rw-r--r--  2.0 unx       88 b- defN 24-Mar-13 15:32 mlrun/utils/version/version.json
--rw-r--r--  2.0 unx     1878 b- defN 24-Mar-13 15:32 mlrun/utils/version/version.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-13 15:32 mlrun-1.7.0rc5.dist-info/LICENSE
--rw-r--r--  2.0 unx    18263 b- defN 24-Mar-13 15:32 mlrun-1.7.0rc5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-13 15:32 mlrun-1.7.0rc5.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-13 15:32 mlrun-1.7.0rc5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Mar-13 15:32 mlrun-1.7.0rc5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    29627 b- defN 24-Mar-13 15:32 mlrun-1.7.0rc5.dist-info/RECORD
-323 files, 3819668 bytes uncompressed, 995946 bytes compressed:  73.9%
+Zip file size: 1050959 bytes, number of entries: 326
+-rw-r--r--  2.0 unx     7248 b- defN 24-Mar-20 16:47 mlrun/__init__.py
+-rw-r--r--  2.0 unx    49229 b- defN 24-Mar-20 16:47 mlrun/__main__.py
+-rw-r--r--  2.0 unx    62775 b- defN 24-Mar-20 16:47 mlrun/config.py
+-rw-r--r--  2.0 unx     7080 b- defN 24-Mar-20 16:47 mlrun/errors.py
+-rw-r--r--  2.0 unx    40866 b- defN 24-Mar-20 16:47 mlrun/execution.py
+-rw-r--r--  2.0 unx    15569 b- defN 24-Mar-20 16:47 mlrun/features.py
+-rw-r--r--  2.0 unx     7023 b- defN 24-Mar-20 16:47 mlrun/k8s_utils.py
+-rw-r--r--  2.0 unx    30481 b- defN 24-Mar-20 16:47 mlrun/kfpops.py
+-rw-r--r--  2.0 unx     8286 b- defN 24-Mar-20 16:47 mlrun/lists.py
+-rw-r--r--  2.0 unx    70583 b- defN 24-Mar-20 16:47 mlrun/model.py
+-rw-r--r--  2.0 unx    13009 b- defN 24-Mar-20 16:47 mlrun/render.py
+-rw-r--r--  2.0 unx    42822 b- defN 24-Mar-20 16:47 mlrun/run.py
+-rw-r--r--  2.0 unx     7776 b- defN 24-Mar-20 16:47 mlrun/secrets.py
+-rw-r--r--  2.0 unx    14211 b- defN 24-Mar-20 16:47 mlrun/api/schemas/__init__.py
+-rw-r--r--  2.0 unx     1187 b- defN 24-Mar-20 16:47 mlrun/artifacts/__init__.py
+-rw-r--r--  2.0 unx    34978 b- defN 24-Mar-20 16:47 mlrun/artifacts/base.py
+-rw-r--r--  2.0 unx    22360 b- defN 24-Mar-20 16:47 mlrun/artifacts/dataset.py
+-rw-r--r--  2.0 unx    14425 b- defN 24-Mar-20 16:47 mlrun/artifacts/manager.py
+-rw-r--r--  2.0 unx    25205 b- defN 24-Mar-20 16:47 mlrun/artifacts/model.py
+-rw-r--r--  2.0 unx    15860 b- defN 24-Mar-20 16:47 mlrun/artifacts/plots.py
+-rw-r--r--  2.0 unx      571 b- defN 24-Mar-20 16:47 mlrun/common/__init__.py
+-rw-r--r--  2.0 unx      745 b- defN 24-Mar-20 16:47 mlrun/common/constants.py
+-rw-r--r--  2.0 unx     1087 b- defN 24-Mar-20 16:47 mlrun/common/helpers.py
+-rw-r--r--  2.0 unx     5181 b- defN 24-Mar-20 16:47 mlrun/common/secrets.py
+-rw-r--r--  2.0 unx      790 b- defN 24-Mar-20 16:47 mlrun/common/types.py
+-rw-r--r--  2.0 unx      571 b- defN 24-Mar-20 16:47 mlrun/common/db/__init__.py
+-rw-r--r--  2.0 unx     2659 b- defN 24-Mar-20 16:47 mlrun/common/db/sql_session.py
+-rw-r--r--  2.0 unx      721 b- defN 24-Mar-20 16:47 mlrun/common/model_monitoring/__init__.py
+-rw-r--r--  2.0 unx     4405 b- defN 24-Mar-20 16:47 mlrun/common/model_monitoring/helpers.py
+-rw-r--r--  2.0 unx     4935 b- defN 24-Mar-20 16:47 mlrun/common/schemas/__init__.py
+-rw-r--r--  2.0 unx     2344 b- defN 24-Mar-20 16:47 mlrun/common/schemas/api_gateway.py
+-rw-r--r--  2.0 unx     2796 b- defN 24-Mar-20 16:47 mlrun/common/schemas/artifact.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-Mar-20 16:47 mlrun/common/schemas/auth.py
+-rw-r--r--  2.0 unx     1707 b- defN 24-Mar-20 16:47 mlrun/common/schemas/background_task.py
+-rw-r--r--  2.0 unx     2858 b- defN 24-Mar-20 16:47 mlrun/common/schemas/client_spec.py
+-rw-r--r--  2.0 unx      888 b- defN 24-Mar-20 16:47 mlrun/common/schemas/clusterization_spec.py
+-rw-r--r--  2.0 unx     1557 b- defN 24-Mar-20 16:47 mlrun/common/schemas/common.py
+-rw-r--r--  2.0 unx     6476 b- defN 24-Mar-20 16:47 mlrun/common/schemas/constants.py
+-rw-r--r--  2.0 unx      750 b- defN 24-Mar-20 16:47 mlrun/common/schemas/datastore_profile.py
+-rw-r--r--  2.0 unx     1026 b- defN 24-Mar-20 16:47 mlrun/common/schemas/events.py
+-rw-r--r--  2.0 unx     3717 b- defN 24-Mar-20 16:47 mlrun/common/schemas/feature_store.py
+-rw-r--r--  2.0 unx     2418 b- defN 24-Mar-20 16:47 mlrun/common/schemas/frontend_spec.py
+-rw-r--r--  2.0 unx     4577 b- defN 24-Mar-20 16:47 mlrun/common/schemas/function.py
+-rw-r--r--  2.0 unx      705 b- defN 24-Mar-20 16:47 mlrun/common/schemas/http.py
+-rw-r--r--  2.0 unx     4203 b- defN 24-Mar-20 16:47 mlrun/common/schemas/hub.py
+-rw-r--r--  2.0 unx     1395 b- defN 24-Mar-20 16:47 mlrun/common/schemas/k8s.py
+-rw-r--r--  2.0 unx      892 b- defN 24-Mar-20 16:47 mlrun/common/schemas/memory_reports.py
+-rw-r--r--  2.0 unx     1768 b- defN 24-Mar-20 16:47 mlrun/common/schemas/notification.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-Mar-20 16:47 mlrun/common/schemas/object.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Mar-20 16:47 mlrun/common/schemas/pipeline.py
+-rw-r--r--  2.0 unx     4277 b- defN 24-Mar-20 16:47 mlrun/common/schemas/project.py
+-rw-r--r--  2.0 unx      776 b- defN 24-Mar-20 16:47 mlrun/common/schemas/regex.py
+-rw-r--r--  2.0 unx      745 b- defN 24-Mar-20 16:47 mlrun/common/schemas/runs.py
+-rw-r--r--  2.0 unx     1554 b- defN 24-Mar-20 16:47 mlrun/common/schemas/runtime_resource.py
+-rw-r--r--  2.0 unx     4287 b- defN 24-Mar-20 16:47 mlrun/common/schemas/schedule.py
+-rw-r--r--  2.0 unx     1484 b- defN 24-Mar-20 16:47 mlrun/common/schemas/secret.py
+-rw-r--r--  2.0 unx      884 b- defN 24-Mar-20 16:47 mlrun/common/schemas/tag.py
+-rw-r--r--  2.0 unx     1823 b- defN 24-Mar-20 16:47 mlrun/common/schemas/workflow.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Mar-20 16:47 mlrun/common/schemas/model_monitoring/__init__.py
+-rw-r--r--  2.0 unx     7822 b- defN 24-Mar-20 16:47 mlrun/common/schemas/model_monitoring/constants.py
+-rw-r--r--  2.0 unx     1431 b- defN 24-Mar-20 16:47 mlrun/common/schemas/model_monitoring/grafana.py
+-rw-r--r--  2.0 unx    12000 b- defN 24-Mar-20 16:47 mlrun/common/schemas/model_monitoring/model_endpoints.py
+-rw-r--r--  2.0 unx     1087 b- defN 24-Mar-20 16:47 mlrun/data_types/__init__.py
+-rw-r--r--  2.0 unx     4647 b- defN 24-Mar-20 16:47 mlrun/data_types/data_types.py
+-rw-r--r--  2.0 unx     6134 b- defN 24-Mar-20 16:47 mlrun/data_types/infer.py
+-rw-r--r--  2.0 unx     9457 b- defN 24-Mar-20 16:47 mlrun/data_types/spark.py
+-rw-r--r--  2.0 unx     9945 b- defN 24-Mar-20 16:47 mlrun/data_types/to_pandas.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Mar-20 16:47 mlrun/datastore/__init__.py
+-rw-r--r--  2.0 unx     9168 b- defN 24-Mar-20 16:47 mlrun/datastore/azure_blob.py
+-rw-r--r--  2.0 unx    24175 b- defN 24-Mar-20 16:47 mlrun/datastore/base.py
+-rw-r--r--  2.0 unx     9018 b- defN 24-Mar-20 16:47 mlrun/datastore/datastore.py
+-rw-r--r--  2.0 unx    15985 b- defN 24-Mar-20 16:47 mlrun/datastore/datastore_profile.py
+-rw-r--r--  2.0 unx     6634 b- defN 24-Mar-20 16:47 mlrun/datastore/dbfs_store.py
+-rw-r--r--  2.0 unx     3767 b- defN 24-Mar-20 16:47 mlrun/datastore/filestore.py
+-rw-r--r--  2.0 unx     6112 b- defN 24-Mar-20 16:47 mlrun/datastore/google_cloud_storage.py
+-rw-r--r--  2.0 unx     1674 b- defN 24-Mar-20 16:47 mlrun/datastore/hdfs.py
+-rw-r--r--  2.0 unx      622 b- defN 24-Mar-20 16:47 mlrun/datastore/helpers.py
+-rw-r--r--  2.0 unx     2779 b- defN 24-Mar-20 16:47 mlrun/datastore/inmem.py
+-rw-r--r--  2.0 unx     5575 b- defN 24-Mar-20 16:47 mlrun/datastore/redis.py
+-rw-r--r--  2.0 unx     8110 b- defN 24-Mar-20 16:47 mlrun/datastore/s3.py
+-rw-r--r--  2.0 unx    40160 b- defN 24-Mar-20 16:47 mlrun/datastore/sources.py
+-rw-r--r--  2.0 unx     1498 b- defN 24-Mar-20 16:47 mlrun/datastore/spark_udf.py
+-rw-r--r--  2.0 unx     1611 b- defN 24-Mar-20 16:47 mlrun/datastore/spark_utils.py
+-rw-r--r--  2.0 unx     6839 b- defN 24-Mar-20 16:47 mlrun/datastore/store_resources.py
+-rw-r--r--  2.0 unx    70714 b- defN 24-Mar-20 16:47 mlrun/datastore/targets.py
+-rw-r--r--  2.0 unx     5227 b- defN 24-Mar-20 16:47 mlrun/datastore/utils.py
+-rw-r--r--  2.0 unx     9252 b- defN 24-Mar-20 16:47 mlrun/datastore/v3io.py
+-rw-r--r--  2.0 unx     1343 b- defN 24-Mar-20 16:47 mlrun/datastore/wasbfs/__init__.py
+-rw-r--r--  2.0 unx     6151 b- defN 24-Mar-20 16:47 mlrun/datastore/wasbfs/fs.py
+-rw-r--r--  2.0 unx     1163 b- defN 24-Mar-20 16:47 mlrun/db/__init__.py
+-rw-r--r--  2.0 unx    18906 b- defN 24-Mar-20 16:47 mlrun/db/base.py
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-20 16:47 mlrun/db/factory.py
+-rw-r--r--  2.0 unx   158600 b- defN 24-Mar-20 16:47 mlrun/db/httpdb.py
+-rw-r--r--  2.0 unx    14814 b- defN 24-Mar-20 16:47 mlrun/db/nopdb.py
+-rw-r--r--  2.0 unx     1584 b- defN 24-Mar-20 16:47 mlrun/feature_store/__init__.py
+-rw-r--r--  2.0 unx    49480 b- defN 24-Mar-20 16:47 mlrun/feature_store/api.py
+-rw-r--r--  2.0 unx    12853 b- defN 24-Mar-20 16:47 mlrun/feature_store/common.py
+-rw-r--r--  2.0 unx    55295 b- defN 24-Mar-20 16:47 mlrun/feature_store/feature_set.py
+-rw-r--r--  2.0 unx    43560 b- defN 24-Mar-20 16:47 mlrun/feature_store/feature_vector.py
+-rw-r--r--  2.0 unx    11210 b- defN 24-Mar-20 16:47 mlrun/feature_store/ingestion.py
+-rw-r--r--  2.0 unx    28882 b- defN 24-Mar-20 16:47 mlrun/feature_store/steps.py
+-rw-r--r--  2.0 unx     1282 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/__init__.py
+-rw-r--r--  2.0 unx    30004 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/base.py
+-rw-r--r--  2.0 unx    11654 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/conversion.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/dask_merger.py
+-rw-r--r--  2.0 unx     8261 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/job.py
+-rw-r--r--  2.0 unx     4429 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/local_merger.py
+-rw-r--r--  2.0 unx    11165 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/spark_merger.py
+-rw-r--r--  2.0 unx     6314 b- defN 24-Mar-20 16:47 mlrun/feature_store/retrieval/storey_merger.py
+-rw-r--r--  2.0 unx      743 b- defN 24-Mar-20 16:47 mlrun/frameworks/__init__.py
+-rw-r--r--  2.0 unx    11487 b- defN 24-Mar-20 16:47 mlrun/frameworks/parallel_coordinates.py
+-rw-r--r--  2.0 unx      962 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/__init__.py
+-rw-r--r--  2.0 unx     8497 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/artifacts_library.py
+-rw-r--r--  2.0 unx    20999 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/mlrun_interface.py
+-rw-r--r--  2.0 unx    55312 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/model_handler.py
+-rw-r--r--  2.0 unx     3445 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/plan.py
+-rw-r--r--  2.0 unx     5727 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/producer.py
+-rw-r--r--  2.0 unx     9131 b- defN 24-Mar-20 16:47 mlrun/frameworks/_common/utils.py
+-rw-r--r--  2.0 unx      750 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/__init__.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/model_handler.py
+-rw-r--r--  2.0 unx      996 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/utils.py
+-rw-r--r--  2.0 unx      787 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/loggers/__init__.py
+-rw-r--r--  2.0 unx    11477 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/loggers/logger.py
+-rw-r--r--  2.0 unx    14748 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/loggers/mlrun_logger.py
+-rw-r--r--  2.0 unx    27936 b- defN 24-Mar-20 16:47 mlrun/frameworks/_dl_common/loggers/tensorboard_logger.py
+-rw-r--r--  2.0 unx      956 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/__init__.py
+-rw-r--r--  2.0 unx     3145 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/artifacts_library.py
+-rw-r--r--  2.0 unx    16885 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/model_handler.py
+-rw-r--r--  2.0 unx     2717 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/pkl_model_server.py
+-rw-r--r--  2.0 unx     4869 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plan.py
+-rw-r--r--  2.0 unx     4061 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/producer.py
+-rw-r--r--  2.0 unx    10477 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/utils.py
+-rw-r--r--  2.0 unx      737 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/loggers/__init__.py
+-rw-r--r--  2.0 unx     5630 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/loggers/logger.py
+-rw-r--r--  2.0 unx     6406 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/loggers/mlrun_logger.py
+-rw-r--r--  2.0 unx      922 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plans/__init__.py
+-rw-r--r--  2.0 unx     4894 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plans/calibration_curve_plan.py
+-rw-r--r--  2.0 unx     6030 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plans/confusion_matrix_plan.py
+-rw-r--r--  2.0 unx     6611 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plans/dataset_plan.py
+-rw-r--r--  2.0 unx     5285 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plans/feature_importance_plan.py
+-rw-r--r--  2.0 unx     6963 b- defN 24-Mar-20 16:47 mlrun/frameworks/_ml_common/plans/roc_curve_plan.py
+-rw-r--r--  2.0 unx      706 b- defN 24-Mar-20 16:47 mlrun/frameworks/auto_mlrun/__init__.py
+-rw-r--r--  2.0 unx    24074 b- defN 24-Mar-20 16:47 mlrun/frameworks/auto_mlrun/auto_mlrun.py
+-rw-r--r--  2.0 unx      721 b- defN 24-Mar-20 16:47 mlrun/frameworks/huggingface/__init__.py
+-rw-r--r--  2.0 unx     6043 b- defN 24-Mar-20 16:47 mlrun/frameworks/huggingface/model_server.py
+-rw-r--r--  2.0 unx    15873 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/__init__.py
+-rw-r--r--  2.0 unx    13791 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/model_handler.py
+-rw-r--r--  2.0 unx     9156 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/model_server.py
+-rw-r--r--  2.0 unx     8265 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/utils.py
+-rw-r--r--  2.0 unx      857 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/callbacks/__init__.py
+-rw-r--r--  2.0 unx     4081 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/callbacks/callback.py
+-rw-r--r--  2.0 unx     5111 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/callbacks/logging_callback.py
+-rw-r--r--  2.0 unx     4061 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/callbacks/mlrun_logging_callback.py
+-rw-r--r--  2.0 unx      842 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/mlrun_interfaces/__init__.py
+-rw-r--r--  2.0 unx     1531 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/mlrun_interfaces/booster_mlrun_interface.py
+-rw-r--r--  2.0 unx    14221 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/mlrun_interfaces/mlrun_interface.py
+-rw-r--r--  2.0 unx     1333 b- defN 24-Mar-20 16:47 mlrun/frameworks/lgbm/mlrun_interfaces/model_mlrun_interface.py
+-rw-r--r--  2.0 unx      791 b- defN 24-Mar-20 16:47 mlrun/frameworks/onnx/__init__.py
+-rw-r--r--  2.0 unx     6085 b- defN 24-Mar-20 16:47 mlrun/frameworks/onnx/dataset.py
+-rw-r--r--  2.0 unx     2399 b- defN 24-Mar-20 16:47 mlrun/frameworks/onnx/mlrun_interface.py
+-rw-r--r--  2.0 unx     6125 b- defN 24-Mar-20 16:47 mlrun/frameworks/onnx/model_handler.py
+-rw-r--r--  2.0 unx     7021 b- defN 24-Mar-20 16:47 mlrun/frameworks/onnx/model_server.py
+-rw-r--r--  2.0 unx    22037 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/__init__.py
+-rw-r--r--  2.0 unx    27885 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/callbacks_handler.py
+-rw-r--r--  2.0 unx    44621 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/mlrun_interface.py
+-rw-r--r--  2.0 unx    22290 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/model_handler.py
+-rw-r--r--  2.0 unx    10094 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/model_server.py
+-rw-r--r--  2.0 unx     4515 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/utils.py
+-rw-r--r--  2.0 unx      896 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/callbacks/__init__.py
+-rw-r--r--  2.0 unx    11500 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/callbacks/callback.py
+-rw-r--r--  2.0 unx    23126 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/callbacks/logging_callback.py
+-rw-r--r--  2.0 unx     9239 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/callbacks/mlrun_logging_callback.py
+-rw-r--r--  2.0 unx    26299 b- defN 24-Mar-20 16:47 mlrun/frameworks/pytorch/callbacks/tensorboard_logging_callback.py
+-rw-r--r--  2.0 unx    10880 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/__init__.py
+-rw-r--r--  2.0 unx     5840 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/estimator.py
+-rw-r--r--  2.0 unx     7089 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/metric.py
+-rw-r--r--  2.0 unx    12203 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/metrics_library.py
+-rw-r--r--  2.0 unx    14054 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/mlrun_interface.py
+-rw-r--r--  2.0 unx     4695 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/model_handler.py
+-rw-r--r--  2.0 unx     1209 b- defN 24-Mar-20 16:47 mlrun/frameworks/sklearn/utils.py
+-rw-r--r--  2.0 unx    10447 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/__init__.py
+-rw-r--r--  2.0 unx    16610 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/mlrun_interface.py
+-rw-r--r--  2.0 unx    28102 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/model_handler.py
+-rw-r--r--  2.0 unx     9529 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/model_server.py
+-rw-r--r--  2.0 unx     4284 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/utils.py
+-rw-r--r--  2.0 unx      844 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/callbacks/__init__.py
+-rw-r--r--  2.0 unx    21855 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/callbacks/logging_callback.py
+-rw-r--r--  2.0 unx     8701 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/callbacks/mlrun_logging_callback.py
+-rw-r--r--  2.0 unx    28419 b- defN 24-Mar-20 16:47 mlrun/frameworks/tf_keras/callbacks/tensorboard_logging_callback.py
+-rw-r--r--  2.0 unx    10276 b- defN 24-Mar-20 16:47 mlrun/frameworks/xgboost/__init__.py
+-rw-r--r--  2.0 unx      878 b- defN 24-Mar-20 16:47 mlrun/frameworks/xgboost/mlrun_interface.py
+-rw-r--r--  2.0 unx    11530 b- defN 24-Mar-20 16:47 mlrun/frameworks/xgboost/model_handler.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Mar-20 16:47 mlrun/frameworks/xgboost/utils.py
+-rw-r--r--  2.0 unx      571 b- defN 24-Mar-20 16:47 mlrun/launcher/__init__.py
+-rw-r--r--  2.0 unx    16432 b- defN 24-Mar-20 16:47 mlrun/launcher/base.py
+-rw-r--r--  2.0 unx     6048 b- defN 24-Mar-20 16:47 mlrun/launcher/client.py
+-rw-r--r--  2.0 unx     2338 b- defN 24-Mar-20 16:47 mlrun/launcher/factory.py
+-rw-r--r--  2.0 unx    10909 b- defN 24-Mar-20 16:47 mlrun/launcher/local.py
+-rw-r--r--  2.0 unx     7469 b- defN 24-Mar-20 16:47 mlrun/launcher/remote.py
+-rw-r--r--  2.0 unx      915 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/__init__.py
+-rw-r--r--  2.0 unx    36535 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/api.py
+-rw-r--r--  2.0 unx    12504 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/application.py
+-rw-r--r--  2.0 unx    38184 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/batch.py
+-rw-r--r--  2.0 unx    27925 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/controller.py
+-rw-r--r--  2.0 unx     1336 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/controller_handler.py
+-rw-r--r--  2.0 unx     4824 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/evidently_application.py
+-rw-r--r--  2.0 unx    25308 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/features_drift_table.py
+-rw-r--r--  2.0 unx     9013 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/helpers.py
+-rw-r--r--  2.0 unx     3938 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/model_endpoint.py
+-rw-r--r--  2.0 unx     7578 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/prometheus.py
+-rw-r--r--  2.0 unx    48198 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stream_processing.py
+-rw-r--r--  2.0 unx     5283 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/tracking_policy.py
+-rw-r--r--  2.0 unx     8669 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/writer.py
+-rw-r--r--  2.0 unx      569 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/applications/__init__.py
+-rw-r--r--  2.0 unx    11647 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/applications/histogram_data_drift.py
+-rw-r--r--  2.0 unx      569 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/metrics/__init__.py
+-rw-r--r--  2.0 unx     4724 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/metrics/histogram_distance.py
+-rw-r--r--  2.0 unx     4525 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/__init__.py
+-rw-r--r--  2.0 unx    22222 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/kv_model_endpoint_store.py
+-rw-r--r--  2.0 unx     5590 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/model_endpoint_store.py
+-rw-r--r--  2.0 unx    16139 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/sql_model_endpoint_store.py
+-rw-r--r--  2.0 unx     1111 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/models/__init__.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/models/base.py
+-rw-r--r--  2.0 unx     1131 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/models/mysql.py
+-rw-r--r--  2.0 unx      765 b- defN 24-Mar-20 16:47 mlrun/model_monitoring/stores/models/sqlite.py
+-rw-r--r--  2.0 unx     7082 b- defN 24-Mar-20 16:47 mlrun/package/__init__.py
+-rw-r--r--  2.0 unx    14589 b- defN 24-Mar-20 16:47 mlrun/package/context_handler.py
+-rw-r--r--  2.0 unx     1204 b- defN 24-Mar-20 16:47 mlrun/package/errors.py
+-rw-r--r--  2.0 unx    15064 b- defN 24-Mar-20 16:47 mlrun/package/packager.py
+-rw-r--r--  2.0 unx    37160 b- defN 24-Mar-20 16:47 mlrun/package/packagers_manager.py
+-rw-r--r--  2.0 unx      769 b- defN 24-Mar-20 16:47 mlrun/package/packagers/__init__.py
+-rw-r--r--  2.0 unx    26625 b- defN 24-Mar-20 16:47 mlrun/package/packagers/default_packager.py
+-rw-r--r--  2.0 unx    25602 b- defN 24-Mar-20 16:47 mlrun/package/packagers/numpy_packagers.py
+-rw-r--r--  2.0 unx    35761 b- defN 24-Mar-20 16:47 mlrun/package/packagers/pandas_packagers.py
+-rw-r--r--  2.0 unx    22322 b- defN 24-Mar-20 16:47 mlrun/package/packagers/python_standard_library_packagers.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Mar-20 16:47 mlrun/package/utils/__init__.py
+-rw-r--r--  2.0 unx     7951 b- defN 24-Mar-20 16:47 mlrun/package/utils/_archiver.py
+-rw-r--r--  2.0 unx     6373 b- defN 24-Mar-20 16:47 mlrun/package/utils/_formatter.py
+-rw-r--r--  2.0 unx    10341 b- defN 24-Mar-20 16:47 mlrun/package/utils/_pickler.py
+-rw-r--r--  2.0 unx     2357 b- defN 24-Mar-20 16:47 mlrun/package/utils/_supported_format.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-Mar-20 16:47 mlrun/package/utils/log_hint_utils.py
+-rw-r--r--  2.0 unx    14695 b- defN 24-Mar-20 16:47 mlrun/package/utils/type_hint_utils.py
+-rw-r--r--  2.0 unx     2352 b- defN 24-Mar-20 16:47 mlrun/platforms/__init__.py
+-rw-r--r--  2.0 unx    19434 b- defN 24-Mar-20 16:47 mlrun/platforms/iguazio.py
+-rw-r--r--  2.0 unx    11828 b- defN 24-Mar-20 16:47 mlrun/platforms/other.py
+-rw-r--r--  2.0 unx     1153 b- defN 24-Mar-20 16:47 mlrun/projects/__init__.py
+-rw-r--r--  2.0 unx    18538 b- defN 24-Mar-20 16:47 mlrun/projects/operations.py
+-rw-r--r--  2.0 unx    40124 b- defN 24-Mar-20 16:47 mlrun/projects/pipelines.py
+-rw-r--r--  2.0 unx   165058 b- defN 24-Mar-20 16:47 mlrun/projects/project.py
+-rw-r--r--  2.0 unx     8289 b- defN 24-Mar-20 16:47 mlrun/runtimes/__init__.py
+-rw-r--r--  2.0 unx    36572 b- defN 24-Mar-20 16:47 mlrun/runtimes/base.py
+-rw-r--r--  2.0 unx     9513 b- defN 24-Mar-20 16:47 mlrun/runtimes/constants.py
+-rw-r--r--  2.0 unx    19149 b- defN 24-Mar-20 16:47 mlrun/runtimes/daskjob.py
+-rw-r--r--  2.0 unx    10508 b- defN 24-Mar-20 16:47 mlrun/runtimes/funcdoc.py
+-rw-r--r--  2.0 unx     4918 b- defN 24-Mar-20 16:47 mlrun/runtimes/function_reference.py
+-rw-r--r--  2.0 unx     7241 b- defN 24-Mar-20 16:47 mlrun/runtimes/generators.py
+-rw-r--r--  2.0 unx    12500 b- defN 24-Mar-20 16:47 mlrun/runtimes/kubejob.py
+-rw-r--r--  2.0 unx    21783 b- defN 24-Mar-20 16:47 mlrun/runtimes/local.py
+-rw-r--r--  2.0 unx    58664 b- defN 24-Mar-20 16:47 mlrun/runtimes/pod.py
+-rw-r--r--  2.0 unx     7326 b- defN 24-Mar-20 16:47 mlrun/runtimes/remotesparkjob.py
+-rw-r--r--  2.0 unx    16004 b- defN 24-Mar-20 16:47 mlrun/runtimes/utils.py
+-rw-r--r--  2.0 unx      569 b- defN 24-Mar-20 16:47 mlrun/runtimes/databricks_job/__init__.py
+-rw-r--r--  2.0 unx     2245 b- defN 24-Mar-20 16:47 mlrun/runtimes/databricks_job/databricks_cancel_task.py
+-rw-r--r--  2.0 unx    12749 b- defN 24-Mar-20 16:47 mlrun/runtimes/databricks_job/databricks_runtime.py
+-rw-r--r--  2.0 unx     8679 b- defN 24-Mar-20 16:47 mlrun/runtimes/databricks_job/databricks_wrapper.py
+-rw-r--r--  2.0 unx     1583 b- defN 24-Mar-20 16:47 mlrun/runtimes/mpijob/__init__.py
+-rw-r--r--  2.0 unx     9161 b- defN 24-Mar-20 16:47 mlrun/runtimes/mpijob/abstract.py
+-rw-r--r--  2.0 unx     3206 b- defN 24-Mar-20 16:47 mlrun/runtimes/mpijob/v1.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Mar-20 16:47 mlrun/runtimes/mpijob/v1alpha1.py
+-rw-r--r--  2.0 unx      794 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/__init__.py
+-rw-r--r--  2.0 unx    10277 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/api_gateway.py
+-rw-r--r--  2.0 unx    48990 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/function.py
+-rw-r--r--  2.0 unx     2942 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/nuclio.py
+-rw-r--r--  2.0 unx    30363 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/serving.py
+-rw-r--r--  2.0 unx      614 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/application/__init__.py
+-rw-r--r--  2.0 unx     9678 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/application/application.py
+-rw-r--r--  2.0 unx     2920 b- defN 24-Mar-20 16:47 mlrun/runtimes/nuclio/application/reverse_proxy.go
+-rw-r--r--  2.0 unx      709 b- defN 24-Mar-20 16:47 mlrun/runtimes/sparkjob/__init__.py
+-rw-r--r--  2.0 unx    41189 b- defN 24-Mar-20 16:47 mlrun/runtimes/sparkjob/spark3job.py
+-rw-r--r--  2.0 unx     1078 b- defN 24-Mar-20 16:47 mlrun/serving/__init__.py
+-rw-r--r--  2.0 unx     6116 b- defN 24-Mar-20 16:47 mlrun/serving/merger.py
+-rw-r--r--  2.0 unx    18010 b- defN 24-Mar-20 16:47 mlrun/serving/remote.py
+-rw-r--r--  2.0 unx    54976 b- defN 24-Mar-20 16:47 mlrun/serving/routers.py
+-rw-r--r--  2.0 unx    21161 b- defN 24-Mar-20 16:47 mlrun/serving/server.py
+-rw-r--r--  2.0 unx      836 b- defN 24-Mar-20 16:47 mlrun/serving/serving_wrapper.py
+-rw-r--r--  2.0 unx    55773 b- defN 24-Mar-20 16:47 mlrun/serving/states.py
+-rw-r--r--  2.0 unx     3871 b- defN 24-Mar-20 16:47 mlrun/serving/utils.py
+-rw-r--r--  2.0 unx    11805 b- defN 24-Mar-20 16:47 mlrun/serving/v1_serving.py
+-rw-r--r--  2.0 unx    23559 b- defN 24-Mar-20 16:47 mlrun/serving/v2_serving.py
+-rw-r--r--  2.0 unx      765 b- defN 24-Mar-20 16:47 mlrun/track/__init__.py
+-rw-r--r--  2.0 unx     3541 b- defN 24-Mar-20 16:47 mlrun/track/tracker.py
+-rw-r--r--  2.0 unx     5726 b- defN 24-Mar-20 16:47 mlrun/track/tracker_manager.py
+-rw-r--r--  2.0 unx      569 b- defN 24-Mar-20 16:47 mlrun/track/trackers/__init__.py
+-rw-r--r--  2.0 unx    23258 b- defN 24-Mar-20 16:47 mlrun/track/trackers/mlflow_tracker.py
+-rw-r--r--  2.0 unx      826 b- defN 24-Mar-20 16:47 mlrun/utils/__init__.py
+-rw-r--r--  2.0 unx    11092 b- defN 24-Mar-20 16:47 mlrun/utils/async_http.py
+-rw-r--r--  2.0 unx     3450 b- defN 24-Mar-20 16:47 mlrun/utils/azure_vault.py
+-rw-r--r--  2.0 unx     7361 b- defN 24-Mar-20 16:47 mlrun/utils/clones.py
+-rw-r--r--  2.0 unx     1897 b- defN 24-Mar-20 16:47 mlrun/utils/condition_evaluator.py
+-rw-r--r--  2.0 unx     1713 b- defN 24-Mar-20 16:47 mlrun/utils/db.py
+-rw-r--r--  2.0 unx    51162 b- defN 24-Mar-20 16:47 mlrun/utils/helpers.py
+-rw-r--r--  2.0 unx     8700 b- defN 24-Mar-20 16:47 mlrun/utils/http.py
+-rw-r--r--  2.0 unx     8133 b- defN 24-Mar-20 16:47 mlrun/utils/logger.py
+-rw-r--r--  2.0 unx     4581 b- defN 24-Mar-20 16:47 mlrun/utils/regex.py
+-rw-r--r--  2.0 unx     7522 b- defN 24-Mar-20 16:47 mlrun/utils/retryer.py
+-rw-r--r--  2.0 unx      869 b- defN 24-Mar-20 16:47 mlrun/utils/singleton.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-Mar-20 16:47 mlrun/utils/v3io_clients.py
+-rw-r--r--  2.0 unx    10447 b- defN 24-Mar-20 16:47 mlrun/utils/vault.py
+-rw-r--r--  2.0 unx      990 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/__init__.py
+-rw-r--r--  2.0 unx    21679 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification_pusher.py
+-rw-r--r--  2.0 unx     2092 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/__init__.py
+-rw-r--r--  2.0 unx     2279 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/base.py
+-rw-r--r--  2.0 unx     2532 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/console.py
+-rw-r--r--  2.0 unx     5221 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/git.py
+-rw-r--r--  2.0 unx     1955 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/ipython.py
+-rw-r--r--  2.0 unx     3898 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/slack.py
+-rw-r--r--  2.0 unx     2390 b- defN 24-Mar-20 16:47 mlrun/utils/notifications/notification/webhook.py
+-rw-r--r--  2.0 unx      614 b- defN 24-Mar-20 16:47 mlrun/utils/version/__init__.py
+-rw-r--r--  2.0 unx       88 b- defN 24-Mar-20 16:48 mlrun/utils/version/version.json
+-rw-r--r--  2.0 unx     1878 b- defN 24-Mar-20 16:47 mlrun/utils/version/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Mar-20 16:48 mlrun-1.7.0rc6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18263 b- defN 24-Mar-20 16:48 mlrun-1.7.0rc6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-20 16:48 mlrun-1.7.0rc6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-Mar-20 16:48 mlrun-1.7.0rc6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Mar-20 16:48 mlrun-1.7.0rc6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    29941 b- defN 24-Mar-20 16:48 mlrun-1.7.0rc6.dist-info/RECORD
+326 files, 3847466 bytes uncompressed, 1003451 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -816,14 +816,23 @@
 
 Filename: mlrun/runtimes/nuclio/nuclio.py
 Comment: 
 
 Filename: mlrun/runtimes/nuclio/serving.py
 Comment: 
 
+Filename: mlrun/runtimes/nuclio/application/__init__.py
+Comment: 
+
+Filename: mlrun/runtimes/nuclio/application/application.py
+Comment: 
+
+Filename: mlrun/runtimes/nuclio/application/reverse_proxy.go
+Comment: 
+
 Filename: mlrun/runtimes/sparkjob/__init__.py
 Comment: 
 
 Filename: mlrun/runtimes/sparkjob/spark3job.py
 Comment: 
 
 Filename: mlrun/serving/__init__.py
@@ -945,26 +954,26 @@
 
 Filename: mlrun/utils/version/version.json
 Comment: 
 
 Filename: mlrun/utils/version/version.py
 Comment: 
 
-Filename: mlrun-1.7.0rc5.dist-info/LICENSE
+Filename: mlrun-1.7.0rc6.dist-info/LICENSE
 Comment: 
 
-Filename: mlrun-1.7.0rc5.dist-info/METADATA
+Filename: mlrun-1.7.0rc6.dist-info/METADATA
 Comment: 
 
-Filename: mlrun-1.7.0rc5.dist-info/WHEEL
+Filename: mlrun-1.7.0rc6.dist-info/WHEEL
 Comment: 
 
-Filename: mlrun-1.7.0rc5.dist-info/entry_points.txt
+Filename: mlrun-1.7.0rc6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlrun-1.7.0rc5.dist-info/top_level.txt
+Filename: mlrun-1.7.0rc6.dist-info/top_level.txt
 Comment: 
 
-Filename: mlrun-1.7.0rc5.dist-info/RECORD
+Filename: mlrun-1.7.0rc6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlrun/config.py

```diff
@@ -320,15 +320,21 @@
             "connections_pool_max_overflow": None,
             # below is a db-specific configuration
             "mysql": {
                 # comma separated mysql modes (globally) to set on runtime
                 # optional values (as per https://dev.mysql.com/doc/refman/8.0/en/sql-mode.html#sql-mode-full):
                 #
                 # if set to "nil" or "none", nothing would be set
-                "modes": "STRICT_TRANS_TABLES",
+                "modes": (
+                    "STRICT_TRANS_TABLES"
+                    ",NO_ZERO_IN_DATE"
+                    ",NO_ZERO_DATE"
+                    ",ERROR_FOR_DIVISION_BY_ZERO"
+                    ",NO_ENGINE_SUBSTITUTION",
+                )
             },
         },
         "jobs": {
             # whether to allow to run local runtimes in the API - configurable to allow the scheduler testing to work
             "allow_local_run": False,
         },
         "authentication": {
@@ -439,15 +445,15 @@
             # whether to allow the docker registry we're pushing to, to be insecure. "enabled", "disabled" or "auto"
             # which will resolve by the existence of secret
             "insecure_push_registry_mode": "auto",
             # the requirement specifier used by the builder when installing mlrun in images when it runs
             # pip install <requirement_specifier>, e.g. mlrun==0.5.4, mlrun~=0.5,
             # git+https://github.com/mlrun/mlrun@development. by default uses the version
             "mlrun_version_specifier": "",
-            "kaniko_image": "gcr.io/kaniko-project/executor:v1.8.0",  # kaniko builder image
+            "kaniko_image": "gcr.io/kaniko-project/executor:v1.21.1",  # kaniko builder image
             "kaniko_init_container_image": "alpine:3.18",
             # image for kaniko init container when docker registry is ECR
             "kaniko_aws_cli_image": "amazon/aws-cli:2.7.10",
             # kaniko sometimes fails to get filesystem from image, this is a workaround to retry the process
             # a known issue in Kaniko - https://github.com/GoogleContainerTools/kaniko/issues/1717
             "kaniko_image_fs_extraction_retries": "3",
             # kaniko sometimes fails to push image to registry due to network issues
```

## mlrun/run.py

```diff
@@ -30,15 +30,14 @@
 import yaml
 from kfp import Client
 
 import mlrun.common.schemas
 import mlrun.errors
 import mlrun.utils.helpers
 from mlrun.kfpops import format_summary_from_kfp_run, show_kfp_run
-from mlrun.runtimes.nuclio.serving import serving_subkind
 
 from .common.helpers import parse_versioned_object_uri
 from .config import config as mlconf
 from .datastore import store_manager
 from .errors import MLRunInvalidArgumentError, MLRunTimeoutError
 from .execution import MLClientCtx
 from .model import RunObject, RunTemplate
@@ -54,14 +53,15 @@
     RuntimeKinds,
     ServingRuntime,
     Spark3Runtime,
     get_runtime_class,
 )
 from .runtimes.databricks_job.databricks_runtime import DatabricksRuntime
 from .runtimes.funcdoc import update_function_entry_points
+from .runtimes.nuclio.application import ApplicationRuntime
 from .runtimes.utils import add_code_metadata, global_context
 from .utils import (
     extend_hub_uri_if_needed,
     get_in,
     logger,
     retry_until_successful,
     run_keys,
@@ -421,27 +421,27 @@
         else:
             raise ValueError("command or code not specified in function spec")
 
     return runtime
 
 
 def new_function(
-    name: str = "",
-    project: str = "",
-    tag: str = "",
-    kind: str = "",
-    command: str = "",
-    image: str = "",
-    args: list = None,
-    runtime=None,
-    mode=None,
-    handler: str = None,
-    source: str = None,
+    name: Optional[str] = "",
+    project: Optional[str] = "",
+    tag: Optional[str] = "",
+    kind: Optional[str] = "",
+    command: Optional[str] = "",
+    image: Optional[str] = "",
+    args: Optional[list] = None,
+    runtime: Optional[Union[mlrun.runtimes.BaseRuntime, dict]] = None,
+    mode: Optional[str] = None,
+    handler: Optional[str] = None,
+    source: Optional[str] = None,
     requirements: Union[str, list[str]] = None,
-    kfp=None,
+    kfp: Optional[bool] = None,
     requirements_file: str = "",
 ):
     """Create a new ML function from base properties
 
     Example::
 
            # define a container based function (the `training.py` must exist in the container workdir)
@@ -531,17 +531,17 @@
         runner.spec.args = args
     runner.kfp = kfp
     if mode:
         runner.spec.mode = mode
     if source:
         runner.spec.build.source = source
     if handler:
-        if kind == RuntimeKinds.serving:
+        if kind in [RuntimeKinds.serving, RuntimeKinds.application]:
             raise MLRunInvalidArgumentError(
-                "cannot set the handler for serving runtime"
+                f"Handler is not supported for {kind} runtime"
             )
         elif kind in RuntimeKinds.nuclio_runtimes():
             runner.spec.function_handler = handler
         else:
             runner.spec.default_handler = handler
 
     if requirements or requirements_file:
@@ -571,41 +571,42 @@
             update_in(runtime, "spec.command", command)
     else:
         update_in(runtime, "spec.function_kind", "mlrun")
     return kind, runtime
 
 
 def code_to_function(
-    name: str = "",
-    project: str = "",
-    tag: str = "",
-    filename: str = "",
-    handler: str = "",
-    kind: str = "",
-    image: str = None,
-    code_output: str = "",
+    name: Optional[str] = "",
+    project: Optional[str] = "",
+    tag: Optional[str] = "",
+    filename: Optional[str] = "",
+    handler: Optional[str] = "",
+    kind: Optional[str] = "",
+    image: Optional[str] = None,
+    code_output: Optional[str] = "",
     embed_code: bool = True,
-    description: str = "",
-    requirements: Union[str, list[str]] = None,
-    categories: list[str] = None,
-    labels: dict[str, str] = None,
-    with_doc: bool = True,
-    ignored_tags=None,
-    requirements_file: str = "",
+    description: Optional[str] = "",
+    requirements: Optional[Union[str, list[str]]] = None,
+    categories: Optional[list[str]] = None,
+    labels: Optional[dict[str, str]] = None,
+    with_doc: Optional[bool] = True,
+    ignored_tags: Optional[str] = None,
+    requirements_file: Optional[str] = "",
 ) -> Union[
     MpiRuntimeV1Alpha1,
     MpiRuntimeV1,
     RemoteRuntime,
     ServingRuntime,
     DaskCluster,
     KubejobRuntime,
     LocalRuntime,
     Spark3Runtime,
     RemoteSparkRuntime,
     DatabricksRuntime,
+    ApplicationRuntime,
 ]:
     """Convenience function to insert code and configure an mlrun runtime.
 
     Easiest way to construct a runtime type object. Provides the most often
     used configuration options for all runtimes as parameters.
 
     Instantiated runtimes are considered 'functions' in mlrun, but they are
@@ -714,134 +715,129 @@
 
         fn.spec.description = description
         fn.metadata.project = project or mlconf.default_project
         fn.metadata.tag = tag
         fn.metadata.categories = categories
         fn.metadata.labels = labels or fn.metadata.labels
 
-    def resolve_nuclio_subkind(kind):
-        is_nuclio = kind.startswith("nuclio")
-        subkind = kind[kind.find(":") + 1 :] if is_nuclio and ":" in kind else None
-        if kind == RuntimeKinds.serving:
-            is_nuclio = True
-            subkind = serving_subkind
-        return is_nuclio, subkind
-
     if (
         not embed_code
         and not code_output
         and (not filename or filename.endswith(".ipynb"))
     ):
         raise ValueError(
-            "a valid code file must be specified "
+            "A valid code file must be specified "
             "when not using the embed_code option"
         )
 
     if kind == RuntimeKinds.databricks and not embed_code:
-        raise ValueError("databricks tasks only support embed_code=True")
+        raise ValueError("Databricks tasks only support embed_code=True")
 
-    is_nuclio, subkind = resolve_nuclio_subkind(kind)
+    if kind == RuntimeKinds.application:
+        if handler:
+            raise MLRunInvalidArgumentError(
+                "Handler is not supported for application runtime"
+            )
+        filename, handler = ApplicationRuntime.get_filename_and_handler()
+
+    is_nuclio, sub_kind = RuntimeKinds.resolve_nuclio_sub_kind(kind)
     code_origin = add_name(add_code_metadata(filename), name)
 
     name, spec, code = nuclio.build_file(
         filename,
         name=name,
         handler=handler or "handler",
-        kind=subkind,
+        kind=sub_kind,
         ignored_tags=ignored_tags,
     )
     spec["spec"]["env"].append(
         {
             "name": "MLRUN_HTTPDB__NUCLIO__EXPLICIT_ACK",
             "value": mlrun.mlconf.httpdb.nuclio.explicit_ack,
         }
     )
     spec_kind = get_in(spec, "kind", "")
     if not kind and spec_kind not in ["", "Function"]:
         kind = spec_kind.lower()
 
-        # if its a nuclio subkind, redo nb parsing
-        is_nuclio, subkind = resolve_nuclio_subkind(kind)
+        # if its a nuclio sub kind, redo nb parsing
+        is_nuclio, sub_kind = RuntimeKinds.resolve_nuclio_sub_kind(kind)
         if is_nuclio:
             name, spec, code = nuclio.build_file(
                 filename,
                 name=name,
                 handler=handler or "handler",
-                kind=subkind,
+                kind=sub_kind,
                 ignored_tags=ignored_tags,
             )
 
     if code_output:
         if code_output == ".":
             code_output = name + ".py"
         if filename == "" or filename.endswith(".ipynb"):
             with open(code_output, "w") as fp:
                 fp.write(code)
         else:
             raise ValueError("code_output option is only used with notebooks")
 
     if is_nuclio:
-        if subkind == serving_subkind:
-            r = ServingRuntime()
-        else:
-            r = RemoteRuntime()
-            r.spec.function_kind = subkind
-        # default_handler is only used in :mlrun subkind, determine the handler to invoke in function.run()
-        r.spec.default_handler = handler if subkind == "mlrun" else ""
-        r.spec.function_handler = (
+        runtime = RuntimeKinds.resolve_nuclio_runtime(kind, sub_kind)
+        # default_handler is only used in :mlrun sub kind, determine the handler to invoke in function.run()
+        runtime.spec.default_handler = handler if sub_kind == "mlrun" else ""
+        runtime.spec.function_handler = (
             handler if handler and ":" in handler else get_in(spec, "spec.handler")
         )
         if not embed_code:
-            r.spec.source = filename
+            runtime.spec.source = filename
         nuclio_runtime = get_in(spec, "spec.runtime")
         if nuclio_runtime and not nuclio_runtime.startswith("py"):
-            r.spec.nuclio_runtime = nuclio_runtime
+            runtime.spec.nuclio_runtime = nuclio_runtime
         if not name:
-            raise ValueError("name must be specified")
-        r.metadata.name = name
-        r.spec.build.code_origin = code_origin
-        r.spec.build.origin_filename = filename or (name + ".ipynb")
-        update_common(r, spec)
-        return r
+            raise ValueError("Missing required parameter: name")
+        runtime.metadata.name = name
+        runtime.spec.build.code_origin = code_origin
+        runtime.spec.build.origin_filename = filename or (name + ".ipynb")
+        update_common(runtime, spec)
+        return runtime
 
     if kind is None or kind in ["", "Function"]:
         raise ValueError("please specify the function kind")
     elif kind in RuntimeKinds.all():
-        r = get_runtime_class(kind)()
+        runtime = get_runtime_class(kind)()
     else:
         raise ValueError(f"unsupported runtime ({kind})")
 
     name, spec, code = nuclio.build_file(filename, name=name, ignored_tags=ignored_tags)
 
     if not name:
         raise ValueError("name must be specified")
     h = get_in(spec, "spec.handler", "").split(":")
-    r.handler = h[0] if len(h) <= 1 else h[1]
-    r.metadata = get_in(spec, "spec.metadata")
-    r.metadata.name = name
-    build = r.spec.build
+    runtime.handler = h[0] if len(h) <= 1 else h[1]
+    runtime.metadata = get_in(spec, "spec.metadata")
+    runtime.metadata.name = name
+    build = runtime.spec.build
     build.code_origin = code_origin
     build.origin_filename = filename or (name + ".ipynb")
     build.extra = get_in(spec, "spec.build.extra")
     build.extra_args = get_in(spec, "spec.build.extra_args")
     build.builder_env = get_in(spec, "spec.build.builder_env")
     if not embed_code:
         if code_output:
-            r.spec.command = code_output
+            runtime.spec.command = code_output
         else:
-            r.spec.command = filename
+            runtime.spec.command = filename
 
     build.image = get_in(spec, "spec.build.image")
-    update_common(r, spec)
-    r.prepare_image_for_deploy()
+    update_common(runtime, spec)
+    runtime.prepare_image_for_deploy()
 
     if with_doc:
-        update_function_entry_points(r, code)
-    r.spec.default_handler = handler
-    return r
+        update_function_entry_points(runtime, code)
+    runtime.spec.default_handler = handler
+    return runtime
 
 
 def _run_pipeline(
     pipeline,
     arguments=None,
     project=None,
     experiment=None,
```

## mlrun/artifacts/base.py

```diff
@@ -84,17 +84,18 @@
         "viewer",
         "inline",
         "format",
         "size",
         "db_key",
         "extra_data",
         "unpackaging_instructions",
+        "producer",
     ]
 
-    _extra_fields = ["annotations", "producer", "sources", "license", "encoding"]
+    _extra_fields = ["annotations", "sources", "license", "encoding"]
     _exclude_fields_from_uid_hash = [
         # if the artifact is first created, it will not have a db_key,
         # exclude it so further updates of the artifacts will have the same hash
         "db_key",
         "extra_data",
     ]
```

## mlrun/artifacts/plots.py

```diff
@@ -8,23 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import base64
+import typing
 from io import BytesIO
 
 from deprecated import deprecated
 
 import mlrun
 
 from ..utils import dict_to_json
 from .base import Artifact, LegacyArtifact
 
+if typing.TYPE_CHECKING:
+    from plotly.graph_objs import Figure
+
 
 class PlotArtifact(Artifact):
     kind = "plot"
 
     _TEMPLATE = """
 <h3 style="text-align:center">{}</h3>
 <img title="{}" src="data:image/png;base64,{}">
@@ -203,18 +207,18 @@
     Plotly artifact is an artifact for saving Plotly generated figures. They will be stored in a html format.
     """
 
     kind = "plotly"
 
     def __init__(
         self,
-        figure=None,
-        key: str = None,
-        target_path: str = None,
-    ):
+        figure: typing.Optional["Figure"] = None,
+        key: typing.Optional[str] = None,
+        target_path: typing.Optional[str] = None,
+    ) -> None:
         """
         Initialize a Plotly artifact with the given figure.
 
         :param figure:      Plotly figure ('plotly.graph_objs.Figure' object) to save as an artifact.
         :param key:         Key for the artifact to be stored in the database.
         :param target_path: Path to save the artifact.
         """
@@ -243,15 +247,15 @@
                 f"`plotly.graph_objs.Figure` but received '{type(figure)}'"
             )
 
         # Continue initializing the plotly artifact:
         self._figure = figure
         self.spec.format = "html"
 
-    def get_body(self):
+    def get_body(self) -> str:
         """
         Get the artifact's body - the Plotly figure's html code.
 
         :return: The figure's html code.
         """
         return self._figure.to_html()
```

## mlrun/datastore/sources.py

```diff
@@ -200,19 +200,19 @@
             key_field=self.key_field or key_field,
             storage_options=data_item.store.get_storage_options(),
             parse_dates=parse_dates,
             **attributes,
         )
 
     def get_spark_options(self):
-        store, path, url = mlrun.store_manager.get_or_create_store(self.path)
+        store, path, _ = mlrun.store_manager.get_or_create_store(self.path)
         spark_options = store.get_spark_options()
         spark_options.update(
             {
-                "path": url,
+                "path": store.spark_url + path,
                 "format": "csv",
                 "header": "true",
                 "inferSchema": "true",
             }
         )
         return spark_options
 
@@ -353,15 +353,15 @@
             end_filter=self.end_time,
             start_filter=self.start_time,
             filter_column=self.time_field or time_field,
             **attributes,
         )
 
     def get_spark_options(self):
-        store, path, url = mlrun.store_manager.get_or_create_store(self.path)
+        store, path, _ = mlrun.store_manager.get_or_create_store(self.path)
         spark_options = store.get_spark_options()
         spark_options.update(
             {
                 "path": store.spark_url + path,
                 "format": "parquet",
             }
         )
@@ -790,15 +790,16 @@
     def to_step(self, key_field=None, time_field=None, context=None):
         import storey
 
         source_args = self.attributes.get("source_args", {})
         explicit_ack = (
             is_explicit_ack_supported(context) and mlrun.mlconf.is_explicit_ack()
         )
-        src_class = storey.AsyncEmitSource(
+        # TODO: Change to AsyncEmitSource once we can drop support for nuclio<1.12.10
+        src_class = storey.SyncEmitSource(
             context=context,
             key_field=self.key_field or key_field,
             full_event=True,
             explicit_ack=explicit_ack,
             **source_args,
         )
```

## mlrun/db/factory.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/launcher/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/launcher/base.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/launcher/client.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/launcher/factory.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/launcher/local.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/launcher/remote.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 MLRun Authors
+# Copyright 2023 Iguazio
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

## mlrun/model_monitoring/api.py

```diff
@@ -700,16 +700,16 @@
     virtual_drift = VirtualDrift()
     drift_results = virtual_drift.check_for_drift_per_feature(
         metrics_results_dictionary=metrics,
         possible_drift_threshold=possible_drift_threshold,
         drift_detected_threshold=drift_threshold,
     )
 
-    # Drift table plot
-    html_plot = FeaturesDriftTablePlot().produce(
+    # Drift table artifact
+    plotly_artifact = FeaturesDriftTablePlot().produce(
         sample_set_statistics=sample_set_statistics,
         inputs_statistics=inputs_statistics,
         metrics=metrics,
         drift_results=drift_results,
     )
 
     # Prepare drift result per feature dictionary
@@ -728,51 +728,45 @@
         tvd=metrics["tvd_mean"],
         hellinger=metrics["hellinger_mean"],
         threshold=drift_threshold,
     )
     # Log the different artifacts
     _log_drift_artifacts(
         context=context,
-        html_plot=html_plot,
+        plotly_artifact=plotly_artifact,
         metrics_per_feature=metrics_per_feature,
         drift_status=drift_status,
         drift_metric=drift_metric,
         artifacts_tag=artifacts_tag,
     )
 
 
 def _log_drift_artifacts(
     context: mlrun.MLClientCtx,
-    html_plot: str,
+    plotly_artifact: mlrun.artifacts.Artifact,
     metrics_per_feature: dict[str, float],
     drift_status: bool,
     drift_metric: float,
     artifacts_tag: str,
 ):
     """
     Log the following artifacts/results:
     1 - Drift table plot which includes a detailed drift analysis per feature
     2 - Drift result per feature in a JSON format
     3 - Results of the total drift analysis
 
     :param context:             MLRun context. Will log the artifacts.
-    :param html_plot:           Body of the html file of the plot.
+    :param plotly_artifact:     The plotly artifact.
     :param metrics_per_feature: Dictionary in which the key is a feature name and the value is the drift numerical
                                 result.
     :param drift_status:        Boolean value that represents the final drift analysis result.
     :param drift_metric:        The final drift numerical result.
     :param artifacts_tag:       Tag to use for all the artifacts resulted from the function.
-
     """
-    context.log_artifact(
-        mlrun.artifacts.Artifact(
-            body=html_plot.encode("utf-8"), format="html", key="drift_table_plot"
-        ),
-        tag=artifacts_tag,
-    )
+    context.log_artifact(plotly_artifact, tag=artifacts_tag)
     context.log_artifact(
         mlrun.artifacts.Artifact(
             body=json.dumps(metrics_per_feature),
             format="json",
             key="features_drift_results",
         ),
         tag=artifacts_tag,
```

## mlrun/model_monitoring/application.py

```diff
@@ -12,21 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import dataclasses
 import json
 import re
 from abc import ABC, abstractmethod
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, cast
 
 import numpy as np
 import pandas as pd
 
 import mlrun.common.helpers
-import mlrun.common.schemas.model_monitoring
+import mlrun.common.model_monitoring.helpers
 import mlrun.common.schemas.model_monitoring.constants as mm_constant
 import mlrun.utils.v3io_clients
 from mlrun.datastore import get_stream_pusher
 from mlrun.datastore.targets import ParquetTarget
 from mlrun.model_monitoring.helpers import get_stream_path
 from mlrun.serving.utils import StepToDict
 from mlrun.utils import logger
@@ -80,24 +80,24 @@
     Inherit from this class to create a custom model monitoring application.
 
     example for very simple custom application::
         # mlrun: start-code
         class MyApp(ApplicationBase):
             def do_tracking(
                 self,
-                sample_df_stats: pd.DataFrame,
-                feature_stats: pd.DataFrame,
+                sample_df_stats: mlrun.common.model_monitoring.helpers.FeatureStats,
+                feature_stats: mlrun.common.model_monitoring.helpers.FeatureStats,
                 start_infer_time: pd.Timestamp,
                 end_infer_time: pd.Timestamp,
                 schedule_time: pd.Timestamp,
                 latest_request: pd.Timestamp,
                 endpoint_id: str,
                 output_stream_uri: str,
             ) -> ModelMonitoringApplicationResult:
-                self.context.log_artifact(TableArtifact("sample_df_stats", df=sample_df_stats))
+                self.context.log_artifact(TableArtifact("sample_df_stats", df=self.dict_to_histogram(sample_df_stats)))
                 return ModelMonitoringApplicationResult(
                     name="data_drift_test",
                     value=0.5,
                     kind=mm_constant.ResultKindApp.data_drift,
                     status=mm_constant.ResultStatusApp.detected,
                 )
 
@@ -122,37 +122,39 @@
         ):
             self._lazy_init(app_name=resolved_event[0])
         results = self.do_tracking(*resolved_event)
         results = results if isinstance(results, list) else [results]
         return results, event
 
     def _lazy_init(self, app_name: str):
-        self.context = self._create_context_for_logging(app_name=app_name)
+        self.context = cast(
+            mlrun.MLClientCtx, self._create_context_for_logging(app_name=app_name)
+        )
 
     @abstractmethod
     def do_tracking(
         self,
         application_name: str,
-        sample_df_stats: pd.DataFrame,
-        feature_stats: pd.DataFrame,
+        sample_df_stats: mlrun.common.model_monitoring.helpers.FeatureStats,
+        feature_stats: mlrun.common.model_monitoring.helpers.FeatureStats,
         sample_df: pd.DataFrame,
         start_infer_time: pd.Timestamp,
         end_infer_time: pd.Timestamp,
         latest_request: pd.Timestamp,
         endpoint_id: str,
         output_stream_uri: str,
     ) -> Union[
         ModelMonitoringApplicationResult, list[ModelMonitoringApplicationResult]
     ]:
         """
         Implement this method with your custom monitoring logic.
 
         :param application_name:         (str) the app name
-        :param sample_df_stats:         (pd.DataFrame) The new sample distribution DataFrame.
-        :param feature_stats:           (pd.DataFrame) The train sample distribution DataFrame.
+        :param sample_df_stats:         (FeatureStats) The new sample distribution dictionary.
+        :param feature_stats:           (FeatureStats) The train sample distribution dictionary.
         :param sample_df:               (pd.DataFrame) The new sample DataFrame.
         :param start_infer_time:        (pd.Timestamp) Start time of the monitoring schedule.
         :param end_infer_time:          (pd.Timestamp) End time of the monitoring schedule.
         :param latest_request:          (pd.Timestamp) Timestamp of the latest request on this endpoint_id.
         :param endpoint_id:             (str) ID of the monitored model endpoint
         :param output_stream_uri:       (str) URI of the output stream for results
 
@@ -163,16 +165,16 @@
 
     @classmethod
     def _resolve_event(
         cls,
         event: dict[str, Any],
     ) -> tuple[
         str,
-        pd.DataFrame,
-        pd.DataFrame,
+        mlrun.common.model_monitoring.helpers.FeatureStats,
+        mlrun.common.model_monitoring.helpers.FeatureStats,
         pd.DataFrame,
         pd.Timestamp,
         pd.Timestamp,
         pd.Timestamp,
         str,
         str,
     ]:
@@ -180,33 +182,29 @@
         Converting the event into a single tuple that will be used for passing the event arguments to the running
         application
 
         :param event: dictionary with all the incoming data
 
         :return: A tuple of:
                      [0] = (str) application name
-                     [1] = (pd.DataFrame) current input statistics
-                     [2] = (pd.DataFrame) train statistics
+                     [1] = (dict) current input statistics
+                     [2] = (dict) train statistics
                      [3] = (pd.DataFrame) current input data
                      [4] = (pd.Timestamp) start time of the monitoring schedule
                      [5] = (pd.Timestamp) end time of the monitoring schedule
                      [6] = (pd.Timestamp) timestamp of the latest request
                      [7] = (str) endpoint id
                      [8] = (str) output stream uri
         """
         start_time = pd.Timestamp(event[mm_constant.ApplicationEvent.START_INFER_TIME])
         end_time = pd.Timestamp(event[mm_constant.ApplicationEvent.END_INFER_TIME])
         return (
             event[mm_constant.ApplicationEvent.APPLICATION_NAME],
-            cls._dict_to_histogram(
-                json.loads(event[mm_constant.ApplicationEvent.CURRENT_STATS])
-            ),
-            cls._dict_to_histogram(
-                json.loads(event[mm_constant.ApplicationEvent.FEATURE_STATS])
-            ),
+            json.loads(event[mm_constant.ApplicationEvent.CURRENT_STATS]),
+            json.loads(event[mm_constant.ApplicationEvent.FEATURE_STATS]),
             ParquetTarget(
                 path=event[mm_constant.ApplicationEvent.SAMPLE_PARQUET_PATH]
             ).as_df(start_time=start_time, end_time=end_time, time_column="timestamp"),
             start_time,
             end_time,
             pd.Timestamp(event[mm_constant.ApplicationEvent.LAST_REQUEST]),
             event[mm_constant.ApplicationEvent.ENDPOINT_ID],
@@ -219,15 +217,17 @@
             f"{app_name}-logger",
             upload_artifacts=True,
             labels={"workflow": "model-monitoring-app-logger"},
         )
         return context
 
     @staticmethod
-    def _dict_to_histogram(histogram_dict: dict[str, dict[str, Any]]) -> pd.DataFrame:
+    def dict_to_histogram(
+        histogram_dict: mlrun.common.model_monitoring.helpers.FeatureStats,
+    ) -> pd.DataFrame:
         """
         Convert histogram dictionary to pandas DataFrame with feature histograms as columns
 
         :param histogram_dict: Histogram dictionary
 
         :returns: Histogram dataframe
         """
```

## mlrun/model_monitoring/batch.py

```diff
@@ -29,14 +29,15 @@
 
 import mlrun.common.helpers
 import mlrun.common.model_monitoring.helpers
 import mlrun.common.schemas.model_monitoring
 import mlrun.data_types.infer
 import mlrun.feature_store as fstore
 import mlrun.utils.v3io_clients
+from mlrun.model_monitoring.helpers import calculate_inputs_statistics
 from mlrun.model_monitoring.metrics.histogram_distance import (
     HellingerDistance,
     HistogramDistanceMetric,
     KullbackLeiblerDivergence,
     TotalVarianceDistance,
 )
 from mlrun.utils import logger
@@ -349,56 +350,14 @@
             drift_status = (
                 mlrun.common.schemas.model_monitoring.DriftStatus.POSSIBLE_DRIFT
             )
 
         return drift_status
 
 
-def calculate_inputs_statistics(
-    sample_set_statistics: dict, inputs: pd.DataFrame
-) -> dict:
-    """
-    Calculate the inputs data statistics for drift monitoring purpose.
-
-    :param sample_set_statistics: The sample set (stored end point's dataset to reference) statistics. The bins of the
-                                  histograms of each feature will be used to recalculate the histograms of the inputs.
-    :param inputs:                The inputs to calculate their statistics and later on - the drift with respect to the
-                                  sample set.
-
-    :returns: The calculated statistics of the inputs data.
-    """
-
-    # Use `DFDataInfer` to calculate the statistics over the inputs:
-    inputs_statistics = mlrun.data_types.infer.DFDataInfer.get_stats(
-        df=inputs,
-        options=mlrun.data_types.infer.InferOptions.Histogram,
-    )
-
-    # Recalculate the histograms over the bins that are set in the sample-set of the end point:
-    for feature in inputs_statistics.keys():
-        if feature in sample_set_statistics:
-            counts, bins = np.histogram(
-                inputs[feature].to_numpy(),
-                bins=sample_set_statistics[feature]["hist"][1],
-            )
-            inputs_statistics[feature]["hist"] = [
-                counts.tolist(),
-                bins.tolist(),
-            ]
-        elif "hist" in inputs_statistics[feature]:
-            # Comply with the other common features' histogram length
-            mlrun.common.model_monitoring.helpers.pad_hist(
-                mlrun.common.model_monitoring.helpers.Histogram(
-                    inputs_statistics[feature]["hist"]
-                )
-            )
-
-    return inputs_statistics
-
-
 class BatchProcessor:
     """
     The main object to handle the batch processing job. This object is used to get the required configurations and
     to manage the main monitoring drift detection process based on the current batch.
     Note that the BatchProcessor object requires access keys along with valid project configurations.
     """
```

## mlrun/model_monitoring/controller.py

```diff
@@ -27,18 +27,18 @@
 import mlrun.common.schemas.model_monitoring.constants as mm_constants
 import mlrun.data_types.infer
 import mlrun.feature_store as fstore
 from mlrun.common.model_monitoring.helpers import FeatureStats, pad_features_hist
 from mlrun.datastore import get_stream_pusher
 from mlrun.datastore.targets import ParquetTarget
 from mlrun.errors import err_to_str
-from mlrun.model_monitoring.batch import calculate_inputs_statistics
 from mlrun.model_monitoring.helpers import (
     _BatchDict,
     batch_dict2timedelta,
+    calculate_inputs_statistics,
     get_monitoring_parquet_path,
     get_stream_path,
 )
 from mlrun.utils import create_logger, datetime_now, logger
 from mlrun.utils.v3io_clients import get_v3io_client
 
 
@@ -441,21 +441,14 @@
         """
         endpoint_id = endpoint[mm_constants.EventFieldType.UID]
         start_times: set[datetime.datetime] = set()
         try:
             m_fs = fstore.get_feature_set(
                 endpoint[mm_constants.EventFieldType.FEATURE_SET_URI]
             )
-            labels = endpoint[mm_constants.EventFieldType.LABEL_NAMES]
-            if labels:
-                if isinstance(labels, str):
-                    labels = json.loads(labels)
-                for label in labels:
-                    if label not in list(m_fs.spec.features.keys()):
-                        m_fs.add_feature(fstore.Feature(name=label, value_type="float"))
 
             for application in applications_names:
                 batch_window = batch_window_generator.get_batch_window(
                     project=project,
                     endpoint=endpoint_id,
                     application=application,
                     first_request=endpoint[mm_constants.EventFieldType.FIRST_REQUEST],
```

## mlrun/model_monitoring/features_drift_table.py

```diff
@@ -17,17 +17,42 @@
 from typing import Callable, Union
 
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 import mlrun.common.schemas.model_monitoring
+from mlrun.artifacts import PlotlyArtifact
 
 # A type for representing a drift result, a tuple of the status and the drift mean:
-DriftResultType = tuple[mlrun.common.schemas.model_monitoring.DriftStatus, float]
+DriftResultType = tuple[
+    mlrun.common.schemas.model_monitoring.constants.ResultStatusApp, float
+]
+
+
+class _PlotlyTableArtifact(PlotlyArtifact):
+    """A custom class for plotly table artifacts"""
+
+    @staticmethod
+    def _disable_table_dragging(figure_html: str) -> str:
+        """
+        Disable the table columns dragging by adding the following
+        JavaScript code
+        """
+        start, end = figure_html.rsplit(";", 1)
+        middle = (
+            ';for (const element of document.getElementsByClassName("table")) '
+            '{element.style.pointerEvents = "none";}'
+        )
+        figure_html = start + middle + end
+        return figure_html
+
+    def get_body(self) -> str:
+        """Get the adjusted HTML representation of the figure"""
+        return self._disable_table_dragging(super().get_body())
 
 
 class FeaturesDriftTablePlot:
     """
     Class for producing a features drift table. The plot is a table with columns of all the statistics and metrics
     provided with two additional plot columns of the histograms and drift status. The rows content will be drawn
     per feature.
@@ -58,17 +83,17 @@
     # Histograms configurations:
     _SAMPLE_SET_HISTOGRAM_COLOR = "rgb(0,112,192)"  # Blue
     _INPUTS_HISTOGRAM_COLOR = "rgb(208,0,106)"  # Magenta
     _HISTOGRAM_OPACITY = 0.75
 
     # Status configurations:
     _STATUS_COLORS = {
-        mlrun.common.schemas.model_monitoring.DriftStatus.NO_DRIFT: "rgb(0,176,80)",  # Green
-        mlrun.common.schemas.model_monitoring.DriftStatus.POSSIBLE_DRIFT: "rgb(255,192,0)",  # Orange
-        mlrun.common.schemas.model_monitoring.DriftStatus.DRIFT_DETECTED: "rgb(208,0,106)",  # Magenta
+        mlrun.common.schemas.model_monitoring.constants.ResultStatusApp.no_detection: "rgb(0,176,80)",  # Green
+        mlrun.common.schemas.model_monitoring.constants.ResultStatusApp.potential_detection: "rgb(255,192,0)",  # Orange
+        mlrun.common.schemas.model_monitoring.constants.ResultStatusApp.detected: "rgb(208,0,106)",  # Magenta
     }
 
     # Font configurations:
     _FONT_SIZE = 10
     _FONT_COLOR = "rgb(68,68,68)"  # Dark Grey
 
     # General configurations:
@@ -93,46 +118,33 @@
 
     def produce(
         self,
         sample_set_statistics: dict,
         inputs_statistics: dict,
         metrics: dict[str, Union[dict, float]],
         drift_results: dict[str, DriftResultType],
-    ) -> str:
+    ) -> _PlotlyTableArtifact:
         """
         Produce the html code of the table plot with the given information and the stored configurations in the class.
 
         :param sample_set_statistics: The sample set calculated statistics dictionary.
         :param inputs_statistics:     The inputs calculated statistics dictionary.
         :param metrics:               The drift detection metrics calculated on the sample set and inputs.
         :param drift_results:         The drift results per feature according to the rules of the monitor.
 
-        :return: The full path to the html file of the plot.
+        :return: The drift table as a plotly artifact.
         """
-        # Plot the drift table:
         figure = self._plot(
             features=list(inputs_statistics.keys()),
             sample_set_statistics=sample_set_statistics,
             inputs_statistics=inputs_statistics,
             metrics=metrics,
             drift_results=drift_results,
         )
-
-        # Get its HTML representation:
-        figure_html = figure.to_html()
-
-        # Turn off the table columns dragging by injecting the following JavaScript code:
-        start, end = figure_html.rsplit(";", 1)
-        middle = (
-            ';for (const element of document.getElementsByClassName("table")) '
-            '{element.style.pointerEvents = "none";}'
-        )
-        figure_html = start + middle + end
-
-        return figure_html
+        return _PlotlyTableArtifact(figure=figure, key="drift_table_plot")
 
     def _read_columns_names(self, statistics_dictionary: dict, drift_metrics: dict):
         """
         Read the available statistics and metrics to include them as columns in the table.
 
         :param statistics_dictionary: A statistics dictionary (one of sample_set or inputs).
         :param drift_metrics:         The metrics dictionary.
@@ -362,18 +374,18 @@
             # Rescale the counts to be in percentages (between 0.0 to 1.0):
             counts = np.array(counts) / sum(counts)
             hovertext = [""] * len(counts)
             # Convert to NumPy for vectorization:
             bins = np.array(bins)
             if bins[0] == -sys.float_info.max:
                 bins[0] = bins[1] - (bins[2] - bins[1])
-                hovertext[0] = f"(-∞, {bins[1]})"
+                hovertext[0] = f"(-inf, {bins[1]})"
             if bins[-1] == sys.float_info.max:
                 bins[-1] = bins[-2] + (bins[-2] - bins[-3])
-                hovertext[-1] = f"({bins[-2]}, ∞)"
+                hovertext[-1] = f"({bins[-2]}, inf)"
             # Center the bins (leave the first one):
             bins = 0.5 * (bins[:-1] + bins[1:])
             # Plot the histogram as a line with filled background below it:
             histogram_bar = go.Bar(
                 x=bins,
                 y=counts,
                 name=name,
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## mlrun/model_monitoring/helpers.py

```diff
@@ -11,14 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import typing
 
+import numpy as np
+import pandas as pd
+
 import mlrun
 import mlrun.common.model_monitoring.helpers
 import mlrun.common.schemas
 from mlrun.common.schemas.model_monitoring import (
     EventFieldType,
 )
 from mlrun.model_monitoring.model_endpoint import ModelEndpoint
@@ -32,18 +35,14 @@
 
 class _BatchDict(typing.TypedDict):
     minutes: int
     hours: int
     days: int
 
 
-class _MLRunNoRunsFoundError(Exception):
-    pass
-
-
 def get_stream_path(
     project: str = None,
     function_name: str = mm_constants.MonitoringFunctionNames.STREAM,
 ):
     """
     Get stream path from the project secret. If wasn't set, take it from the system configurations
 
@@ -208,7 +207,49 @@
             bumped_last_request=bumped_last_request,
         )
         db.patch_model_endpoint(
             project=project,
             endpoint_id=model_endpoint.metadata.uid,
             attributes={EventFieldType.LAST_REQUEST: bumped_last_request},
         )
+
+
+def calculate_inputs_statistics(
+    sample_set_statistics: dict, inputs: pd.DataFrame
+) -> dict:
+    """
+    Calculate the inputs data statistics for drift monitoring purpose.
+
+    :param sample_set_statistics: The sample set (stored end point's dataset to reference) statistics. The bins of the
+                                  histograms of each feature will be used to recalculate the histograms of the inputs.
+    :param inputs:                The inputs to calculate their statistics and later on - the drift with respect to the
+                                  sample set.
+
+    :returns: The calculated statistics of the inputs data.
+    """
+
+    # Use `DFDataInfer` to calculate the statistics over the inputs:
+    inputs_statistics = mlrun.data_types.infer.DFDataInfer.get_stats(
+        df=inputs,
+        options=mlrun.data_types.infer.InferOptions.Histogram,
+    )
+
+    # Recalculate the histograms over the bins that are set in the sample-set of the end point:
+    for feature in inputs_statistics.keys():
+        if feature in sample_set_statistics:
+            counts, bins = np.histogram(
+                inputs[feature].to_numpy(),
+                bins=sample_set_statistics[feature]["hist"][1],
+            )
+            inputs_statistics[feature]["hist"] = [
+                counts.tolist(),
+                bins.tolist(),
+            ]
+        elif "hist" in inputs_statistics[feature]:
+            # Comply with the other common features' histogram length
+            mlrun.common.model_monitoring.helpers.pad_hist(
+                mlrun.common.model_monitoring.helpers.Histogram(
+                    inputs_statistics[feature]["hist"]
+                )
+            )
+
+    return inputs_statistics
```

## mlrun/model_monitoring/stream_processing.py

```diff
@@ -583,14 +583,16 @@
 
     def do(self, event):
         logger.info("ProcessBeforeParquet1", event=event)
         # Remove the following keys from the event
         for key in [
             EventFieldType.FEATURES,
             EventFieldType.NAMED_FEATURES,
+            EventFieldType.PREDICTION,
+            EventFieldType.NAMED_PREDICTIONS,
         ]:
             event.pop(key, None)
 
         # Split entities dictionary to separate dictionaries within the event
         value = event.get("entities")
         if value is not None:
             event = {**value, **event}
```

## mlrun/model_monitoring/applications/histogram_data_drift.py

```diff
@@ -9,29 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
-from typing import Final, Optional, Protocol
+from typing import Final, Optional, Protocol, cast
 
 import numpy as np
-from pandas import DataFrame, Timestamp
+from pandas import DataFrame, Series, Timestamp
 
+import mlrun.artifacts
+import mlrun.common.model_monitoring.helpers
+import mlrun.model_monitoring.features_drift_table as mm_drift_table
 from mlrun.common.schemas.model_monitoring.constants import (
     MLRUN_HISTOGRAM_DATA_DRIFT_APP_NAME,
+    EventFieldType,
     ResultKindApp,
     ResultStatusApp,
 )
 from mlrun.model_monitoring.application import (
     ModelMonitoringApplicationBase,
     ModelMonitoringApplicationResult,
 )
-from mlrun.model_monitoring.batch import (
+from mlrun.model_monitoring.metrics.histogram_distance import (
     HellingerDistance,
     HistogramDistanceMetric,
     KullbackLeiblerDivergence,
     TotalVarianceDistance,
 )
 
 
@@ -111,94 +115,173 @@
         self._value_classifier = value_classifier or DataDriftClassifier()
         assert self._REQUIRED_METRICS <= set(
             self.metrics
         ), "TVD and Hellinger distance are required for the general data drift result"
 
     def _compute_metrics_per_feature(
         self, sample_df_stats: DataFrame, feature_stats: DataFrame
-    ) -> dict[type[HistogramDistanceMetric], list[float]]:
+    ) -> DataFrame:
         """Compute the metrics for the different features and labels"""
-        metrics_per_feature: dict[type[HistogramDistanceMetric], list[float]] = {
-            metric_class: [] for metric_class in self.metrics
-        }
+        metrics_per_feature = DataFrame(
+            columns=[metric_class.NAME for metric_class in self.metrics]
+        )
 
-        for (sample_feat, sample_hist), (reference_feat, reference_hist) in zip(
-            sample_df_stats.items(), feature_stats.items()
-        ):
-            assert sample_feat == reference_feat, "The features do not match"
+        for feature_name in feature_stats:
+            sample_hist = np.asarray(sample_df_stats[feature_name])
+            reference_hist = np.asarray(feature_stats[feature_name])
             self.context.logger.info(
-                "Computing metrics for feature", feature_name=sample_feat
+                "Computing metrics for feature", feature_name=feature_name
             )
-            sample_arr = np.asarray(sample_hist)
-            reference_arr = np.asarray(reference_hist)
-            for metric in self.metrics:
-                metric_name = metric.NAME
-                self.context.logger.debug(
-                    "Computing data drift metric",
-                    metric_name=metric_name,
-                    feature_name=sample_feat,
-                )
-                metrics_per_feature[metric].append(
-                    metric(distrib_t=sample_arr, distrib_u=reference_arr).compute()
-                )
+            metrics_per_feature.loc[feature_name] = {  # pyright: ignore[reportCallIssue,reportArgumentType]
+                metric.NAME: metric(
+                    distrib_t=sample_hist, distrib_u=reference_hist
+                ).compute()
+                for metric in self.metrics
+            }
         self.context.logger.info("Finished computing the metrics")
 
         return metrics_per_feature
 
     def _add_general_drift_result(
         self, results: list[ModelMonitoringApplicationResult], value: float
     ) -> None:
+        """Add the general drift result to the results list and log it"""
+        status = self._value_classifier.value_to_status(value)
         results.append(
             ModelMonitoringApplicationResult(
                 name="general_drift",
                 value=value,
                 kind=self.METRIC_KIND,
-                status=self._value_classifier.value_to_status(value),
+                status=status,
             )
         )
 
     def _get_results(
-        self, metrics_per_feature: dict[type[HistogramDistanceMetric], list[float]]
+        self, metrics_per_feature: DataFrame
     ) -> list[ModelMonitoringApplicationResult]:
         """Average the metrics over the features and add the status"""
         results: list[ModelMonitoringApplicationResult] = []
-        hellinger_tvd_values: list[float] = []
-        for metric_class, metric_values in metrics_per_feature.items():
-            self.context.logger.debug(
-                "Averaging metric over the features", metric_name=metric_class.NAME
-            )
-            value = np.mean(metric_values)
-            if metric_class == KullbackLeiblerDivergence:
+
+        self.context.logger.debug("Averaging metrics over the features")
+        metrics_mean = metrics_per_feature.mean().to_dict()
+
+        self.context.logger.debug("Creating the results")
+        for name, value in metrics_mean.items():
+            if name == KullbackLeiblerDivergence.NAME:
                 # This metric is not bounded from above [0, inf).
                 # No status is currently reported for KL divergence
                 status = ResultStatusApp.irrelevant
             else:
                 status = self._value_classifier.value_to_status(value)
-            if metric_class in self._REQUIRED_METRICS:
-                hellinger_tvd_values.append(value)
             results.append(
                 ModelMonitoringApplicationResult(
-                    name=f"{metric_class.NAME}_mean",
+                    name=f"{name}_mean",
                     value=value,
                     kind=self.METRIC_KIND,
                     status=status,
                 )
             )
 
         self._add_general_drift_result(
-            results=results, value=np.mean(hellinger_tvd_values)
+            results=results,
+            value=np.mean(
+                [
+                    metrics_mean[HellingerDistance.NAME],
+                    metrics_mean[TotalVarianceDistance.NAME],
+                ]
+            ),
         )
 
+        self.context.logger.info("Finished with the results")
         return results
 
+    @staticmethod
+    def _remove_timestamp_feature(
+        sample_set_statistics: mlrun.common.model_monitoring.helpers.FeatureStats,
+    ) -> mlrun.common.model_monitoring.helpers.FeatureStats:
+        """
+        Drop the 'timestamp' feature if it exists, as it is irrelevant
+        in the plotly artifact
+        """
+        sample_set_statistics = mlrun.common.model_monitoring.helpers.FeatureStats(
+            sample_set_statistics.copy()
+        )
+        if EventFieldType.TIMESTAMP in sample_set_statistics:
+            del sample_set_statistics[EventFieldType.TIMESTAMP]
+        return sample_set_statistics
+
+    def _log_json_artifact(self, drift_per_feature_values: Series) -> None:
+        """Log the drift values as a JSON artifact"""
+        self.context.logger.debug("Logging drift value per feature JSON artifact")
+        self.context.log_artifact(
+            mlrun.artifacts.Artifact(
+                body=drift_per_feature_values.to_json(),
+                format="json",
+                key="features_drift_results",
+            )
+        )
+        self.context.logger.debug("Logged JSON artifact successfully")
+
+    def _log_plotly_table_artifact(
+        self,
+        sample_set_statistics: mlrun.common.model_monitoring.helpers.FeatureStats,
+        inputs_statistics: mlrun.common.model_monitoring.helpers.FeatureStats,
+        metrics_per_feature: DataFrame,
+        drift_per_feature_values: Series,
+    ) -> None:
+        """Log the Plotly drift table artifact"""
+        self.context.logger.debug(
+            "Feature stats",
+            sample_set_statistics=sample_set_statistics,
+            inputs_statistics=inputs_statistics,
+        )
+
+        self.context.logger.debug("Computing drift results per feature")
+        drift_results = {
+            cast(str, key): (self._value_classifier.value_to_status(value), value)
+            for key, value in drift_per_feature_values.items()
+        }
+        self.context.logger.debug("Logging plotly artifact")
+        self.context.log_artifact(
+            mm_drift_table.FeaturesDriftTablePlot().produce(
+                sample_set_statistics=sample_set_statistics,
+                inputs_statistics=inputs_statistics,
+                metrics=metrics_per_feature.T.to_dict(),
+                drift_results=drift_results,
+            )
+        )
+        self.context.logger.debug("Logged plotly artifact successfully")
+
+    def _log_drift_artifacts(
+        self,
+        sample_set_statistics: mlrun.common.model_monitoring.helpers.FeatureStats,
+        inputs_statistics: mlrun.common.model_monitoring.helpers.FeatureStats,
+        metrics_per_feature: DataFrame,
+        log_json_artifact: bool = True,
+    ) -> None:
+        """Log JSON and Plotly drift data per feature artifacts"""
+        drift_per_feature_values = metrics_per_feature[
+            [HellingerDistance.NAME, TotalVarianceDistance.NAME]
+        ].mean(axis=1)
+
+        if log_json_artifact:
+            self._log_json_artifact(drift_per_feature_values)
+
+        self._log_plotly_table_artifact(
+            sample_set_statistics=self._remove_timestamp_feature(sample_set_statistics),
+            inputs_statistics=inputs_statistics,
+            metrics_per_feature=metrics_per_feature,
+            drift_per_feature_values=drift_per_feature_values,
+        )
+
     def do_tracking(
         self,
         application_name: str,
-        sample_df_stats: DataFrame,
-        feature_stats: DataFrame,
+        sample_df_stats: mlrun.common.model_monitoring.helpers.FeatureStats,
+        feature_stats: mlrun.common.model_monitoring.helpers.FeatureStats,
         sample_df: DataFrame,
         start_infer_time: Timestamp,
         end_infer_time: Timestamp,
         latest_request: Timestamp,
         endpoint_id: str,
         output_stream_uri: str,
     ) -> list[ModelMonitoringApplicationResult]:
@@ -206,13 +289,20 @@
         Calculate and return the data drift metrics, averaged over the features.
 
         Refer to `ModelMonitoringApplicationBase` for the meaning of the
         function arguments.
         """
         self.context.logger.debug("Starting to run the application")
         metrics_per_feature = self._compute_metrics_per_feature(
-            sample_df_stats=sample_df_stats, feature_stats=feature_stats
+            sample_df_stats=self.dict_to_histogram(sample_df_stats),
+            feature_stats=self.dict_to_histogram(feature_stats),
+        )
+        self.context.logger.debug("Saving artifacts")
+        self._log_drift_artifacts(
+            inputs_statistics=feature_stats,
+            sample_set_statistics=sample_df_stats,
+            metrics_per_feature=metrics_per_feature,
         )
         self.context.logger.debug("Computing average per metric")
         results = self._get_results(metrics_per_feature)
         self.context.logger.debug("Finished running the application", results=results)
         return results
```

## mlrun/projects/project.py

```diff
@@ -1371,22 +1371,15 @@
 
     def register_artifacts(self):
         """register the artifacts in the MLRun DB (under this project)"""
         artifact_manager = self._get_artifact_manager()
         artifact_path = mlrun.utils.helpers.template_artifact_path(
             self.spec.artifact_path or mlrun.mlconf.artifact_path, self.metadata.name
         )
-        # TODO: To correctly maintain the list of artifacts from an exported project,
-        #  we need to maintain the different trees that generated them
-        producer = ArtifactProducer(
-            "project",
-            self.metadata.name,
-            self.metadata.name,
-            tag=self._get_hexsha() or str(uuid.uuid4()),
-        )
+        project_tag = self._get_project_tag()
         for artifact_dict in self.spec.artifacts:
             if _is_imported_artifact(artifact_dict):
                 import_from = artifact_dict["import_from"]
                 if is_relative_path(import_from):
                     # source path should be relative to the project context
                     import_from = path.join(self.spec.get_code_path(), import_from)
 
@@ -1398,14 +1391,23 @@
             else:
                 artifact = dict_to_artifact(artifact_dict)
                 if is_relative_path(artifact.src_path):
                     # source path should be relative to the project context
                     artifact.src_path = path.join(
                         self.spec.get_code_path(), artifact.src_path
                     )
+                producer = self._resolve_artifact_producer(artifact, project_tag)
+                # log the artifact only if it doesn't already exist
+                if (
+                    producer.name != self.metadata.name
+                    and self._resolve_existing_artifact(
+                        artifact,
+                    )
+                ):
+                    continue
                 artifact_manager.log_artifact(
                     producer, artifact, artifact_path=artifact_path
                 )
 
     def _get_artifact_manager(self):
         if self._artifact_manager:
             return self._artifact_manager
@@ -1494,20 +1496,28 @@
         am = self._get_artifact_manager()
         artifact_path = extend_artifact_path(
             artifact_path, self.spec.artifact_path or mlrun.mlconf.artifact_path
         )
         artifact_path = mlrun.utils.helpers.template_artifact_path(
             artifact_path, self.metadata.name
         )
-        producer = ArtifactProducer(
-            "project",
-            self.metadata.name,
-            self.metadata.name,
-            tag=self._get_hexsha() or str(uuid.uuid4()),
-        )
+        producer = self._resolve_artifact_producer(item)
+        if producer.name != self.metadata.name:
+            # the artifact producer is retained, log it only if it doesn't already exist
+            if existing_artifact := self._resolve_existing_artifact(
+                item,
+                tag,
+            ):
+                artifact_key = item if isinstance(item, str) else item.key
+                logger.info(
+                    "Artifact already exists, skipping logging",
+                    key=artifact_key,
+                    tag=tag,
+                )
+                return existing_artifact
         item = am.log_artifact(
             producer,
             item,
             body,
             tag=tag,
             local_path=local_path,
             artifact_path=artifact_path,
@@ -2399,33 +2409,83 @@
             )
         elif url and url.endswith(".tar.gz"):
             clone_tgz(url, self.spec.context, self._secrets)
         elif url and url.endswith(".zip"):
             clone_zip(url, self.spec.context, self._secrets)
 
     def create_remote(self, url, name="origin", branch=None):
-        """create remote for the project git
+        """Create remote for the project git
+
+         This method creates a new remote repository associated with the project's Git repository.
+         If a remote with the specified name already exists, it will not be overwritten.
+
+         If you wish to update the URL of an existing remote, use the `set_remote` method instead.
 
         :param url:    remote git url
         :param name:   name for the remote (default is 'origin')
         :param branch: Git branch to use as source
         """
+        self.set_remote(url, name=name, branch=branch, overwrite=False)
+
+    def set_remote(self, url, name="origin", branch=None, overwrite=True):
+        """Create or update a remote for the project git repository.
+
+        This method allows you to manage remote repositories associated with the project.
+        It checks if a remote with the specified name already exists.
+
+        If a remote with the same name does not exist, it will be created.
+        If a remote with the same name already exists,
+        the behavior depends on the value of the 'overwrite' flag.
+
+        :param url: remote git url
+        :param name: name for the remote (default is 'origin')
+        :param branch: Git branch to use as source
+        :param overwrite: if True (default), updates the existing remote with the given URL if it already exists.
+                          if False, raises an error when attempting to create a remote with a name that already exists.
+        :raises MLRunConflictError: If a remote with the same name already exists and overwrite
+                                     is set to False.
+        """
         self._ensure_git_repo()
+        if self._remote_exists(name):
+            if overwrite:
+                self.spec.repo.delete_remote(name)
+            else:
+                raise mlrun.errors.MLRunConflictError(
+                    f"Remote '{name}' already exists in the project, "
+                    f"each remote in the project must have a unique name."
+                    "Use 'set_remote' with 'override=True' inorder to update the remote, or choose a different name."
+                )
         self.spec.repo.create_remote(name, url=url)
         url = url.replace("https://", "git://")
         if not branch:
             try:
                 branch = self.spec.repo.active_branch.name
             except Exception:
                 pass
         if branch:
             url = f"{url}#{branch}"
         self.spec._source = self.spec.source or url
         self.spec.origin_url = self.spec.origin_url or url
 
+    def remove_remote(self, name):
+        """Remove a remote from the project's Git repository.
+
+        This method removes the remote repository associated with the specified name from the project's Git repository.
+
+        :param name: Name of the remote to remove.
+        """
+        if self._remote_exists(name):
+            self.spec.repo.delete_remote(name)
+        else:
+            logger.warning(f"The remote '{name}' does not exist. Nothing to remove.")
+
+    def _remote_exists(self, name):
+        """Check if a remote with the given name already exists"""
+        return any(remote.name == name for remote in self.spec.repo.remotes)
+
     def _ensure_git_repo(self):
         if self.spec.repo:
             return
         context = self.context
         git_dir_path = path.join(context, ".git")
 
         if not path.exists(git_dir_path):
@@ -3329,15 +3389,20 @@
         :param tree: the producer id (tree)
         :return: Artifact object
         """
         db = mlrun.db.get_run_db(secrets=self._secrets)
         artifact = db.read_artifact(
             key, tag, iter=iter, project=self.metadata.name, tree=tree
         )
-        return dict_to_artifact(artifact)
+
+        # in tests, if an artifact is not found, the db returns None
+        # in real usage, the db should raise an exception
+        if artifact:
+            return dict_to_artifact(artifact)
+        return None
 
     def list_artifacts(
         self,
         name=None,
         tag=None,
         labels: Optional[Union[dict[str, str], list[str]]] = None,
         since=None,
@@ -3757,14 +3822,91 @@
         if not path.isfile(abs_path):
             raise mlrun.errors.MLRunInvalidArgumentError(
                 f"Invalid '{param_name}': '{file_path}'. Got a path to a non-existing file. "
                 f"Path must be absolute or relative to the project code path i.e. "
                 f"<project.spec.get_code_path()>/<{param_name}>)."
             )
 
+    def _resolve_artifact_producer(
+        self,
+        artifact: typing.Union[str, Artifact],
+        project_producer_tag: str = None,
+    ) -> typing.Optional[ArtifactProducer]:
+        """
+        Resolve the artifact producer of the given artifact.
+        If the artifact's producer is a run, the artifact is registered with the original producer.
+        Otherwise, the artifact is registered with the current project as the producer.
+
+        :param artifact:                The artifact to resolve its producer.
+        :param project_producer_tag:    The tag to use for the project as the producer. If not provided, a tag will be
+        generated for the project.
+        :return:                        A tuple of the resolved producer and the resolved artifact.
+        """
+
+        if not isinstance(artifact, str) and artifact.producer:
+            # if the artifact was imported from a yaml file, the producer can be a dict
+            if isinstance(artifact.spec.producer, ArtifactProducer):
+                producer_dict = artifact.spec.producer.get_meta()
+            else:
+                producer_dict = artifact.spec.producer
+
+            if producer_dict.get("kind", "") == "run":
+                return ArtifactProducer(
+                    name=producer_dict.get("name", ""),
+                    kind=producer_dict.get("kind", ""),
+                    project=producer_dict.get("project", ""),
+                    tag=producer_dict.get("tag", ""),
+                )
+
+        # do not retain the artifact's producer, replace it with the project as the producer
+        project_producer_tag = project_producer_tag or self._get_project_tag()
+        return ArtifactProducer(
+            kind="project",
+            name=self.metadata.name,
+            project=self.metadata.name,
+            tag=project_producer_tag,
+        )
+
+    def _resolve_existing_artifact(
+        self,
+        item: typing.Union[str, Artifact],
+        tag: str = None,
+    ) -> typing.Optional[Artifact]:
+        """
+        Check if there is and existing artifact with the given item and tag.
+        If there is, return the existing artifact. Otherwise, return None.
+
+        :param item:    The item (or key) to check if there is an existing artifact for.
+        :param tag:     The tag to check if there is an existing artifact for.
+        :return:        The existing artifact if there is one, otherwise None.
+        """
+        try:
+            if isinstance(item, str):
+                existing_artifact = self.get_artifact(key=item, tag=tag)
+            else:
+                existing_artifact = self.get_artifact(
+                    key=item.key,
+                    tag=item.tag,
+                    iter=item.iter,
+                    tree=item.tree,
+                )
+            if existing_artifact is not None:
+                return existing_artifact.from_dict(existing_artifact)
+        except mlrun.errors.MLRunNotFoundError:
+            logger.debug(
+                "No existing artifact was found",
+                key=item if isinstance(item, str) else item.key,
+                tag=tag if isinstance(item, str) else item.tag,
+                tree=None if isinstance(item, str) else item.tree,
+            )
+            return None
+
+    def _get_project_tag(self):
+        return self._get_hexsha() or str(uuid.uuid4())
+
 
 def _set_as_current_default_project(project: MlrunProject):
     mlrun.mlconf.default_project = project.metadata.name
     pipeline_context.set(project)
 
 
 def _init_function_from_dict(
@@ -3842,14 +3984,26 @@
                 filename=url,
                 image=image,
                 kind=kind or "job",
                 handler=handler,
                 tag=tag,
             )
 
+    elif image and kind in mlrun.runtimes.RuntimeKinds.nuclio_runtimes():
+        func = new_function(
+            name,
+            command=relative_url,
+            image=image,
+            kind=kind,
+            handler=handler,
+            tag=tag,
+        )
+        if kind != mlrun.runtimes.RuntimeKinds.application:
+            logger.info("Function code not specified, setting entry point to image")
+            func.from_image(image)
     else:
         raise ValueError(f"Unsupported function url:handler {url}:{handler} or no spec")
 
     if with_repo:
         # mark source to be enriched before run with project source (enrich_function_object)
         func.spec.build.source = "./"
     if requirements or requirements_file:
```

## mlrun/runtimes/__init__.py

```diff
@@ -39,14 +39,16 @@
 from .mpijob import MpiRuntimeContainer, MpiRuntimeV1, MpiRuntimeV1Alpha1  # noqa
 from .nuclio import (
     RemoteRuntime,
     ServingRuntime,
     new_v2_model_server,
     nuclio_init_hook,
 )
+from .nuclio.application import ApplicationRuntime
+from .nuclio.serving import serving_subkind
 from .remotesparkjob import RemoteSparkRuntime
 from .sparkjob import Spark3Runtime
 
 # for legacy imports (MLModelServer moved from here to /serving)
 from ..serving import MLModelServer, new_v1_model_server  # noqa isort: skip
 
 
@@ -97,28 +99,30 @@
     spark = "spark"
     remotespark = "remote-spark"
     mpijob = "mpijob"
     serving = "serving"
     local = "local"
     handler = "handler"
     databricks = "databricks"
+    application = "application"
 
     @staticmethod
     def all():
         return [
             RuntimeKinds.remote,
             RuntimeKinds.nuclio,
             RuntimeKinds.serving,
             RuntimeKinds.dask,
             RuntimeKinds.job,
             RuntimeKinds.spark,
             RuntimeKinds.remotespark,
             RuntimeKinds.mpijob,
             RuntimeKinds.local,
             RuntimeKinds.databricks,
+            RuntimeKinds.application,
         ]
 
     @staticmethod
     def runtime_with_handlers():
         return [
             RuntimeKinds.dask,
             RuntimeKinds.job,
@@ -143,14 +147,15 @@
 
     @staticmethod
     def nuclio_runtimes():
         return [
             RuntimeKinds.remote,
             RuntimeKinds.nuclio,
             RuntimeKinds.serving,
+            RuntimeKinds.application,
         ]
 
     @staticmethod
     def local_runtimes():
         return [
             RuntimeKinds.local,
             RuntimeKinds.handler,
@@ -207,14 +212,43 @@
     def requires_image_name_for_execution(kind):
         if RuntimeKinds.is_local_runtime(kind):
             return False
 
         # both spark and remote spark uses different mechanism for assigning images
         return kind not in [RuntimeKinds.spark, RuntimeKinds.remotespark]
 
+    @staticmethod
+    def resolve_nuclio_runtime(kind: str, sub_kind: str):
+        kind = kind.split(":")[0]
+        if kind not in RuntimeKinds.nuclio_runtimes():
+            raise ValueError(
+                f"Kind {kind} is not a nuclio runtime, available runtimes are {RuntimeKinds.nuclio_runtimes()}"
+            )
+
+        if sub_kind == serving_subkind:
+            return ServingRuntime()
+
+        if kind == RuntimeKinds.application:
+            return ApplicationRuntime()
+
+        runtime = RemoteRuntime()
+        runtime.spec.function_kind = sub_kind
+        return runtime
+
+    @staticmethod
+    def resolve_nuclio_sub_kind(kind):
+        is_nuclio = kind.startswith("nuclio")
+        sub_kind = kind[kind.find(":") + 1 :] if is_nuclio and ":" in kind else None
+        if kind == RuntimeKinds.serving:
+            is_nuclio = True
+            sub_kind = serving_subkind
+        elif kind == RuntimeKinds.application:
+            is_nuclio = True
+        return is_nuclio, sub_kind
+
 
 def get_runtime_class(kind: str):
     if kind == RuntimeKinds.mpijob:
         return MpiRuntimeContainer.selector()
 
     if kind == RuntimeKinds.spark:
         return Spark3Runtime
@@ -224,10 +258,11 @@
         RuntimeKinds.nuclio: RemoteRuntime,
         RuntimeKinds.serving: ServingRuntime,
         RuntimeKinds.dask: DaskCluster,
         RuntimeKinds.job: KubejobRuntime,
         RuntimeKinds.local: LocalRuntime,
         RuntimeKinds.remotespark: RemoteSparkRuntime,
         RuntimeKinds.databricks: DatabricksRuntime,
+        RuntimeKinds.application: ApplicationRuntime,
     }
 
     return kind_runtime_map[kind]
```

## mlrun/runtimes/base.py

```diff
@@ -782,15 +782,15 @@
         return self
 
     def with_requirements(
         self,
         requirements: Optional[list[str]] = None,
         overwrite: bool = False,
         prepare_image_for_deploy: bool = True,
-        requirements_file: str = "",
+        requirements_file: Optional[str] = "",
     ):
         """add package requirements from file or list to build spec.
 
         :param requirements:                a list of python packages
         :param requirements_file:           a local python requirements file path
         :param overwrite:                   overwrite existing requirements
         :param prepare_image_for_deploy:    prepare the image/base_image spec for deployment
```

## mlrun/runtimes/pod.py

```diff
@@ -981,15 +981,15 @@
     A parent class for runtimes that generate k8s resources when executing.
     """
 
     kind = "job"
     _is_nested = True
 
     def __init__(self, spec=None, metadata=None):
-        super().__init__(metadata, spec)
+        super().__init__(metadata=metadata, spec=spec)
         self.verbose = False
 
     @property
     def spec(self) -> KubeResourceSpec:
         return self._spec
 
     @spec.setter
```

## mlrun/runtimes/nuclio/function.py

```diff
@@ -287,14 +287,17 @@
     def status(self) -> NuclioStatus:
         return self._status
 
     @status.setter
     def status(self, status):
         self._status = self._verify_dict(status, "status", NuclioStatus)
 
+    def pre_deploy_validation(self):
+        pass
+
     def set_config(self, key, value):
         self.spec.config[key] = value
         return self
 
     def with_annotations(self, annotations: dict):
         """set a key/value annotations for function"""
 
@@ -599,15 +602,14 @@
 
         if save_record:
             self.save(versioned=False)
 
         return self.spec.command
 
     def _wait_for_function_deployment(self, db, verbose=False):
-        text = ""
         state = ""
         last_log_timestamp = 1
         while state not in ["ready", "error", "unhealthy"]:
             sleep(
                 int(mlrun.mlconf.httpdb.logs.nuclio.pull_deploy_status_default_interval)
             )
             try:
@@ -954,14 +956,61 @@
             raise RuntimeError(f"bad function response {resp.status_code}: {resp.text}")
 
         data = resp.content
         if resp.headers["content-type"] == "application/json":
             data = json.loads(data)
         return data
 
+    def with_sidecar(
+        self,
+        name: str = None,
+        image: str = None,
+        ports: typing.Optional[typing.Union[int, list[int]]] = None,
+        command: typing.Optional[str] = None,
+        args: typing.Optional[list[str]] = None,
+    ):
+        """
+        Add a sidecar container to the function pod
+        :param name:    Sidecar container name.
+        :param image:   Sidecar container image.
+        :param ports:   Sidecar container ports to expose. Can be a single port or a list of ports.
+        :param command: Sidecar container command instead of the image entrypoint.
+        :param args:    Sidecar container command args (requires command to be set).
+        """
+        name = name or f"{self.metadata.name}-sidecar"
+        sidecar = self._set_sidecar(name)
+        if image:
+            sidecar["image"] = image
+
+        ports = mlrun.utils.helpers.as_list(ports)
+        sidecar["ports"] = [
+            {
+                "name": "http",
+                "containerPort": port,
+                "protocol": "TCP",
+            }
+            for port in ports
+        ]
+
+        if command:
+            sidecar["command"] = command
+
+        if args:
+            sidecar["args"] = args
+
+    def _set_sidecar(self, name: str) -> dict:
+        self.spec.config.setdefault("spec.sidecars", [])
+        sidecars = self.spec.config["spec.sidecars"]
+        for sidecar in sidecars:
+            if sidecar["name"] == name:
+                return sidecar
+
+        sidecars.append({"name": name})
+        return sidecars[-1]
+
     def _trigger_of_kind_exists(self, kind: str) -> bool:
         if not self.spec.config:
             return False
 
         for name, spec in self.spec.config.items():
             if isinstance(spec, dict):
                 if spec.get("kind") == kind:
```

## mlrun/serving/states.py

```diff
@@ -1157,27 +1157,19 @@
         event.body = {"id": event.id}
         return event
 
     def run(self, event, *args, **kwargs):
         if self._controller:
             # async flow (using storey)
             event._awaitable_result = None
-            if self.context.is_mock:
-                resp = self._controller.emit(
-                    event, return_awaitable_result=self._wait_for_result
-                )
-                if self._wait_for_result and resp:
-                    return resp.await_result()
-            else:
-                resp_awaitable = self._controller.emit(
-                    event, await_result=self._wait_for_result
-                )
-                if self._wait_for_result:
-                    return resp_awaitable
-                return self._await_and_return_id(resp_awaitable, event)
+            resp = self._controller.emit(
+                event, return_awaitable_result=self._wait_for_result
+            )
+            if self._wait_for_result and resp:
+                return resp.await_result()
             event = copy(event)
             event.body = {"id": event.id}
             return event
 
         if len(self._start_steps) == 0:
             return event
         next_obj = self._start_steps[0]
@@ -1564,18 +1556,14 @@
                 # if responder step (return result), add Complete()
                 step.async_object.to(storey.Complete(full_event=True))
                 wait_for_result = True
 
     source_args = context.get_param("source_args", {})
     explicit_ack = is_explicit_ack_supported(context) and mlrun.mlconf.is_explicit_ack()
 
-    if context.is_mock:
-        source_class = storey.SyncEmitSource
-    else:
-        source_class = storey.AsyncEmitSource
-
-    default_source = source_class(
+    # TODO: Change to AsyncEmitSource once we can drop support for nuclio<1.12.10
+    default_source = storey.SyncEmitSource(
         context=context,
         explicit_ack=explicit_ack,
         **source_args,
     )
     return default_source, wait_for_result
```

## mlrun/utils/version/version.json

### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'git_commit'": "'cbfd1ee5f41bee97ff90efbce14bac0a56b58dce'", "'version'": "'1.7.0-rc6'"}*

```diff
@@ -1,4 +1,4 @@
 {
-    "git_commit": "d3324e482f4a4182ee0c8eda4af0d312718b599d",
-    "version": "1.7.0-rc5"
+    "git_commit": "cbfd1ee5f41bee97ff90efbce14bac0a56b58dce",
+    "version": "1.7.0-rc6"
 }
```

## Comparing `mlrun-1.7.0rc5.dist-info/LICENSE` & `mlrun-1.7.0rc6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlrun-1.7.0rc5.dist-info/METADATA` & `mlrun-1.7.0rc6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlrun
-Version: 1.7.0rc5
+Version: 1.7.0rc6
 Summary: Tracking and config of machine learning runs
 Home-page: https://github.com/mlrun/mlrun
 Author: Yaron Haviv
 Author-email: yaronh@iguazio.com
 License: Apache License 2.0
 Keywords: mlrun,mlops,data-science,machine-learning,experiment-tracking
 Classifier: Development Status :: 4 - Beta
```

## Comparing `mlrun-1.7.0rc5.dist-info/RECORD` & `mlrun-1.7.0rc6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 mlrun/__init__.py,sha256=o9dHUfVFADfsi6GnOPLr2OkfkHdPvOnA7rkoECen0-I,7248
 mlrun/__main__.py,sha256=vg-HMhJqQ3OYt31YmijjBh6-6AZQVe4FvDYn4MwEpYs,49229
-mlrun/config.py,sha256=mAhLKO6P0i8r_vGDCMNFV0cJv4Pb7mRmm9HR3rudwWI,62563
+mlrun/config.py,sha256=DMwxalJOY6E5_JyygKq1LFKUN2vL_sop3gssHm4LWyg,62775
 mlrun/errors.py,sha256=HmOAdfpL0bCDisZMUoJPOumneq71ko49Ph-XBL-A4xA,7080
 mlrun/execution.py,sha256=meZ_qSdTmnpqW7DKv7LdBmuE1Ut34E1RbK2kO0MD_QM,40866
 mlrun/features.py,sha256=nPDvy8tJuxwbRr843oWcnLBrqMJDPUanzn2Sb3BBi6w,15569
 mlrun/k8s_utils.py,sha256=YyFZT2WNZrJkcZoqxrkduQgzQ1X-7195O0mmEqvaIug,7023
 mlrun/kfpops.py,sha256=nVQUjLVBhXqkL2OTWJUo4qFIfNVEXUKIXJmRpBW0MVU,30481
 mlrun/lists.py,sha256=ev-gLBPc_az03yQEHrKyDPq_Bjosa4D_XFiVbRIpmRY,8286
 mlrun/model.py,sha256=e9tJG8-wP3gPywDu7wJMNsusLTGpVA9WpBbILFwR5Ns,70583
 mlrun/render.py,sha256=aMH3U2z7ELpW8MwYEGOrqLdEUwMX29shqy6V6-KbgiM,13009
-mlrun/run.py,sha256=1GZk2f3xU2OrBE4aHMzVe0RUpwc1DokWiVwdwnTszlU,42400
+mlrun/run.py,sha256=br2oHhmDvcMSwEEuEBWITTRqGXiFaaIEzNYG21RVhKc,42822
 mlrun/secrets.py,sha256=Nl_7ZNSErd-AOH19vVx_PjrLg9bJM9L-BvEYoPolB1c,7776
 mlrun/api/schemas/__init__.py,sha256=LhfO3myrnLVxC0MYCAc1_LTuqhRlYV3H7BwJkjOu3dQ,14211
 mlrun/artifacts/__init__.py,sha256=LxEWcMYPawJYvNOl6H2_UvrxdLTNYfKeZcMEKFZnGgA,1187
-mlrun/artifacts/base.py,sha256=qAM4Tjcduf3unCvYTVV3jzMTqDWgMhYft2O-fVv5kbQ,34970
+mlrun/artifacts/base.py,sha256=2UYjwp7o_Fxhr1sMYE5mSUpxGA8yt2ZU1_UicreL7hk,34978
 mlrun/artifacts/dataset.py,sha256=hKdKtyAJqPWUGs1yefOAxa10s_ar3o7MaO7oiiD_HqU,22360
 mlrun/artifacts/manager.py,sha256=p6CmIJH91vm9DsEZHgHxKYTHU2BvF9IwpLv85cqoHNs,14425
 mlrun/artifacts/model.py,sha256=DXT24CH1ZgQLz9HcWBfjRAEhCBfznoa7-pB52N9qMOI,25205
-mlrun/artifacts/plots.py,sha256=dHt7Ardo4yZWaPtlUN3b78eB8NXV8XKigPP0u0poRl0,15701
+mlrun/artifacts/plots.py,sha256=RPJxfzS_3dKAXiY2N1LchS7c9LsrJMg42OAVyDn0mK0,15860
 mlrun/common/__init__.py,sha256=xY3wHC4TEJgez7qtnn1pQvHosi8-5UJOCtyGBS7FcGE,571
 mlrun/common/constants.py,sha256=OwcN3HroG3l94Kx1B-247cp1UyqC0IVLc_TCFGWmrg4,745
 mlrun/common/helpers.py,sha256=BAhyuUnZvD_BT43i0_1EszuSbKgZx7bFy2KRIWP0XeA,1087
 mlrun/common/secrets.py,sha256=vc8WV82EZsCB5ENjUkObFOzZP59aZ1w8F82PTnqwBnc,5181
 mlrun/common/types.py,sha256=V_jCEFCJZcycFVsPzEToCRQja5bqW0zRAAVaGN_QYxQ,790
 mlrun/common/db/__init__.py,sha256=xY3wHC4TEJgez7qtnn1pQvHosi8-5UJOCtyGBS7FcGE,571
 mlrun/common/db/sql_session.py,sha256=Znc8KE2oLy4lg3_vRki1sVlNx59TgDSOTCXfU561hBU,2659
@@ -74,26 +74,26 @@
 mlrun/datastore/filestore.py,sha256=nS3Ie6jG41NDiW_as9tF8Nu5maaSVEKYKUr1IQtPhuA,3767
 mlrun/datastore/google_cloud_storage.py,sha256=ri5bTqTNLij3ujlPoKlptDPi7oN6JgqIiVGWYoEmgsE,6112
 mlrun/datastore/hdfs.py,sha256=jCuuPbnITezNYug9iYNLEJW87GGXSqW6H-UiqAynfdw,1674
 mlrun/datastore/helpers.py,sha256=-bKveE9rteLd0hJd6OSMuMbfz09W_OXyu1G5O2ihZjs,622
 mlrun/datastore/inmem.py,sha256=6PAltUk7uyYlDgnsaJPOkg_P98iku1ys2e2wpAmPRkc,2779
 mlrun/datastore/redis.py,sha256=yJ8xYHAR4DyYzsAMLQmsdzO-VVUTQABkIxcWhVHeUFI,5575
 mlrun/datastore/s3.py,sha256=EIPAXJGZ9kpQVbb_utFFZskDM21fAGz4m6QEAGecABU,8110
-mlrun/datastore/sources.py,sha256=6rK3pmpQ0Mzk1p3yEvMSqiaJOpjXGsMpXOcDYlcHaP8,40060
+mlrun/datastore/sources.py,sha256=1cQ697He_2avwLH6_6bMB2LBl1arBvSfdL-cYmH3UP8,40160
 mlrun/datastore/spark_udf.py,sha256=NnnB3DZxZb-rqpRy7b-NC7QWXuuqFn3XkBDc86tU4mQ,1498
 mlrun/datastore/spark_utils.py,sha256=50rllp6xXpXY__1LbU7aTXUU5ca8dKAfoskPre3npZo,1611
 mlrun/datastore/store_resources.py,sha256=dfMdFy2urilECtlwLJr5CSG12MA645b-NPYDnbr5s1A,6839
 mlrun/datastore/targets.py,sha256=YjjvXnaEEj0ojxiOxoRSuIrbzAvuRSpFxX-9_zJFaZ0,70714
 mlrun/datastore/utils.py,sha256=YKK9q1C0LmveQFnbh1Dkb8LwA4WbOYFTsNxziC8d0E4,5227
 mlrun/datastore/v3io.py,sha256=oCAMpST6sKnjm5CaNsTrcwqk3bvUFzuKBvNFmUJpPfw,9252
 mlrun/datastore/wasbfs/__init__.py,sha256=s5Ul-0kAhYqFjKDR2X0O2vDGDbLQQduElb32Ev56Te4,1343
 mlrun/datastore/wasbfs/fs.py,sha256=MnSj7Q4OKA2L55ihCmUnj2t3GA3B77oLMdAw-yxvN9w,6151
 mlrun/db/__init__.py,sha256=WqJ4x8lqJ7ZoKbhEyFqkYADd9P6E3citckx9e9ZLcIU,1163
 mlrun/db/base.py,sha256=d6J2g2uFvJh8CcAYoFR4DxPvKsAjByKxLqGENWDoluc,18906
-mlrun/db/factory.py,sha256=wTEKHEmdDkylM6IkTYvmEYVF8gn2HdjLoLoWICCyatI,2403
+mlrun/db/factory.py,sha256=ibIrE5QkIIyzDU1FXKrfbc31cZiRLYKDZb8dqCpQwyU,2397
 mlrun/db/httpdb.py,sha256=JtVbbetPzhpZNYb5meXMevPIRGkGu2KBbb9QTADYvLs,158600
 mlrun/db/nopdb.py,sha256=FoEFMfnh1aSs-mcXlwA8GnnbQCIoTtFkflbFpUF5bMY,14814
 mlrun/feature_store/__init__.py,sha256=n1F5m1svFW2chbE2dJdWzZJJiYS4E-y8PQsG9Q-F0lU,1584
 mlrun/feature_store/api.py,sha256=bO5I_lkIPLv8j3AXYOAseSBI8RrsGwQ9m7isepuADkw,49480
 mlrun/feature_store/common.py,sha256=DKmoRk04NCS1gv7qZuEUa2-g8WsfR6IWjYctcrqKVlg,12853
 mlrun/feature_store/feature_set.py,sha256=iIEFt85Bpc4Q0jNqNXLptVZfULpFBHT5iLSzrZVYvbY,55295
 mlrun/feature_store/feature_vector.py,sha256=2sGbHAXdkm92-R29HXeFxwScvZM4M2gk-t9RteaHc4c,43560
@@ -187,36 +187,36 @@
 mlrun/frameworks/tf_keras/callbacks/logging_callback.py,sha256=5GjK4cfq_5gmyl9L9nJSk8qTwaVH0eGkTnZinE5jjtQ,21855
 mlrun/frameworks/tf_keras/callbacks/mlrun_logging_callback.py,sha256=RuR4tuPNCAeUC_6z6MEdMc_OzejFs3lEMSxvO5k5mUo,8701
 mlrun/frameworks/tf_keras/callbacks/tensorboard_logging_callback.py,sha256=bdhMM6ZaCQObhzGry8Sg-uVJ89P7U2nr6RnIQoNDy_Q,28419
 mlrun/frameworks/xgboost/__init__.py,sha256=opkcSxdS4y-FF6EO2KHHmtEqpACk06RU2y6ilnFK-Zc,10276
 mlrun/frameworks/xgboost/mlrun_interface.py,sha256=QcP_mTKBjxvRyWcNnju0BlvXBDOqNH9B1XBoxvEojAk,878
 mlrun/frameworks/xgboost/model_handler.py,sha256=e7IwdrmAaQ5Yy_fqOirN7oi-xEJgg_Gqh83Dw1w-U34,11530
 mlrun/frameworks/xgboost/utils.py,sha256=5zLzHoeI3n2FuA_rdGzi404QCTLfQx1TYEyUWhZogs8,1069
-mlrun/launcher/__init__.py,sha256=pZgS6ZN126aJme4z5spCX-RmdchShxMnQeCPya8AsQI,577
-mlrun/launcher/base.py,sha256=EGnfzZd0HUkS92lcFJ0c6AxTqM_Chpa-WzdGMNsPZNk,16438
-mlrun/launcher/client.py,sha256=pnHqTSGl3FnwzOh7FicrGl0JOWZ3naKjay3MOkbIzLI,6054
-mlrun/launcher/factory.py,sha256=tk6foFWox7f_xaeTgkWTx9ht_5fv0XzLDR8ucdb8oTE,2344
-mlrun/launcher/local.py,sha256=s6waNbLAUC6qb0bpWWHCq2aveRGUSaEbAL7x1F1cgxQ,10915
-mlrun/launcher/remote.py,sha256=zxPaN6yElLiZ51ABSz8qfnulNXpDFuW_xN3vNy2xiDQ,7475
+mlrun/launcher/__init__.py,sha256=JL8qkT1lLr1YvW6iP0hmwDTaSR2RfrMDx0-1gWRhTOE,571
+mlrun/launcher/base.py,sha256=GHEZoxrgW1EIjYu9y6rGKLWwKBxEj6TqZd1ntSJ0CuY,16432
+mlrun/launcher/client.py,sha256=q3bmydSpO2x2Fbgy18W1uvaLbtxzJFlj1Uq6YNVndUU,6048
+mlrun/launcher/factory.py,sha256=RW7mfzEFi8fR0M-4W1JQg1iq3_muUU6OTqT_3l4Ubrk,2338
+mlrun/launcher/local.py,sha256=6E83lCJ8Ma4WPCQYzo3P6c4tvpIipJsokZ3zMrCORbk,10909
+mlrun/launcher/remote.py,sha256=2DGInyx0um5BRUEA5DYcnLXzVKTIv8JxeXogWdxl48o,7469
 mlrun/model_monitoring/__init__.py,sha256=XaYyvWsIXpjJQ2gCPj8tFvfSbRSEEqgDtNz4tCE5H4g,915
-mlrun/model_monitoring/api.py,sha256=GXQNIVjjoMK-lM2MRRdQxQPnyfNhzm3ZgyxgSTcF3OM,36626
-mlrun/model_monitoring/application.py,sha256=Omy8t8GKqtCachQ67iovM1e0DQ24WXCH7K9QfjJ42Gw,12282
-mlrun/model_monitoring/batch.py,sha256=s2QCB0NW6Aiwy8JXveOb5-ULcwr5cCp4zG1z1yCkkog,39836
-mlrun/model_monitoring/controller.py,sha256=9HIM0Ko2c4D-1d2q4--Bebuch8r6CMZHGrtef5jVZg8,28342
+mlrun/model_monitoring/api.py,sha256=urggp5P_lpfLO1RO4YVdT_jDhIMF8Xqr22H3OYhRZnw,36535
+mlrun/model_monitoring/application.py,sha256=w87IuSgkIUXV5T6HpMiWWCsxFoikD6Mk8JpoyoefUCg,12504
+mlrun/model_monitoring/batch.py,sha256=nVEj-NtgqE4m9-LPMiWht-ZEbw4YY24jjaskuTcsPqs,38184
+mlrun/model_monitoring/controller.py,sha256=OUqrZkYuCP2_t5pSEZ4gOemejWbjnNLTcdMEAKTBths,27925
 mlrun/model_monitoring/controller_handler.py,sha256=J9Y9ppLsQaxyYRl21165Rr7QuI9EM-mk-5veAqs4Bi0,1336
 mlrun/model_monitoring/evidently_application.py,sha256=o9PsDsjyRfcbuC1X1gb2ww5nzWCsR_KheabtpxKZ5yY,4824
-mlrun/model_monitoring/features_drift_table.py,sha256=1HrL11_0zvl8LjKSjluEaE92WlCmGwoeqoBazxYog6M,24866
-mlrun/model_monitoring/helpers.py,sha256=Y7X-YjIaV2LN4Aiski50IEIP0dLCv6uTfzwzS5FVisE,7302
+mlrun/model_monitoring/features_drift_table.py,sha256=c6GpKtpOJbuT1u5uMWDL_S-6N4YPOmlktWMqPme3KFY,25308
+mlrun/model_monitoring/helpers.py,sha256=OsMBvRS_kSFe4cdarwVrrlwGeRDOesUm8zmasfRcfQg,9013
 mlrun/model_monitoring/model_endpoint.py,sha256=BBtxdY5ciormI_al4zshmIp0GN7hGhOCn-hLgpCXek0,3938
 mlrun/model_monitoring/prometheus.py,sha256=cUR4y73GutJB_pA_VCBDl9YtK4PcIJp2wj2rnLVmYi4,7578
-mlrun/model_monitoring/stream_processing.py,sha256=o2EmztZH3SZTawZwcvwCsaxGwNWmoZdw3YS1-YJJG0o,48113
+mlrun/model_monitoring/stream_processing.py,sha256=XKj9ToKj7VgF_Yxb6I27r1AoVU64EwflGC1966oIUaQ,48198
 mlrun/model_monitoring/tracking_policy.py,sha256=9P0oRjFMfoqKY7Zv2rv7abKgnKkiepFJfimWx-LOm0M,5283
 mlrun/model_monitoring/writer.py,sha256=IWPzPenoAkfIxlvn0IdcdB19Nxqmg4mjbo3-RnYWw9A,8669
 mlrun/model_monitoring/applications/__init__.py,sha256=6CsTXAxeLbbf8yfCADTaxmiavqwrLEdYFJ-qc5kgDAY,569
-mlrun/model_monitoring/applications/histogram_data_drift.py,sha256=FeEKXYY7ORiBOKNUI45z8Z2xXzzuIKIai1WQnPMc5bU,8005
+mlrun/model_monitoring/applications/histogram_data_drift.py,sha256=IG1qRXs316OdjcLLEHeKGH4t6WZabt8o92RLk-iB9e4,11647
 mlrun/model_monitoring/metrics/__init__.py,sha256=6CsTXAxeLbbf8yfCADTaxmiavqwrLEdYFJ-qc5kgDAY,569
 mlrun/model_monitoring/metrics/histogram_distance.py,sha256=E9_WIl2vd6qNvoHVHoFcnuQk3ekbFWOdi8aU7sHrfk4,4724
 mlrun/model_monitoring/stores/__init__.py,sha256=adU_G07jkD3JUT8__d0jAxs9nNomL7igKmd6uVM9L50,4525
 mlrun/model_monitoring/stores/kv_model_endpoint_store.py,sha256=SVHoaG4cfwntPfQMj6ZEzL5lGDYG67orCIAIb5-G9SE,22222
 mlrun/model_monitoring/stores/model_endpoint_store.py,sha256=stinaLq9W1iq2UJiTbPnk28Mvaeail7gwcJYHbrVjfE,5590
 mlrun/model_monitoring/stores/sql_model_endpoint_store.py,sha256=S5SA2P2BfLeg5lXCrEnMutghFffdmE59SCnQUiEjP7w,16139
 mlrun/model_monitoring/stores/models/__init__.py,sha256=5Djb73mfM9PxWE5EFUzrpLVLkuGaA34APibi_l-lu8k,1111
@@ -242,49 +242,52 @@
 mlrun/package/utils/type_hint_utils.py,sha256=JYrek6vuN3z7e6MGUD3qBLDfQ03C4puZXNTpDSj-VrM,14695
 mlrun/platforms/__init__.py,sha256=ArWn_iZiEE6qz7hvY_1RqMkFnHGuKjP3k5xYKnfKA58,2352
 mlrun/platforms/iguazio.py,sha256=M89zXuCd1bbcIANSy4ec-9evXIs7nPRVo3D0YhKvEtE,19434
 mlrun/platforms/other.py,sha256=T1BibmEBNggM62YJ6oejRmcVv_1besfH5DDHhCaDkRg,11828
 mlrun/projects/__init__.py,sha256=Lv5rfxyXJrw6WGOWJKhBz66M6t3_zsNMCfUD6waPwx4,1153
 mlrun/projects/operations.py,sha256=SiDHd7cqh9u23AVpETbkJE6WmOnB434zBrwM-StZLQY,18538
 mlrun/projects/pipelines.py,sha256=SMXBmIeuopwPpU0o2VFvaPXgbmaj-2WfCJryN6mZvZY,40124
-mlrun/projects/project.py,sha256=7BJwLO9pdEfrP55Ppf2z3nLOQ_gPWQIhgt_pZvqKtm4,158052
-mlrun/runtimes/__init__.py,sha256=vsoNA9ts_VPvGN9YPYKAjkxZe1RaZu22D5t-tiMyP-4,7034
-mlrun/runtimes/base.py,sha256=Faxa44TFCu7xA3UzYl36u1ZMpITJpTkiFJ7j-oRhJVA,36562
+mlrun/projects/project.py,sha256=S8nL7it4E92OUWGE6PSjoQQsGNV22Q5bnRsaI2LEL2E,165058
+mlrun/runtimes/__init__.py,sha256=tTDfia4cr0gUy2rEtLTj4Nz6M_JJd6utzkFi-ogDvXg,8289
+mlrun/runtimes/base.py,sha256=pXZAuE5kzOwdSBUjscdXzgfjdfzW4PxLq9d3Mf0IQbI,36572
 mlrun/runtimes/constants.py,sha256=oP3OxdYCpbvadJ3zP1JGkqGBKaBheNkCnJISWha9x58,9513
 mlrun/runtimes/daskjob.py,sha256=xvN8ajs3-_voqxrfz6b3rh_idNw4ypRAkPRWGOnDMGA,19149
 mlrun/runtimes/funcdoc.py,sha256=FHwnLfFzoD6yGlsAJXAl_3VTtudgg4fTrsw_XqLOkC0,10508
 mlrun/runtimes/function_reference.py,sha256=iWKRe4r2GTc5S8FOIASYUNLwwne8NqIui51PFr8Q4mg,4918
 mlrun/runtimes/generators.py,sha256=v28HdNgxdHvj888G1dTnUeQZz-D9iTO0hoGeZbCdiuQ,7241
 mlrun/runtimes/kubejob.py,sha256=UfSm7hiPLAtM0TfIE5nbBdSvrbsKWCZfvKP-SZhGyAk,12500
 mlrun/runtimes/local.py,sha256=u9MhASzF7VRt_yT6_mZPze_hDvAaBxonPk_KafRG3Gg,21783
-mlrun/runtimes/pod.py,sha256=6s-ZLNudzoILXfpvb0_DPWujMrKXaza_yc2rfId8wss,58650
+mlrun/runtimes/pod.py,sha256=id1mxg6lCIWQA55x0Yk3-fLwtnR9MisRkwRoIW0rWCE,58664
 mlrun/runtimes/remotesparkjob.py,sha256=ORkKmZRz_V3YiNE1NF7JIa_hI_LWbKEyI15Qb6R6g5I,7326
 mlrun/runtimes/utils.py,sha256=G4t29elE2PBT7WQZmrEOTIFAJUmeu6zXGEWwgz533vg,16004
 mlrun/runtimes/databricks_job/__init__.py,sha256=kXGBqhLN0rlAx0kTXhozGzFsIdSqW0uTSKMmsLgq_is,569
 mlrun/runtimes/databricks_job/databricks_cancel_task.py,sha256=sIqIg5DQAf4j0wCPA-G0GoxY6vacRddxCy5KDUZszek,2245
 mlrun/runtimes/databricks_job/databricks_runtime.py,sha256=a9W7A8sboteQov0Z9uVcthEU3FGYFf2cdAsi-vdjH1w,12749
 mlrun/runtimes/databricks_job/databricks_wrapper.py,sha256=-kzz5b3YBit6sGWojjREW_aHHRTx72zzTbxWGxvUplE,8679
 mlrun/runtimes/mpijob/__init__.py,sha256=jZf2uPBv6IB18Jj-dGSQ9NU5_xxni7XS4dnDZGwESFE,1583
 mlrun/runtimes/mpijob/abstract.py,sha256=AqIb-nEKZaRO7x1GxJea6cXg_Tn3Dr4WiWZUz3ywCjU,9161
 mlrun/runtimes/mpijob/v1.py,sha256=_RUlFo_3NcFf7x-QpUNVm8f7qNbRDIdUmPf_ijrv54U,3206
 mlrun/runtimes/mpijob/v1alpha1.py,sha256=w_971wwL03hW_ksgHJXdjTdjhxCs9KJ0zNqHSQ9whIM,1034
 mlrun/runtimes/nuclio/__init__.py,sha256=gx1kizzKv8pGT5TNloN1js1hdbxqDw3rM90sLVYVffY,794
 mlrun/runtimes/nuclio/api_gateway.py,sha256=t4im6F8f-zPYYXrHXCFr46Rw6sGgvydIpxpgxncTUMQ,10277
-mlrun/runtimes/nuclio/function.py,sha256=glnE8K-4rQVfQB2hCeLt8OtcpG2NFwKgEB8aRClcSJ4,47402
+mlrun/runtimes/nuclio/function.py,sha256=bCK_EVrLe2NfAelVpKtQrOYVnsPMiT91sB2_aJzLP_o,48990
 mlrun/runtimes/nuclio/nuclio.py,sha256=sLK8KdGO1LbftlL3HqPZlFOFTAAuxJACZCVl1c0Ha6E,2942
 mlrun/runtimes/nuclio/serving.py,sha256=hzkXKCVgU6uXLYfO3H15ZWJIQiSbcKY2M_WLybHW1hM,30363
+mlrun/runtimes/nuclio/application/__init__.py,sha256=rRs5vasy_G9IyoTpYIjYDafGoL6ifFBKgBtsXn31Atw,614
+mlrun/runtimes/nuclio/application/application.py,sha256=IxBvE7XcQKgtPWJqib32v6ANigxbK0-yfKC3vq0mjG4,9678
+mlrun/runtimes/nuclio/application/reverse_proxy.go,sha256=RDR2BuO7E87Ek9DYjvEaF5manuxcuVaVY7eZX986GFI,2920
 mlrun/runtimes/sparkjob/__init__.py,sha256=_KPvk0qefeLtHO6lxQE_AMOGiMTG_OT48eRCE4Z2ldw,709
 mlrun/runtimes/sparkjob/spark3job.py,sha256=yU-PxEI2pDJK5LHXTTcmrdjmO1Jwrj5Zyf8NwPDnZyA,41189
 mlrun/serving/__init__.py,sha256=_6HRAOuS2Ehjo3vwx5h1aI_-JppxEAsl4VfEERAbGFE,1078
 mlrun/serving/merger.py,sha256=PXLn3A21FiLteJHaDSLm5xKNT-80eTTjfHUJnBX1gKY,6116
 mlrun/serving/remote.py,sha256=jLFjMfgPx_PwJkpRHYbKrB9EQZcD4gZ-iczzHl1o0zs,18010
 mlrun/serving/routers.py,sha256=YN8k6eWWraqWOU3SqYFda7ky-oV_O0--zAuPEGwKdPI,54976
 mlrun/serving/server.py,sha256=42wWLtMb1AWeXtSXzSv0bKfQkxAQreqxs40Q0C_Bc-c,21161
 mlrun/serving/serving_wrapper.py,sha256=R670-S6PX_d5ER6jiHtRvacuPyFzQH0mEf2K0sBIIOM,836
-mlrun/serving/states.py,sha256=Jd08eDKSeh_PmR5HEwmCDYmCinOUUUacHwWW_URnjK0,56175
+mlrun/serving/states.py,sha256=EUkltwQlNNU6mjsUc8f3Rq65SGiAICkCAxbHw2jUqBk,55773
 mlrun/serving/utils.py,sha256=WO0n_YTO0YVPTjp_90zxRl4vey4flDgw5vaOHK5p_qY,3871
 mlrun/serving/v1_serving.py,sha256=by4myxlnwyZ0ijQ5fURilGCK1sUpdQL2Il1VR3Xqpxg,11805
 mlrun/serving/v2_serving.py,sha256=z1jTy0ObRFpV5nxMk-FGL2PoTQf-L01sYjfdA6_NqJc,23559
 mlrun/track/__init__.py,sha256=LWRUHJt8JyFW17FyNPOVyWd-NXTf1iptzsK9KFj5fuY,765
 mlrun/track/tracker.py,sha256=y-UdhC2nzM6r-yHCwvrfiHRr93xsr4JRsZTxDrTTRJo,3541
 mlrun/track/tracker_manager.py,sha256=IYBl99I62IC6VCCmG1yt6JoHNOQXa53C4DURJ2sWgio,5726
 mlrun/track/trackers/__init__.py,sha256=9xft8YjJnblwqt8f05htmOt_eDzVBVQN07RfY_SYLCs,569
@@ -309,15 +312,15 @@
 mlrun/utils/notifications/notification/base.py,sha256=gnmhNl59K9h4BGVAk77gVHWw-3kphchRL3Cwm-R0Cp4,2279
 mlrun/utils/notifications/notification/console.py,sha256=leZrjwu3fFA1sCYsTxDXEGZ02SWTUk4GNzp7tT2uaCc,2532
 mlrun/utils/notifications/notification/git.py,sha256=5pJs3LFzuz2h3JO9vAGo3BL00-WZFdUcCaO2XaZh-1I,5221
 mlrun/utils/notifications/notification/ipython.py,sha256=d47s-fW4TgqOJZOSdmzBQvdh2oDHoFw-ENLgNcAQSWU,1955
 mlrun/utils/notifications/notification/slack.py,sha256=5JysqIpUYUZKXPSeeZtbl7qb2L9dj7p2NvnEBcEsZkA,3898
 mlrun/utils/notifications/notification/webhook.py,sha256=QHezCuN5uXkLcroAGxGrhGHaxAdUvkDLIsp27_Yrfd4,2390
 mlrun/utils/version/__init__.py,sha256=7kkrB7hEZ3cLXoWj1kPoDwo4MaswsI2JVOBpbKgPAgc,614
-mlrun/utils/version/version.json,sha256=ZRswxH-AwVSByZa3TM00R47LdOv7o0_cYL3CzdifHz0,88
+mlrun/utils/version/version.json,sha256=ILF1rc0HYdLIjaV0EoivXDa8o11QVEm_vR_0HbZkVBA,88
 mlrun/utils/version/version.py,sha256=eEW0tqIAkU9Xifxv8Z9_qsYnNhn3YH7NRAfM-pPLt1g,1878
-mlrun-1.7.0rc5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlrun-1.7.0rc5.dist-info/METADATA,sha256=_bRlth3i1-0z_O8MHjRjyJPFlevk6zBa_kGp53B3mOE,18263
-mlrun-1.7.0rc5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mlrun-1.7.0rc5.dist-info/entry_points.txt,sha256=1Owd16eAclD5pfRCoJpYC2ZJSyGNTtUr0nCELMioMmU,46
-mlrun-1.7.0rc5.dist-info/top_level.txt,sha256=NObLzw3maSF9wVrgSeYBv-fgnHkAJ1kEkh12DLdd5KM,6
-mlrun-1.7.0rc5.dist-info/RECORD,,
+mlrun-1.7.0rc6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlrun-1.7.0rc6.dist-info/METADATA,sha256=aTGZl-fqFbpXsw_iPz64qD7nl2dBrtDqZuuxItHHQ3Q,18263
+mlrun-1.7.0rc6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mlrun-1.7.0rc6.dist-info/entry_points.txt,sha256=1Owd16eAclD5pfRCoJpYC2ZJSyGNTtUr0nCELMioMmU,46
+mlrun-1.7.0rc6.dist-info/top_level.txt,sha256=NObLzw3maSF9wVrgSeYBv-fgnHkAJ1kEkh12DLdd5KM,6
+mlrun-1.7.0rc6.dist-info/RECORD,,
```

