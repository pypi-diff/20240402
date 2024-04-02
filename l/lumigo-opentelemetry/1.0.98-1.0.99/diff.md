# Comparing `tmp/lumigo_opentelemetry-1.0.98-py3-none-any.whl.zip` & `tmp/lumigo_opentelemetry-1.0.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,105 +1,109 @@
-Zip file size: 78926 bytes, number of entries: 103
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 ci/__init__.py
--rw-r--r--  2.0 unx    14467 b- defN 23-Aug-21 13:33 ci/tested_versions_utils.py
--rw-r--r--  2.0 unx        7 b- defN 23-Aug-21 13:34 lumigo_opentelemetry/VERSION
--rw-r--r--  2.0 unx     7092 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/__init__.py
--rw-r--r--  2.0 unx     2089 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/dependencies/__init__.py
--rw-r--r--  2.0 unx      129 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/__init__.py
--rw-r--r--  2.0 unx    10112 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/__init__.py
--rw-r--r--  2.0 unx      622 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/package.py
--rw-r--r--  2.0 unx      608 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/version.py
--rw-r--r--  2.0 unx     1617 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/extensions/__init__.py
--rw-r--r--  2.0 unx    13523 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/extensions/dynamodb.py
--rw-r--r--  2.0 unx     4159 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/extensions/lmbd.py
--rw-r--r--  2.0 unx     5472 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/extensions/sqs.py
--rw-r--r--  2.0 unx     4954 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/external/botocore/extensions/types.py
--rw-r--r--  2.0 unx      976 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/__init__.py
--rw-r--r--  2.0 unx      719 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/instrumentation_utils.py
--rw-r--r--  2.0 unx     1999 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/instrumentations.py
--rw-r--r--  2.0 unx      489 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/boto/__init__.py
--rw-r--r--  2.0 unx     1178 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/botocore/__init__.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py
--rw-r--r--  2.0 unx     1286 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/fastapi/__init__.py
--rw-r--r--  2.0 unx     2237 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py
--rw-r--r--  2.0 unx      972 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/flask/__init__.py
--rw-r--r--  2.0 unx     1146 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/grpcio/__init__.py
--rw-r--r--  2.0 unx     1249 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/grpcio/common.py
--rw-r--r--  2.0 unx     2831 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_client.py
--rw-r--r--  2.0 unx     2943 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_server.py
--rw-r--r--  2.0 unx     1438 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/kafka_python/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/pika/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/pymongo/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/pymysql/__init__.py
--rw-r--r--  2.0 unx      719 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/requests/__init__.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/libs/__init__.py
--rw-r--r--  2.0 unx     2010 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/libs/general_utils.py
--rw-r--r--  2.0 unx      948 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/libs/json_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/resources/__init__.py
--rw-r--r--  2.0 unx     8250 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/resources/detectors.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/utils/__init__.py
--rw-r--r--  2.0 unx      156 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/utils/aws_utils.py
--rw-r--r--  2.0 unx      197 b- defN 23-Aug-21 13:33 lumigo_opentelemetry/utils/config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/ci/__init__.py
--rw-r--r--  2.0 unx     7385 b- defN 23-Aug-21 13:33 test/ci/test_tested_versions.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/components/__init__.py
--rw-r--r--  2.0 unx     1023 b- defN 23-Aug-21 13:33 test/components/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/components/fastapi_external_apis/__init__.py
--rw-r--r--  2.0 unx      131 b- defN 23-Aug-21 13:33 test/components/fastapi_external_apis/app.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/components/tests/__init__.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Aug-21 13:33 test/components/tests/test_attr_max_size.py
--rw-r--r--  2.0 unx     1204 b- defN 23-Aug-21 13:33 test/components/tests/test_execution_tags.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/conftest.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/boto3/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/boto3/conftest.py
--rw-r--r--  2.0 unx      460 b- defN 23-Aug-21 13:33 test/integration/boto3/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/boto3/tests/__init__.py
--rw-r--r--  2.0 unx     2425 b- defN 23-Aug-21 13:33 test/integration/boto3/tests/test_boto3.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/fastapi/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/fastapi/conftest.py
--rw-r--r--  2.0 unx      536 b- defN 23-Aug-21 13:33 test/integration/fastapi/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/fastapi/tests/__init__.py
--rw-r--r--  2.0 unx     4623 b- defN 23-Aug-21 13:33 test/integration/fastapi/tests/test_fastapi.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/flask/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/flask/conftest.py
--rw-r--r--  2.0 unx      285 b- defN 23-Aug-21 13:33 test/integration/flask/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/flask/tests/__init__.py
--rw-r--r--  2.0 unx     2560 b- defN 23-Aug-21 13:33 test/integration/flask/tests/test_flask.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/grpcio/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/grpcio/app/__init__.py
--rw-r--r--  2.0 unx     2211 b- defN 23-Aug-21 13:33 test/integration/grpcio/app/greeter_server.py
--rw-r--r--  2.0 unx     1922 b- defN 23-Aug-21 13:33 test/integration/grpcio/app/helloworld_pb2.py
--rw-r--r--  2.0 unx     7290 b- defN 23-Aug-21 13:33 test/integration/grpcio/app/helloworld_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/grpcio/tests/__init__.py
--rw-r--r--  2.0 unx     5270 b- defN 23-Aug-21 13:33 test/integration/grpcio/tests/test_grpcio.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/kafka_python/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/kafka_python/conftest.py
--rw-r--r--  2.0 unx     1661 b- defN 23-Aug-21 13:33 test/integration/kafka_python/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/kafka_python/tests/__init__.py
--rw-r--r--  2.0 unx     2904 b- defN 23-Aug-21 13:33 test/integration/kafka_python/tests/test_kafka_python.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/pika/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/pika/conftest.py
--rw-r--r--  2.0 unx     2442 b- defN 23-Aug-21 13:33 test/integration/pika/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/pika/tests/__init__.py
--rw-r--r--  2.0 unx     2842 b- defN 23-Aug-21 13:33 test/integration/pika/tests/test_pika.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/pymongo/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/pymongo/conftest.py
--rw-r--r--  2.0 unx      795 b- defN 23-Aug-21 13:33 test/integration/pymongo/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/pymongo/tests/__init__.py
--rw-r--r--  2.0 unx     1281 b- defN 23-Aug-21 13:33 test/integration/pymongo/tests/test_pymongo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/pymysql/__init__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-21 13:33 test/integration/pymysql/conftest.py
--rw-r--r--  2.0 unx      277 b- defN 23-Aug-21 13:33 test/integration/pymysql/app/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/integration/pymysql/tests/__init__.py
--rw-r--r--  2.0 unx      887 b- defN 23-Aug-21 13:33 test/integration/pymysql/tests/test_pymysql.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 13:33 test/test_utils/__init__.py
--rw-r--r--  2.0 unx     2412 b- defN 23-Aug-21 13:33 test/test_utils/spans_parser.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-21 13:34 lumigo_opentelemetry-1.0.98.dist-info/LICENSE
--rw-r--r--  2.0 unx    21605 b- defN 23-Aug-21 13:34 lumigo_opentelemetry-1.0.98.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-21 13:34 lumigo_opentelemetry-1.0.98.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Aug-21 13:34 lumigo_opentelemetry-1.0.98.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       29 b- defN 23-Aug-21 13:34 lumigo_opentelemetry-1.0.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    10193 b- defN 23-Aug-21 13:34 lumigo_opentelemetry-1.0.98.dist-info/RECORD
-103 files, 206058 bytes uncompressed, 62092 bytes compressed:  69.9%
+Zip file size: 80820 bytes, number of entries: 107
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 ci/__init__.py
+-rw-r--r--  2.0 unx    14467 b- defN 23-Aug-23 05:34 ci/tested_versions_utils.py
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-23 05:35 lumigo_opentelemetry/VERSION
+-rw-r--r--  2.0 unx     7092 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/__init__.py
+-rw-r--r--  2.0 unx     2089 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/dependencies/__init__.py
+-rw-r--r--  2.0 unx      129 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/__init__.py
+-rw-r--r--  2.0 unx    10112 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/__init__.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/package.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/version.py
+-rw-r--r--  2.0 unx     1617 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/extensions/__init__.py
+-rw-r--r--  2.0 unx    13523 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/extensions/dynamodb.py
+-rw-r--r--  2.0 unx     4159 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/extensions/lmbd.py
+-rw-r--r--  2.0 unx     5472 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/extensions/sqs.py
+-rw-r--r--  2.0 unx     4954 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/external/botocore/extensions/types.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/__init__.py
+-rw-r--r--  2.0 unx      719 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/instrumentation_utils.py
+-rw-r--r--  2.0 unx     2077 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/instrumentations.py
+-rw-r--r--  2.0 unx      489 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/boto/__init__.py
+-rw-r--r--  2.0 unx     1178 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/botocore/__init__.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py
+-rw-r--r--  2.0 unx     1286 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/fastapi/__init__.py
+-rw-r--r--  2.0 unx     2237 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py
+-rw-r--r--  2.0 unx      972 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/flask/__init__.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/grpcio/__init__.py
+-rw-r--r--  2.0 unx     1249 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/grpcio/common.py
+-rw-r--r--  2.0 unx     2831 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_client.py
+-rw-r--r--  2.0 unx     2943 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_server.py
+-rw-r--r--  2.0 unx     1438 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/kafka_python/__init__.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/pika/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/pymongo/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/pymysql/__init__.py
+-rw-r--r--  2.0 unx     1254 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/redis/__init__.py
+-rw-r--r--  2.0 unx      719 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/requests/__init__.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/libs/__init__.py
+-rw-r--r--  2.0 unx     2010 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/libs/general_utils.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/libs/json_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/resources/__init__.py
+-rw-r--r--  2.0 unx     8250 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/resources/detectors.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/utils/__init__.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/utils/aws_utils.py
+-rw-r--r--  2.0 unx      197 b- defN 23-Aug-23 05:34 lumigo_opentelemetry/utils/config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/ci/__init__.py
+-rw-r--r--  2.0 unx     7385 b- defN 23-Aug-23 05:34 test/ci/test_tested_versions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/components/__init__.py
+-rw-r--r--  2.0 unx     1023 b- defN 23-Aug-23 05:34 test/components/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/components/fastapi_external_apis/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Aug-23 05:34 test/components/fastapi_external_apis/app.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/components/tests/__init__.py
+-rw-r--r--  2.0 unx     1357 b- defN 23-Aug-23 05:34 test/components/tests/test_attr_max_size.py
+-rw-r--r--  2.0 unx     1204 b- defN 23-Aug-23 05:34 test/components/tests/test_execution_tags.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/conftest.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/boto3/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/boto3/conftest.py
+-rw-r--r--  2.0 unx      460 b- defN 23-Aug-23 05:34 test/integration/boto3/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/boto3/tests/__init__.py
+-rw-r--r--  2.0 unx     2425 b- defN 23-Aug-23 05:34 test/integration/boto3/tests/test_boto3.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/fastapi/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/fastapi/conftest.py
+-rw-r--r--  2.0 unx      536 b- defN 23-Aug-23 05:34 test/integration/fastapi/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/fastapi/tests/__init__.py
+-rw-r--r--  2.0 unx     4623 b- defN 23-Aug-23 05:34 test/integration/fastapi/tests/test_fastapi.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/flask/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/flask/conftest.py
+-rw-r--r--  2.0 unx      285 b- defN 23-Aug-23 05:34 test/integration/flask/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/flask/tests/__init__.py
+-rw-r--r--  2.0 unx     2560 b- defN 23-Aug-23 05:34 test/integration/flask/tests/test_flask.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/grpcio/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/grpcio/app/__init__.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-Aug-23 05:34 test/integration/grpcio/app/greeter_server.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-Aug-23 05:34 test/integration/grpcio/app/helloworld_pb2.py
+-rw-r--r--  2.0 unx     7290 b- defN 23-Aug-23 05:34 test/integration/grpcio/app/helloworld_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/grpcio/tests/__init__.py
+-rw-r--r--  2.0 unx     5270 b- defN 23-Aug-23 05:34 test/integration/grpcio/tests/test_grpcio.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/kafka_python/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/kafka_python/conftest.py
+-rw-r--r--  2.0 unx     1661 b- defN 23-Aug-23 05:34 test/integration/kafka_python/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/kafka_python/tests/__init__.py
+-rw-r--r--  2.0 unx     2904 b- defN 23-Aug-23 05:34 test/integration/kafka_python/tests/test_kafka_python.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/pika/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/pika/conftest.py
+-rw-r--r--  2.0 unx     2442 b- defN 23-Aug-23 05:34 test/integration/pika/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/pika/tests/__init__.py
+-rw-r--r--  2.0 unx     2842 b- defN 23-Aug-23 05:34 test/integration/pika/tests/test_pika.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/pymongo/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/pymongo/conftest.py
+-rw-r--r--  2.0 unx      795 b- defN 23-Aug-23 05:34 test/integration/pymongo/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/pymongo/tests/__init__.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-Aug-23 05:34 test/integration/pymongo/tests/test_pymongo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/pymysql/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-23 05:34 test/integration/pymysql/conftest.py
+-rw-r--r--  2.0 unx      277 b- defN 23-Aug-23 05:34 test/integration/pymysql/app/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/pymysql/tests/__init__.py
+-rw-r--r--  2.0 unx      887 b- defN 23-Aug-23 05:34 test/integration/pymysql/tests/test_pymysql.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/redis/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/integration/redis/tests/__init__.py
+-rw-r--r--  2.0 unx     1994 b- defN 23-Aug-23 05:34 test/integration/redis/tests/test_redis.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-23 05:34 test/test_utils/__init__.py
+-rw-r--r--  2.0 unx     2412 b- defN 23-Aug-23 05:34 test/test_utils/spans_parser.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-23 05:35 lumigo_opentelemetry-1.0.99.dist-info/LICENSE
+-rw-r--r--  2.0 unx    21667 b- defN 23-Aug-23 05:35 lumigo_opentelemetry-1.0.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-23 05:35 lumigo_opentelemetry-1.0.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Aug-23 05:35 lumigo_opentelemetry-1.0.99.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       29 b- defN 23-Aug-23 05:35 lumigo_opentelemetry-1.0.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    10586 b- defN 23-Aug-23 05:35 lumigo_opentelemetry-1.0.99.dist-info/RECORD
+107 files, 209843 bytes uncompressed, 63340 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -87,14 +87,17 @@
 
 Filename: lumigo_opentelemetry/instrumentations/pymongo/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/instrumentations/pymysql/__init__.py
 Comment: 
 
