# Comparing `tmp/friendli_client-1.3.3.tar.gz` & `tmp/friendli_client-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendli_client-1.3.3.tar", max compression
+gzip compressed data, was "friendli_client-1.3.4.tar", max compression
```

## Comparing `friendli_client-1.3.3.tar` & `friendli_client-1.3.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0    10173 2024-03-23 07:44:00.431260 friendli_client-1.3.3/LICENSE
--rw-r--r--   0        0        0     6417 2024-04-01 05:27:02.865670 friendli_client-1.3.3/README.md
--rw-r--r--   0        0        0      615 2024-03-23 07:44:00.431488 friendli_client-1.3.3/friendli/__init__.py
--rw-r--r--   0        0        0     5840 2024-03-23 07:45:31.687903 friendli_client-1.3.3/friendli/auth.py
--rw-r--r--   0        0        0      188 2024-03-23 07:44:00.431696 friendli_client-1.3.3/friendli/cli/__init__.py
--rw-r--r--   0        0        0      628 2024-03-23 07:44:00.431779 friendli_client-1.3.3/friendli/cli/api/__init__.py
--rw-r--r--   0        0        0     5374 2024-03-23 07:45:31.688080 friendli_client-1.3.3/friendli/cli/api/chat_completions.py
--rw-r--r--   0        0        0     4513 2024-03-23 07:45:31.688225 friendli_client-1.3.3/friendli/cli/api/completions.py
--rw-r--r--   0        0        0     3058 2024-03-23 07:44:00.432077 friendli_client-1.3.3/friendli/cli/api/text_to_image.py
--rw-r--r--   0        0        0     4424 2024-03-23 07:45:31.688350 friendli_client-1.3.3/friendli/cli/endpoint.py
--rw-r--r--   0        0        0     3572 2024-04-01 05:27:02.865992 friendli_client-1.3.3/friendli/cli/login.py
--rw-r--r--   0        0        0     5150 2024-03-23 07:45:31.697680 friendli_client-1.3.3/friendli/cli/main.py
--rw-r--r--   0        0        0    13640 2024-04-01 05:27:02.866334 friendli_client-1.3.3/friendli/cli/model.py
--rw-r--r--   0        0        0     2727 2024-03-23 07:45:31.688685 friendli_client-1.3.3/friendli/cli/project.py
--rw-r--r--   0        0        0     2074 2024-03-23 07:45:31.688798 friendli_client-1.3.3/friendli/cli/team.py
--rw-r--r--   0        0        0      125 2024-03-23 07:44:00.432644 friendli_client-1.3.3/friendli/client/__init__.py
--rw-r--r--   0        0        0      133 2024-03-23 07:44:00.432730 friendli_client-1.3.3/friendli/client/graphql/__init__.py
--rw-r--r--   0        0        0     4089 2024-03-28 02:42:37.445063 friendli_client-1.3.3/friendli/client/graphql/base.py
--rw-r--r--   0        0        0     6510 2024-03-23 07:45:31.689104 friendli_client-1.3.3/friendli/client/graphql/endpoint.py
--rw-r--r--   0        0        0      791 2024-03-23 07:45:31.689199 friendli_client-1.3.3/friendli/client/graphql/model.py
--rw-r--r--   0        0        0     1014 2024-03-23 07:45:31.689334 friendli_client-1.3.3/friendli/client/graphql/team.py
--rw-r--r--   0        0        0     1914 2024-03-23 07:45:31.689457 friendli_client-1.3.3/friendli/client/graphql/user.py
--rw-r--r--   0        0        0       88 2024-03-23 07:44:00.433180 friendli_client-1.3.3/friendli/client/http/__init__.py
--rw-r--r--   0        0        0    14158 2024-03-23 07:44:00.433245 friendli_client-1.3.3/friendli/client/http/base.py
--rw-r--r--   0        0        0      977 2024-03-23 07:45:31.689581 friendli_client-1.3.3/friendli/client/http/login.py
--rw-r--r--   0        0        0     1567 2024-03-23 07:45:31.689696 friendli_client-1.3.3/friendli/context.py
--rw-r--r--   0        0        0      104 2024-03-23 07:44:00.433476 friendli_client-1.3.3/friendli/di/__init__.py
--rw-r--r--   0        0        0     1507 2024-03-23 07:44:00.433535 friendli_client-1.3.3/friendli/di/injector.py
--rw-r--r--   0        0        0      620 2024-03-23 07:44:00.433592 friendli_client-1.3.3/friendli/di/modules.py
--rw-r--r--   0        0        0     1132 2024-04-01 05:27:02.855212 friendli_client-1.3.3/friendli/enums.py
--rw-r--r--   0        0        0     6853 2024-03-23 07:44:00.433757 friendli_client-1.3.3/friendli/errors.py
--rw-r--r--   0        0        0     9607 2024-03-23 07:45:31.689953 friendli_client-1.3.3/friendli/formatter.py
--rw-r--r--   0        0        0     1728 2024-03-23 07:44:00.433885 friendli_client-1.3.3/friendli/logging.py
--rw-r--r--   0        0        0       92 2024-03-23 07:44:00.433966 friendli_client-1.3.3/friendli/modules/__init__.py
--rw-r--r--   0        0        0      100 2024-04-01 05:27:02.866577 friendli_client-1.3.3/friendli/modules/converter/__init__.py
--rw-r--r--   0        0        0    19437 2024-04-01 05:27:02.880294 friendli_client-1.3.3/friendli/modules/converter/base.py
--rw-r--r--   0        0        0     9527 2024-04-01 05:27:02.867303 friendli_client-1.3.3/friendli/modules/converter/convert.py
--rw-r--r--   0        0        0     5642 2024-04-01 05:27:02.867676 friendli_client-1.3.3/friendli/modules/converter/interface.py
--rw-r--r--   0        0        0     5154 2024-04-01 05:27:02.880632 friendli_client-1.3.3/friendli/modules/converter/maps.py
--rw-r--r--   0        0        0    21332 2024-03-23 07:44:00.434590 friendli_client-1.3.3/friendli/modules/converter/models/blenderbot.py
--rw-r--r--   0        0        0    11658 2024-03-23 07:44:00.434754 friendli_client-1.3.3/friendli/modules/converter/models/bloom.py
--rw-r--r--   0        0        0    10057 2024-03-23 07:44:00.434840 friendli_client-1.3.3/friendli/modules/converter/models/codegen.py
--rw-r--r--   0        0        0    12677 2024-03-23 07:44:00.434944 friendli_client-1.3.3/friendli/modules/converter/models/falcon.py
--rw-r--r--   0        0        0    10036 2024-03-23 07:44:00.435022 friendli_client-1.3.3/friendli/modules/converter/models/gpt2.py
--rw-r--r--   0        0        0    13562 2024-03-23 07:44:00.435075 friendli_client-1.3.3/friendli/modules/converter/models/gpt_neox.py
--rw-r--r--   0        0        0    17772 2024-03-23 07:45:31.681200 friendli_client-1.3.3/friendli/modules/converter/models/gptj.py
--rw-r--r--   0        0        0    21030 2024-04-01 05:27:02.880954 friendli_client-1.3.3/friendli/modules/converter/models/llama.py
--rw-r--r--   0        0        0     4497 2024-04-01 05:27:02.881269 friendli_client-1.3.3/friendli/modules/converter/models/mistral.py
--rw-r--r--   0        0        0     9076 2024-03-23 07:44:00.435422 friendli_client-1.3.3/friendli/modules/converter/models/mixtral.py
--rw-r--r--   0        0        0    16219 2024-03-23 07:45:31.690394 friendli_client-1.3.3/friendli/modules/converter/models/mpt.py
--rw-r--r--   0        0        0    12005 2024-03-23 07:44:00.435561 friendli_client-1.3.3/friendli/modules/converter/models/opt.py
--rw-r--r--   0        0        0    14295 2024-03-23 07:44:00.435615 friendli_client-1.3.3/friendli/modules/converter/models/phi_msft.py
--rw-r--r--   0        0        0    18719 2024-03-23 07:45:31.690533 friendli_client-1.3.3/friendli/modules/converter/models/t5.py
--rw-r--r--   0        0        0     8572 2024-04-01 05:27:02.856275 friendli_client-1.3.3/friendli/modules/converter/saver.py
--rw-r--r--   0        0        0      897 2024-04-01 05:27:02.868163 friendli_client-1.3.3/friendli/modules/converter/schema.py
--rw-r--r--   0        0        0     8859 2024-04-01 05:27:02.868604 friendli_client-1.3.3/friendli/modules/converter/utils.py
--rw-r--r--   0        0        0      100 2024-04-01 05:27:02.868880 friendli_client-1.3.3/friendli/modules/quantizer/__init__.py
--rw-r--r--   0        0        0      104 2024-04-01 05:27:02.869198 friendli_client-1.3.3/friendli/modules/quantizer/awq/__init__.py
--rw-r--r--   0        0        0    19257 2024-03-29 06:31:13.323145 friendli_client-1.3.3/friendli/modules/quantizer/awq/base.py
--rw-r--r--   0        0        0     7090 2024-03-23 07:45:31.691153 friendli_client-1.3.3/friendli/modules/quantizer/awq/models/gpt_neox.py
--rw-r--r--   0        0        0     5917 2024-03-23 07:45:31.691329 friendli_client-1.3.3/friendli/modules/quantizer/awq/models/gptj.py
--rw-r--r--   0        0        0    10738 2024-03-23 07:44:00.436552 friendli_client-1.3.3/friendli/modules/quantizer/awq/models/llama.py
--rw-r--r--   0        0        0     6606 2024-03-23 07:45:31.691500 friendli_client-1.3.3/friendli/modules/quantizer/awq/models/mpt.py
--rw-r--r--   0        0        0     7764 2024-03-23 07:44:00.436774 friendli_client-1.3.3/friendli/modules/quantizer/awq/utils.py
--rw-r--r--   0        0        0    17760 2024-04-01 05:27:02.875306 friendli_client-1.3.3/friendli/modules/quantizer/base.py
--rw-r--r--   0        0        0     3410 2024-03-29 06:31:13.323701 friendli_client-1.3.3/friendli/modules/quantizer/layers.py
--rw-r--r--   0        0        0     4317 2024-04-01 05:27:02.875674 friendli_client-1.3.3/friendli/modules/quantizer/maps.py
--rw-r--r--   0        0        0     3043 2024-04-01 05:27:02.875967 friendli_client-1.3.3/friendli/modules/quantizer/models/llama.py
--rw-r--r--   0        0        0     3212 2024-04-01 05:27:02.876235 friendli_client-1.3.3/friendli/modules/quantizer/models/mixtral.py
--rw-r--r--   0        0        0     2734 2024-04-01 05:27:02.876417 friendli_client-1.3.3/friendli/modules/quantizer/models/mpt.py
--rw-r--r--   0        0        0      107 2024-04-01 05:27:02.869544 friendli_client-1.3.3/friendli/modules/quantizer/schema/__init__.py
--rw-r--r--   0        0        0     2270 2024-04-01 05:27:02.876584 friendli_client-1.3.3/friendli/modules/quantizer/schema/config.py
--rw-r--r--   0        0        0     2798 2024-04-01 05:27:02.869949 friendli_client-1.3.3/friendli/modules/quantizer/schema/data.py
--rw-r--r--   0        0        0      112 2024-04-01 05:27:02.870119 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/__init__.py
--rw-r--r--   0        0        0    24897 2024-03-29 06:31:13.324766 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/base.py
--rw-r--r--   0        0        0     7496 2024-03-23 07:44:00.437677 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/bloom.py
--rw-r--r--   0        0        0     8777 2024-03-23 07:44:00.437822 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/codegen.py
--rw-r--r--   0        0        0    10437 2024-03-23 07:44:00.437905 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/falcon.py
--rw-r--r--   0        0        0     5466 2024-03-23 07:44:00.438023 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/gpt2.py
--rw-r--r--   0        0        0     9062 2024-03-23 07:44:00.438118 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/gpt_neox.py
--rw-r--r--   0        0        0     6961 2024-03-23 07:44:00.438231 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/gptj.py
--rw-r--r--   0        0        0     9431 2024-03-23 07:44:00.438321 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/llama.py
--rw-r--r--   0        0        0     5290 2024-03-23 07:44:00.438456 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/mpt.py
--rw-r--r--   0        0        0     5231 2024-03-23 07:44:00.438570 friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/opt.py
--rw-r--r--   0        0        0    16812 2024-03-29 06:31:13.325448 friendli_client-1.3.3/friendli/modules/quantizer/utils.py
--rw-r--r--   0        0        0        0 2024-03-23 07:44:00.438713 friendli_client-1.3.3/friendli/py.typed
--rw-r--r--   0        0        0       92 2024-03-23 07:44:00.438851 friendli_client-1.3.3/friendli/schema/__init__.py
--rw-r--r--   0        0        0       96 2024-03-23 07:44:00.438936 friendli_client-1.3.3/friendli/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2024-03-23 07:44:00.439023 friendli_client-1.3.3/friendli/schema/api/v1/__init__.py
--rw-r--r--   0        0        0      104 2024-03-23 07:44:00.439115 friendli_client-1.3.3/friendli/schema/api/v1/chat/__init__.py
--rw-r--r--   0        0        0     1296 2024-03-23 07:44:00.439195 friendli_client-1.3.3/friendli/schema/api/v1/chat/completions.py
--rw-r--r--   0        0        0      114 2024-03-23 07:44:00.439279 friendli_client-1.3.3/friendli/schema/api/v1/codegen/__init__.py
--rw-r--r--   0        0        0     2208 2024-03-23 17:30:34.571138 friendli_client-1.3.3/friendli/schema/api/v1/codegen/chat_completions_pb2.py
--rw-r--r--   0        0        0     2566 2024-03-23 17:30:34.590757 friendli_client-1.3.3/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi
--rw-r--r--   0        0        0     4490 2024-03-23 17:30:34.587704 friendli_client-1.3.3/friendli/schema/api/v1/codegen/completions_pb2.py
--rw-r--r--   0        0        0     7473 2024-03-23 17:30:34.626738 friendli_client-1.3.3/friendli/schema/api/v1/codegen/completions_pb2.pyi
--rw-r--r--   0        0        0     1738 2024-03-23 17:30:34.588575 friendli_client-1.3.3/friendli/schema/api/v1/codegen/text_to_image_pb2.py
--rw-r--r--   0        0        0     1515 2024-03-23 17:30:34.601470 friendli_client-1.3.3/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi
--rw-r--r--   0        0        0     1027 2024-03-23 17:10:00.027875 friendli_client-1.3.3/friendli/schema/api/v1/completions.py
--rw-r--r--   0        0        0      106 2024-03-23 07:44:00.439954 friendli_client-1.3.3/friendli/schema/api/v1/images/__init__.py
--rw-r--r--   0        0        0      809 2024-03-23 07:44:00.440011 friendli_client-1.3.3/friendli/schema/api/v1/images/image.py
--rw-r--r--   0        0        0      599 2024-03-23 17:11:01.998576 friendli_client-1.3.3/friendli/schema/api/v1/proto/chat_completions.proto
--rw-r--r--   0        0        0     1885 2024-03-23 17:10:53.862166 friendli_client-1.3.3/friendli/schema/api/v1/proto/completions.proto
--rw-r--r--   0        0        0      413 2024-03-23 17:11:26.541100 friendli_client-1.3.3/friendli/schema/api/v1/proto/text_to_image.proto
--rw-r--r--   0        0        0       92 2024-03-23 07:44:00.440304 friendli_client-1.3.3/friendli/schema/config/__init__.py
--rw-r--r--   0        0        0      503 2024-03-23 07:45:31.691688 friendli_client-1.3.3/friendli/schema/config/endpoint.py
--rw-r--r--   0        0        0      101 2024-03-23 07:44:00.440453 friendli_client-1.3.3/friendli/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2024-03-23 07:44:00.440524 friendli_client-1.3.3/friendli/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     5476 2024-03-23 07:45:31.691894 friendli_client-1.3.3/friendli/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0      332 2024-03-23 07:45:31.691954 friendli_client-1.3.3/friendli/schema/resource/v1/common.py
--rw-r--r--   0        0        0     1147 2024-03-23 07:45:31.692013 friendli_client-1.3.3/friendli/schema/resource/v1/endpoint.py
--rw-r--r--   0        0        0      243 2024-04-01 05:27:02.870428 friendli_client-1.3.3/friendli/schema/resource/v1/model.py
--rw-r--r--   0        0        0      753 2024-03-23 07:44:00.440859 friendli_client-1.3.3/friendli/schema/resource/v1/transfer.py
--rw-r--r--   0        0        0       88 2024-03-23 07:44:00.440946 friendli_client-1.3.3/friendli/sdk/__init__.py
--rw-r--r--   0        0        0      102 2024-03-23 07:44:00.441027 friendli_client-1.3.3/friendli/sdk/api/__init__.py
--rw-r--r--   0        0        0     8240 2024-04-01 05:27:02.870789 friendli_client-1.3.3/friendli/sdk/api/base.py
--rw-r--r--   0        0        0       93 2024-03-23 07:44:00.441212 friendli_client-1.3.3/friendli/sdk/api/chat/__init__.py
--rw-r--r--   0        0        0     1241 2024-03-23 07:45:31.692330 friendli_client-1.3.3/friendli/sdk/api/chat/chat.py
--rw-r--r--   0        0        0    14282 2024-03-24 03:13:46.041262 friendli_client-1.3.3/friendli/sdk/api/chat/completions.py
--rw-r--r--   0        0        0    51810 2024-03-24 02:58:22.771406 friendli_client-1.3.3/friendli/sdk/api/completions.py
--rw-r--r--   0        0        0       95 2024-03-23 07:44:00.441601 friendli_client-1.3.3/friendli/sdk/api/images/__init__.py
--rw-r--r--   0        0        0     1060 2024-03-23 07:45:31.692695 friendli_client-1.3.3/friendli/sdk/api/images/images.py
--rw-r--r--   0        0        0     5861 2024-03-23 07:44:00.441778 friendli_client-1.3.3/friendli/sdk/api/images/text_to_image.py
--rw-r--r--   0        0        0     3839 2024-03-26 05:01:47.745171 friendli_client-1.3.3/friendli/sdk/client.py
--rw-r--r--   0        0        0      112 2024-03-23 07:44:00.441930 friendli_client-1.3.3/friendli/sdk/resource/__init__.py
--rw-r--r--   0        0        0     2520 2024-03-23 07:45:31.692919 friendli_client-1.3.3/friendli/sdk/resource/base.py
--rw-r--r--   0        0        0     1836 2024-03-23 07:45:31.692986 friendli_client-1.3.3/friendli/sdk/resource/endpoint.py
--rw-r--r--   0        0        0     1033 2024-03-23 07:45:31.693053 friendli_client-1.3.3/friendli/sdk/resource/model.py
--rw-r--r--   0        0        0      706 2024-03-23 07:44:00.442165 friendli_client-1.3.3/friendli/settings.py
--rw-r--r--   0        0        0       97 2024-03-23 07:44:00.442244 friendli_client-1.3.3/friendli/utils/__init__.py
--rw-r--r--   0        0        0     1076 2024-03-23 07:44:00.442303 friendli_client-1.3.3/friendli/utils/compat.py
--rw-r--r--   0        0        0     1294 2024-03-23 07:45:31.693160 friendli_client-1.3.3/friendli/utils/decorator.py
--rw-r--r--   0        0        0     3868 2024-03-23 07:45:31.693285 friendli_client-1.3.3/friendli/utils/format.py
--rw-r--r--   0        0        0     2340 2024-03-26 14:38:52.593456 friendli_client-1.3.3/friendli/utils/fs.py
--rw-r--r--   0        0        0      666 2024-03-23 07:44:00.442613 friendli_client-1.3.3/friendli/utils/prompt.py
--rw-r--r--   0        0        0     1408 2024-03-23 07:44:00.442676 friendli_client-1.3.3/friendli/utils/request.py
--rw-r--r--   0        0        0     1384 2024-03-23 07:44:00.442732 friendli_client-1.3.3/friendli/utils/testing.py
--rw-r--r--   0        0        0    19793 2024-03-23 07:44:00.442810 friendli_client-1.3.3/friendli/utils/transfer.py
--rw-r--r--   0        0        0     3575 2024-03-23 07:44:00.442892 friendli_client-1.3.3/friendli/utils/url.py
--rw-r--r--   0        0        0     3323 2024-03-23 07:45:31.693409 friendli_client-1.3.3/friendli/utils/validate.py
--rw-r--r--   0        0        0     1513 2024-03-23 07:44:00.443024 friendli_client-1.3.3/friendli/utils/version.py
--rw-r--r--   0        0        0     3406 2024-04-01 05:27:02.849839 friendli_client-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     8172 1970-01-01 00:00:00.000000 friendli_client-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-04-02 02:48:33.811614 friendli_client-1.3.4/LICENSE
+-rw-r--r--   0        0        0     6417 2024-04-02 02:48:33.811690 friendli_client-1.3.4/README.md
+-rw-r--r--   0        0        0      615 2024-04-02 02:48:33.811781 friendli_client-1.3.4/friendli/__init__.py
+-rw-r--r--   0        0        0     5840 2024-04-02 02:48:33.811867 friendli_client-1.3.4/friendli/auth.py
+-rw-r--r--   0        0        0      188 2024-04-02 02:48:33.811963 friendli_client-1.3.4/friendli/cli/__init__.py
+-rw-r--r--   0        0        0      628 2024-04-02 02:48:33.812042 friendli_client-1.3.4/friendli/cli/api/__init__.py
+-rw-r--r--   0        0        0     5374 2024-04-02 02:48:33.812163 friendli_client-1.3.4/friendli/cli/api/chat_completions.py
+-rw-r--r--   0        0        0     4513 2024-04-02 02:48:33.812254 friendli_client-1.3.4/friendli/cli/api/completions.py
+-rw-r--r--   0        0        0     3058 2024-04-02 02:48:33.812352 friendli_client-1.3.4/friendli/cli/api/text_to_image.py
+-rw-r--r--   0        0        0     4424 2024-04-02 02:48:33.812456 friendli_client-1.3.4/friendli/cli/endpoint.py
+-rw-r--r--   0        0        0     3572 2024-04-02 02:48:33.812528 friendli_client-1.3.4/friendli/cli/login.py
+-rw-r--r--   0        0        0     5150 2024-04-02 02:48:33.812599 friendli_client-1.3.4/friendli/cli/main.py
+-rw-r--r--   0        0        0    13525 2024-04-02 03:20:05.465045 friendli_client-1.3.4/friendli/cli/model.py
+-rw-r--r--   0        0        0     2727 2024-04-02 02:48:33.812754 friendli_client-1.3.4/friendli/cli/project.py
+-rw-r--r--   0        0        0     2074 2024-04-02 02:48:33.812829 friendli_client-1.3.4/friendli/cli/team.py
+-rw-r--r--   0        0        0      125 2024-04-02 02:48:33.812930 friendli_client-1.3.4/friendli/client/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-02 02:48:33.813027 friendli_client-1.3.4/friendli/client/graphql/__init__.py
+-rw-r--r--   0        0        0     4089 2024-04-02 02:48:33.813084 friendli_client-1.3.4/friendli/client/graphql/base.py
+-rw-r--r--   0        0        0     6510 2024-04-02 02:48:33.813155 friendli_client-1.3.4/friendli/client/graphql/endpoint.py
+-rw-r--r--   0        0        0      791 2024-04-02 02:48:33.813247 friendli_client-1.3.4/friendli/client/graphql/model.py
+-rw-r--r--   0        0        0     1014 2024-04-02 02:48:33.813437 friendli_client-1.3.4/friendli/client/graphql/team.py
+-rw-r--r--   0        0        0     1914 2024-04-02 02:48:33.813534 friendli_client-1.3.4/friendli/client/graphql/user.py
+-rw-r--r--   0        0        0       88 2024-04-02 02:48:33.813643 friendli_client-1.3.4/friendli/client/http/__init__.py
+-rw-r--r--   0        0        0    14158 2024-04-02 02:48:33.813750 friendli_client-1.3.4/friendli/client/http/base.py
+-rw-r--r--   0        0        0      977 2024-04-02 02:48:33.813870 friendli_client-1.3.4/friendli/client/http/login.py
+-rw-r--r--   0        0        0     1567 2024-04-02 02:48:33.813946 friendli_client-1.3.4/friendli/context.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.814074 friendli_client-1.3.4/friendli/di/__init__.py
+-rw-r--r--   0        0        0     1507 2024-04-02 02:48:33.814149 friendli_client-1.3.4/friendli/di/injector.py
+-rw-r--r--   0        0        0      620 2024-04-02 02:48:33.814218 friendli_client-1.3.4/friendli/di/modules.py
+-rw-r--r--   0        0        0     1132 2024-04-02 02:48:33.814282 friendli_client-1.3.4/friendli/enums.py
+-rw-r--r--   0        0        0     6853 2024-04-02 02:48:33.814354 friendli_client-1.3.4/friendli/errors.py
+-rw-r--r--   0        0        0     9607 2024-04-02 02:48:33.814426 friendli_client-1.3.4/friendli/formatter.py
+-rw-r--r--   0        0        0     1728 2024-04-02 02:48:33.814495 friendli_client-1.3.4/friendli/logging.py
+-rw-r--r--   0        0        0       92 2024-04-02 02:48:33.814585 friendli_client-1.3.4/friendli/modules/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-02 02:48:33.814672 friendli_client-1.3.4/friendli/modules/converter/__init__.py
+-rw-r--r--   0        0        0    19733 2024-04-02 02:48:33.814763 friendli_client-1.3.4/friendli/modules/converter/base.py
+-rw-r--r--   0        0        0     9671 2024-04-02 03:20:05.465257 friendli_client-1.3.4/friendli/modules/converter/convert.py
+-rw-r--r--   0        0        0     5642 2024-04-02 02:48:33.814912 friendli_client-1.3.4/friendli/modules/converter/interface.py
+-rw-r--r--   0        0        0     5154 2024-04-02 02:48:33.814984 friendli_client-1.3.4/friendli/modules/converter/maps.py
+-rw-r--r--   0        0        0    21332 2024-04-02 02:48:33.815139 friendli_client-1.3.4/friendli/modules/converter/models/blenderbot.py
+-rw-r--r--   0        0        0    11658 2024-04-02 02:48:33.815310 friendli_client-1.3.4/friendli/modules/converter/models/bloom.py
+-rw-r--r--   0        0        0    10057 2024-04-02 02:48:33.815391 friendli_client-1.3.4/friendli/modules/converter/models/codegen.py
+-rw-r--r--   0        0        0    12677 2024-04-02 02:48:33.815479 friendli_client-1.3.4/friendli/modules/converter/models/falcon.py
+-rw-r--r--   0        0        0    10036 2024-04-02 02:48:33.815575 friendli_client-1.3.4/friendli/modules/converter/models/gpt2.py
+-rw-r--r--   0        0        0    13562 2024-04-02 02:48:33.815649 friendli_client-1.3.4/friendli/modules/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0    17772 2024-04-02 02:48:33.815747 friendli_client-1.3.4/friendli/modules/converter/models/gptj.py
+-rw-r--r--   0        0        0    21030 2024-04-02 02:48:33.815852 friendli_client-1.3.4/friendli/modules/converter/models/llama.py
+-rw-r--r--   0        0        0     4497 2024-04-02 02:48:33.815929 friendli_client-1.3.4/friendli/modules/converter/models/mistral.py
+-rw-r--r--   0        0        0     9076 2024-04-02 02:48:33.816002 friendli_client-1.3.4/friendli/modules/converter/models/mixtral.py
+-rw-r--r--   0        0        0    16219 2024-04-02 02:48:33.816074 friendli_client-1.3.4/friendli/modules/converter/models/mpt.py
+-rw-r--r--   0        0        0    12005 2024-04-02 02:48:33.816146 friendli_client-1.3.4/friendli/modules/converter/models/opt.py
+-rw-r--r--   0        0        0    14295 2024-04-02 02:48:33.816216 friendli_client-1.3.4/friendli/modules/converter/models/phi_msft.py
+-rw-r--r--   0        0        0    18719 2024-04-02 02:48:33.816290 friendli_client-1.3.4/friendli/modules/converter/models/t5.py
+-rw-r--r--   0        0        0     8800 2024-04-02 03:20:05.465458 friendli_client-1.3.4/friendli/modules/converter/saver.py
+-rw-r--r--   0        0        0      897 2024-04-02 02:48:33.816450 friendli_client-1.3.4/friendli/modules/converter/schema.py
+-rw-r--r--   0        0        0     8858 2024-04-02 03:20:05.465654 friendli_client-1.3.4/friendli/modules/converter/utils.py
+-rw-r--r--   0        0        0      100 2024-04-02 02:48:33.816595 friendli_client-1.3.4/friendli/modules/quantizer/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.816695 friendli_client-1.3.4/friendli/modules/quantizer/awq/__init__.py
+-rw-r--r--   0        0        0    19257 2024-04-02 02:48:33.816791 friendli_client-1.3.4/friendli/modules/quantizer/awq/base.py
+-rw-r--r--   0        0        0     7090 2024-04-02 02:48:33.816891 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gpt_neox.py
+-rw-r--r--   0        0        0     5917 2024-04-02 02:48:33.816955 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gptj.py
+-rw-r--r--   0        0        0    10738 2024-04-02 02:48:33.817034 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/llama.py
+-rw-r--r--   0        0        0     6606 2024-04-02 02:48:33.817101 friendli_client-1.3.4/friendli/modules/quantizer/awq/models/mpt.py
+-rw-r--r--   0        0        0     7764 2024-04-02 02:48:33.817162 friendli_client-1.3.4/friendli/modules/quantizer/awq/utils.py
+-rw-r--r--   0        0        0    17760 2024-04-02 02:48:33.817232 friendli_client-1.3.4/friendli/modules/quantizer/base.py
+-rw-r--r--   0        0        0     3410 2024-04-02 02:48:33.817304 friendli_client-1.3.4/friendli/modules/quantizer/layers.py
+-rw-r--r--   0        0        0     4317 2024-04-02 02:48:33.817360 friendli_client-1.3.4/friendli/modules/quantizer/maps.py
+-rw-r--r--   0        0        0     3043 2024-04-02 02:48:33.817444 friendli_client-1.3.4/friendli/modules/quantizer/models/llama.py
+-rw-r--r--   0        0        0     3212 2024-04-02 02:48:33.817517 friendli_client-1.3.4/friendli/modules/quantizer/models/mixtral.py
+-rw-r--r--   0        0        0     2734 2024-04-02 02:48:33.817567 friendli_client-1.3.4/friendli/modules/quantizer/models/mpt.py
+-rw-r--r--   0        0        0      107 2024-04-02 02:48:33.817642 friendli_client-1.3.4/friendli/modules/quantizer/schema/__init__.py
+-rw-r--r--   0        0        0     2270 2024-04-02 02:48:33.817712 friendli_client-1.3.4/friendli/modules/quantizer/schema/config.py
+-rw-r--r--   0        0        0     2798 2024-04-02 02:48:33.817762 friendli_client-1.3.4/friendli/modules/quantizer/schema/data.py
+-rw-r--r--   0        0        0      112 2024-04-02 02:48:33.817836 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/__init__.py
+-rw-r--r--   0        0        0    24897 2024-04-02 02:48:33.817896 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/base.py
+-rw-r--r--   0        0        0     7496 2024-04-02 02:48:33.818011 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/bloom.py
+-rw-r--r--   0        0        0     8777 2024-04-02 02:48:33.818086 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/codegen.py
+-rw-r--r--   0        0        0    10437 2024-04-02 02:48:33.818138 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/falcon.py
+-rw-r--r--   0        0        0     5466 2024-04-02 02:48:33.818193 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt2.py
+-rw-r--r--   0        0        0     9062 2024-04-02 02:48:33.818263 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt_neox.py
+-rw-r--r--   0        0        0     6961 2024-04-02 02:48:33.818328 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gptj.py
+-rw-r--r--   0        0        0     9431 2024-04-02 02:48:33.818404 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/llama.py
+-rw-r--r--   0        0        0     5290 2024-04-02 02:48:33.818545 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/mpt.py
+-rw-r--r--   0        0        0     5231 2024-04-02 02:48:33.818597 friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/opt.py
+-rw-r--r--   0        0        0    16812 2024-04-02 02:48:33.818673 friendli_client-1.3.4/friendli/modules/quantizer/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:48:33.818734 friendli_client-1.3.4/friendli/py.typed
+-rw-r--r--   0        0        0       92 2024-04-02 02:48:33.818949 friendli_client-1.3.4/friendli/schema/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-02 02:48:33.819059 friendli_client-1.3.4/friendli/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-02 02:48:33.819140 friendli_client-1.3.4/friendli/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.819223 friendli_client-1.3.4/friendli/schema/api/v1/chat/__init__.py
+-rw-r--r--   0        0        0     1296 2024-04-02 02:48:33.819279 friendli_client-1.3.4/friendli/schema/api/v1/chat/completions.py
+-rw-r--r--   0        0        0      114 2024-04-02 02:48:33.819350 friendli_client-1.3.4/friendli/schema/api/v1/codegen/__init__.py
+-rw-r--r--   0        0        0     2208 2024-04-02 02:48:33.819433 friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.py
+-rw-r--r--   0        0        0     2566 2024-04-02 02:48:33.819560 friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi
+-rw-r--r--   0        0        0     4490 2024-04-02 02:48:33.819650 friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.py
+-rw-r--r--   0        0        0     7473 2024-04-02 02:48:33.819710 friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.pyi
+-rw-r--r--   0        0        0     1738 2024-04-02 02:48:33.819776 friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.py
+-rw-r--r--   0        0        0     1515 2024-04-02 02:48:33.819906 friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi
+-rw-r--r--   0        0        0     1027 2024-04-02 02:48:33.819978 friendli_client-1.3.4/friendli/schema/api/v1/completions.py
+-rw-r--r--   0        0        0      106 2024-04-02 02:48:33.820119 friendli_client-1.3.4/friendli/schema/api/v1/images/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-02 02:48:33.820203 friendli_client-1.3.4/friendli/schema/api/v1/images/image.py
+-rw-r--r--   0        0        0      599 2024-04-02 02:48:33.820303 friendli_client-1.3.4/friendli/schema/api/v1/proto/chat_completions.proto
+-rw-r--r--   0        0        0     1885 2024-04-02 02:48:33.820359 friendli_client-1.3.4/friendli/schema/api/v1/proto/completions.proto
+-rw-r--r--   0        0        0      413 2024-04-02 02:48:33.820415 friendli_client-1.3.4/friendli/schema/api/v1/proto/text_to_image.proto
+-rw-r--r--   0        0        0       92 2024-04-02 02:48:33.820516 friendli_client-1.3.4/friendli/schema/config/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-02 02:48:33.820569 friendli_client-1.3.4/friendli/schema/config/endpoint.py
+-rw-r--r--   0        0        0      101 2024-04-02 02:48:33.820645 friendli_client-1.3.4/friendli/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-02 02:48:33.820721 friendli_client-1.3.4/friendli/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     5476 2024-04-02 02:48:33.820787 friendli_client-1.3.4/friendli/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0      332 2024-04-02 02:48:33.820845 friendli_client-1.3.4/friendli/schema/resource/v1/common.py
+-rw-r--r--   0        0        0     1147 2024-04-02 02:48:33.820909 friendli_client-1.3.4/friendli/schema/resource/v1/endpoint.py
+-rw-r--r--   0        0        0      243 2024-04-02 02:48:33.820971 friendli_client-1.3.4/friendli/schema/resource/v1/model.py
+-rw-r--r--   0        0        0      753 2024-04-02 02:48:33.821026 friendli_client-1.3.4/friendli/schema/resource/v1/transfer.py
+-rw-r--r--   0        0        0       88 2024-04-02 02:48:33.821101 friendli_client-1.3.4/friendli/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-02 02:48:33.821171 friendli_client-1.3.4/friendli/sdk/api/__init__.py
+-rw-r--r--   0        0        0     8240 2024-04-02 02:48:33.821245 friendli_client-1.3.4/friendli/sdk/api/base.py
+-rw-r--r--   0        0        0       93 2024-04-02 02:48:33.821329 friendli_client-1.3.4/friendli/sdk/api/chat/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-02 02:48:33.821390 friendli_client-1.3.4/friendli/sdk/api/chat/chat.py
+-rw-r--r--   0        0        0    14282 2024-04-02 02:48:33.821480 friendli_client-1.3.4/friendli/sdk/api/chat/completions.py
+-rw-r--r--   0        0        0    51810 2024-04-02 02:48:33.821608 friendli_client-1.3.4/friendli/sdk/api/completions.py
+-rw-r--r--   0        0        0       95 2024-04-02 02:48:33.821724 friendli_client-1.3.4/friendli/sdk/api/images/__init__.py
+-rw-r--r--   0        0        0     1060 2024-04-02 02:48:33.821774 friendli_client-1.3.4/friendli/sdk/api/images/images.py
+-rw-r--r--   0        0        0     5861 2024-04-02 02:48:33.821830 friendli_client-1.3.4/friendli/sdk/api/images/text_to_image.py
+-rw-r--r--   0        0        0     3839 2024-04-02 02:48:33.821876 friendli_client-1.3.4/friendli/sdk/client.py
+-rw-r--r--   0        0        0      112 2024-04-02 02:48:33.821942 friendli_client-1.3.4/friendli/sdk/resource/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-02 02:48:33.821994 friendli_client-1.3.4/friendli/sdk/resource/base.py
+-rw-r--r--   0        0        0     1836 2024-04-02 02:48:33.822044 friendli_client-1.3.4/friendli/sdk/resource/endpoint.py
+-rw-r--r--   0        0        0     1033 2024-04-02 02:48:33.822099 friendli_client-1.3.4/friendli/sdk/resource/model.py
+-rw-r--r--   0        0        0      706 2024-04-02 02:48:33.822146 friendli_client-1.3.4/friendli/settings.py
+-rw-r--r--   0        0        0       97 2024-04-02 02:48:33.822213 friendli_client-1.3.4/friendli/utils/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 02:48:33.822265 friendli_client-1.3.4/friendli/utils/compat.py
+-rw-r--r--   0        0        0     1294 2024-04-02 02:48:33.822319 friendli_client-1.3.4/friendli/utils/decorator.py
+-rw-r--r--   0        0        0     3868 2024-04-02 02:48:33.822376 friendli_client-1.3.4/friendli/utils/format.py
+-rw-r--r--   0        0        0     2340 2024-04-02 02:48:33.822424 friendli_client-1.3.4/friendli/utils/fs.py
+-rw-r--r--   0        0        0      666 2024-04-02 02:48:33.822474 friendli_client-1.3.4/friendli/utils/prompt.py
+-rw-r--r--   0        0        0     1408 2024-04-02 02:48:33.822531 friendli_client-1.3.4/friendli/utils/request.py
+-rw-r--r--   0        0        0     1384 2024-04-02 02:48:33.822580 friendli_client-1.3.4/friendli/utils/testing.py
+-rw-r--r--   0        0        0    19793 2024-04-02 02:48:33.822653 friendli_client-1.3.4/friendli/utils/transfer.py
+-rw-r--r--   0        0        0     3575 2024-04-02 02:48:33.822730 friendli_client-1.3.4/friendli/utils/url.py
+-rw-r--r--   0        0        0     3323 2024-04-02 02:48:33.822785 friendli_client-1.3.4/friendli/utils/validate.py
+-rw-r--r--   0        0        0     1513 2024-04-02 02:48:33.822833 friendli_client-1.3.4/friendli/utils/version.py
+-rw-r--r--   0        0        0     3406 2024-04-02 03:20:05.471738 friendli_client-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8172 1970-01-01 00:00:00.000000 friendli_client-1.3.4/PKG-INFO
```

### Comparing `friendli_client-1.3.3/LICENSE` & `friendli_client-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/README.md` & `friendli_client-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/__init__.py` & `friendli_client-1.3.4/friendli/__init__.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/auth.py` & `friendli_client-1.3.4/friendli/auth.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/api/__init__.py` & `friendli_client-1.3.4/friendli/cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/api/chat_completions.py` & `friendli_client-1.3.4/friendli/cli/api/chat_completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/api/completions.py` & `friendli_client-1.3.4/friendli/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/api/text_to_image.py` & `friendli_client-1.3.4/friendli/cli/api/text_to_image.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/endpoint.py` & `friendli_client-1.3.4/friendli/cli/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/login.py` & `friendli_client-1.3.4/friendli/cli/login.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/main.py` & `friendli_client-1.3.4/friendli/cli/main.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/model.py` & `friendli_client-1.3.4/friendli/cli/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,27 +221,22 @@
         CheckpointFileType.HDF5: "model.h5",
         CheckpointFileType.SAFETENSORS: "model.safetensors",
     }
     output_model_file_name = (
         output_model_file_name or default_names[output_ckpt_file_type]
     )
 
