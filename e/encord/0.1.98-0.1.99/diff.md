# Comparing `tmp/encord-0.1.98.tar.gz` & `tmp/encord-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.98.tar", max compression
+gzip compressed data, was "encord-0.1.99.tar", max compression
```

## Comparing `encord-0.1.98.tar` & `encord-0.1.99.tar`

### file list

```diff
@@ -1,94 +1,95 @@
--rw-r--r--   0        0        0    11330 2023-11-07 11:19:20.118082 encord-0.1.98/LICENSE
--rw-r--r--   0        0        0     2027 2023-11-07 11:19:20.118082 encord-0.1.98/README.md
--rw-r--r--   0        0        0      158 2023-11-07 11:19:20.130082 encord-0.1.98/encord/__init__.py
--rw-r--r--   0        0        0      100 2023-11-07 11:19:20.130082 encord-0.1.98/encord/_version.py
--rw-r--r--   0        0        0    50071 2023-11-07 11:19:20.130082 encord-0.1.98/encord/client.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.130082 encord-0.1.98/encord/common/__init__.py
--rw-r--r--   0        0        0       45 2023-11-07 11:19:20.130082 encord-0.1.98/encord/common/constants.py
--rw-r--r--   0        0        0      568 2023-11-07 11:19:20.130082 encord-0.1.98/encord/common/deprecated.py
--rw-r--r--   0        0        0      508 2023-11-07 11:19:20.130082 encord-0.1.98/encord/common/enum.py
--rw-r--r--   0        0        0      260 2023-11-07 11:19:20.130082 encord-0.1.98/encord/common/utils.py
--rw-r--r--   0        0        0    10776 2023-11-07 11:19:20.130082 encord-0.1.98/encord/configs.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.130082 encord-0.1.98/encord/constants/__init__.py
--rw-r--r--   0        0        0      866 2023-11-07 11:19:20.130082 encord-0.1.98/encord/constants/enums.py
--rw-r--r--   0        0        0     3196 2023-11-07 11:19:20.130082 encord-0.1.98/encord/constants/model.py
--rw-r--r--   0        0        0     4522 2023-11-07 11:19:20.130082 encord-0.1.98/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-11-07 11:19:20.130082 encord-0.1.98/encord/constants/string_constants.py
--rw-r--r--   0        0        0    16025 2023-11-07 11:19:20.134082 encord-0.1.98/encord/dataset.py
--rw-r--r--   0        0        0     6355 2023-11-07 11:19:20.134082 encord-0.1.98/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/bundle.py
--rw-r--r--   0        0        0      319 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/common.py
--rw-r--r--   0        0        0     1258 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/constants.py
--rw-r--r--   0        0        0     7173 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/limits.py
--rw-r--r--   0        0        0     8531 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/querier.py
--rw-r--r--   0        0        0      747 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/query_methods.py
--rw-r--r--   0        0        0     1738 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/request.py
--rw-r--r--   0        0        0     6225 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/utils.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/v2/__init__.py
--rw-r--r--   0        0        0     3464 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/v2/api_client.py
--rw-r--r--   0        0        0      964 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/v2/error_utils.py
--rw-r--r--   0        0        0      223 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/v2/payloads.py
--rw-r--r--   0        0        0     2249 2023-11-07 11:19:20.134082 encord-0.1.98/encord/http/v2/request_signer.py
--rw-r--r--   0        0        0      662 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/__init__.py
--rw-r--r--   0        0        0    17930 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/answers.py
--rw-r--r--   0        0        0     9547 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/attributes.py
--rw-r--r--   0        0        0     5233 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/bitmask.py
--rw-r--r--   0        0        0     3215 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/classification.py
--rw-r--r--   0        0        0    24224 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/classification_instance.py
--rw-r--r--   0        0        0     2112 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/common.py
--rw-r--r--   0        0        0      579 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/constants.py
--rw-r--r--   0        0        0     5656 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3361 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/frames.py
--rw-r--r--   0        0        0     4385 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0      444 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/metadata.py
--rw-r--r--   0        0        0     6020 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/ontology_element.py
--rw-r--r--   0        0        0    65064 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0     3462 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/ontology_object.py
--rw-r--r--   0        0        0    39709 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/ontology_object_instance.py
--rw-r--r--   0        0        0    10964 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0     5167 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/options.py
--rw-r--r--   0        0        0      529 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/project.py
--rw-r--r--   0        0        0     1249 2023-11-07 11:19:20.134082 encord-0.1.98/encord/objects/utils.py
--rw-r--r--   0        0        0     2747 2023-11-07 11:19:20.134082 encord-0.1.98/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/__init__.py
--rw-r--r--   0        0        0      929 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/analytics.py
--rw-r--r--   0        0        0      982 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/api_key.py
--rw-r--r--   0        0        0      486 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/base_dto/__init__.py
--rw-r--r--   0        0        0      371 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/base_dto/base_dto_interface.py
--rw-r--r--   0        0        0     1544 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/base_dto/base_dto_pydantic_v1.py
--rw-r--r--   0        0        0     1607 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/base_dto/base_dto_pydantic_v2.py
--rw-r--r--   0        0        0     5257 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    35050 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/dataset.py
--rw-r--r--   0        0        0      829 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      256 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/formatter.py
--rw-r--r--   0        0        0     1592 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/label_log.py
--rw-r--r--   0        0        0    11889 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6667 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/model.py
--rw-r--r--   0        0        0     3419 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/ontology.py
--rw-r--r--   0        0        0     8834 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0      314 2023-11-07 11:19:20.134082 encord-0.1.98/encord/orm/workflow.py
--rw-r--r--   0        0        0    41336 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-11-07 11:19:20.134082 encord-0.1.98/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    30665 2023-11-07 11:19:20.134082 encord-0.1.98/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4275 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/common.py
--rw-r--r--   0        0        0     3469 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-11-07 11:19:20.134082 encord-0.1.98/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     2016 2023-11-07 11:19:20.134082 encord-0.1.98/pyproject.toml
--rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 encord-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0    11331 2023-12-01 10:35:22.428183 encord-0.1.99/LICENSE
+-rw-r--r--   0        0        0     2027 2023-12-01 10:35:22.428183 encord-0.1.99/README.md
+-rw-r--r--   0        0        0      158 2023-12-01 10:35:22.440183 encord-0.1.99/encord/__init__.py
+-rw-r--r--   0        0        0      100 2023-12-01 10:35:22.440183 encord-0.1.99/encord/_version.py
+-rw-r--r--   0        0        0    51479 2023-12-01 10:35:22.440183 encord-0.1.99/encord/client.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.440183 encord-0.1.99/encord/common/__init__.py
+-rw-r--r--   0        0        0      102 2023-12-01 10:35:22.440183 encord-0.1.99/encord/common/constants.py
+-rw-r--r--   0        0        0      568 2023-12-01 10:35:22.440183 encord-0.1.99/encord/common/deprecated.py
+-rw-r--r--   0        0        0      508 2023-12-01 10:35:22.440183 encord-0.1.99/encord/common/enum.py
+-rw-r--r--   0        0        0      891 2023-12-01 10:35:22.440183 encord-0.1.99/encord/common/time_parser.py
+-rw-r--r--   0        0        0      260 2023-12-01 10:35:22.440183 encord-0.1.99/encord/common/utils.py
+-rw-r--r--   0        0        0    10767 2023-12-01 10:35:22.440183 encord-0.1.99/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.440183 encord-0.1.99/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-12-01 10:35:22.440183 encord-0.1.99/encord/constants/enums.py
+-rw-r--r--   0        0        0     3196 2023-12-01 10:35:22.440183 encord-0.1.99/encord/constants/model.py
+-rw-r--r--   0        0        0     4522 2023-12-01 10:35:22.440183 encord-0.1.99/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-12-01 10:35:22.440183 encord-0.1.99/encord/constants/string_constants.py
+-rw-r--r--   0        0        0    16003 2023-12-01 10:35:22.440183 encord-0.1.99/encord/dataset.py
+-rw-r--r--   0        0        0     6355 2023-12-01 10:35:22.440183 encord-0.1.99/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/bundle.py
+-rw-r--r--   0        0        0      319 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/common.py
+-rw-r--r--   0        0        0     1258 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/constants.py
+-rw-r--r--   0        0        0     7813 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/limits.py
+-rw-r--r--   0        0        0     8579 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/querier.py
+-rw-r--r--   0        0        0      747 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1738 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/request.py
+-rw-r--r--   0        0        0     6225 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/utils.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/v2/__init__.py
+-rw-r--r--   0        0        0     5014 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/v2/api_client.py
+-rw-r--r--   0        0        0     1091 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/v2/error_utils.py
+-rw-r--r--   0        0        0      223 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/v2/payloads.py
+-rw-r--r--   0        0        0     2437 2023-12-01 10:35:22.440183 encord-0.1.99/encord/http/v2/request_signer.py
+-rw-r--r--   0        0        0      662 2023-12-01 10:35:22.440183 encord-0.1.99/encord/objects/__init__.py
+-rw-r--r--   0        0        0    17930 2023-12-01 10:35:22.440183 encord-0.1.99/encord/objects/answers.py
+-rw-r--r--   0        0        0     9547 2023-12-01 10:35:22.440183 encord-0.1.99/encord/objects/attributes.py
+-rw-r--r--   0        0        0     5233 2023-12-01 10:35:22.440183 encord-0.1.99/encord/objects/bitmask.py
+-rw-r--r--   0        0        0     3215 2023-12-01 10:35:22.440183 encord-0.1.99/encord/objects/classification.py
+-rw-r--r--   0        0        0    24260 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/classification_instance.py
+-rw-r--r--   0        0        0     2112 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/common.py
+-rw-r--r--   0        0        0      617 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/constants.py
+-rw-r--r--   0        0        0     5656 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3361 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/frames.py
+-rw-r--r--   0        0        0     4385 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0      444 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/metadata.py
+-rw-r--r--   0        0        0     6020 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/ontology_element.py
+-rw-r--r--   0        0        0    68131 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0     3462 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0    39745 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/ontology_object_instance.py
+-rw-r--r--   0        0        0    10964 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0     5167 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/options.py
+-rw-r--r--   0        0        0      588 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/project.py
+-rw-r--r--   0        0        0     1249 2023-12-01 10:35:22.444184 encord-0.1.99/encord/objects/utils.py
+-rw-r--r--   0        0        0     2747 2023-12-01 10:35:22.444184 encord-0.1.99/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/__init__.py
+-rw-r--r--   0        0        0      929 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/analytics.py
+-rw-r--r--   0        0        0      982 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/api_key.py
+-rw-r--r--   0        0        0      486 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/base_dto/__init__.py
+-rw-r--r--   0        0        0      371 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/base_dto/base_dto_interface.py
+-rw-r--r--   0        0        0     1544 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/base_dto/base_dto_pydantic_v1.py
+-rw-r--r--   0        0        0     1634 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/base_dto/base_dto_pydantic_v2.py
+-rw-r--r--   0        0        0     5257 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    35084 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/dataset.py
+-rw-r--r--   0        0        0      829 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      256 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1592 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/label_log.py
+-rw-r--r--   0        0        0    12041 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6694 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/model.py
+-rw-r--r--   0        0        0     3419 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/ontology.py
+-rw-r--r--   0        0        0     9129 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0      314 2023-12-01 10:35:22.444184 encord-0.1.99/encord/orm/workflow.py
+-rw-r--r--   0        0        0    41131 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-12-01 10:35:22.444184 encord-0.1.99/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    30584 2023-12-01 10:35:22.444184 encord-0.1.99/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4285 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/common.py
+-rw-r--r--   0        0        0     3469 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-12-01 10:35:22.444184 encord-0.1.99/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1597 2023-12-01 10:35:22.444184 encord-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0     3106 1970-01-01 00:00:00.000000 encord-0.1.99/PKG-INFO
```

### Comparing `encord-0.1.98/LICENSE` & `encord-0.1.99/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `encord-0.1.98/README.md` & `encord-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/client.py` & `encord-0.1.99/encord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from math import ceil
 from pathlib import Path
 from typing import Iterable, List, Optional, Tuple, Union, cast
 
 import requests
 
 import encord.exceptions
-from encord.configs import ENCORD_DOMAIN, ApiKeyConfig, Config, EncordConfig
+from encord.configs import ENCORD_DOMAIN, ApiKeyConfig, Config, EncordConfig, SshConfig
 from encord.constants.enums import DataType
 from encord.constants.model import AutomationModels, Device
 from encord.constants.string_constants import (
     FITTED_BOUNDING_BOX,
     INTERPOLATION,
     TYPE_DATASET,
     TYPE_PROJECT,
@@ -63,24 +63,28 @@
 from encord.http.querier import Querier
 from encord.http.utils import (
     CloudUploadSettings,
     upload_images_to_encord,
     upload_to_signed_url_list,
     upload_video_to_encord,
 )
+from encord.http.v2.api_client import ApiClient
+from encord.http.v2.payloads import Page
+from encord.orm.analytics import (
+    CollaboratorTimer,
+    CollaboratorTimerParams,
+    CollaboratorTimersGroupBy,
+)
 from encord.orm.api_key import ApiKeyMeta
 from encord.orm.cloud_integration import CloudIntegration
 from encord.orm.dataset import (
     DEFAULT_DATASET_ACCESS_SETTINGS,
     AddPrivateDataResponse,
     DataRow,
     DataRows,
-)
-from encord.orm.dataset import Dataset as OrmDataset
-from encord.orm.dataset import (
     DatasetAccessSettings,
     DatasetData,
     DatasetDataLongPolling,
     DatasetLinkItems,
     DatasetUser,
     DatasetUserRole,
     DatasetUsers,
@@ -90,14 +94,15 @@
     ImageGroupOCR,
     Images,
     LongPollingStatus,
     ReEncodeVideoTask,
     SingleImage,
     Video,
 )
+from encord.orm.dataset import Dataset as OrmDataset
 from encord.orm.label_log import LabelLog, LabelLogParams
 from encord.orm.label_row import (
     AnnotationTaskStatus,
     LabelRow,
     LabelRowMetadata,
     LabelStatus,
     Review,
@@ -119,49 +124,60 @@
     TrainingMetadata,
 )
 from encord.orm.project import (
     CopyDatasetAction,
     CopyDatasetOptions,
     CopyLabelsOptions,
     CopyProjectPayload,
-)
-from encord.orm.project import Project as OrmProject
-from encord.orm.project import (
     ProjectCopy,
     ProjectCopyOptions,
     ProjectDataset,
     ProjectUsers,
+    TaskPriorityParams,
 )
+from encord.orm.project import Project as OrmProject
 from encord.orm.workflow import (
     LabelWorkflowGraphNode,
     LabelWorkflowGraphNodePayload,
     WorkflowAction,
 )
 from encord.project_ontology.classification_type import ClassificationType
 from encord.project_ontology.object_type import ObjectShape
 from encord.project_ontology.ontology import Ontology
-from encord.utilities.client_utilities import optional_set_to_list, parse_datetime
+from encord.utilities.client_utilities import optional_datetime_to_iso_str, optional_set_to_list
 from encord.utilities.project_user import ProjectUser, ProjectUserRole
 
 LONG_POLLING_RESPONSE_RETRY_N = 3
 LONG_POLLING_SLEEP_ON_FAILURE_SECONDS = 10
 LONG_POLLING_MAX_REQUEST_TIME_SECONDS = 60
 
 logger = logging.getLogger(__name__)
 
 
-class EncordClient(object):
+class EncordClient:
     """
     Encord client. Allows you to query db items associated
     with a project (e.g. label rows, datasets).
     """
 
-    def __init__(self, querier: Querier, config: Config):
+    def __init__(self, querier: Querier, config: Config, api_client: Optional[ApiClient] = None):
         self._querier = querier
         self._config: Config = config
+        self._api_client = api_client
+
+    def _get_api_client(self) -> ApiClient:
+        if not isinstance(self._config, SshConfig):
+            raise EncordException(
+                "This functionality requires private SSH key authentication. API keys are not supported."
+            )
+
+        if not self._api_client:
+            raise RuntimeError("ApiClient should exist when authenticated with SSH key.")
+
+        return self._api_client
 
     @staticmethod
     def initialise(
         resource_id: Optional[str] = None,
         api_key: Optional[str] = None,
         domain: str = ENCORD_DOMAIN,
         requests_settings: RequestsSettings = DEFAULT_REQUESTS_SETTINGS,
@@ -354,16 +370,16 @@
 
         Raises:
             AuthorisationError: If the dataset API key is invalid.
             ResourceNotFoundError: If no dataset exists by the specified dataset EntityId.
             UnknownError: If an error occurs while retrieving the dataset.
         """
 
-        created_before = parse_datetime("created_before", created_before)
-        created_after = parse_datetime("created_after", created_after)
+        created_before = optional_datetime_to_iso_str("created_before", created_before)
+        created_after = optional_datetime_to_iso_str("created_after", created_after)
 
         data_rows = cast(
             List[DataRow],
             self._querier.get_multiple(
                 DataRows,
                 payload={
                     "title_eq": title_eq,
@@ -658,15 +674,15 @@
 
                 if files_finished_count != files_total_count:
                     print(f"Processed {files_finished_count}/{files_total_count} files")
                 else:
                     print("Processed all files, dataset data linking and task creation is performed, please wait")
 
                 failed_requests_count = 0
-            except requests.exceptions.RequestException:
+            except (requests.exceptions.RequestException, encord.exceptions.RequestException):
                 failed_requests_count += 1
 
                 if failed_requests_count >= LONG_POLLING_RESPONSE_RETRY_N:
                     raise
 
                 time.sleep(LONG_POLLING_SLEEP_ON_FAILURE_SECONDS)
 
@@ -706,14 +722,18 @@
 
 
 class EncordClientProject(EncordClient):
     """
     DEPRECATED - prefer using the :class:`encord.project.Project` instead
     """
 
+    @property
+    def project_hash(self) -> str:
+        return self._config.resource_id  # type: ignore[attr-defined]
+
     def get_project(self, include_labels_metadata=True) -> OrmProject:
         """
         Retrieve project info (pointers to data, labels).
 
         Args:
             include_labels_metadata: if false, label row metadata information will not be returned.
 
@@ -747,16 +767,16 @@
         """
         This function is documented in :meth:`encord.project.Project.list_label_rows`.
         """
 
         label_statuses_values = (
             [label_status.value for label_status in label_statuses] if label_statuses is not None else None
         )
-        edited_before = parse_datetime("edited_before", edited_before)
-        edited_after = parse_datetime("edited_after", edited_after)
+        edited_before = optional_datetime_to_iso_str("edited_before", edited_before)
+        edited_after = optional_datetime_to_iso_str("edited_after", edited_after)
 
         payload = {
             "edited_before": edited_before,
             "edited_after": edited_after,
             "label_statuses": label_statuses_values,
             "shadow_data_state": shadow_data_state.value if shadow_data_state else None,
             "include_uninitialised_labels": include_uninitialised_labels,
@@ -1315,14 +1335,27 @@
         """
         self._querier.basic_setter(
             LabelWorkflowGraphNode,
             label_hashes,
             payload=LabelWorkflowGraphNodePayload({"action": WorkflowAction.COMPLETE.value}),
         )
 
+    def workflow_set_priority(self, params: TaskPriorityParams) -> None:
+        self._get_api_client().post(
+            Path(f"projects/{self.project_hash}/priorities"),
+            params=None,
+            payload=params,
+            result_type=None,
+        )
+
+    def get_collaborator_timers_page(self, params: CollaboratorTimerParams) -> Page[CollaboratorTimer]:
+        return self._get_api_client().get(
+            Path("analytics/collaborators/timers"), params=params, result_type=Page[CollaboratorTimer]
+        )
+
 
 def _device_to_string(device: Device) -> str:
     if not isinstance(device, Device):
         if device is None or not Device.has_value(device):  # Backward compatibility with string options
             raise EncordException(message="You must pass a device from the `from encord.constants.model.Device` enum.")
         return cast(str, device)
```