+Filename: lumigo_opentelemetry/instrumentations/redis/__init__.py
+Comment: 
+
 Filename: lumigo_opentelemetry/instrumentations/requests/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py
 Comment: 
 
 Filename: lumigo_opentelemetry/libs/__init__.py
@@ -279,32 +282,41 @@
 
 Filename: test/integration/pymysql/tests/__init__.py
 Comment: 
 
 Filename: test/integration/pymysql/tests/test_pymysql.py
 Comment: 
 
+Filename: test/integration/redis/__init__.py
+Comment: 
+
+Filename: test/integration/redis/tests/__init__.py
+Comment: 
+
+Filename: test/integration/redis/tests/test_redis.py
+Comment: 
+
 Filename: test/test_utils/__init__.py
 Comment: 
 
 Filename: test/test_utils/spans_parser.py
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.98.dist-info/LICENSE
+Filename: lumigo_opentelemetry-1.0.99.dist-info/LICENSE
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.98.dist-info/METADATA
+Filename: lumigo_opentelemetry-1.0.99.dist-info/METADATA
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.98.dist-info/WHEEL
+Filename: lumigo_opentelemetry-1.0.99.dist-info/WHEEL
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.98.dist-info/entry_points.txt
+Filename: lumigo_opentelemetry-1.0.99.dist-info/entry_points.txt
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.98.dist-info/top_level.txt
+Filename: lumigo_opentelemetry-1.0.99.dist-info/top_level.txt
 Comment: 
 