-    model_output_path = os.path.join(output_dir, output_model_file_name)
-    tokenizer_output_dir = output_dir
-    attr_output_path = os.path.join(output_dir, output_attr_file_name)
-
     try:
         convert_checkpoint(
             model_name_or_path=model_name_or_path,
-            model_output_path=model_output_path,
+            output_model_file_name=output_model_file_name,
             output_ckpt_file_type=output_ckpt_file_type,
+            output_attr_file_name=output_attr_file_name,
             output_dir=output_dir,
             data_type=data_type,
-            tokenizer_output_dir=tokenizer_output_dir,
-            attr_output_path=attr_output_path,
             cache_dir=cache_dir,
             dry_run=dry_run,
             quantize=quantize,
             quant_config=quant_config,
         )
     except (NotFoundError, CheckpointConversionError, InvalidConfigError) as exc:
         secho_error_and_exit(str(exc))
@@ -340,23 +335,28 @@
         CheckpointFileType.HDF5: "adapter.h5",
         CheckpointFileType.SAFETENSORS: "adapter.safetensors",
     }
     output_adapter_filename = (
         output_adapter_filename or default_names[output_adapter_file_type]
     )
 
-    adapter_output_path = os.path.join(output_dir, output_adapter_filename)
-    attr_output_path = os.path.join(output_dir, output_attr_filename)
-
     try:
         convert_adapter_checkpoint(
             adapter_name_or_path=adapter_name_or_path,
-            adapter_output_path=adapter_output_path,
-            adapter_attr_output_path=attr_output_path,
+            output_attr_filename=output_attr_filename,
+            output_dir=output_dir,
+            output_adapter_filename=output_adapter_filename,
             base_model_name_or_path=base_model_name_or_path,
             data_type=data_type,
             output_adapter_file_type=output_adapter_file_type,
             cache_dir=cache_dir,
             dry_run=dry_run,
         )
     except (NotFoundError, CheckpointConversionError, InvalidConfigError) as exc:
         secho_error_and_exit(str(exc))