### Comparing `encord-0.1.98/encord/common/deprecated.py` & `encord-0.1.99/encord/common/deprecated.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/configs.py` & `encord-0.1.99/encord/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,38 +26,37 @@
     Encoding,
     PublicFormat,
     load_ssh_private_key,
 )
 
 import encord.exceptions
 from encord.constants.string_constants import ALL_RESOURCE_TYPES
+from encord.exceptions import ResourceNotFoundError
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 
 ENCORD_DOMAIN = "https://api.encord.com"
 ENCORD_PUBLIC_PATH = "/public"
 ENCORD_PUBLIC_USER_PATH = "/public/user"
 ENCORD_ENDPOINT = ENCORD_DOMAIN + ENCORD_PUBLIC_PATH
 ENCORD_USER_ENDPOINT = ENCORD_DOMAIN + ENCORD_PUBLIC_USER_PATH
 WEBSOCKET_PATH = "/websocket"
-WEBSOCKET_DOMAIN = "wss://message-api.cord.tech"
+WEBSOCKET_DOMAIN = "wss://ws.encord.com"
 WEBSOCKET_ENDPOINT = WEBSOCKET_DOMAIN + WEBSOCKET_PATH
 
 _CORD_PROJECT_ID = "CORD_PROJECT_ID"
 _ENCORD_PROJECT_ID = "ENCORD_PROJECT_ID"
 _CORD_DATASET_ID = "CORD_DATASET_ID"
 _ENCORD_DATASET_ID = "ENCORD_DATASET_ID"
 _CORD_API_KEY = "CORD_API_KEY"
 _ENCORD_API_KEY = "ENCORD_API_KEY"
 _ENCORD_SSH_KEY = "ENCORD_SSH_KEY"
 _ENCORD_SSH_KEY_FILE = "ENCORD_SSH_KEY_FILE"
 
 logger = logging.getLogger(__name__)
 