-Filename: lumigo_opentelemetry-1.0.98.dist-info/RECORD
+Filename: lumigo_opentelemetry-1.0.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lumigo_opentelemetry/VERSION

```diff
@@ -1 +1 @@
-1.0.98
+1.0.99
```

## lumigo_opentelemetry/instrumentations/instrumentations.py

```diff
@@ -11,27 +11,29 @@
 from .flask import instrumentor as flask_instrumentor
 from .grpcio import instrumentor as grpc_instrumentor
 from .kafka_python import instrumentor as kafka_python_instrumentor
 from .pika import instrumentor as pika_instrumentor
 from .pymongo import instrumentor as pymongo_instrumentor
 from .pymysql import instrumentor as pymysql_instrumentor
 from .requests import instrumentor as requests_instrumentor
+from .redis import instrumentor as redis_instrumentor
 
 installed_instrumentations: List[str] = []
 instrumentors: List[AbstractInstrumentor] = [
     boto_instrumentor,
     botocore_instrumentor,
     fastapi_instrumentor,
     flask_instrumentor,
     grpc_instrumentor,
     kafka_python_instrumentor,
     pika_instrumentor,
     pymongo_instrumentor,
     pymysql_instrumentor,
     requests_instrumentor,
+    redis_instrumentor,
 ]
 for instrumentor in instrumentors:
     try:
         instrumentor.check_if_applicable()
     except ImportError:
         continue
```