+
+    msg = (
+        f"Checkpoint({adapter_name_or_path}) can be converted."
+        if dry_run
+        else f"Checkpoint({adapter_name_or_path}) has been converted successfully."
+    )
+    typer.secho(msg)
```

### Comparing `friendli_client-1.3.3/friendli/cli/project.py` & `friendli_client-1.3.4/friendli/cli/project.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/cli/team.py` & `friendli_client-1.3.4/friendli/cli/team.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/graphql/base.py` & `friendli_client-1.3.4/friendli/client/graphql/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/graphql/endpoint.py` & `friendli_client-1.3.4/friendli/client/graphql/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/graphql/model.py` & `friendli_client-1.3.4/friendli/client/graphql/model.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/graphql/team.py` & `friendli_client-1.3.4/friendli/client/graphql/team.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/graphql/user.py` & `friendli_client-1.3.4/friendli/client/graphql/user.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/http/base.py` & `friendli_client-1.3.4/friendli/client/http/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/client/http/login.py` & `friendli_client-1.3.4/friendli/client/http/login.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/context.py` & `friendli_client-1.3.4/friendli/context.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/di/injector.py` & `friendli_client-1.3.4/friendli/di/injector.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/di/modules.py` & `friendli_client-1.3.4/friendli/di/modules.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/enums.py` & `friendli_client-1.3.4/friendli/enums.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/errors.py` & `friendli_client-1.3.4/friendli/errors.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/formatter.py` & `friendli_client-1.3.4/friendli/formatter.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/logging.py` & `friendli_client-1.3.4/friendli/logging.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/base.py` & `friendli_client-1.3.4/friendli/modules/converter/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,31 +411,38 @@
                 valid_options=[None, {}],
             )
 
         if self.adapter_config.target_modules is not None:
             for target_module in self.adapter_config.target_modules:
                 if (
                     target_module
-                    in MODEL_TYPE_TO_UNSUPPORTED_LORA_TARGET_MODULES_MAP[
+                    not in MODEL_TYPE_TO_SUPPORTED_LORA_TARGET_MODULES_MAP[
                         self.config.model_type
                     ]
                 ):
-                    raise NotSupportedCheckpointError(
-                        invalid_option=f"target_module={target_module}",
-                        valid_options=list(
-                            MODEL_TYPE_TO_SUPPORTED_LORA_TARGET_MODULES_MAP[
-                                self.config.model_type
-                            ]
-                        ),
+                    if (
+                        target_module
+                        in MODEL_TYPE_TO_UNSUPPORTED_LORA_TARGET_MODULES_MAP[
+                            self.config.model_type
+                        ]
+                    ):
+                        raise NotSupportedCheckpointError(
+                            invalid_option=f"target_module={target_module}",
+                            valid_options=list(
+                                MODEL_TYPE_TO_SUPPORTED_LORA_TARGET_MODULES_MAP[
+                                    self.config.model_type
+                                ]
+                            ),
+                        )
+
+                    logger.warn(
+                        "Target module %s does not exist in the base model (%s). Will be ignored.",
+                        target_module,
+                        self.adapter_config.base_model_name_or_path,
                     )
-                logger.warn(
-                    "Target module %s does not exist in the base model (%s). Will be ignored.",
-                    target_module,
-                    self.adapter_config.base_model_name_or_path,
-                )
 
         if (self.adapter_config.layers_to_transform is not None) and (
             self.adapter_config != list(range(self.converter.decoder_layer_num))
         ):
             raise NotSupportedCheckpointError(
                 invalid_option=f"layers_to_transform={self.adapter_config.layers_to_transform}",
                 valid_options=[
```

### Comparing `friendli_client-1.3.3/friendli/modules/converter/convert.py` & `friendli_client-1.3.4/friendli/modules/converter/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,35 +37,37 @@
 from friendli.modules.quantizer.schema.config import OneOfQuantConfig
 
 # pylint: enable=import-outside-toplevel, wrong-import-position, wrong-import-order, ungrouped-imports
 
 
 def convert_checkpoint(  # pylint: disable=too-many-branches
     model_name_or_path: str,
-    model_output_path: str,
-    output_ckpt_file_type: CheckpointFileType,
+    output_model_file_name: str,
+    output_attr_file_name: str,
     output_dir: str,
+    output_ckpt_file_type: CheckpointFileType,
     *,
     data_type: Optional[ModelDataType] = None,
-    tokenizer_output_dir: Optional[str] = None,
-    attr_output_path: Optional[str] = None,
     cache_dir: Optional[str] = None,
     dry_run: bool = False,
     quantize: bool = False,
     quant_config: Optional[OneOfQuantConfig] = None,
 ) -> None:
     """Convert HuggingFace model checkpoint to Friendli format.
 
     Args:
         model_name_or_path (str): Hugging Face model name or local path to the checkpoint.
-        model_output_path (str): Path to the converted checkpoint to save.
+        output_model_file_name (str): File name of converted checkpoint to save.
+        output_attr_file_name (str): File name of the attribute YAML file for
+            the converted checkpoint.
+        output_dir (str) : Directory path to save the converted checkpoint and the attribute YAML,
+            and tokenizer configuration file.
+        output_ckpt_file_type (CheckpointFileType): The file type of converted checkpoint.
         data_type (Optional[ModelDataType]): Converted checkpoint data type.
             Defaults to torch_dtype in 'config.json'
-        tokenizer_output_dir (Optional[str], optional): Directory path to save 'tokenizer.json'
-            for the converted checkpoint. Defaults to None.
         attr_output_path (Optional[str], optional): Path to create the attribute YAML file for
             the converted checkpoint. Defaults to None.
         cache_dir (Optional[str], optional): Path for downloading checkpoint. Defaults to None.
         dry_run (bool, optional): Check only if checkpoint is convertable. Defaults to False.
         quantize (bool, optional): Enable quantization. Defaults to False.
         quant_config (Optional[OneOfQuantConfig], optional): Quantization configuration.
             Defaults to None.
@@ -73,14 +75,15 @@
     Raises:
         InValidconfigError: Raised when data_type is not supported.
         NotFoundError: Raised when `model_name_or_path` or `tokenizer_output_dir` is not found.
         NotSupportedCheckpointError: Raised when model architecture is not supported to convert.
 
     """
     # pylint: disable=too-many-locals
+    model_output_path = os.path.join(output_dir, output_model_file_name)
     model_config = get_model_pretrained_config(
         model_name_or_path, model_output_path, cache_dir
     )
     generation_config = get_model_generation_config(model_name_or_path, cache_dir)
 
     model_arch = get_model_arch(model_config)
     hf_factory, converter_factory = get_hf_converter_factory(model_arch)
@@ -118,80 +121,77 @@
 
         logger.info(
             "Hugging Face checkpoint(%s) is successfully loaded!",
             model_name_or_path,
         )
 
         convert_info_list = converter.get_convert_info_list()
-        with get_saver(output_ckpt_file_type, output_dir) as saver:
+        with get_saver(
+            output_ckpt_file_type, output_dir, output_model_file_name
+        ) as saver:
             for name, w in converter.convert(model, convert_info_list):
                 saver.save_tensor(name, w)
 
         logger.info(
             "Hugging Face checkpoint(%s) is successfully converted to Friendli format!",
             model_name_or_path,
         )
 
-    if attr_output_path is not None:
-        if (
-            quant_config
-            and quant_config.mode == QuantMode.FP8
-            and ModelDataType.FP8_E4M3
-        ):
-            model_config.torch_dtype = (
-                get_torch_data_type(data_type)
-                if data_type
-                else model_config.torch_dtype
-            )
-            setattr(model_config, "use_fp8_e4m3", True)
-            assert output_dir is not None
-            model_config.to_json_file(os.path.join(output_dir, "config.json"))
-        else:
-            attr = converter.get_attributes()
-            with open(attr_output_path, "w", encoding="utf-8") as file:
-                yaml.dump(attr, file, sort_keys=False)
-
-    if tokenizer_output_dir is not None:
-        try:
-            saved_tokenizer_file_paths = save_tokenizer(
-                model_name_or_path=model_name_or_path,
-                cache_dir=cache_dir,
-                save_dir=tokenizer_output_dir,
-            )
-        except TokenizerNotFoundError as exc:
-            logger.warn(str(exc))
+    # Save attr.yaml
+    attr_output_path = os.path.join(output_dir, output_attr_file_name)
+    if quant_config and quant_config.mode == QuantMode.FP8 and ModelDataType.FP8_E4M3:
+        model_config.torch_dtype = (
+            get_torch_data_type(data_type) if data_type else model_config.torch_dtype
+        )
+        setattr(model_config, "use_fp8_e4m3", True)
+        model_config.to_json_file(os.path.join(output_dir, "config.json"))
+    else:
+        attr = converter.get_attributes()
+        with open(attr_output_path, "w", encoding="utf-8") as file:
+            yaml.dump(attr, file, sort_keys=False)
+
+    # Save tokenizer files.
+    tokenizer_output_dir = output_dir
+    try:
+        saved_tokenizer_file_paths = save_tokenizer(
+            model_name_or_path=model_name_or_path,
+            cache_dir=cache_dir,
+            save_dir=tokenizer_output_dir,
+        )
+    except TokenizerNotFoundError as exc:
+        logger.warn(str(exc))
 
-        if not (
-            quant_config
-            and quant_config.mode == QuantMode.FP8
-            and ModelDataType.FP8_E4M3
-        ):
-            for path in saved_tokenizer_file_paths:
-                if path != "tokenizer.json":
-                    try:
-                        os.remove(path)
-                    except FileNotFoundError:
-                        logger.warn(
-                            "Tried to delete unnecessary tokenizer file %s but the file "
-                            "is not found.",
-                            path,
-                        )
+    if not (
+        quant_config and quant_config.mode == QuantMode.FP8 and ModelDataType.FP8_E4M3
+    ):
+        for path in saved_tokenizer_file_paths:
+            if "tokenizer.json" not in path:
+                try:
+                    os.remove(path)
+                except FileNotFoundError:
+                    logger.warn(
+                        "Tried to delete unnecessary tokenizer file %s but the file "
+                        "is not found.",
+                        path,
+                    )
 
 
 def convert_adapter_checkpoint(  # pylint: disable=too-many-locals, too-many-arguments
     adapter_name_or_path: str,
-    adapter_output_path: str,
-    adapter_attr_output_path: str,
+    output_attr_filename: str,
+    output_dir: str,
+    output_adapter_filename: str,
     base_model_name_or_path: Optional[str],
     data_type: Optional[ModelDataType],
     output_adapter_file_type: CheckpointFileType,
     cache_dir: Optional[str],
     dry_run: bool = False,
 ) -> None:
     """Convert HuggingFace model checkpoint to Friendli format."""
+    adapter_attr_output_path = os.path.join(output_dir, output_attr_filename)
     adapter_config = get_adapter_config(adapter_name_or_path, cache_dir)
     base_model_name_or_path = (
         base_model_name_or_path or adapter_config.base_model_name_or_path
     )
     model_config = get_model_pretrained_config(
         base_model_name_or_path,
         adapter_attr_output_path,
@@ -228,20 +228,21 @@
             model, adapter_name_or_path, cache_dir=cache_dir, torch_dtype=torch.float32
         )
         logger.info(
             "Hugging Face adapter checkpoint (%s) is successfully loaded!",
             adapter_name_or_path,
         )
         convert_dict = adapter_converter.get_convert_info_list()
-        with get_saver(output_adapter_file_type, adapter_output_path) as saver:
+        with get_saver(
+            output_adapter_file_type, output_dir, output_adapter_filename
+        ) as saver:
             for name, w in adapter_converter.convert(model, convert_dict):
                 saver.save_tensor(name, w)
 
-        if adapter_attr_output_path is not None:
-            attr = adapter_converter.get_attributes()
-            with open(adapter_attr_output_path, "w", encoding="utf-8") as file:
-                yaml.dump([attr], file, sort_keys=False)
-
         logger.info(
             "Hugging Face checkpoint (%s) is successfully converted to Friendli format!",
             adapter_name_or_path,
         )
+
+    attr = adapter_converter.get_attributes()
+    with open(adapter_attr_output_path, "w", encoding="utf-8") as file:
+        yaml.dump([attr], file, sort_keys=False)
```

### Comparing `friendli_client-1.3.3/friendli/modules/converter/interface.py` & `friendli_client-1.3.4/friendli/modules/converter/interface.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/maps.py` & `friendli_client-1.3.4/friendli/modules/converter/maps.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/blenderbot.py` & `friendli_client-1.3.4/friendli/modules/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/bloom.py` & `friendli_client-1.3.4/friendli/modules/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/codegen.py` & `friendli_client-1.3.4/friendli/modules/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/falcon.py` & `friendli_client-1.3.4/friendli/modules/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/gpt2.py` & `friendli_client-1.3.4/friendli/modules/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/gpt_neox.py` & `friendli_client-1.3.4/friendli/modules/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/gptj.py` & `friendli_client-1.3.4/friendli/modules/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/llama.py` & `friendli_client-1.3.4/friendli/modules/converter/models/llama.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/mistral.py` & `friendli_client-1.3.4/friendli/modules/converter/models/mistral.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/mixtral.py` & `friendli_client-1.3.4/friendli/modules/converter/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/mpt.py` & `friendli_client-1.3.4/friendli/modules/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/opt.py` & `friendli_client-1.3.4/friendli/modules/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/phi_msft.py` & `friendli_client-1.3.4/friendli/modules/converter/models/phi_msft.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/models/t5.py` & `friendli_client-1.3.4/friendli/modules/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/saver.py` & `friendli_client-1.3.4/friendli/modules/converter/saver.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,34 +19,36 @@
 
 from friendli.enums import CheckpointFileType
 from friendli.errors import CheckpointConversionError
 from friendli.logging import logger
 
 
 def get_saver(
-    ckpt_file_type: CheckpointFileType,
-    output_dir: str,
+    ckpt_file_type: CheckpointFileType, output_dir: str, output_file_name: str
 ) -> CheckpointSaver:
     """Create a saver that corresponds to the file type."""
     if ckpt_file_type == CheckpointFileType.HDF5:
-        return HDF5Saver(output_dir)
+        return HDF5Saver(output_dir, output_file_name)
     if ckpt_file_type == CheckpointFileType.SAFETENSORS:
-        return SafetensorsSaver(output_dir)
+        return SafetensorsSaver(output_dir, output_file_name)
     raise CheckpointConversionError(
         f"Output file type {ckpt_file_type} is not supported."
     )
 
 
 class CheckpointSaver(AbstractContextManager):
     """Abstract for savers."""
 
-    def __init__(self, output_dir: Union[str, os.PathLike]) -> None:
+    def __init__(
+        self, output_dir: Union[str, os.PathLike], output_file_name: str
+    ) -> None:
         """Check that the output file already exists."""
         super().__init__()
-        self.output_dir = output_dir
+        self._output_dir = output_dir
+        self._output_file_name = output_file_name
 
     @abstractmethod
     def save_tensor(self, tensor_id: str, t: Union[np.ndarray, torch.Tensor]) -> None:
         """Save the tensor in the file."""
         raise NotImplementedError
 
     @abstractmethod
@@ -62,18 +64,18 @@
         """Exit for context manager."""
         self.close()
 
 
 class HDF5Saver(CheckpointSaver):
     """Saver for HDF5."""
 
-    def __init__(self, output_dir: str) -> None:
+    def __init__(self, output_dir: str, output_file_name: str) -> None:
         """Create a HDF5 file."""
-        super().__init__(output_dir)
-        self._out_f = h5py.File(output_dir + "model.h5", "w")
+        super().__init__(output_dir, output_file_name)
+        self._out_f = h5py.File(os.path.join(output_dir, output_file_name), "w")
 
     def save_tensor(self, tensor_id: str, t: Union[np.ndarray, torch.Tensor]) -> None:
         """Create a group if not exists, and save the tensor in the file."""
         assert isinstance(t, np.ndarray)
         self._out_f[tensor_id] = t
 
     def close(self) -> None:
@@ -154,18 +156,19 @@
     """Saver for Safetensors.
 
     This temporally saves the converted tensors in local memory.
     Then, all of the tensors are saved in the file at a time when close() is called,
     because Safetensors does not support stream saving.
     """
 
-    def __init__(self, output_dir: Union[str, os.PathLike]) -> None:
+    def __init__(
+        self, output_dir: Union[str, os.PathLike], output_file_name: str
+    ) -> None:
         """Initialize a saver."""
-        super().__init__(output_dir)
-        self._output_dir = output_dir
+        super().__init__(output_dir, output_file_name)
         self._tensors: Dict[str, Union[np.ndarray, torch.Tensor]] = {}
         self._saver: UnionSafetensorsSaverInterface = UnionSafetensorsSaverInterface()
 
     def save_tensor(self, tensor_id: str, t: Union[np.ndarray, torch.Tensor]) -> None:
         """Save the tensor in the local memory."""
         self._tensors[tensor_id] = t
 
@@ -187,20 +190,20 @@
                 last_block_size = 0
 
             sharded_tensors[-1][key] = weight
             last_block_size += weight_size
             total_size += weight_size
 
         if len(sharded_tensors) == 1:
-            return {"model.safetensors": sharded_tensors[0]}, None
+            return {self._output_file_name: sharded_tensors[0]}, None
 
         weight_map = {}
         shards = {}
         for idx, shard in enumerate(sharded_tensors):
-            shard_file = "model.safetensors".replace(
+            shard_file = self._output_file_name.replace(
                 ".safetensors",
                 f"-{idx + 1:05d}-of-{len(sharded_tensors):05d}.safetensors",
             )
             shards[shard_file] = shard
             for key in shard.keys():
                 weight_map[key] = shard_file
 
@@ -215,15 +218,15 @@
         max_shard_size = "10GB"
         shards, index = self.shard_checkpoint(max_shard_size)
 
         for shard_file, shard in shards.items():
             self._saver.save_file(shard, os.path.join(self._output_dir, shard_file))
 
         if index is None:
-            path_to_weights = os.path.join(self._output_dir, "model.safetensors")
+            path_to_weights = os.path.join(self._output_dir, self._output_file_name)
             logger.info("Model weights saved in (%s)", path_to_weights)
         else:
             save_index_file = os.path.join(
                 self._output_dir, "model.safetensors.index.json"
             )
             # Save the index as well
             with open(save_index_file, "w", encoding="utf-8") as f:
```

### Comparing `friendli_client-1.3.3/friendli/modules/converter/schema.py` & `friendli_client-1.3.4/friendli/modules/converter/schema.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/converter/utils.py` & `friendli_client-1.3.4/friendli/modules/converter/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
 ) -> Tuple[str, ...]:
     """Try to save `tokenizer.json` of a pretrained model."""
     if not os.path.isdir(save_dir):
         raise NotFoundError(f"Directory '{save_dir}' is not found.")
 
     tokenizer = get_tokenizer(model_name_or_path, cache_dir=cache_dir)
     saved_file_paths = tokenizer.save_pretrained(save_directory=save_dir)
-
     tokenizer_json_path = None
     for path in saved_file_paths:
         if "tokenizer.json" == os.path.basename(path):
             tokenizer_json_path = path
             break
 
     if tokenizer_json_path is None:
```

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/awq/base.py` & `friendli_client-1.3.4/friendli/modules/quantizer/awq/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/awq/models/gpt_neox.py` & `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/awq/models/gptj.py` & `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/gptj.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/awq/models/llama.py` & `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/llama.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/awq/models/mpt.py` & `friendli_client-1.3.4/friendli/modules/quantizer/awq/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/awq/utils.py` & `friendli_client-1.3.4/friendli/modules/quantizer/awq/utils.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/base.py` & `friendli_client-1.3.4/friendli/modules/quantizer/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/layers.py` & `friendli_client-1.3.4/friendli/modules/quantizer/layers.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/maps.py` & `friendli_client-1.3.4/friendli/modules/quantizer/maps.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/models/llama.py` & `friendli_client-1.3.4/friendli/modules/quantizer/models/llama.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/models/mixtral.py` & `friendli_client-1.3.4/friendli/modules/quantizer/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/models/mpt.py` & `friendli_client-1.3.4/friendli/modules/quantizer/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/schema/config.py` & `friendli_client-1.3.4/friendli/modules/quantizer/schema/config.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/schema/data.py` & `friendli_client-1.3.4/friendli/modules/quantizer/schema/data.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/base.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/bloom.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/bloom.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/codegen.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/codegen.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/falcon.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/falcon.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/gpt2.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/gpt_neox.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/gptj.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/gptj.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/llama.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/llama.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/mpt.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/mpt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/smoothquant/models/opt.py` & `friendli_client-1.3.4/friendli/modules/quantizer/smoothquant/models/opt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/modules/quantizer/utils.py` & `friendli_client-1.3.4/friendli/modules/quantizer/utils.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/chat/completions.py` & `friendli_client-1.3.4/friendli/schema/api/v1/chat/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/codegen/chat_completions_pb2.py` & `friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi` & `friendli_client-1.3.4/friendli/schema/api/v1/codegen/chat_completions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/codegen/completions_pb2.py` & `friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/codegen/completions_pb2.pyi` & `friendli_client-1.3.4/friendli/schema/api/v1/codegen/completions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/codegen/text_to_image_pb2.py` & `friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi` & `friendli_client-1.3.4/friendli/schema/api/v1/codegen/text_to_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/completions.py` & `friendli_client-1.3.4/friendli/schema/api/v1/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/images/image.py` & `friendli_client-1.3.4/friendli/schema/api/v1/images/image.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/proto/chat_completions.proto` & `friendli_client-1.3.4/friendli/schema/api/v1/proto/chat_completions.proto`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/api/v1/proto/completions.proto` & `friendli_client-1.3.4/friendli/schema/api/v1/proto/completions.proto`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/resource/v1/attributes.py` & `friendli_client-1.3.4/friendli/schema/resource/v1/attributes.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/resource/v1/endpoint.py` & `friendli_client-1.3.4/friendli/schema/resource/v1/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/schema/resource/v1/transfer.py` & `friendli_client-1.3.4/friendli/schema/resource/v1/transfer.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/api/base.py` & `friendli_client-1.3.4/friendli/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/api/chat/chat.py` & `friendli_client-1.3.4/friendli/sdk/api/chat/chat.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/api/chat/completions.py` & `friendli_client-1.3.4/friendli/sdk/api/chat/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/api/completions.py` & `friendli_client-1.3.4/friendli/sdk/api/completions.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/api/images/images.py` & `friendli_client-1.3.4/friendli/sdk/api/images/images.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/api/images/text_to_image.py` & `friendli_client-1.3.4/friendli/sdk/api/images/text_to_image.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/client.py` & `friendli_client-1.3.4/friendli/sdk/client.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/resource/base.py` & `friendli_client-1.3.4/friendli/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/resource/endpoint.py` & `friendli_client-1.3.4/friendli/sdk/resource/endpoint.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/sdk/resource/model.py` & `friendli_client-1.3.4/friendli/sdk/resource/model.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/settings.py` & `friendli_client-1.3.4/friendli/settings.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/compat.py` & `friendli_client-1.3.4/friendli/utils/compat.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/decorator.py` & `friendli_client-1.3.4/friendli/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/format.py` & `friendli_client-1.3.4/friendli/utils/format.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/fs.py` & `friendli_client-1.3.4/friendli/utils/fs.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/prompt.py` & `friendli_client-1.3.4/friendli/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/request.py` & `friendli_client-1.3.4/friendli/utils/request.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/testing.py` & `friendli_client-1.3.4/friendli/utils/testing.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/transfer.py` & `friendli_client-1.3.4/friendli/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/url.py` & `friendli_client-1.3.4/friendli/utils/url.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/validate.py` & `friendli_client-1.3.4/friendli/utils/validate.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/friendli/utils/version.py` & `friendli_client-1.3.4/friendli/utils/version.py`

 * *Files identical despite different names*

### Comparing `friendli_client-1.3.3/pyproject.toml` & `friendli_client-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "friendli-client"
-version = "1.3.3"
+version = "1.3.4"
 description = "Client of Friendli Suite."
 license = "Apache-2.0"
 authors = ["FriendliAI teams <eng@friendli.ai>"]
 packages = [
     { include = "friendli" },
 ]
 include = ["friendli/py.typed"]
```

### Comparing `friendli_client-1.3.3/PKG-INFO` & `friendli_client-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: friendli-client
-Version: 1.3.3
+Version: 1.3.4
 Summary: Client of Friendli Suite.
 Home-page: https://friendli.ai/
 License: Apache-2.0
 Keywords: generative-ai,serving,llm,inference,finetuning
 Author: FriendliAI teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: friendli-client Version: 1.3.3 Summary: Client of
+Metadata-Version: 2.1 Name: friendli-client Version: 1.3.4 Summary: Client of
 Friendli Suite. Home-page: https://friendli.ai/ License: Apache-2.0 Keywords:
 generative-ai,serving,llm,inference,finetuning Author: FriendliAI teams Author-
 email: eng@friendli.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
```