-from encord.exceptions import ResourceNotFoundError
-
 
 class BaseConfig(ABC):
     def __init__(self, endpoint: str, requests_settings: RequestsSettings = DEFAULT_REQUESTS_SETTINGS):
         self.read_timeout: int = requests_settings.read_timeout
         self.write_timeout: int = requests_settings.write_timeout
         self.connect_timeout: int = requests_settings.connect_timeout
```

### Comparing `encord-0.1.98/encord/constants/enums.py` & `encord-0.1.99/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/constants/model.py` & `encord-0.1.99/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/constants/model_weights.py` & `encord-0.1.99/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/constants/string_constants.py` & `encord-0.1.99/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/dataset.py` & `encord-0.1.99/encord/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from typing import Dict, Iterable, List, Optional, TextIO, Union
 from uuid import UUID
 
 from encord.client import EncordClientDataset
 from encord.constants.enums import DataType
 from encord.http.utils import CloudUploadSettings
 from encord.orm.cloud_integration import CloudIntegration
-from encord.orm.dataset import AddPrivateDataResponse, DataRow
-from encord.orm.dataset import Dataset as OrmDataset
 from encord.orm.dataset import (
+    AddPrivateDataResponse,
+    DataRow,
     DatasetAccessSettings,
     DatasetDataLongPolling,
     DatasetUser,
     DatasetUserRole,
     Image,
     ImageGroupOCR,
     StorageLocation,
 )
+from encord.orm.dataset import Dataset as OrmDataset
 
 
 class Dataset:
     """
     Access dataset related data and manipulate the dataset.
     """
```

### Comparing `encord-0.1.98/encord/exceptions.py` & `encord-0.1.99/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/http/bundle.py` & `encord-0.1.99/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/http/constants.py` & `encord-0.1.99/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/http/error_utils.py` & `encord-0.1.99/encord/http/error_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,39 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from encord.exceptions import *
+from encord.exceptions import (
+    AnswerDictionaryError,
+    AuthenticationError,
+    AuthorisationError,
+    CorruptedLabelError,
+    DetectionRangeInvalidError,
+    DuplicateSshKeyError,
+    FeatureDoesNotExistError,
+    FileSizeNotSupportedError,
+    FileTypeNotSupportedError,
+    GenericServerError,
+    InvalidArgumentsError,
+    InvalidDateFormatError,
+    MethodNotAllowedError,
+    ModelFeaturesInconsistentError,
+    ModelWeightsInconsistentError,
+    MultiLabelLimitError,
+    OperationNotAllowed,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    SshKeyNotFound,
+    UnknownException,
+    UploadOperationNotSupportedError,
+    WrongProjectTypeError,
+)
 
 # Error messages
 AUTHENTICATION_ERROR = ["AUTHENTICATION_ERROR"]
 AUTHORISATION_ERROR = ["AUTHORISATION_ERROR"]
 RESOURCE_NOT_FOUND_ERROR = ["RESOURCE_NOT_FOUND_ERROR"]
 METHOD_NOT_ALLOWED_ERROR = ["METHOD_NOT_ALLOWED_ERROR"]
 UNKNOWN_ERROR = ["UNKNOWN_ERROR"]
```

### Comparing `encord-0.1.98/encord/http/querier.py` & `encord-0.1.99/encord/http/querier.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # under the License.
 import dataclasses
 import logging
 import platform
 import random
 import uuid
 from contextlib import contextmanager
-from typing import Any, Generator, List, Tuple, Type, TypeVar
+from typing import Any, Generator, List, Optional, Tuple, Type, TypeVar
 
 import requests
 import requests.exceptions
 from requests import Session
 from requests.adapters import HTTPAdapter, Retry
 
 from encord._version import __version__ as encord_version
 from encord.configs import BaseConfig
-from encord.exceptions import *
+from encord.exceptions import RequestException, ResourceNotFoundError
 from encord.http.common import (
     HEADER_CLOUD_TRACE_CONTEXT,
     HEADER_USER_AGENT,
     RequestContext,
 )
 from encord.http.error_utils import check_error_response
 from encord.http.query_methods import QueryMethods