## test/components/tests/test_attr_max_size.py

```diff
@@ -32,9 +32,9 @@
         children = spans_container.get_non_internal_children()
         self.assertEqual(1, len(children))
         child_attributes = children[0]["attributes"]
         self.assert_attribute_length(child_attributes, 1)
 
     def assert_attribute_length(self, child_attributes: dict, length: int) -> None:
         for k, v in child_attributes.items():
-            if type(v) == str:
+            if isinstance(v, str):
                 assert len(v) == length
```

## Comparing `lumigo_opentelemetry-1.0.98.dist-info/LICENSE` & `lumigo_opentelemetry-1.0.99.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lumigo_opentelemetry-1.0.98.dist-info/METADATA` & `lumigo_opentelemetry-1.0.99.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumigo-opentelemetry
-Version: 1.0.98
+Version: 1.0.99
 Summary: Lumigo OpenTelemetry Distribution for Python
 Home-page: https://github.com/lumigo-io/opentelemetry-python-distro
 Author: Lumigo LTD (https://lumigo.io)
 Author-email: support@lumigo.io
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/lumigo-io/opentelemetry-python-distro/issues
 Platform: UNKNOWN
@@ -30,14 +30,15 @@
 Requires-Dist: opentelemetry-instrumentation-flask (==0.36b0)
 Requires-Dist: opentelemetry-instrumentation-grpc (==0.36b0)
 Requires-Dist: opentelemetry-instrumentation-kafka-python (==0.36b0)
 Requires-Dist: opentelemetry-instrumentation-pika (==0.36b0)
 Requires-Dist: opentelemetry-instrumentation-pymongo (==0.36b0)
 Requires-Dist: opentelemetry-instrumentation-pymysql (==0.36b0)
 Requires-Dist: opentelemetry-instrumentation-requests (==0.36b0)
+Requires-Dist: opentelemetry-instrumentation-redis (==0.36b0)
 
 # Lumigo OpenTelemetry Distro for Python :stars:
 
 [![Tracer Testing](https://github.com/lumigo-io/opentelemetry-python-distro/actions/workflows/push-actions.yml/badge.svg)](https://github.com/lumigo-io/opentelemetry-python-distro/actions/workflows/push-actions.yml)
 ![Version](https://badge.fury.io/py/lumigo_opentelemetry.svg)
 
 The Lumigo OpenTelemetry Distribution for Python is a package that provides no-code distributed tracing for containerized applications.
```

## Comparing `lumigo_opentelemetry-1.0.98.dist-info/RECORD` & `lumigo_opentelemetry-1.0.99.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 ci/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ci/tested_versions_utils.py,sha256=1BZdsu2oQTZCLcbWCCVGE7qQUf1hUaziPcQjctc03oU,14467
-lumigo_opentelemetry/VERSION,sha256=txRS4xEaHNWzjzsBV3gYCIn_zUkFg6AJXvb9cz5Xk64,7
+lumigo_opentelemetry/VERSION,sha256=EhCEDjvtcAiT_niPS1IFySOFEWm8mUEcLUdYEVaHaUY,7
 lumigo_opentelemetry/__init__.py,sha256=JtebPnMRuIjRn1c_TSzhl1YHUeuG3PCGYnt8JT_u684,7092
 lumigo_opentelemetry/dependencies/__init__.py,sha256=AJLmzofXEez21Yiq8YNit4VccNUkmSSpdrO-CLyyqlI,2089
 lumigo_opentelemetry/external/__init__.py,sha256=b_diXhRyW-W_Lr8dRLIhn3PZVtTvPdQgoNa2chqTgGE,129
 lumigo_opentelemetry/external/botocore/__init__.py,sha256=tbqRMfUKknQI-vK_YnCOstXfc0Bw2Wq846CAzNX7_Sk,10112
 lumigo_opentelemetry/external/botocore/package.py,sha256=6xvfRpU_C3wlSO6pto7MhGtkPoCHDEiRO_Fh4DiC_50,622
 lumigo_opentelemetry/external/botocore/version.py,sha256=0aVi6CQVN6owJvia58MfV2U7QDhpcdEvHlvDAZMJt9M,608
 lumigo_opentelemetry/external/botocore/extensions/__init__.py,sha256=w9ZW1Lz9cHAHoKoZBLJU9IMURpxJymwVX4xXPzEj0Ro,1617
 lumigo_opentelemetry/external/botocore/extensions/dynamodb.py,sha256=qvoprNdCV_CxBQH1YC2hTrhN4i7YlPKMou8xzOuNYfc,13523
 lumigo_opentelemetry/external/botocore/extensions/lmbd.py,sha256=vL08WGSdl71cmb6vniJThhqOq_l7G1QkeAc5ymQ-S9E,4159
 lumigo_opentelemetry/external/botocore/extensions/sqs.py,sha256=aK-d_S7qhYeMSe-pOc60euZh-WcQqXspUHJiicUwIKk,5472
 lumigo_opentelemetry/external/botocore/extensions/types.py,sha256=MpZ3UT7SUHs-o54iPZobvaL0Os1Urb6M4PdFAVYgQ7o,4954
 lumigo_opentelemetry/instrumentations/__init__.py,sha256=uehRQj1ACn1cCs2-wMafgEIvu66mmAH1Lp6em2xrG3g,976
 lumigo_opentelemetry/instrumentations/instrumentation_utils.py,sha256=EwvBLzfV519ugpBwG3HTFXhRrbKoOlDiMwq_ILcp9Dk,719
-lumigo_opentelemetry/instrumentations/instrumentations.py,sha256=1Vs3UKXxlFLO1rslCZeIaAUBgJilDS1P13DmT35MjNM,1999
+lumigo_opentelemetry/instrumentations/instrumentations.py,sha256=3Ay_NZZ5bWBAqcbVRsYsKTdfnm5LOMb6cXvbihMBlG4,2077
 lumigo_opentelemetry/instrumentations/boto/__init__.py,sha256=nRDuKDpjW8s8rOUWhO0B61-TVzMCnc8xSdhzSkgewT0,489
 lumigo_opentelemetry/instrumentations/botocore/__init__.py,sha256=E1LzQl998TeQn5cmFnnk_SXU2onKKgJJCl_Iw8OCyB8,1178
 lumigo_opentelemetry/instrumentations/botocore/parsers/__init__.py,sha256=iFCrXomSIRVo1oCG-KjDNyv8lIiOFcOvpL5x1qEwGqg,6194
 lumigo_opentelemetry/instrumentations/fastapi/__init__.py,sha256=GhpbMaRRN3u7IeU8wF60_vD_tWiRc7PHRNuEC87Cp50,1286
 lumigo_opentelemetry/instrumentations/fastapi/parsers/__init__.py,sha256=ZvQsBiY_IkgLGqvMjviwwQZ83VwYfmDXaECw299x8MI,2237
 lumigo_opentelemetry/instrumentations/flask/__init__.py,sha256=kBrV0sAd5Bh2KgRBhIZ3-oR7sKEm7UASoMhEpHLU03E,972
 lumigo_opentelemetry/instrumentations/grpcio/__init__.py,sha256=1R1RNuLTyhoy_Q6Zk2m45A0Ca4CBbOtRB6Vw4iNtWwk,1146
 lumigo_opentelemetry/instrumentations/grpcio/common.py,sha256=rKOpHJuMUGat3QRVrv_1HtesuJaqhemTVp9D-tD_ym4,1249
 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_client.py,sha256=AR16FVQNZgsMa8SJNoJpIPWJNyohKZ6N13qIRTdiL7g,2831
 lumigo_opentelemetry/instrumentations/grpcio/grpc_instrument_server.py,sha256=Hwhzz696lxyvdwp94V1w9bcRfuo4b2Dsqz7m193tH_g,2943
 lumigo_opentelemetry/instrumentations/kafka_python/__init__.py,sha256=Mr2ieOyVYnwzY-_efZO0TInCqSIdy8rUEtppAA40PPY,1438
 lumigo_opentelemetry/instrumentations/pika/__init__.py,sha256=9AZCXy9YxmHgS336nx9B2c5EoKStoKK2WH36M76Qggo,1066
 lumigo_opentelemetry/instrumentations/pymongo/__init__.py,sha256=dojEYX79c0sPN7XrmEQfa9zqvrOptf1p6F_jHUp6Pqg,496
 lumigo_opentelemetry/instrumentations/pymysql/__init__.py,sha256=szPK7IayZ9OHof-xsNCVH2G0PybbKUgjh7CR-Iisqgk,496
+lumigo_opentelemetry/instrumentations/redis/__init__.py,sha256=kRCKZ7Z32yNTvR3aGWbHZPQP4aWSNhcSrna2fxp5k8k,1254
 lumigo_opentelemetry/instrumentations/requests/__init__.py,sha256=VSwfZ27du4BerZUBrzCMntxcjeK7tGjSLprG0f-UkoI,719
 lumigo_opentelemetry/instrumentations/requests/parsers/__init__.py,sha256=ztp7eoG-uF9_vr5_0UkfqkOJqS3mMCKuN0lS0I9alJs,2325
 lumigo_opentelemetry/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lumigo_opentelemetry/libs/general_utils.py,sha256=Tmnehzd5m-UPIr0jMdmigo9PCRwpQREoc3rU4SX_Hlo,2010
 lumigo_opentelemetry/libs/json_utils.py,sha256=JoTwFP-a6NPXWilAve5n-BlzPvuQgqAHitLD9gK7Mbc,948
 lumigo_opentelemetry/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lumigo_opentelemetry/resources/detectors.py,sha256=FJzdEi4KVfZFxWgjeyxBEXWT2rPuWIGEmBFnf7ip14E,8250
@@ -43,15 +44,15 @@
 test/ci/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/ci/test_tested_versions.py,sha256=vZpfaIJX3et4NHsIWqiVjMoV6ljgx_4wPlEI4oUzAa0,7385
 test/components/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/components/app/__init__.py,sha256=XtOkzzEI13at4wdtlcglBJ7Q8iHLz3ILdlzjfc_SHsY,1023
 test/components/fastapi_external_apis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/components/fastapi_external_apis/app.py,sha256=rKBB0Q_TiUJoNpNFvvdPjnXW7NKJm6u2Hf9IaRdPlgQ,131
 test/components/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test/components/tests/test_attr_max_size.py,sha256=qlmBztvaC2y0KhCd6ctm2zd9-T1LPf4xTec8ThUsXCo,1353
+test/components/tests/test_attr_max_size.py,sha256=4Ac3hEOWzOw0y1VVHMe_ay5EEouNiMdvkDSdMoFjsAc,1357
 test/components/tests/test_execution_tags.py,sha256=9xMJKZ5Fd-QnwNOmGponUoG8_Ek1yPkyjCcud-Z58p4,1204
 test/integration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/integration/conftest.py,sha256=xKSb_VbrDakoumLC-ZyNNSu3M-OXGNTJQtKtEZzLwRQ,171
 test/integration/boto3/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/integration/boto3/conftest.py,sha256=xKSb_VbrDakoumLC-ZyNNSu3M-OXGNTJQtKtEZzLwRQ,171
 test/integration/boto3/app/__init__.py,sha256=LQ5XVDmlkBtOfVmqV2t2yORsxEITbSZHHt7_PcvtDFs,460
 test/integration/boto3/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -89,15 +90,18 @@
 test/integration/pymongo/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/integration/pymongo/tests/test_pymongo.py,sha256=bAseNx7aTLynnSv4iiVyJh8ioaCcc9H6etzXs-a8Xu0,1281
 test/integration/pymysql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/integration/pymysql/conftest.py,sha256=xKSb_VbrDakoumLC-ZyNNSu3M-OXGNTJQtKtEZzLwRQ,171
 test/integration/pymysql/app/__init__.py,sha256=DxI7YNhpihPkcSM2g6xEju0PLwYbb1HxPrw-ooxjIQk,277
 test/integration/pymysql/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/integration/pymysql/tests/test_pymysql.py,sha256=cOG-v1LwAAwE18WwfJM1J4vYCnkdkpLWZRs8RaBiumA,887
+test/integration/redis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+test/integration/redis/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+test/integration/redis/tests/test_redis.py,sha256=qlZknKbQhDpBrTbmep926yXWyrrcQVNbDie-EP8TT2o,1994
 test/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_utils/spans_parser.py,sha256=6YeKvfbAdH6hSY85pCjE85Cxac7jeew_EaWV8fs7ppY,2412
-lumigo_opentelemetry-1.0.98.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-lumigo_opentelemetry-1.0.98.dist-info/METADATA,sha256=rkDWklcw26srJ6eztDj74mX0t5b7O_dFAzySUrBzhSk,21605
-lumigo_opentelemetry-1.0.98.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-lumigo_opentelemetry-1.0.98.dist-info/entry_points.txt,sha256=ylawlrv1CUnt8PQed8NYSHsMi_KOj5q8lkb9WPKqXMU,64
-lumigo_opentelemetry-1.0.98.dist-info/top_level.txt,sha256=yheMbVr4dp39_04tHKbNcmqdpVtRKVOk3XilKaB8orw,29
-lumigo_opentelemetry-1.0.98.dist-info/RECORD,,
+lumigo_opentelemetry-1.0.99.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+lumigo_opentelemetry-1.0.99.dist-info/METADATA,sha256=HGC1TNZlQOaIQJyZWXwHFv0Y55TcryoS7f5-OCVp9js,21667
+lumigo_opentelemetry-1.0.99.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+lumigo_opentelemetry-1.0.99.dist-info/entry_points.txt,sha256=ylawlrv1CUnt8PQed8NYSHsMi_KOj5q8lkb9WPKqXMU,64
+lumigo_opentelemetry-1.0.99.dist-info/top_level.txt,sha256=yheMbVr4dp39_04tHKbNcmqdpVtRKVOk3XilKaB8orw,29
+lumigo_opentelemetry-1.0.99.dist-info/RECORD,,
```