```

### Comparing `encord-0.1.98/encord/http/query_methods.py` & `encord-0.1.99/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/http/request.py` & `encord-0.1.99/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/http/utils.py` & `encord-0.1.99/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/http/v2/api_client.py` & `encord-0.1.99/encord/http/v2/api_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import platform
+import random
+import uuid
 from pathlib import Path
 from typing import Optional, Type, TypeVar
 from urllib.parse import urljoin
 
 import requests
-from requests import Response
+from requests import PreparedRequest, Response
 
 from encord._version import __version__ as encord_version
 from encord.configs import UserConfig
 from encord.exceptions import RequestException
 from encord.http.common import (
     HEADER_CLOUD_TRACE_CONTEXT,
     HEADER_USER_AGENT,
@@ -38,56 +40,95 @@
             x_cloud_trace_context = x_cloud_trace_context.split(";")[0]
             trace_id, span_id = (x_cloud_trace_context.split("/") + [None, None])[:2]
             return RequestContext(trace_id=trace_id, span_id=span_id)
         except Exception:
             return RequestContext()
 
     @staticmethod
+    def _exception_context(request: requests.PreparedRequest) -> RequestContext:
+        try:
+            x_cloud_trace_context = request.headers.get(HEADER_CLOUD_TRACE_CONTEXT)
+            if x_cloud_trace_context is None:
+                return RequestContext()
+
+            x_cloud_trace_context = x_cloud_trace_context.split(";")[0]
+            trace_id, span_id = (x_cloud_trace_context.split("/") + [None, None])[:2]
+            return RequestContext(trace_id=trace_id, span_id=span_id)
+        except Exception:
+            return RequestContext()
+
+    @staticmethod
     def _user_agent():
         return f"encord-sdk-python/{encord_version} python/{platform.python_version()}"
 
+    @staticmethod
+    def _tracing_id() -> str:
+        return f"{uuid.uuid4().hex}/{random.randint(1, 2**63 - 1)};o=1"
+
     def _build_url(self, path: Path) -> str:
         return urljoin(self._domain, str(self._base_path / path))
 
     def _headers(self):
         return {
             "Accept": "application/json",
             "Accept-Encoding": "gzip",
             "Content-Type": "application/json",
             HEADER_USER_AGENT: self._user_agent(),
+            HEADER_CLOUD_TRACE_CONTEXT: self._tracing_id(),
         }
 
     def get(self, path: Path, params: Optional[BaseDTO], result_type: Type[T]) -> T:
         params_dict = params.to_dict() if params is not None else None
         req = requests.Request(
             method="GET", url=self._build_url(path), headers=self._headers(), params=params_dict
         ).prepare()
 
+        return self._request(req, result_type=result_type)  # type: ignore
+
+    def post(
+        self, path: Path, params: Optional[BaseDTO], payload: Optional[BaseDTO], result_type: Optional[Type[T]]
+    ) -> T:
+        params_dict = params.to_dict() if params is not None else None
+        req = requests.Request(
+            method="POST",
+            url=self._build_url(path),
+            headers=self._headers(),
+            params=params_dict,
+            json=payload.to_dict() if payload is not None else None,
+        ).prepare()
+
+        return self._request(req, result_type=result_type)  # type: ignore
+
+    def _request(self, req: PreparedRequest, result_type: Optional[Type[T]]):
         req = sign_request(req, self._config.public_key_hex, self._config.private_key)
 
         timeouts = (self._config.connect_timeout, self._config.read_timeout)
         req_settings = self._config.requests_settings
         with create_new_session(
             max_retries=req_settings.max_retries,
             backoff_factor=req_settings.backoff_factor,
             connect_retries=req_settings.connection_retries,
         ) as session:
+            context = self._exception_context(req)
+
             res = session.send(req, timeout=timeouts)
-            context = self._exception_context_from_response(res)
 
             if res.status_code != 200:
                 self._handle_error(res, context)
 
             try:
                 res_json = res.json()
             except Exception as e:
                 raise RequestException(f"Error parsing JSON response: {res.text}", context=context) from e
 
+            if result_type is None:
+                return None
+
             return result_type.from_dict(res_json)
 
     @staticmethod
     def _handle_error(response: Response, context: RequestContext):
         try:
             description = response.json()
-            handle_error_response(response.status_code, context=context, message=description["message"])
+            handle_error_response(response.status_code, context=context, message=description.get("message"))
         except Exception:
             handle_error_response(response.status_code, context=context)
```

### Comparing `encord-0.1.98/encord/http/v2/error_utils.py` & `encord-0.1.99/encord/http/v2/error_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from encord.exceptions import *
+from encord.exceptions import (
+    AuthenticationError,
+    AuthorisationError,
+    MethodNotAllowedError,
+    ResourceNotFoundError,
+    UnknownException,
+)
 
 HTTP_UNAUTHORIZED = 401
 HTTP_FORBIDDEN = 403
 HTTP_NOT_FOUND = 404
 HTTP_METHOD_NOT_ALLOWED = 405
 HTTP_GENERAL_ERROR = 500
```

### Comparing `encord-0.1.98/encord/http/v2/request_signer.py` & `encord-0.1.99/encord/http/v2/request_signer.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,16 +35,19 @@
         return b""
 
 
 def sign_request(request: PreparedRequest, key_id: str, private_key: Ed25519PrivateKey):
     assert request.method is not None
 
     content_digest = _sfv_str("sha-256", hashlib.sha256(_request_body_bytes(request)).digest())
+    # Moving 'created' time to be a bit in the past, since sometimes requests are failing
+    # due to the clock skew.
+    # This is to be fixed on server side and removed from here.
     signature_params: Dict[str, Union[str, int]] = {
-        "created": int(datetime.now().timestamp()),
+        "created": int(datetime.now().timestamp()) - 30,
         "keyid": key_id,
         "alg": "ed25519",
     }
 
     signature_elements = {
         "@method": request.method.upper(),
         "@request-target": request.path_url,
```

### Comparing `encord-0.1.98/encord/objects/__init__.py` & `encord-0.1.99/encord/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/answers.py` & `encord-0.1.99/encord/objects/answers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/attributes.py` & `encord-0.1.99/encord/objects/attributes.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/bitmask.py` & `encord-0.1.99/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/classification.py` & `encord-0.1.99/encord/objects/classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/classification_instance.py` & `encord-0.1.99/encord/objects/classification_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     List,
     NoReturn,
     Optional,
     Sequence,
     Union,
 )
 
-from dateutil.parser import parse
-
+from encord.common.time_parser import parse_datetime
 from encord.constants.enums import DataType
 from encord.exceptions import LabelRowError
 from encord.objects.answers import Answer, ValueType, _get_static_answer_map
 from encord.objects.attributes import (
     Attribute,
     ChecklistAttribute,
     RadioAttribute,
@@ -445,20 +444,20 @@
         last_edited_at: datetime = field(default_factory=datetime.now)
         last_edited_by: Optional[str] = None
         reviews: Optional[List[dict]] = None
 
         @staticmethod
         def from_dict(d: dict) -> ClassificationInstance.FrameData:
             if "lastEditedAt" in d:
-                last_edited_at = parse(d["lastEditedAt"])
+                last_edited_at = parse_datetime(d["lastEditedAt"])
             else:
                 last_edited_at = datetime.now()
 
             return ClassificationInstance.FrameData(
-                created_at=parse(d["createdAt"]),
+                created_at=parse_datetime(d["createdAt"]),
                 created_by=d["createdBy"],
                 confidence=d["confidence"],
                 manual_annotation=d["manualAnnotation"],
                 last_edited_at=last_edited_at,
                 last_edited_by=d.get("lastEditedBy"),
                 reviews=d.get("reviews"),
             )
```

### Comparing `encord-0.1.98/encord/objects/common.py` & `encord-0.1.99/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/constants.py` & `encord-0.1.99/encord/objects/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
+# for backwards compatibility
+from encord.common.constants import DATETIME_LONG_STRING_FORMAT
+
 DEFAULT_CONFIDENCE = 1.0
 DEFAULT_MANUAL_ANNOTATION = True
-DATETIME_LONG_STRING_FORMAT = "%a, %d %b %Y %H:%M:%S %Z"
 AVAILABLE_COLORS = (
     "#D33115",
     "#E27300",
     "#16406C",
     "#FE9200",
     "#FCDC00",
     "#DBDF00",
```

### Comparing `encord-0.1.98/encord/objects/coordinates.py` & `encord-0.1.99/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/frames.py` & `encord-0.1.99/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/internal_helpers.py` & `encord-0.1.99/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/ontology_element.py` & `encord-0.1.99/encord/objects/ontology_element.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/ontology_labels_impl.py` & `encord-0.1.99/encord/objects/ontology_labels_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from datetime import datetime
+from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Type, Union
 
 from encord.client import EncordClientProject
 from encord.client import LabelRow as OrmLabelRow
 from encord.constants.enums import DataType
 from encord.exceptions import LabelRowError, WrongProjectTypeError
 from encord.http.bundle import Bundle, BundleResultHandler, BundleResultMapper
@@ -46,14 +47,15 @@
     LabelRowMetadata,
     LabelStatus,
     WorkflowGraphNode,
 )
 from encord.orm.ontology import (  # pylint: disable=unused-import # for backward compatibility
     OntologyUserRole,
 )
+from encord.orm.project import TaskPriorityParams
 
 log = logging.getLogger(__name__)
 
 OntologyTypes = Union[Type[Object], Type[Classification]]
 OntologyClasses = Union[Object, Classification]
 
 
@@ -83,15 +85,18 @@
     the labels for that data row.
 
     You can access a many metadata fields with this class directly. If you want to read or write labels you will need to
     call :meth:`.initialise_labels()` first. To upload your added labels call :meth:`.save()`.
     """
 
     def __init__(
-        self, label_row_metadata: LabelRowMetadata, project_client: EncordClientProject, ontology: Ontology
+        self,
+        label_row_metadata: LabelRowMetadata,
+        project_client: EncordClientProject,
+        ontology: Ontology,
     ) -> None:
         self._project_client = project_client
         self._ontology = ontology
 
         self._label_row_read_only_data: LabelRowV2.LabelRowReadOnlyData = self._parse_label_row_metadata(
             label_row_metadata
         )
@@ -143,15 +148,15 @@
         **Note**: This method is not supported for workflow-based projects. Please see our
         :ref:`workflow documentation <tutorials/workflows:Workflows>`
         for more details.
         """
 
         if self.__is_tms2_project:
             raise WrongProjectTypeError(
-                '"label"_status property returns incorrect results for workflow-based projects.\
+                '"label_status" property returns incorrect results for workflow-based projects.\
              Please use "workflow_graph_node" property instead.'
             )
 
         return self._label_row_read_only_data.label_status
 
     @property
     def annotation_task_status(self) -> AnnotationTaskStatus:
@@ -226,14 +231,28 @@
         """
         This is `None` for image groups without performance optimisation, as there is no single underlying width
         for this data type.
         """
         return self._label_row_read_only_data.height
 
     @property
+    def priority(self) -> Optional[float]:
+        """
+        Get workflow priority for the task associated with the data unit.
+
+        This property only works for workflow-based project.
+
+        It is None for label rows in "complete" state.
+        """
+        if not self.__is_tms2_project:
+            raise WrongProjectTypeError('"priority" property only works with workflow-based projects.')
+
+        return self._label_row_read_only_data.priority
+
+    @property
     def ontology_structure(self) -> OntologyStructure:
         """Get the corresponding ontology structure"""
         return self._ontology.structure
 
     @property
     def is_labelling_initialised(self) -> bool:
         """
@@ -757,14 +776,28 @@
             raise LabelRowError(
                 "For this operation you will need to initialise labelling first. Call the .initialise_labels() "
                 "to do so first."
             )
 
         self._project_client.workflow_complete([self.label_hash])
 
+    def set_priority(self, priority: float) -> None:
+        """
+        Set priority for task in workflow project.
+
+        Args:
+            priority: float value from 0.0 to 1.0, where 1.0 is the highest priority
+        """
+        if not self.__is_tms2_project:
+            raise WrongProjectTypeError("Setting priority only possible for workflow-based projects")
+
+        params = TaskPriorityParams(priorities=[(self.data_hash, priority)])
+
+        self._project_client.workflow_set_priority(params)
+
     class FrameView:
         """
         This class can be used to inspect what object/classification instances are on a given frame or
         what metadata, such as a image file size, is on a given frame.
         """
 
         def __init__(
@@ -970,14 +1003,15 @@
         fps: Optional[float]
         dataset_hash: str
         dataset_title: str
         data_title: str
         width: Optional[int]
         height: Optional[int]
         data_link: Optional[str]
+        priority: Optional[float]
         frame_level_data: Dict[int, LabelRowV2.FrameLevelImageGroupData] = field(default_factory=dict)
         image_hash_to_frame: Dict[str, int] = field(default_factory=dict)
         frame_to_image_hash: Dict[int, str] = field(default_factory=dict)
 
     def _to_object_answers(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = {}
         for obj in self._objects_map.values():
@@ -1233,14 +1267,15 @@
             created_at=label_row_metadata.created_at,
             last_edited_at=label_row_metadata.last_edited_at,
             duration=label_row_metadata.duration,
             fps=label_row_metadata.frames_per_second,
             number_of_frames=label_row_metadata.number_of_frames,
             width=label_row_metadata.width,
             height=label_row_metadata.height,
+            priority=label_row_metadata.priority,
         )
 
     def _parse_label_row_dict(self, label_row_dict: dict) -> LabelRowReadOnlyData:
         frame_level_data = self._parse_image_group_frame_level_data(label_row_dict["data_units"])
         image_hash_to_frame = {item.image_hash: item.frame_number for item in frame_level_data.values()}
         frame_to_image_hash = {item.frame_number: item.image_hash for item in frame_level_data.values()}
         data_type = DataType(label_row_dict["data_type"])
@@ -1267,36 +1302,39 @@
             data_link = None
             height = None
             width = None
 
         else:
             raise NotImplementedError(f"The data type {data_type} is not implemented yet.")
 
-        return self.LabelRowReadOnlyData(
+        return LabelRowV2.LabelRowReadOnlyData(
             label_hash=label_row_dict["label_hash"],
             dataset_hash=label_row_dict["dataset_hash"],
             dataset_title=label_row_dict["dataset_title"],
             data_title=label_row_dict["data_title"],
             data_hash=label_row_dict["data_hash"],
             data_type=data_type,
             label_status=LabelStatus(label_row_dict["label_status"]),
             annotation_task_status=label_row_dict.get("annotation_task_status"),
-            workflow_graph_node=label_row_dict.get("workflow_graph_node"),
+            workflow_graph_node=label_row_dict.get(
+                "workflow_graph_node", self._label_row_read_only_data.workflow_graph_node
+            ),
             is_shadow_data=self.is_shadow_data,
             created_at=label_row_dict["created_at"],
             last_edited_at=label_row_dict["last_edited_at"],
             frame_level_data=frame_level_data,
             image_hash_to_frame=image_hash_to_frame,
             frame_to_image_hash=frame_to_image_hash,
             duration=self.duration,
             fps=self.fps,
             number_of_frames=self.number_of_frames,
             data_link=data_link,
             height=height,
             width=width,
+            priority=label_row_dict.get("priority", self._label_row_read_only_data.priority),
         )
 
     def _parse_labels_from_dict(self, label_row_dict: dict):
         classification_answers = label_row_dict["classification_answers"]
 
         for data_unit in label_row_dict["data_units"].values():
             data_type = DataType(label_row_dict["data_type"])
@@ -1378,29 +1416,51 @@
 
         label_class = ontology.get_child_by_hash(feature_hash, type_=Object)
         object_instance = ObjectInstance(label_class, object_hash=object_hash)
 
         coordinates = self._get_coordinates(frame_object_label)
         object_frame_instance_info = ObjectInstance.FrameInfo.from_dict(frame_object_label)
 
-        object_instance.set_for_frames(coordinates=coordinates, frames=frame, **asdict(object_frame_instance_info))
+        object_instance.set_for_frames(
+            coordinates=coordinates,
+            frames=frame,
+            created_at=object_frame_instance_info.created_at,
+            created_by=object_frame_instance_info.created_by,
+            last_edited_at=object_frame_instance_info.last_edited_at,
+            last_edited_by=object_frame_instance_info.last_edited_by,
+            confidence=object_frame_instance_info.confidence,
+            manual_annotation=object_frame_instance_info.manual_annotation,
+            reviews=object_frame_instance_info.reviews,
+            is_deleted=object_frame_instance_info.is_deleted,
+        )
         return object_instance
 
     def _add_coordinates_to_object_instance(
         self,
         frame_object_label: dict,
         frame: int = 0,
     ) -> None:
         object_hash = frame_object_label["objectHash"]
         object_instance = self._objects_map[object_hash]
 
         coordinates = self._get_coordinates(frame_object_label)
         object_frame_instance_info = ObjectInstance.FrameInfo.from_dict(frame_object_label)
 
-        object_instance.set_for_frames(coordinates=coordinates, frames=frame, **asdict(object_frame_instance_info))
+        object_instance.set_for_frames(
+            coordinates=coordinates,
+            frames=frame,
+            created_at=object_frame_instance_info.created_at,
+            created_by=object_frame_instance_info.created_by,
+            last_edited_at=object_frame_instance_info.last_edited_at,
+            last_edited_by=object_frame_instance_info.last_edited_by,
+            confidence=object_frame_instance_info.confidence,
+            manual_annotation=object_frame_instance_info.manual_annotation,
+            reviews=object_frame_instance_info.reviews,
+            is_deleted=object_frame_instance_info.is_deleted,
+        )
 
     def _get_coordinates(self, frame_object_label: dict) -> Coordinates:
         if "boundingBox" in frame_object_label:
             return BoundingBoxCoordinates.from_dict(frame_object_label)
         if "rotatableBoundingBox" in frame_object_label:
             return RotatableBoundingBoxCoordinates.from_dict(frame_object_label)
         elif "polygon" in frame_object_label:
@@ -1451,31 +1511,49 @@
         feature_hash = frame_classification_label["featureHash"]
         classification_hash = frame_classification_label["classificationHash"]
 
         label_class = self._ontology.structure.get_child_by_hash(feature_hash, type_=Classification)
         classification_instance = ClassificationInstance(label_class, classification_hash=classification_hash)
 
         frame_view = ClassificationInstance.FrameData.from_dict(frame_classification_label)
-        classification_instance.set_for_frames(frame, **asdict(frame_view))
+        classification_instance.set_for_frames(
+            frame,
+            created_at=frame_view.created_at,
+            created_by=frame_view.created_by,
+            confidence=frame_view.confidence,
+            manual_annotation=frame_view.manual_annotation,
+            last_edited_at=frame_view.last_edited_at,
+            last_edited_by=frame_view.last_edited_by,
+            reviews=frame_view.reviews,
+        )
+
         answers_dict = classification_answers[classification_hash]["classifications"]
         self._add_static_answers_from_dict(classification_instance, answers_dict)
 
         return classification_instance
 
     def _add_static_answers_from_dict(
         self, classification_instance: ClassificationInstance, answers_list: List[dict]
     ) -> None:
         classification_instance.set_answer_from_list(answers_list)
 
     def _add_frames_to_classification_instance(self, frame_classification_label: dict, frame: int) -> None:
         object_hash = frame_classification_label["classificationHash"]
         classification_instance = self._classifications_map[object_hash]
         frame_view = ClassificationInstance.FrameData.from_dict(frame_classification_label)
-
-        classification_instance.set_for_frames(frame, **asdict(frame_view))
+        classification_instance.set_for_frames(
+            frame,
+            created_at=frame_view.created_at,
+            created_by=frame_view.created_by,
+            confidence=frame_view.confidence,
+            manual_annotation=frame_view.manual_annotation,
+            last_edited_at=frame_view.last_edited_at,
+            last_edited_by=frame_view.last_edited_by,
+            reviews=frame_view.reviews,
+        )
 
     def _check_labelling_is_initalised(self):
         if not self.is_labelling_initialised:
             raise LabelRowError(
                 "For this operation you will need to initialise labelling first. Call the `.initialise_labels()` "
                 "to do so first."
             )
```

### Comparing `encord-0.1.98/encord/objects/ontology_object.py` & `encord-0.1.99/encord/objects/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/ontology_object_instance.py` & `encord-0.1.99/encord/objects/ontology_object_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Union,
 )
 
-from dateutil.parser import parse
-
+from encord.common.time_parser import parse_datetime
 from encord.constants.enums import DataType
 from encord.exceptions import LabelRowError
 from encord.objects import ChecklistAttribute, RadioAttribute, TextAttribute
 from encord.objects.answers import (
     Answer,
     _get_static_answer_map,
     get_default_answer_from_attribute,
@@ -628,20 +627,20 @@
         manual_annotation: bool = DEFAULT_MANUAL_ANNOTATION
         reviews: Optional[List[dict]] = None
         is_deleted: Optional[bool] = None
 
         @staticmethod
         def from_dict(d: dict):
             if "lastEditedAt" in d:
-                last_edited_at = parse(d["lastEditedAt"])
+                last_edited_at = parse_datetime(d["lastEditedAt"])
             else:
                 last_edited_at = datetime.now()
 
             return ObjectInstance.FrameInfo(
-                created_at=parse(d["createdAt"]),
+                created_at=parse_datetime(d["createdAt"]),
                 created_by=d["createdBy"],
                 last_edited_at=last_edited_at,
                 last_edited_by=d.get("lastEditedBy"),
                 confidence=d["confidence"],
                 manual_annotation=d["manualAnnotation"],
                 reviews=d.get("reviews"),
                 is_deleted=d.get("isDeleted"),
```

### Comparing `encord-0.1.98/encord/objects/ontology_structure.py` & `encord-0.1.99/encord/objects/ontology_structure.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/options.py` & `encord-0.1.99/encord/objects/options.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/objects/utils.py` & `encord-0.1.99/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/ontology.py` & `encord-0.1.99/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/analytics.py` & `encord-0.1.99/encord/orm/analytics.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/api_key.py` & `encord-0.1.99/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/base_dto/base_dto_pydantic_v1.py` & `encord-0.1.99/encord/orm/base_dto/base_dto_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/base_dto/base_dto_pydantic_v2.py` & `encord-0.1.99/encord/orm/base_dto/base_dto_pydantic_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Any, Dict, Type, TypeVar
 
 # TODO: invent some dependency version dependent type checking to get rid of this ignore
-from pydantic import ConfigDict  # type: ignore[attr-defined]
-from pydantic import BaseModel, ValidationError
+from pydantic import (  # type: ignore[attr-defined]
+    BaseModel,
+    ConfigDict,  # type: ignore[attr-defined]
+    ValidationError,
+)
 
 from encord.common.utils import snake_to_camel
 from encord.exceptions import EncordException
 from encord.orm.base_dto.base_dto_interface import BaseDTOInterface, T
 
 
 class BaseDTO(BaseDTOInterface, BaseModel):
```

### Comparing `encord-0.1.98/encord/orm/base_orm.py` & `encord-0.1.99/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/dataset.py` & `encord-0.1.99/encord/orm/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 import json
 from collections import OrderedDict
 from datetime import datetime
 from enum import Enum, IntEnum
 from typing import Any, Dict, List, Optional
 from uuid import UUID
 
-from dateutil import parser
-
 from encord.common.constants import DATETIME_STRING_FORMAT
 from encord.common.deprecated import deprecated
+from encord.common.time_parser import parse_datetime
 from encord.constants.enums import DataType
 from encord.exceptions import EncordException
 from encord.orm import base_orm
 from encord.orm.formatter import Formatter
 from encord.utilities.common import _get_dict_without_none_keys
 
 
@@ -151,16 +150,16 @@
         return ImageData(
             title=json_dict["title"],
             file_link=json_dict["file_link"],
             file_type=json_dict["file_type"],
             file_size=json_dict["file_size"],
             image_hash=json_dict["image_hash"],
             storage_location=json_dict["storage_location"],
-            created_at=parser.parse(json_dict["created_at"]),
-            last_edited_at=parser.parse(json_dict["last_edited_at"]),
+            created_at=parse_datetime(json_dict["created_at"]),
+            last_edited_at=parse_datetime(json_dict["last_edited_at"]),
             height=json_dict["height"],
             width=json_dict["width"],
             signed_url=json_dict.get("signed_url"),
         )
 
     @classmethod
     def from_list(cls, json_list: List) -> List[ImageData]:
@@ -266,15 +265,15 @@
     @data_type.setter
     def data_type(self, value: DataType) -> None:
         """DEPRECATED. Do not this function as it will never update the created_at in the server."""
         self["data_type"] = value.to_upper_case_string()
 
     @property
     def created_at(self) -> datetime:
-        return parser.parse(self["created_at"])
+        return parse_datetime(self["created_at"])
 
     @created_at.setter
     def created_at(self, value: datetime) -> None:
         """DEPRECATED. Do not this function as it will never update the created_at in the server."""
         self["created_at"] = value.strftime(DATETIME_STRING_FORMAT)
 
     @property
@@ -332,15 +331,15 @@
         each image in this group can have a different dimension. Inspect the
         :meth:`images <encord.data.DataRow.images>` to get the height of individual images.
         """
         return self["height"]
 
     @property
     def last_edited_at(self) -> datetime:
-        return parser.parse(self["last_edited_at"])
+        return parse_datetime(self["last_edited_at"])
 
     @property
     def file_link(self) -> Optional[str]:
         """
         A permanent file link of the given data asset. When stored in
         :meth:`StorageLocation.CORD_STORAGE <encord.orm.dataset.StorageLocation.CORD_STORAGE>` this will be the
         internal file path. In private bucket storage location this will be the full path to the file.
@@ -480,17 +479,17 @@
         backing_item_uuid = UUID(backing_item_uuid_value) if backing_item_uuid_value else None
 
         return DataRow(
             uid=json_dict["data_hash"],
             title=json_dict["data_title"],
             # The API server currently returns upper-cased DataType strings.
             data_type=data_type,
-            created_at=parser.parse(json_dict["created_at"]),
+            created_at=parse_datetime(json_dict["created_at"]),
             client_metadata=json_dict.get("client_metadata"),
-            last_edited_at=parser.parse(json_dict["last_edited_at"]),
+            last_edited_at=parse_datetime(json_dict["last_edited_at"]),
             width=json_dict["width"],
             height=json_dict["height"],
             file_link=json_dict["file_link"],
             file_size=json_dict["file_size"],
             file_type=json_dict["file_type"],
             storage_location=StorageLocation(json_dict["storage_location"]),
             frames_per_second=json_dict["frames_per_second"],
@@ -791,15 +790,15 @@
     GCP = (2,)
     AZURE = 3
     OTC = 4
 
     NEW_STORAGE = -99
     """
     This is a placeholder for a new storage location that is not yet supported by your SDK version.
-    Please update your SDK to the latest version. 
+    Please update your SDK to the latest version.
     """
 
     @staticmethod
     def from_str(string_location: str) -> StorageLocation:
         return STORAGE_LOCATION_BY_STR[string_location]
 
     def get_str(self) -> str:
@@ -991,15 +990,15 @@
 )
 
 
 @dataclasses.dataclass
 class ImagesDataFetchOptions:
     fetch_signed_urls: bool = False
     """
-    Whether to fetch signed urls for each individual image. Only set this to true if you need to download the 
+    Whether to fetch signed urls for each individual image. Only set this to true if you need to download the
     images.
     """
 
 
 class LongPollingStatus(str, Enum):
     PENDING = "PENDING"
     """Job will automatically start soon (waiting in queue) or already started processing."""
```

### Comparing `encord-0.1.98/encord/orm/dataset_with_user_role.py` & `encord-0.1.99/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/label_log.py` & `encord-0.1.99/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/label_row.py` & `encord-0.1.99/encord/orm/label_row.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import datetime
 from collections import OrderedDict
 from dataclasses import asdict, dataclass
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
+from encord.common.time_parser import parse_datetime
 from encord.orm import base_orm
 from encord.orm.formatter import Formatter
 
 
 class LabelRow(base_orm.BaseORM):
     """
     A label row contains a data unit or a collection of data units and associated
@@ -276,23 +277,25 @@
     number_of_frames: int
     duration: Optional[float]
     """Only available for the VIDEO data_type"""
     frames_per_second: Optional[int]
     """Only available for the VIDEO data_type"""
     height: Optional[int]
     width: Optional[int]
+    priority: Optional[float] = None
+    """Only available for not complete tasks"""
 
     @classmethod
     def from_dict(cls, json_dict: Dict) -> LabelRowMetadata:
         created_at = json_dict.get("created_at", None)
         if created_at is not None:
-            created_at = datetime.datetime.fromisoformat(created_at)
+            created_at = parse_datetime(created_at)
         last_edited_at = json_dict.get("last_edited_at", None)
         if last_edited_at is not None:
-            last_edited_at = datetime.datetime.fromisoformat(last_edited_at)
+            last_edited_at = parse_datetime(last_edited_at)
 
         annotation_task_status = (
             AnnotationTaskStatus(json_dict["annotation_task_status"])
             if json_dict["annotation_task_status"] is not None
             else None
         )
 
@@ -311,14 +314,15 @@
             workflow_graph_node=WorkflowGraphNode.from_optional_dict(json_dict.get("workflow_graph_node")),
             is_shadow_data=json_dict.get("is_shadow_data", False),
             number_of_frames=json_dict["number_of_frames"],
             duration=json_dict.get("duration", None),
             frames_per_second=json_dict.get("frames_per_second", None),
             height=json_dict.get("height"),
             width=json_dict.get("width"),
+            priority=json_dict.get("priority"),
         )
 
     @classmethod
     def from_list(cls, json_list: list) -> List[LabelRowMetadata]:
         ret = []
         for i in json_list:
             ret.append(cls.from_dict(i))
```

### Comparing `encord-0.1.98/encord/orm/labeling_algorithm.py` & `encord-0.1.99/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/model.py` & `encord-0.1.99/encord/orm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 # under the License.
 from collections import OrderedDict
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
-from dateutil.parser import parse
-
+from encord.common.time_parser import parse_datetime
 from encord.constants.model import AutomationModels
 from encord.exceptions import EncordException
 from encord.orm import base_orm
 from encord.orm.formatter import Formatter
 from encord.utilities.common import ENCORD_CONTACT_SUPPORT_EMAIL
 
 
@@ -134,15 +133,15 @@
 
     @staticmethod
     def get_created_at(json_dict: dict) -> Optional[datetime]:
         created_at = json_dict["created_at"]
         if created_at is None:
             return None
 
-        return parse(created_at)
+        return parse_datetime(created_at)
 
     @staticmethod
     def get_model_training_labels(json_dict: dict) -> Optional[ModelTrainingLabel]:
         model_training_labels = json_dict["model_training_labels"]
         if model_training_labels is None:
             return None
```

### Comparing `encord-0.1.98/encord/orm/ontology.py` & `encord-0.1.99/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/project.py` & `encord-0.1.99/encord/orm/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 # under the License.
 from __future__ import annotations
 
 import datetime
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
+from uuid import UUID
 
 from encord.common.enum import StringEnum
 from encord.orm import base_orm
+from encord.orm.base_dto import BaseDTO
 
 
 class Project(base_orm.BaseORM):
     """
     DEPRECATED - prefer using the `encord.project.Project` class instead.
 
     A project defines a label ontology and is a collection of datasets and label rows.
@@ -73,14 +75,15 @@
             ("created_at", datetime.datetime),
             ("last_edited_at", datetime.datetime),
             ("editor_ontology", (dict, str)),
             ("datasets", (list, str)),
             ("label_rows", (list, str)),
             ("ontology_hash", str),
             ("source_projects", list),
+            ("workflow_manager_uuid", str),
         ]
     )
 
     NON_UPDATABLE_FIELDS = {"editor_ontology", "datasets", "label_rows"}
 
     def get_labels_list(self) -> List[Optional[str]]:
         """
@@ -140,14 +143,18 @@
     def created_at(self) -> datetime.datetime:
         return self["created_at"]
 
     @property
     def last_edited_at(self) -> datetime.datetime:
         return self["last_edited_at"]
 
+    @property
+    def workflow_manager_uuid(self) -> UUID:
+        return self["workflow_manager_uuid"]
+
 
 class ProjectCopy:
     pass
 
 
 class ProjectUsers:
     pass
@@ -296,7 +303,11 @@
 
 class ProjectImporterCvatInfo(base_orm.BaseORM):
     DB_FIELDS = OrderedDict(
         [
             ("export_type", CvatExportType),
         ]
     )
+
+
+class TaskPriorityParams(BaseDTO):
+    priorities: List[Tuple[str, float]]
```

### Comparing `encord-0.1.98/encord/orm/project_api_key.py` & `encord-0.1.99/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/orm/project_with_user_role.py` & `encord-0.1.99/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/project.py` & `encord-0.1.99/encord/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Iterable, List, Optional, Set, Tuple, Union
 
 from encord.client import EncordClientProject
 from encord.common.deprecated import deprecated
 from encord.constants.model import AutomationModels, Device
 from encord.http.bundle import Bundle
 from encord.http.v2.api_client import ApiClient
-from encord.http.v2.payloads import Page
 from encord.objects import LabelRowV2, OntologyStructure
 from encord.ontology import Ontology
 from encord.orm.analytics import (
     CollaboratorTimer,
     CollaboratorTimerParams,
     CollaboratorTimersGroupBy,
 )
@@ -35,19 +34,16 @@
 
 
 class Project:
     """
     Access project related data and manipulate the project.
     """
 
-    def __init__(
-        self, client: EncordClientProject, project_instance: OrmProject, ontology: Ontology, client_v2: ApiClient
-    ):
+    def __init__(self, client: EncordClientProject, project_instance: OrmProject, ontology: Ontology):
         self._client = client
-        self._client_v2 = client_v2
         self._project_instance = project_instance
         self._ontology = ontology
 
     @property
     def project_hash(self) -> str:
         """
         Get the project hash (i.e. the Project ID).
@@ -993,17 +989,15 @@
             after=after,
             before=before,
             group_by=CollaboratorTimersGroupBy.DATA_UNIT if group_by_data_unit else CollaboratorTimersGroupBy.PROJECT,
             page_size=100,
         )
 
         while True:
-            page = self._client_v2.get(
-                Path("analytics/collaborators/timers"), params=params, result_type=Page[CollaboratorTimer]
-            )
+            page = self._client.get_collaborator_timers_page(params)
 
             yield from page.results
 
             if page.next_page_token is not None:
                 params.page_token = page.next_page_token
             else:
                 break
```

### Comparing `encord-0.1.98/encord/project_ontology/classification_attribute.py` & `encord-0.1.99/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/project_ontology/classification_option.py` & `encord-0.1.99/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/project_ontology/ontology.py` & `encord-0.1.99/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/project_ontology/ontology_classification.py` & `encord-0.1.99/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/project_ontology/ontology_object.py` & `encord-0.1.99/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/user_client.py` & `encord-0.1.99/encord/user_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import base64
 import logging
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from dateutil import parser as datetime_parser
-
 from encord.client import EncordClient, EncordClientDataset, EncordClientProject
 from encord.common.deprecated import deprecated
+from encord.common.time_parser import parse_datetime
 from encord.configs import SshConfig, UserConfig, get_env_ssh_key
 from encord.constants.string_constants import TYPE_DATASET, TYPE_ONTOLOGY, TYPE_PROJECT
 from encord.dataset import Dataset
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
 from encord.http.utils import (
     CloudUploadSettings,
@@ -25,41 +24,40 @@
 from encord.objects import OntologyStructure
 from encord.objects.common import (
     DeidentifyRedactTextMode,
     SaveDeidentifiedDicomCondition,
 )
 from encord.ontology import Ontology
 from encord.orm.cloud_integration import CloudIntegration
-from encord.orm.dataset import DEFAULT_DATASET_ACCESS_SETTINGS, CreateDatasetResponse
-from encord.orm.dataset import Dataset as OrmDataset
 from encord.orm.dataset import (
+    DEFAULT_DATASET_ACCESS_SETTINGS,
+    CreateDatasetResponse,
     DatasetAccessSettings,
     DatasetAPIKey,
     DatasetInfo,
     DatasetScope,
     DatasetUserRole,
     DicomDeidentifyTask,
     Images,
     StorageLocation,
 )
+from encord.orm.dataset import Dataset as OrmDataset
 from encord.orm.dataset_with_user_role import DatasetWithUserRole
 from encord.orm.ontology import Ontology as OrmOntology
 from encord.orm.project import (
     BenchmarkQaWorkflowSettings,
     CvatExportType,
     ManualReviewWorkflowSettings,
-)
-from encord.orm.project import Project as OrmProject
-from encord.orm.project import (
     ProjectImporter,
     ProjectImporterCvatInfo,
     ProjectWorkflowSettings,
     ProjectWorkflowType,
     ReviewMode,
 )
+from encord.orm.project import Project as OrmProject
 from encord.orm.project_api_key import ProjectAPIKey
 from encord.orm.project_with_user_role import ProjectWithUserRole
 from encord.project import Project
 from encord.utilities.client_utilities import (
     APIKeyScopes,
     CvatImporterError,
     CvatImporterSuccess,
@@ -114,28 +112,28 @@
             * Organisation admin of the project
 
         Args:
             project_hash: The Project ID
         """
         config = SshConfig(self.user_config, resource_type=TYPE_PROJECT, resource_id=project_hash)
         querier = Querier(config)
-        client = EncordClientProject(querier=querier, config=config)
+        client = EncordClientProject(querier=querier, config=config, api_client=self._api_client)
 
         orm_project = client.get_project(include_labels_metadata=False)
 
         # Querying ontology using project querier to avoid permission error,
         # as there might be only read-only ontology structure access in scope of the project,
         # not full access, that is implied by get_ontology method
         ontology_hash = orm_project["ontology_hash"]
         config = SshConfig(self.user_config, resource_type=TYPE_ONTOLOGY, resource_id=ontology_hash)
 
         orm_ontology = querier.basic_getter(OrmOntology, config.resource_id)
         project_ontology = Ontology(querier, config, orm_ontology)
 
-        return Project(client, orm_project, project_ontology, client_v2=self._api_client)
+        return Project(client, orm_project, project_ontology)
 
     def get_ontology(self, ontology_hash: str) -> Ontology:
         config = SshConfig(self.user_config, resource_type=TYPE_ONTOLOGY, resource_id=ontology_hash)
         querier = Querier(config)
         orm_ontology = querier.basic_getter(OrmOntology, ontology_hash)
         return Ontology(querier, config, orm_ontology)
 
@@ -239,16 +237,16 @@
             payload={
                 "filter": properties_filter,
                 "enable_storage_api": True,
             },
         )
 
         def convert_dates(dataset):
-            dataset["created_at"] = datetime_parser.isoparse(dataset["created_at"])
-            dataset["last_edited_at"] = datetime_parser.isoparse(dataset["last_edited_at"])
+            dataset["created_at"] = parse_datetime(dataset["created_at"])
+            dataset["last_edited_at"] = parse_datetime(dataset["last_edited_at"])
             return dataset
 
         return [
             {"dataset": DatasetInfo(**convert_dates(d.dataset)), "user_role": DatasetUserRole(d.user_role)}
             for d in data
         ]
 
@@ -640,15 +638,15 @@
                 else:
                     continue
             elif not isinstance(clause, ListingFilter):
                 continue
 
             if clause.value.endswith("before") or clause.value.endswith("after"):
                 if isinstance(val, str):
-                    val = datetime_parser.isoparse(val)
+                    val = parse_datetime(val)
                 if isinstance(val, datetime):
                     val = val.isoformat()
                 else:
                     raise ValueError(f"Value for {clause.name} filter should be a datetime")
 
             ret[clause.value] = val
```

### Comparing `encord-0.1.98/encord/utilities/client_utilities.py` & `encord-0.1.99/encord/utilities/client_utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import pprint
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Set, TypeVar, Union
 
-from dateutil import parser as datetime_parser
+from encord.common.time_parser import parse_datetime
 
 
 def pretty_print(data):
     return pprint.pformat(data, indent=4, width=10)
 
 
 class APIKeyScopes(Enum):
@@ -116,19 +116,19 @@
 
 @dataclass
 class CvatImporterError:
     dataset_hash: str
     issues: Issues
 
 
-def parse_datetime(key: str, val: Optional[Union[str, datetime]]) -> Optional[str]:
+def optional_datetime_to_iso_str(key: str, val: Optional[Union[str, datetime]]) -> Optional[str]:
     if not val:
         return None
     if isinstance(val, str):
-        return datetime_parser.isoparse(val).isoformat()
+        return parse_datetime(val).isoformat()
     if isinstance(val, datetime):
         return val.isoformat()
     else:
         raise ValueError(f"Value for {key} should be a datetime")
 
 
 T = TypeVar("T")
```

### Comparing `encord-0.1.98/encord/utilities/label_utilities.py` & `encord-0.1.99/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/encord/utilities/project_user.py` & `encord-0.1.99/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.98/pyproject.toml` & `encord-0.1.99/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.98"
+version = "0.1.99"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["encord"]
 packages = [
     { include = "encord"},
 ]
@@ -24,60 +24,42 @@
 cryptography = ">=3.4.8"
 tqdm = "^4.32.1"
 pydantic = ">=1.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pre-commit = "^3.3.0"
-black = "^23.7.0"
 sphinx-tabs = "^3.3.1"
 sphinx-autodoc-typehints = "1.15.2"
 sphinx-codeautolink = "^0.10.0"
 sphinx-copybutton = "^0.5.0"
 sphinx-toolbox = "^3.4.0"
 prettyprinter = "0.18.0"
-isort = "^5.12.0"
 pydata-sphinx-theme = "^0.8.1"
 sphinx-gallery = "^0.10.1"
 deepdiff = "^6.2.1"
 types-requests = "^2.25.0"
-pylint = "^2.17.5"
-autoflake = "^2.2.1"
-mypy = "^1.5.1"
+mypy = "^1.6.1"
 types-python-dateutil = "^2.8.19"
 types-tqdm = "^4.32.1"
 pyyaml = "^6.0.1"
-pyright = "^1.1.325"
+pyright = "^1.1.336"
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 120
-include = 'encord\/.*'
-
-[tool.isort]
-# setting isort to a compatibility mode with `black`
-# https://pycqa.github.io/isort/docs/configuration/black_compatibility.html
-profile = "black"
-
-[tool.pylint.'MASTER']
-ignore = "tests"
-
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 120
 disable = "all"
 enable = "C0123, C0200, C0209, E0401, E0602, E1101, E1205, W0611, W0621, W1309, W1404, W1514"
 
-[tool.autoflake]
-check = false
-expand-star-imports = true
-ignore-init-module-imports = true
-in-place = true
-recursive = true
-remove-all-unused-imports = true
-remove-duplicate-keys = true
-remove-unused-variables = true
-
 [tool.mypy]
 ignore_missing_imports = true
+
+[tool.ruff]
+target-version = "py38"
+line-length = 120
+extend-select = ["W", "Q", "I"]
+ignore = ["F401", "E402"]
+
+exclude = ['docs']
```

### Comparing `encord-0.1.98/PKG-INFO` & `encord-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.98
+Version: 0.1.99
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.98 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.99 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

