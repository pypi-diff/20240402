# Comparing `tmp/botocore-a-la-carte-1.34.8.tar.gz` & `tmp/botocore-a-la-carte-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-1.34.8.tar", last modified: Wed Dec 27 01:07:04 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-1.34.9.tar", last modified: Thu Dec 28 01:07:05 2023, max compression
```

## Comparing `botocore-a-la-carte-1.34.8.tar` & `botocore-a-la-carte-1.34.9.tar`

### file list

```diff
@@ -1,1994 +1,1994 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.223362 botocore-a-la-carte-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-27 01:07:04.223362 botocore-a-la-carte-1.34.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-12-27 01:07:03.000000 botocore-a-la-carte-1.34.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.079362 botocore-a-la-carte-1.34.8/botocore/
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30640 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    43803 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    23156 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/awsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)   266617 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    51241 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/configloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    37230 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/configprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    84788 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.079362 botocore-a-la-carte-1.34.8/botocore/crt/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/crt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25318 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/crt/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.079362 botocore-a-la-carte-1.34.8/botocore/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2023-12-27 01:06:28.000000 botocore-a-la-carte-1.34.8/botocore/data/_retry.json
--rw-r--r--   0 runner    (1001) docker     (127)   837068 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/data/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/data/partitions.json
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/data/sdk-default-configuration.json
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.079362 botocore-a-la-carte-1.34.8/botocore/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/docstringparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/restdoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/style.py
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/method.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/sharedexample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/docs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    22934 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/errorfactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20449 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (127)    22804 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    54728 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    25060 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/httpchecksum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18582 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/httpsession.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20597 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    27392 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45607 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    32426 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore/retries/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/special.py
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retries/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    14700 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/retryhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33122 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    49184 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    30691 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/signers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15152 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)   135342 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13767 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore/vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/requests/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore/vendored/requests/packages/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/requests/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore/vendored/requests/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/requests/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/requests/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    34549 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/vendored/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/botocore/waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-27 01:07:03.000000 botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    91179 2023-12-27 01:07:04.000000 botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 01:07:03.000000 botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-27 01:07:03.000000 botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 01:07:03.000000 botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_static/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/_static/logos/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_static/logos/aws_dark_theme_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_static/logos/aws_light_theme_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   136184 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_static/shortbreadv1.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_templates/sidebar/close-icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/_templates/sidebar/feedback.html
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/client_upgrades.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9881 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.083362 botocore-a-la-carte-1.34.8/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/development/changesfor10.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/development/designnotes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/awsrequest.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/eventstream.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/response.rst
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/reference/stubber.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/docs/source/topics/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/topics/document_type.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/topics/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/topics/paginators.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21074 2023-12-27 01:07:04.223362 botocore-a-la-carte-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-27 01:07:03.000000 botocore-a-la-carte-1.34.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18817 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.043362 botocore-a-la-carte-1.34.8/tests/acceptance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.047362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/acm/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/acm/acm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/autoscaling/autoscaling.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudformation/cloudformation.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudfront/cloudfront.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudhsm/cloudhsm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudsearch/cloudsearch.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudtrail/cloudtrail.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudwatch/cloudwatch.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudwatchlogs/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cloudwatchlogs/cloudwatchlogs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/codecommit/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/codecommit/codecommit.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/codedeploy/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/codedeploy/codedeploy.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/codepipeline/codepipeline.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cognitosync/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cognitosync/cognitosync.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/configservice/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/configservice/configservice.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/datapipeline/datapipeline.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/devicefarm/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/devicefarm/devicefarm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/directconnect/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/directconnect/directconnect.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/directoryservice/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/directoryservice/directoryservice.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/dynamodb/dynamodb.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/dynamodbstreams/dynamodbstreams.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ec2/ec2.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ecs/ecs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/efs/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/efs/efs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elasticache/elasticache.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elasticbeanstalk/elasticbeanstalk.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.087362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elasticloadbalancing/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elasticloadbalancing/elasticloadbalancing.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/elastictranscoder/elastictranscoder.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/emr/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/emr/emr.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/es/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/es/es.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/glacier/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/glacier/glacier.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/iam/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/iam/iam.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/importexport/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/importexport/importexport.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/kinesis/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/kinesis/kinesis.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/kms/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/kms/kms.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/lambda/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/lambda/lambda.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/machinelearning/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/machinelearning/machinelearning.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/opsworks/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/opsworks/opsworks.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/rds/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/rds/rds.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/redshift/redshift.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/route53/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/route53/route53.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/route53domains/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/route53domains/route53domains.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ses/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ses/ses.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/sns/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/sns/sns.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/sqs/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/sqs/sqs.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/ssm/ssm.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/storagegateway/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/storagegateway/storagegateway.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/sts/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/sts/sts.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/support/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/support/support.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/swf/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/swf/swf.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/waf/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/waf/waf.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/workspaces/workspaces.feature
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.091362 botocore-a-la-carte-1.34.8/tests/acceptance/features/steps/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/acceptance/features/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/cmd-runner
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20184 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/profile-tests.json
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/crt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/crt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/csm/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/csm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32068 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/csm/cases.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.047362 botocore-a-la-carte-1.34.8/tests/functional/csm/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.047362 botocore-a-la-carte-1.34.8/tests/functional/csm/data/csmtest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/csm/data/csmtest/2018-06-19/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/csm/data/csmtest/2018-06-19/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/csm/test_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_glacier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_lex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_shared_example_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/docs/test_streaming_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.067362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)    22841 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/account/
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/account/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/acm/
--rw-r--r--   0 runner    (1001) docker     (127)    21886 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/acm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/acm-pca/
--rw-r--r--   0 runner    (1001) docker     (127)    22050 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amp/
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amp/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplify/
--rw-r--r--   0 runner    (1001) docker     (127)    18190 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    17633 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)    20036 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (127)    20036 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appconfig/
--rw-r--r--   0 runner    (1001) docker     (127)    21296 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (127)    20586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appfabric/
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.099362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appflow/
--rw-r--r--   0 runner    (1001) docker     (127)    16921 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appintegrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/application-autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)    21870 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/application-insights/
--rw-r--r--   0 runner    (1001) docker     (127)    20378 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appmesh/
--rw-r--r--   0 runner    (1001) docker     (127)    27442 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apprunner/
--rw-r--r--   0 runner    (1001) docker     (127)    13113 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appstream/
--rw-r--r--   0 runner    (1001) docker     (127)    16617 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appsync/
--rw-r--r--   0 runner    (1001) docker     (127)    19065 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/arc-zonal-shift/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/athena/
--rw-r--r--   0 runner    (1001) docker     (127)    21588 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/athena/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/auditmanager/
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)    20943 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/autoscaling-plans/
--rw-r--r--   0 runner    (1001) docker     (127)    20748 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/b2bi/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backup/
--rw-r--r--   0 runner    (1001) docker     (127)    20319 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backup/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backup-gateway/
--rw-r--r--   0 runner    (1001) docker     (127)    19742 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backupstorage/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/batch/
--rw-r--r--   0 runner    (1001) docker     (127)    21970 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/batch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bcm-data-exports/
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock/
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-agent/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-agent-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/billingconductor/
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/braket/
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/braket/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/budgets/
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ce/
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ce/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime/
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-identity/
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-media-pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-meetings/
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-messaging/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-voice/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cleanroomsml/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloud9/
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.103362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)    22851 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)    22794 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudfront-keyvaluestore/
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudtrail-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeartifact/
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codebuild/
--rw-r--r--   0 runner    (1001) docker     (127)    22152 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codecommit/
--rw-r--r--   0 runner    (1001) docker     (127)    22192 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codedeploy/
--rw-r--r--   0 runner    (1001) docker     (127)    22628 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguru-reviewer/
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguru-security/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (127)    20979 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar/
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar-connections/
--rw-r--r--   0 runner    (1001) docker     (127)    17324 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar-notifications/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-identity/
--rw-r--r--   0 runner    (1001) docker     (127)    19386 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-idp/
--rw-r--r--   0 runner    (1001) docker     (127)    19634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-sync/
--rw-r--r--   0 runner    (1001) docker     (127)    14934 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/comprehend/
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/compute-optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)    17680 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)    22442 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/config/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connect/
--rw-r--r--   0 runner    (1001) docker     (127)    15251 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connect-contact-lens/
--rw-r--r--   0 runner    (1001) docker     (127)    13647 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectcases/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectparticipant/
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.107362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/controltower/
--rw-r--r--   0 runner    (1001) docker     (127)    17946 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cost-optimization-hub/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cur/
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cur/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/customer-profiles/
--rw-r--r--   0 runner    (1001) docker     (127)    14392 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/databrew/
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dataexchange/
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (127)    12336 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datasync/
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datazone/
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dax/
--rw-r--r--   0 runner    (1001) docker     (127)    15954 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dax/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/detective/
--rw-r--r--   0 runner    (1001) docker     (127)    20995 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/detective/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/devicefarm/
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/devops-guru/
--rw-r--r--   0 runner    (1001) docker     (127)    14899 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/directconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    22318 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/discovery/
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dlm/
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dms/
--rw-r--r--   0 runner    (1001) docker     (127)    22724 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/docdb/
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/docdb-elastic/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/drs/
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/drs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ds/
--rw-r--r--   0 runner    (1001) docker     (127)    21848 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ds/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)    23714 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (127)    21894 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ebs/
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    24360 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ec2-instance-connect/
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecr/
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecr-public/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)    22320 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/efs/
--rw-r--r--   0 runner    (1001) docker     (127)    30883 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/efs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/eks/
--rw-r--r--   0 runner    (1001) docker     (127)    21884 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/eks/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/eks-auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elastic-inference/
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)    22662 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (127)    22443 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (127)    13747 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.111362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elb/
--rw-r--r--   0 runner    (1001) docker     (127)    60943 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elbv2/
--rw-r--r--   0 runner    (1001) docker     (127)    23058 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr/
--rw-r--r--   0 runner    (1001) docker     (127)    23324 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr-containers/
--rw-r--r--   0 runner    (1001) docker     (127)    19317 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr-serverless/
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/entityresolution/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/es/
--rw-r--r--   0 runner    (1001) docker     (127)    22276 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/es/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/events/
--rw-r--r--   0 runner    (1001) docker     (127)    27931 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/events/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/evidently/
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/finspace/
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/finspace-data/
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/firehose/
--rw-r--r--   0 runner    (1001) docker     (127)    22109 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fis/
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fis/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fms/
--rw-r--r--   0 runner    (1001) docker     (127)    27852 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/forecast/
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/forecastquery/
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/frauddetector/
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/freetier/
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fsx/
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/gamelift/
--rw-r--r--   0 runner    (1001) docker     (127)    19526 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/glacier/
--rw-r--r--   0 runner    (1001) docker     (127)    22919 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/glue/
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/glue/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/grafana/
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/greengrass/
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/groundstation/
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/guardduty/
--rw-r--r--   0 runner    (1001) docker     (127)    22142 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/health/
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/health/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/healthlake/
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/honeycode/
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iam/
--rw-r--r--   0 runner    (1001) docker     (127)    19907 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iam/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/identitystore/
--rw-r--r--   0 runner    (1001) docker     (127)    16697 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/importexport/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.115362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector/
--rw-r--r--   0 runner    (1001) docker     (127)    17418 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector-scan/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector2/
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot/
--rw-r--r--   0 runner    (1001) docker     (127)    20619 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-data/
--rw-r--r--   0 runner    (1001) docker     (127)    20951 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-jobs-data/
--rw-r--r--   0 runner    (1001) docker     (127)    21019 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-roborunner/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-roborunner/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot1click-devices/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot1click-projects/
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotevents/
--rw-r--r--   0 runner    (1001) docker     (127)    15723 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotevents-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (127)    17218 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (127)    21179 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotsitewise/
--rw-r--r--   0 runner    (1001) docker     (127)    17087 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotwireless/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivs/
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivs-realtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivschat/
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kafka/
--rw-r--r--   0 runner    (1001) docker     (127)    20270 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kendra/
--rw-r--r--   0 runner    (1001) docker     (127)    14778 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kendra-ranking/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/keyspaces/
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis/
--rw-r--r--   0 runner    (1001) docker     (127)    82124 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-archived-media/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-media/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-signaling/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.119362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kms/
--rw-r--r--   0 runner    (1001) docker     (127)    30432 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lakeformation/
--rw-r--r--   0 runner    (1001) docker     (127)    21882 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lambda/
--rw-r--r--   0 runner    (1001) docker     (127)    31675 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/launch-wizard/
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lex-models/
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lex-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lexv2-models/
--rw-r--r--   0 runner    (1001) docker     (127)    14969 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lexv2-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    14995 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager/
--rw-r--r--   0 runner    (1001) docker     (127)    22410 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager-linux-subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager-user-subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lightsail/
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/location/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/location/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/logs/
--rw-r--r--   0 runner    (1001) docker     (127)    22354 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/logs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/m2/
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/m2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/machinelearning/
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/macie2/
--rw-r--r--   0 runner    (1001) docker     (127)    20283 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/managedblockchain-query/
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-agreement/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-deployment/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-entitlement/
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplacecommerceanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (127)    20124 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/medialive/
--rw-r--r--   0 runner    (1001) docker     (127)    16980 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackage/
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackage-vod/
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediastore/
--rw-r--r--   0 runner    (1001) docker     (127)    14019 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediastore-data/
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.123362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediatailor/
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/medical-imaging/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/memorydb/
--rw-r--r--   0 runner    (1001) docker     (127)    18197 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (127)    20413 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mgh/
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mgn/
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migration-hub-refactor-spaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhub-config/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mobile/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mq/
--rw-r--r--   0 runner    (1001) docker     (127)    21851 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mq/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mturk/
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mwaa/
--rw-r--r--   0 runner    (1001) docker     (127)    16500 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptune/
--rw-r--r--   0 runner    (1001) docker     (127)    23114 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptune-graph/
--rw-r--r--   0 runner    (1001) docker     (127)    35316 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptunedata/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/network-firewall/
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/networkmonitor/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/nimble/
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/oam/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/oam/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/omics/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/omics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)    22279 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (127)    10849 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opsworks/
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (127)    14040 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)    16439 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/osis/
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/osis/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/outposts/
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/panorama/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/payment-cryptography/
--rw-r--r--   0 runner    (1001) docker     (127)    10938 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/payment-cryptography-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pca-connector-ad/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize/
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize-events/
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.127362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pi/
--rw-r--r--   0 runner    (1001) docker     (127)    19304 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint/
--rw-r--r--   0 runner    (1001) docker     (127)    16135 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-email/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-sms-voice/
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/
--rw-r--r--   0 runner    (1001) docker     (127)    14862 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/polly/
--rw-r--r--   0 runner    (1001) docker     (127)    20690 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/polly/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pricing/
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/proton/
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/proton/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qbusiness/
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qconnect/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qldb/
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qldb-session/
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ram/
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ram/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rbin/
--rw-r--r--   0 runner    (1001) docker     (127)    18942 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rds/
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rds/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rds-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)    22964 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift-data/
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift-serverless/
--rw-r--r--   0 runner    (1001) docker     (127)    15116 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rekognition/
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/repostspace/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resource-explorer-2/
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resource-groups/
--rw-r--r--   0 runner    (1001) docker     (127)    22400 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/robomaker/
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (127)    18406 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53/
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-cluster/
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-control-config/
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-readiness/
--rw-r--r--   0 runner    (1001) docker     (127)    10826 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53domains/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53resolver/
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rum/
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rum/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.131362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3/
--rw-r--r--   0 runner    (1001) docker     (127)   316784 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3control/
--rw-r--r--   0 runner    (1001) docker     (127)   139555 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3outposts/
--rw-r--r--   0 runner    (1001) docker     (127)    19194 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (127)    21882 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-a2i-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-edge/
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-geospatial/
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    22040 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/savingsplans/
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sdb/
--rw-r--r--   0 runner    (1001) docker     (127)    14829 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (127)    22819 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/securityhub/
--rw-r--r--   0 runner    (1001) docker     (127)    22238 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/securitylake/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (127)    19316 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/service-quotas/
--rw-r--r--   0 runner    (1001) docker     (127)    20579 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (127)    22367 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicecatalog-appregistry/
--rw-r--r--   0 runner    (1001) docker     (127)    22417 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (127)    22005 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ses/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ses/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sesv2/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/shield/
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/shield/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/signer/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/signer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sms/
--rw-r--r--   0 runner    (1001) docker     (127)    21030 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sms/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sms-voice/
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/snow-device-management/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/snowball/
--rw-r--r--   0 runner    (1001) docker     (127)    26886 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sns/
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sns/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.135362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sqs/
--rw-r--r--   0 runner    (1001) docker     (127)    21883 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-contacts/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-incidents/
--rw-r--r--   0 runner    (1001) docker     (127)    17107 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-sap/
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso/
--rw-r--r--   0 runner    (1001) docker     (127)    18738 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso-admin/
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso-oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    18528 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    22447 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/storagegateway/
--rw-r--r--   0 runner    (1001) docker     (127)    22807 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sts/
--rw-r--r--   0 runner    (1001) docker     (127)    43190 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sts/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/support/
--rw-r--r--   0 runner    (1001) docker     (127)    16259 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/support/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/support-app/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/swf/
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/swf/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/synthetics/
--rw-r--r--   0 runner    (1001) docker     (127)    22195 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/textract/
--rw-r--r--   0 runner    (1001) docker     (127)    18248 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/textract/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/timestream-query/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/timestream-write/
--rw-r--r--   0 runner    (1001) docker     (127)    11561 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/tnb/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/transcribe/
--rw-r--r--   0 runner    (1001) docker     (127)    21332 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/transfer/
--rw-r--r--   0 runner    (1001) docker     (127)    22106 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/translate/
--rw-r--r--   0 runner    (1001) docker     (127)    18708 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/translate/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/trustedadvisor/
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/voice-id/
--rw-r--r--   0 runner    (1001) docker     (127)    13102 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/vpc-lattice/
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/waf/
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/waf/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/waf-regional/
--rw-r--r--   0 runner    (1001) docker     (127)    30573 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wafv2/
--rw-r--r--   0 runner    (1001) docker     (127)    30139 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (127)    18030 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wisdom/
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workdocs/
--rw-r--r--   0 runner    (1001) docker     (127)    13118 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/worklink/
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workmail/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workmailmessageflow/
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.139362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces-thin-client/
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces-web/
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/xray/
--rw-r--r--   0 runner    (1001) docker     (127)    21937 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/xray/endpoint-tests-1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/leak/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/leak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/leak/test_resource_leaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.067362 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    57976 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/waiters-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    77688 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/sdk-default-configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.067362 botocore-a-la-carte-1.34.8/tests/functional/models/test-discovery-endpoint/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/models/test-discovery-endpoint/2020-08-20/
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/retries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/retries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/retries/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/retries/test_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_client_class_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_client_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_cloudsearchdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_cognito_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    19034 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_context_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    44025 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_docdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_endpoint_rulesets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_event_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_eventbridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_h2_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_importexport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_iot_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_kinesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_lex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_machinelearning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_model_backcompat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_model_completeness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_modeled_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_paginator_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_public_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (127)    28286 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_response_shadowing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14043 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (127)   131506 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_s3_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_s3_control_redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_s3express.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_service_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_service_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_six_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_six_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14292 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_tagged_unions_unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/test_waiter_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/functional/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/functional/utils/credentialprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.143362 botocore-a-la-carte-1.34.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test-credentials
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_client_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_cognito_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_elastictranscoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_emr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_glacier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (127)    53990 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12697 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/integration/test_waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.authz
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.creq
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.req
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-multiline/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.authz
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.creq
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.req
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-order/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.authz
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.creq
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.req
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.151362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-trim/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.authz
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.creq
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.req
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-unreserved/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.authz
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.creq
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.req
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-utf8/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.authz
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.creq
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.req
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.creq
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.req
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.authz
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.creq
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.req
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.creq
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.req
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.authz
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.creq
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.req
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.authz
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.creq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.req
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.155362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.authz
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.creq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.req
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.authz
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.creq
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.req
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.authz
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.creq
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.req
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.authz
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.creq
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.req
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.authz
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.creq
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.req
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.creq
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.req
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.creq
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.req
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.req
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.authz
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.creq
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.req
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.159362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.authz
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.creq
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.req
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.authz
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.creq
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.req
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-space/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.authz
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.creq
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.req
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.authz
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.creq
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.req
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sts
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-case/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.authz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.req
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-sort/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.authz
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.creq
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.req
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-value-case/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.authz
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.creq
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.req
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.authz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.req
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.163362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.authz
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.req
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sts
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.authz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.creq
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.req
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.authz
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.creq
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.req
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-query/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.authz
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.creq
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.req
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.authz
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.creq
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.req
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.authz
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.creq
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.req
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sreq
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sts
--rw-r--r--   0 runner    (1001) docker     (127)    45993 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/test_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/auth/test_sigv4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_bad_profile
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_bad
--rw-r--r--   0 runner    (1001) docker     (127)    51200 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_badbytes
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_nested
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_nested_bad
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_nocreds
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_other
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_credentials
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_services_config
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_sso_session_config
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_third_config
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/boto_config
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/boto_config_empty
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/cfg/foo_config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/crt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/crt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.167362 botocore-a-la-carte-1.34.8/tests/unit/crt/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/crt/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/crt/auth/test_crt_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/crt/auth/test_crt_sigv4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.071362 botocore-a-la-carte-1.34.8/tests/unit/data/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/aws/s3/2006-03-01.normal.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/baz.json
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/compressed.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.071362 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/aws-region.json
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/default-values.json
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/eventbridge.json
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/fns.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/headers.json
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/local-region-override.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/parse-arn.json
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/parse-url.json
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/partition-fn.json
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/uri-encode.json
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/valid-hostlabel.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/aws-region.json
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/default-values.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/deprecated-param.json
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/eventbridge.json
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/fns.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/headers.json
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/local-region-override.json
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/parse-arn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/parse-url.json
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/partition-fn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/uri-encode.json
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/foo.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/non_ascii.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data/someservice/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/someservice/2012-10-01.normal.json
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/someservice/2013-08-21.normal.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data/sub/fie.normal.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.071362 botocore-a-la-carte-1.34.8/tests/unit/data_overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.171362 botocore-a-la-carte-1.34.8/tests/unit/data_overrides/someservice/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/data_overrides/someservice/2012-10-01.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/test_docstringparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/test_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13495 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_sharedexample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/docs/test_waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.071362 botocore-a-la-carte-1.34.8/tests/unit/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/protocols/input/
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/input/ec2.json
--rw-r--r--   0 runner    (1001) docker     (127)    21711 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/input/json.json
--rw-r--r--   0 runner    (1001) docker     (127)    23390 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/input/query.json
--rw-r--r--   0 runner    (1001) docker     (127)    51262 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/input/rest-json.json
--rw-r--r--   0 runner    (1001) docker     (127)    46773 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/input/rest-xml.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/protocols/output/
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/output/ec2.json
--rw-r--r--   0 runner    (1001) docker     (127)    19354 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/output/json.json
--rw-r--r--   0 runner    (1001) docker     (127)    23397 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/output/query.json
--rw-r--r--   0 runner    (1001) docker     (127)    29610 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/output/rest-json.json
--rw-r--r--   0 runner    (1001) docker     (127)    31012 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/protocols/output/rest-xml.json
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/put_object_data
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.071362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/datapipeline-create-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/directconnect-delete-connection.json
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/dynamodb-put-item.json
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/elastictranscoder-delete-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/opsworks-delete-stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/storagegateway-delete-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/errors/swf-deprecate-domain.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.175362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/datapipeline-create-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/directconnect-delete-connection.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/dynamodb-put-item.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/elastictranscoder-delete-pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/opsworks-delete-stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/storagegateway-delete-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/swf-deprecate-domain.json
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/test_response_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.071362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.179362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.xml
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.xml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.xml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/ec2-describe-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/ec2-describe-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.xml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/iam-get-user.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/iam-get-user.xml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/importexport-get-status.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/importexport-get-status.xml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.xml
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/s3-create-bucket.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/s3-create-bucket.xml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/s3-list-objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/s3-list-objects.xml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/ses-delete-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/ses-delete-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/sns-delete-topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/sns-delete-topic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/sqs-delete-queue.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/sts-get-session-token.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/errors/sts-get-session-token.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.223362 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.xml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.json
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.xml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.xml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.xml
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.json
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.xml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.json
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.xml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21940 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json
--rw-r--r--   0 runner    (1001) docker     (127)    22671 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-allocate-address.json
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-allocate-address.xml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.json
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.xml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-associate-address.json
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-associate-address.xml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.xml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-attach-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-attach-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.xml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-route-table.json
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.xml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-subnet.json
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-subnet.xml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-vpc.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-vpc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.json
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.xml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.xml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml
--rw-r--r--   0 runner    (1001) docker     (127)   248956 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json
--rw-r--r--   0 runner    (1001) docker     (127)   314117 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.json
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-tags.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-tags.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.json
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.json
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.json
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.xml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-detach-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-detach-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-get-password-data.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-get-password-data.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.xml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-volume.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.xml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-register-image.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-register-image.xml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.json
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.xml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-run-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-start-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-start-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-stop-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-stop-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.xml
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.json
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.json
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.json
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.xml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.json
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.json
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.json
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.json
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json
--rw-r--r--   0 runner    (1001) docker     (127)    19095 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json
--rw-r--r--   0 runner    (1001) docker     (127)    22855 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.json
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.xml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-user.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-user.xml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-access-keys.json
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.xml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-roles.json
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-roles.xml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-users.json
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-users.xml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/importexport-list-jobs.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-events.json
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-events.xml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.json
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-events.json
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-resize.json
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-resize.xml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.json
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.json
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.json
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.json
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.xml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.json
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-buckets.json
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.json
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-objects.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-delete-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-delete-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-send-quota.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-send-quota.xml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.json
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-list-identities.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-list-identities.xml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-send-email.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-send-email.xml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-send-raw-email.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-send-raw-email.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.xml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.xml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-add-permission.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-add-permission.xml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.xml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-create-topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-create-topic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-topics.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-topics.xml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-publish.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-publish.xml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-subscribe.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-subscribe.xml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-add-permission.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-change-message-visibility-batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-create-queue.json
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-delete-message-batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-get-queue-url.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-list-queues.json
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-receive-message.json
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-send-message-batch.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-send-message.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sts-get-session-token.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:07:04.223362 botocore-a-la-carte-1.34.8/tests/unit/retries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/test_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/test_special.py
--rw-r--r--   0 runner    (1001) docker     (127)    26367 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/retries/test_throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    35112 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_auth_bearer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_auth_sigv4.py
--rw-r--r--   0 runner    (1001) docker     (127)    30747 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_awsrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    93962 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)    39978 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_configloader.py
--rw-r--r--   0 runner    (1001) docker     (127)   138173 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    20712 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    18355 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_endpoint_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_errorfactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15485 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_eventstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    63533 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    27457 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_http_client_exception_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19734 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_http_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    27402 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_httpchecksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_idempotency.py
--rw-r--r--   0 runner    (1001) docker     (127)    19334 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    47606 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35401 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    57408 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)    58705 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17041 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    50089 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_retryhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_s3_addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19004 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    40231 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    35824 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_session_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    43689 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)   126991 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33648 2023-12-27 01:06:29.000000 botocore-a-la-carte-1.34.8/tests/unit/test_waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.902469 botocore-a-la-carte-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-28 01:07:05.902469 botocore-a-la-carte-1.34.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.758468 botocore-a-la-carte-1.34.9/botocore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30640 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43803 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23156 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266617 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    51241 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/configloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37230 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/configprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84788 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.758468 botocore-a-la-carte-1.34.9/botocore/crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/crt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25318 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/crt/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.758468 botocore-a-la-carte-1.34.9/botocore/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/data/_retry.json
+-rw-r--r--   0 runner    (1001) docker     (127)   838376 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/data/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/data/partitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/data/sdk-default-configuration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.758468 botocore-a-la-carte-1.34.9/botocore/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/docstringparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/restdoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/sharedexample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/docs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16441 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22934 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/endpoint_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/errorfactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20449 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22804 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54728 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25060 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/httpchecksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18582 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/httpsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20597 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27392 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45607 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32426 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retries/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/retryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33122 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49184 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30691 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15152 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135342 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13767 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore/vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/requests/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore/vendored/requests/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/requests/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore/vendored/requests/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/requests/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/requests/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/vendored/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/botocore/waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    91179 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_static/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/_static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_static/logos/aws_dark_theme_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_static/logos/aws_light_theme_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   136184 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_static/shortbreadv1.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.762468 botocore-a-la-carte-1.34.9/docs/source/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_templates/sidebar/close-icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/_templates/sidebar/feedback.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/client_upgrades.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9881 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/development/changesfor10.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/development/designnotes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/awsrequest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/eventstream.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/response.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/reference/stubber.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/docs/source/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/topics/document_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/topics/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/topics/paginators.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21074 2023-12-28 01:07:05.906469 botocore-a-la-carte-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-28 01:07:05.000000 botocore-a-la-carte-1.34.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18817 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.722468 botocore-a-la-carte-1.34.9/tests/acceptance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.726467 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/acm/acm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/autoscaling/autoscaling.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudformation/cloudformation.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudfront/cloudfront.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudhsm/cloudhsm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudsearch/cloudsearch.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudtrail/cloudtrail.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudwatch/cloudwatch.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudwatchlogs/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cloudwatchlogs/cloudwatchlogs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/codecommit/codecommit.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/codedeploy/codedeploy.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/codepipeline/codepipeline.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cognitosync/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cognitosync/cognitosync.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/configservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/configservice/configservice.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/datapipeline/datapipeline.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/devicefarm/devicefarm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/directconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/directconnect/directconnect.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/directoryservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/directoryservice/directoryservice.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/dynamodb/dynamodb.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/dynamodbstreams/dynamodbstreams.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ec2/ec2.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ecs/ecs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/efs/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/efs/efs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.766468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elasticache/elasticache.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elasticbeanstalk/elasticbeanstalk.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elasticloadbalancing/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elasticloadbalancing/elasticloadbalancing.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/elastictranscoder/elastictranscoder.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/emr/emr.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/es/es.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/glacier/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/glacier/glacier.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/iam/iam.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/importexport/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/importexport/importexport.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/kinesis/kinesis.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/kms/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/kms/kms.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/lambda/lambda.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/machinelearning/machinelearning.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/opsworks/opsworks.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/rds/rds.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/redshift/redshift.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/route53/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/route53/route53.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/route53domains/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/route53domains/route53domains.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ses/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ses/ses.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/sns/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/sns/sns.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/sqs/sqs.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/ssm/ssm.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/storagegateway/storagegateway.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/sts/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/sts/sts.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/support/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/support/support.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/swf/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/swf/swf.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/waf/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/waf/waf.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/workspaces/workspaces.feature
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.770468 botocore-a-la-carte-1.34.9/tests/acceptance/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/acceptance/features/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/cmd-runner
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20184 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/profile-tests.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/crt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/crt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/csm/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/csm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32068 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/csm/cases.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.726467 botocore-a-la-carte-1.34.9/tests/functional/csm/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.726467 botocore-a-la-carte-1.34.9/tests/functional/csm/data/csmtest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/csm/data/csmtest/2018-06-19/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/csm/data/csmtest/2018-06-19/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/csm/test_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_glacier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_shared_example_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/docs/test_streaming_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.746468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)    22841 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/account/
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/account/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)    21886 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/acm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/acm-pca/
+-rw-r--r--   0 runner    (1001) docker     (127)    22050 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amp/
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amp/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplify/
+-rw-r--r--   0 runner    (1001) docker     (127)    18190 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    17633 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)    20036 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20036 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.778468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)    21296 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    20586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appfabric/
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    16921 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/application-autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)    21870 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/application-insights/
+-rw-r--r--   0 runner    (1001) docker     (127)    20378 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appmesh/
+-rw-r--r--   0 runner    (1001) docker     (127)    27442 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apprunner/
+-rw-r--r--   0 runner    (1001) docker     (127)    13113 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appstream/
+-rw-r--r--   0 runner    (1001) docker     (127)    16617 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appsync/
+-rw-r--r--   0 runner    (1001) docker     (127)    19065 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/arc-zonal-shift/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)    21588 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/athena/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)    20943 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/autoscaling-plans/
+-rw-r--r--   0 runner    (1001) docker     (127)    20748 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/b2bi/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)    20319 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backup/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backup-gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)    19742 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)    21970 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/batch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bcm-data-exports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock/
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-agent/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-agent-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/braket/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/budgets/
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ce/
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ce/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime/
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-identity/
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-media-pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-meetings/
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.782468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-voice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cleanroomsml/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloud9/
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)    22851 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)    22794 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudfront-keyvaluestore/
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudtrail-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codebuild/
+-rw-r--r--   0 runner    (1001) docker     (127)    22152 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (127)    22192 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (127)    22628 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguru-reviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguru-security/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar/
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar-connections/
+-rw-r--r--   0 runner    (1001) docker     (127)    17324 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar-notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-identity/
+-rw-r--r--   0 runner    (1001) docker     (127)    19386 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-idp/
+-rw-r--r--   0 runner    (1001) docker     (127)    19634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-sync/
+-rw-r--r--   0 runner    (1001) docker     (127)    14934 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/comprehend/
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/compute-optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    17680 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    22442 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/config/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.786468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connect-contact-lens/
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectcases/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectparticipant/
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/controltower/
+-rw-r--r--   0 runner    (1001) docker     (127)    17946 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cost-optimization-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cur/
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cur/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/customer-profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    14392 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/databrew/
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datasync/
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datazone/
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dax/
+-rw-r--r--   0 runner    (1001) docker     (127)    15954 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dax/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/detective/
+-rw-r--r--   0 runner    (1001) docker     (127)    20995 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/detective/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/devops-guru/
+-rw-r--r--   0 runner    (1001) docker     (127)    14899 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/directconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    22318 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dlm/
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dms/
+-rw-r--r--   0 runner    (1001) docker     (127)    22724 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/docdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/docdb-elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/drs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ds/
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ds/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    23714 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (127)    21894 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ebs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    24360 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ec2-instance-connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecr/
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecr-public/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22320 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/efs/
+-rw-r--r--   0 runner    (1001) docker     (127)    30883 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/efs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.790468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)    21884 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/eks/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/eks-auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elastic-inference/
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)    22662 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (127)    22443 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elb/
+-rw-r--r--   0 runner    (1001) docker     (127)    60943 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elbv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    23058 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)    23324 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr-containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19317 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr-serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/es/
+-rw-r--r--   0 runner    (1001) docker     (127)    22276 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/es/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/events/
+-rw-r--r--   0 runner    (1001) docker     (127)    27931 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/events/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/evidently/
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/finspace/
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/finspace-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/firehose/
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fis/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fms/
+-rw-r--r--   0 runner    (1001) docker     (127)    27852 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)    15258 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/forecastquery/
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/freetier/
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fsx/
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/gamelift/
+-rw-r--r--   0 runner    (1001) docker     (127)    19526 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/glacier/
+-rw-r--r--   0 runner    (1001) docker     (127)    22919 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/glue/
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/glue/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/grafana/
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/greengrass/
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/groundstation/
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/guardduty/
+-rw-r--r--   0 runner    (1001) docker     (127)    22142 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/health/
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/health/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.794468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/healthlake/
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/honeycode/
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)    19907 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iam/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/identitystore/
+-rw-r--r--   0 runner    (1001) docker     (127)    16697 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/importexport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector/
+-rw-r--r--   0 runner    (1001) docker     (127)    17418 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector-scan/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot/
+-rw-r--r--   0 runner    (1001) docker     (127)    20619 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    20951 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-jobs-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-roborunner/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-roborunner/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot1click-devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot1click-projects/
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotevents/
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotevents-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotfleethub/
+-rw-r--r--   0 runner    (1001) docker     (127)    17218 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (127)    21179 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotsitewise/
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivs-realtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivschat/
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)    20270 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kendra/
+-rw-r--r--   0 runner    (1001) docker     (127)    14778 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kendra-ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (127)    82124 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.798468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-archived-media/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-media/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-signaling/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    20264 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20264 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kms/
+-rw-r--r--   0 runner    (1001) docker     (127)    30432 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (127)    21882 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)    31675 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/launch-wizard/
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lex-models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lex-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lexv2-models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lexv2-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    14995 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager-linux-subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager-user-subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lightsail/
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/location/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/location/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22354 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/logs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutequipment/
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/m2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/m2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/macie2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20283 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/managedblockchain-query/
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-agreement/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-entitlement/
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplacecommerceanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)    20124 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.802468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/medialive/
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackage-vod/
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    14019 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediastore-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/medical-imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/memorydb/
+-rw-r--r--   0 runner    (1001) docker     (127)    18197 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (127)    20413 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mgh/
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mgn/
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migration-hub-refactor-spaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhub-config/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mobile/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mq/
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mq/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mturk/
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mwaa/
+-rw-r--r--   0 runner    (1001) docker     (127)    16500 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptune/
+-rw-r--r--   0 runner    (1001) docker     (127)    23114 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptune-graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    35316 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptunedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/network-firewall/
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/networkmonitor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/nimble/
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/oam/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/oam/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/omics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/omics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)    22279 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)    16439 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/osis/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/osis/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)    21656 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.806468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/panorama/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/payment-cryptography/
+-rw-r--r--   0 runner    (1001) docker     (127)    10938 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/payment-cryptography-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pca-connector-ad/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize/
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize-events/
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pi/
+-rw-r--r--   0 runner    (1001) docker     (127)    19304 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-email/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-sms-voice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)    14862 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/polly/
+-rw-r--r--   0 runner    (1001) docker     (127)    20690 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/polly/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/proton/
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/proton/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qbusiness/
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qldb/
+-rw-r--r--   0 runner    (1001) docker     (127)    16004 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qldb-session/
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ram/
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ram/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rbin/
+-rw-r--r--   0 runner    (1001) docker     (127)    18942 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rds/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rds-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift-serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)    15116 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rekognition/
+-rw-r--r--   0 runner    (1001) docker     (127)    18365 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/repostspace/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resource-explorer-2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resource-groups/
+-rw-r--r--   0 runner    (1001) docker     (127)    22400 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/robomaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.810468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (127)    18406 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53/
+-rw-r--r--   0 runner    (1001) docker     (127)    19968 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-control-config/
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-readiness/
+-rw-r--r--   0 runner    (1001) docker     (127)    10826 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53domains/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rum/
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rum/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)   316784 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3control/
+-rw-r--r--   0 runner    (1001) docker     (127)   139555 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3outposts/
+-rw-r--r--   0 runner    (1001) docker     (127)    19194 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    21882 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-a2i-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-edge/
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-geospatial/
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    22040 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/savingsplans/
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    14829 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22819 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/securityhub/
+-rw-r--r--   0 runner    (1001) docker     (127)    22238 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/securitylake/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)    19316 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/service-quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20579 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    22367 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicecatalog-appregistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    22417 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (127)    22005 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ses/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ses/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.814468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sesv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/shield/
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/shield/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/signer/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/signer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)    21030 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sms/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sms-voice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/snow-device-management/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/snowball/
+-rw-r--r--   0 runner    (1001) docker     (127)    26886 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sns/
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sns/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sqs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21883 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-contacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-incidents/
+-rw-r--r--   0 runner    (1001) docker     (127)    17107 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-sap/
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso/
+-rw-r--r--   0 runner    (1001) docker     (127)    18738 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso-admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso-oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    18528 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    22447 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (127)    22807 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sts/
+-rw-r--r--   0 runner    (1001) docker     (127)    43190 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sts/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/support/
+-rw-r--r--   0 runner    (1001) docker     (127)    16259 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/support/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/support-app/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/swf/
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/swf/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/synthetics/
+-rw-r--r--   0 runner    (1001) docker     (127)    22195 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/textract/
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/textract/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/timestream-query/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/timestream-write/
+-rw-r--r--   0 runner    (1001) docker     (127)    11561 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/tnb/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)    21332 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)    22106 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)    18708 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/translate/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/trustedadvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/voice-id/
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/vpc-lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/waf/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/waf/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.818468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/waf-regional/
+-rw-r--r--   0 runner    (1001) docker     (127)    30573 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wafv2/
+-rw-r--r--   0 runner    (1001) docker     (127)    30139 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (127)    18030 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wisdom/
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/worklink/
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workmail/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workmailmessageflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces-thin-client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10570 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces-web/
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/xray/
+-rw-r--r--   0 runner    (1001) docker     (127)    21937 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/xray/endpoint-tests-1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/leak/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/leak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/leak/test_resource_leaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.746468 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    57976 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/waiters-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77688 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/sdk-default-configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.746468 botocore-a-la-carte-1.34.9/tests/functional/models/test-discovery-endpoint/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/models/test-discovery-endpoint/2020-08-20/
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/retries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/retries/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/retries/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_client_class_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_client_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_cloudsearchdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_cognito_idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19034 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_context_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44025 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_docdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_endpoint_rulesets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_event_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_eventbridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_h2_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_importexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_iot_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_machinelearning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_model_backcompat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_model_completeness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_modeled_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_paginator_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_public_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28286 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_response_shadowing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14043 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131506 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_s3_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_s3_control_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_s3express.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_service_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_service_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_six_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_six_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14292 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_tagged_unions_unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/test_waiter_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.822468 botocore-a-la-carte-1.34.9/tests/functional/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/functional/utils/credentialprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.826468 botocore-a-la-carte-1.34.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test-credentials
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_client_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_cognito_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14122 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_elastictranscoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_emr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_glacier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53990 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/integration/test_waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.830468 botocore-a-la-carte-1.34.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.830468 botocore-a-la-carte-1.34.9/tests/unit/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.830468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.830468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.req
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-key-duplicate/get-header-key-duplicate.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.830468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-multiline/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.req
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-multiline/get-header-value-multiline.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-order/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.req
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-order/get-header-value-order.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-trim/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.req
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-header-value-trim/get-header-value-trim.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-unreserved/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.req
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-unreserved/get-unreserved.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-utf8/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.req
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-utf8/get-utf8.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.req
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla/get-vanilla.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.req
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-empty-query-key/get-vanilla-empty-query-key.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.req
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query/get-vanilla-query.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.834468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.req
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-encoded/get-vanilla-query-order-encoded.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.req
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key/get-vanilla-query-order-key.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.req
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-key-case/get-vanilla-query-order-key-case.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.req
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-order-value/get-vanilla-query-order-value.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.req
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-query-unreserved/get-vanilla-query-unreserved.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.req
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-utf8-query/get-vanilla-utf8-query.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.req
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/get-vanilla-with-session-token/get-vanilla-with-session-token.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.req
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative/get-relative.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.req
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-relative-relative/get-relative-relative.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.838468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.req
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash/get-slash.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.req
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-dot-slash/get-slash-dot-slash.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.req
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slash-pointless-dot/get-slash-pointless-dot.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.req
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-slashes/get-slashes.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-space/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.req
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-space/get-space.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.req
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/get-special-character/get-special-character.sts
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-case/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.req
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-case/post-header-key-case.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-sort/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.req
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-key-sort/post-header-key-sort.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-value-case/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.req
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-header-value-case/post-header-value-case.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.842468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.req
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.req
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sts
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.req
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla/post-vanilla.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.req
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-empty-query-value/post-vanilla-empty-query-value.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-query/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.creq
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.req
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-vanilla-query/post-vanilla-query.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.req
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded/post-x-www-form-urlencoded.sts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.846468 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.authz
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.creq
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.req
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sreq
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-x-www-form-urlencoded-parameters/post-x-www-form-urlencoded-parameters.sts
+-rw-r--r--   0 runner    (1001) docker     (127)    45993 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/test_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/auth/test_sigv4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_bad_profile
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_bad
+-rw-r--r--   0 runner    (1001) docker     (127)    51200 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_badbytes
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_nested
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_nested_bad
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_nocreds
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_other
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_credentials
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_services_config
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_sso_session_config
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_third_config
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/boto_config
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/boto_config_empty
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/cfg/foo_config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/crt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/crt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/crt/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/crt/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/crt/auth/test_crt_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/crt/auth/test_crt_sigv4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.750468 botocore-a-la-carte-1.34.9/tests/unit/data/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/data/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/aws/s3/2006-03-01.normal.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/baz.json
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/compressed.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.750468 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/aws-region.json
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/default-values.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/eventbridge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/fns.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/headers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/local-region-override.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/parse-arn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/parse-url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/partition-fn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/uri-encode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/valid-hostlabel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.850468 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/aws-region.json
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/default-values.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/deprecated-param.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/eventbridge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/fns.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/headers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/local-region-override.json
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/parse-arn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/parse-url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/partition-fn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/uri-encode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/foo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/non_ascii.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/data/someservice/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/someservice/2012-10-01.normal.json
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/someservice/2013-08-21.normal.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/data/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data/sub/fie.normal.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.750468 botocore-a-la-carte-1.34.9/tests/unit/data_overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/data_overrides/someservice/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/data_overrides/someservice/2012-10-01.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2023-12-28 01:06:26.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/test_docstringparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/test_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_sharedexample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/docs/test_waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.750468 botocore-a-la-carte-1.34.9/tests/unit/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/protocols/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/input/ec2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21711 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/input/json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23390 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/input/query.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51262 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/input/rest-json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46773 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/input/rest-xml.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/protocols/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/output/ec2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/output/json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23397 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/output/query.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29610 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/output/rest-json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31012 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/protocols/output/rest-xml.json
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/put_object_data
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.854468 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.750468 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.858468 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/datapipeline-create-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/directconnect-delete-connection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/dynamodb-put-item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/elastictranscoder-delete-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/opsworks-delete-stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/storagegateway-delete-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/errors/swf-deprecate-domain.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.858468 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/datapipeline-create-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/directconnect-delete-connection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/dynamodb-put-item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/elastictranscoder-delete-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/opsworks-delete-stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/storagegateway-delete-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/swf-deprecate-domain.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/test_response_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.750468 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.858468 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/autoscaling-delete-policy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/cloudformation-cancel-update-stack.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/cloudwatch-describe-alarm-history.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/ec2-describe-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/ec2-describe-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/elb-describe-load-balancers.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/iam-get-user.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/iam-get-user.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/importexport-get-status.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/importexport-get-status.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/rds-describe-db-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/route53-get-hosted-zone.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/s3-create-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/s3-create-bucket.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/s3-list-objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/s3-list-objects.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/ses-delete-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/ses-delete-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/sns-delete-topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/sns-delete-topic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/sqs-delete-queue.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/sts-get-session-token.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/errors/sts-get-session-token.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.902469 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-launch-configurations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-notification-configurations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-policies.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-activities.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scheduled-actions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-tags.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-describe-stacks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-list-stacks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-cloud-front-origin-access-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarm-history.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-describe-alarms.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21940 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22671 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-allocate-address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-allocate-address.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-assign-private-ip-addresses.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-associate-address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-associate-address.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-associate-route-table.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-attach-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-attach-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-attach-vpn-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-spot-instance-requests.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-confirm-product-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-copy-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-customer-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-route-table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-spot-datafeed-subscription.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-subnet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-subnet.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-vpc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-vpc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-vpn-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-delete-internet-gateway.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-customer-gateways.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instance-attribute.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-key-pairs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-placement-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   248956 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json
+-rw-r--r--   0 runner    (1001) docker     (127)   314117 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-tags.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.json
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.json
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-detach-network-interface.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-detach-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-detach-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-get-password-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-get-password-data.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-key-pair.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-modify-snapshot-attribute.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-monitor-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-register-image.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-register-image.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.json
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-replace-network-acl-association.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-run-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-start-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-start-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-stop-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-stop-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-check-dns-availability.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-storage-location.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-delete-application.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.json
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22855 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancers.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-user.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-user.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-access-keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-account-aliases.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-mfa-devices.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-roles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-roles.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-users.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-users.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/importexport-list-jobs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-event-subscriptions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-events.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-events.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-events.json
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-resize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-resize.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.json
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.json
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-location.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-policy.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-buckets.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-objects.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-delete-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-delete-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-send-quota.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-send-quota.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-list-identities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-list-identities.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-send-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-send-email.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-send-raw-email.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-send-raw-email.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-set-identity-dkim-enabled.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-verify-domain-dkim.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-verify-domain-identity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-add-permission.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-add-permission.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-confirm-subscription.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-create-topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-create-topic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-topics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-topics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-publish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-publish.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-subscribe.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-subscribe.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-add-permission.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-change-message-visibility-batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-create-queue.json
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-delete-message-batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-get-queue-url.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-list-queues.json
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-receive-message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-send-message-batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-send-message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sts-get-session-token.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:05.902469 botocore-a-la-carte-1.34.9/tests/unit/retries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/test_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26367 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/retries/test_throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35112 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_auth_bearer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_auth_sigv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93962 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39978 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_configloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138173 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20712 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18355 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_endpoint_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_errorfactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15485 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63533 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27457 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_http_client_exception_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19734 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27402 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_httpchecksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_idempotency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47606 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35401 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57408 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58705 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17041 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50089 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_retryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_s3_addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19004 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40231 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35824 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_session_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43689 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126991 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33648 2023-12-28 01:06:27.000000 botocore-a-la-carte-1.34.9/tests/unit/test_waiters.py
```

### Comparing `botocore-a-la-carte-1.34.8/LICENSE.txt` & `botocore-a-la-carte-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/NOTICE` & `botocore-a-la-carte-1.34.9/NOTICE`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/PKG-INFO` & `botocore-a-la-carte-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte
-Version: 1.34.8
+Version: 1.34.9
 Summary: botocore re-uploaded with a-la-carte data packages.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-1.34.8/README.rst` & `botocore-a-la-carte-1.34.9/README.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/__init__.py` & `botocore-a-la-carte-1.34.9/botocore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import logging
 import os
 import re
 
-__version__ = '1.34.8'
+__version__ = '1.34.9'
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
```

### Comparing `botocore-a-la-carte-1.34.8/botocore/args.py` & `botocore-a-la-carte-1.34.9/botocore/args.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/auth.py` & `botocore-a-la-carte-1.34.9/botocore/auth.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/awsrequest.py` & `botocore-a-la-carte-1.34.9/botocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/cacert.pem` & `botocore-a-la-carte-1.34.9/botocore/cacert.pem`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/client.py` & `botocore-a-la-carte-1.34.9/botocore/client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/compat.py` & `botocore-a-la-carte-1.34.9/botocore/compat.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/compress.py` & `botocore-a-la-carte-1.34.9/botocore/compress.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/config.py` & `botocore-a-la-carte-1.34.9/botocore/config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/configloader.py` & `botocore-a-la-carte-1.34.9/botocore/configloader.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/configprovider.py` & `botocore-a-la-carte-1.34.9/botocore/configprovider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/credentials.py` & `botocore-a-la-carte-1.34.9/botocore/credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/crt/__init__.py` & `botocore-a-la-carte-1.34.9/botocore/crt/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/crt/auth.py` & `botocore-a-la-carte-1.34.9/botocore/crt/auth.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/data/_retry.json` & `botocore-a-la-carte-1.34.9/botocore/data/_retry.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/data/endpoints.json` & `botocore-a-la-carte-1.34.9/botocore/data/endpoints.json`

 * *Files identical despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997433666934%*

 * *Differences: {"'partitions'": "{0: {'services': {'ds': {'endpoints': {'ca-west-1': {replace: "*

 * *                 "OrderedDict([('variants', [OrderedDict([('hostname', "*

 * *                 "'ds-fips.ca-west-1.amazonaws.com'), ('tags', ['fips'])])])])}, 'fips-ca-west-1': "*

 * *                 "OrderedDict([('credentialScope', OrderedDict([('region', 'ca-west-1')])), "*

 * *                 "('deprecated', True), ('hostname', 'ds-fips.ca-west-1.amazonaws.com')])}}, "*

 * *                 "'rds': {'endpoints': {'ca-west-1': OrderedDict([( […]*

```diff
@@ -6510,15 +6510,24 @@
                                     "hostname": "ds-fips.ca-central-1.amazonaws.com",
                                     "tags": [
                                         "fips"
                                     ]
                                 }
                             ]
                         },
-                        "ca-west-1": {},
+                        "ca-west-1": {
+                            "variants": [
+                                {
+                                    "hostname": "ds-fips.ca-west-1.amazonaws.com",
+                                    "tags": [
+                                        "fips"
+                                    ]
+                                }
+                            ]
+                        },
                         "eu-central-1": {},
                         "eu-central-2": {},
                         "eu-north-1": {},
                         "eu-south-1": {},
                         "eu-south-2": {},
                         "eu-west-1": {},
                         "eu-west-2": {},
@@ -6526,14 +6535,21 @@
                         "fips-ca-central-1": {
                             "credentialScope": {
                                 "region": "ca-central-1"
                             },
                             "deprecated": true,
                             "hostname": "ds-fips.ca-central-1.amazonaws.com"
                         },
+                        "fips-ca-west-1": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "hostname": "ds-fips.ca-west-1.amazonaws.com"
+                        },
                         "fips-us-east-1": {
                             "credentialScope": {
                                 "region": "us-east-1"
                             },
                             "deprecated": true,
                             "hostname": "ds-fips.us-east-1.amazonaws.com"
                         },
@@ -16499,14 +16515,31 @@
                         "ca-central-1-fips": {
                             "credentialScope": {
                                 "region": "ca-central-1"
                             },
                             "deprecated": true,
                             "hostname": "rds-fips.ca-central-1.amazonaws.com"
                         },
+                        "ca-west-1": {
+                            "variants": [
+                                {
+                                    "hostname": "rds-fips.ca-west-1.amazonaws.com",
+                                    "tags": [
+                                        "fips"
+                                    ]
+                                }
+                            ]
+                        },
+                        "ca-west-1-fips": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "hostname": "rds-fips.ca-west-1.amazonaws.com"
+                        },
                         "eu-central-1": {},
                         "eu-central-2": {},
                         "eu-north-1": {},
                         "eu-south-1": {},
                         "eu-south-2": {},
                         "eu-west-1": {},
                         "eu-west-2": {},
@@ -16517,14 +16550,21 @@
                         "rds-fips.ca-central-1": {
                             "credentialScope": {
                                 "region": "ca-central-1"
                             },
                             "deprecated": true,
                             "hostname": "rds-fips.ca-central-1.amazonaws.com"
                         },
+                        "rds-fips.ca-west-1": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "hostname": "rds-fips.ca-west-1.amazonaws.com"
+                        },
                         "rds-fips.us-east-1": {
                             "credentialScope": {
                                 "region": "us-east-1"
                             },
                             "deprecated": true,
                             "hostname": "rds-fips.us-east-1.amazonaws.com"
                         },
@@ -16559,14 +16599,28 @@
                                     "hostname": "rds-fips.ca-central-1.amazonaws.com",
                                     "tags": [
                                         "fips"
                                     ]
                                 }
                             ]
                         },
+                        "rds.ca-west-1": {
+                            "credentialScope": {
+                                "region": "ca-west-1"
+                            },
+                            "deprecated": true,
+                            "variants": [
+                                {
+                                    "hostname": "rds-fips.ca-west-1.amazonaws.com",
+                                    "tags": [
+                                        "fips"
+                                    ]
+                                }
+                            ]
+                        },
                         "rds.us-east-1": {
                             "credentialScope": {
                                 "region": "us-east-1"
                             },
                             "deprecated": true,
                             "variants": [
                                 {
```

### Comparing `botocore-a-la-carte-1.34.8/botocore/data/partitions.json` & `botocore-a-la-carte-1.34.9/botocore/data/partitions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/data/sdk-default-configuration.json` & `botocore-a-la-carte-1.34.9/botocore/data/sdk-default-configuration.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/discovery.py` & `botocore-a-la-carte-1.34.9/botocore/discovery.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/__init__.py` & `botocore-a-la-carte-1.34.9/botocore/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/__init__.py` & `botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/docstringparser.py` & `botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/restdoc.py` & `botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/restdoc.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/bcdoc/style.py` & `botocore-a-la-carte-1.34.9/botocore/docs/bcdoc/style.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/client.py` & `botocore-a-la-carte-1.34.9/botocore/docs/client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/docstring.py` & `botocore-a-la-carte-1.34.9/botocore/docs/docstring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/example.py` & `botocore-a-la-carte-1.34.9/botocore/docs/example.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/method.py` & `botocore-a-la-carte-1.34.9/botocore/docs/method.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/paginator.py` & `botocore-a-la-carte-1.34.9/botocore/docs/paginator.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/params.py` & `botocore-a-la-carte-1.34.9/botocore/docs/params.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/service.py` & `botocore-a-la-carte-1.34.9/botocore/docs/service.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/shape.py` & `botocore-a-la-carte-1.34.9/botocore/docs/shape.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/sharedexample.py` & `botocore-a-la-carte-1.34.9/botocore/docs/sharedexample.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/translator.py` & `botocore-a-la-carte-1.34.9/botocore/docs/translator.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/utils.py` & `botocore-a-la-carte-1.34.9/botocore/docs/utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/docs/waiter.py` & `botocore-a-la-carte-1.34.9/botocore/docs/waiter.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/endpoint.py` & `botocore-a-la-carte-1.34.9/botocore/endpoint.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/endpoint_provider.py` & `botocore-a-la-carte-1.34.9/botocore/endpoint_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/errorfactory.py` & `botocore-a-la-carte-1.34.9/botocore/errorfactory.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/eventstream.py` & `botocore-a-la-carte-1.34.9/botocore/eventstream.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/exceptions.py` & `botocore-a-la-carte-1.34.9/botocore/exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/handlers.py` & `botocore-a-la-carte-1.34.9/botocore/handlers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/history.py` & `botocore-a-la-carte-1.34.9/botocore/history.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/hooks.py` & `botocore-a-la-carte-1.34.9/botocore/hooks.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/httpchecksum.py` & `botocore-a-la-carte-1.34.9/botocore/httpchecksum.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/httpsession.py` & `botocore-a-la-carte-1.34.9/botocore/httpsession.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/loaders.py` & `botocore-a-la-carte-1.34.9/botocore/loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/model.py` & `botocore-a-la-carte-1.34.9/botocore/model.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/monitoring.py` & `botocore-a-la-carte-1.34.9/botocore/monitoring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/paginate.py` & `botocore-a-la-carte-1.34.9/botocore/paginate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/parsers.py` & `botocore-a-la-carte-1.34.9/botocore/parsers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/regions.py` & `botocore-a-la-carte-1.34.9/botocore/regions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/response.py` & `botocore-a-la-carte-1.34.9/botocore/response.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/adaptive.py` & `botocore-a-la-carte-1.34.9/botocore/retries/adaptive.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/base.py` & `botocore-a-la-carte-1.34.9/botocore/retries/base.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/bucket.py` & `botocore-a-la-carte-1.34.9/botocore/retries/bucket.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/quota.py` & `botocore-a-la-carte-1.34.9/botocore/retries/quota.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/special.py` & `botocore-a-la-carte-1.34.9/botocore/retries/special.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/standard.py` & `botocore-a-la-carte-1.34.9/botocore/retries/standard.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retries/throttling.py` & `botocore-a-la-carte-1.34.9/botocore/retries/throttling.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/retryhandler.py` & `botocore-a-la-carte-1.34.9/botocore/retryhandler.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/serialize.py` & `botocore-a-la-carte-1.34.9/botocore/serialize.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/session.py` & `botocore-a-la-carte-1.34.9/botocore/session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/signers.py` & `botocore-a-la-carte-1.34.9/botocore/signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/stub.py` & `botocore-a-la-carte-1.34.9/botocore/stub.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/tokens.py` & `botocore-a-la-carte-1.34.9/botocore/tokens.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/translate.py` & `botocore-a-la-carte-1.34.9/botocore/translate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/useragent.py` & `botocore-a-la-carte-1.34.9/botocore/useragent.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/utils.py` & `botocore-a-la-carte-1.34.9/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/validate.py` & `botocore-a-la-carte-1.34.9/botocore/validate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/vendored/requests/exceptions.py` & `botocore-a-la-carte-1.34.9/botocore/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/vendored/requests/packages/urllib3/exceptions.py` & `botocore-a-la-carte-1.34.9/botocore/vendored/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/vendored/six.py` & `botocore-a-la-carte-1.34.9/botocore/vendored/six.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore/waiter.py` & `botocore-a-la-carte-1.34.9/botocore/waiter.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/PKG-INFO` & `botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte
-Version: 1.34.8
+Version: 1.34.9
 Summary: botocore re-uploaded with a-la-carte data packages.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-1.34.8/botocore_a_la_carte.egg-info/SOURCES.txt` & `botocore-a-la-carte-1.34.9/botocore_a_la_carte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/Makefile` & `botocore-a-la-carte-1.34.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/make.bat` & `botocore-a-la-carte-1.34.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_static/404.html` & `botocore-a-la-carte-1.34.9/docs/source/_static/404.html`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_static/css/custom.css` & `botocore-a-la-carte-1.34.9/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_static/js/custom.js` & `botocore-a-la-carte-1.34.9/docs/source/_static/js/custom.js`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_static/logos/aws_dark_theme_logo.svg` & `botocore-a-la-carte-1.34.9/docs/source/_static/logos/aws_dark_theme_logo.svg`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_static/logos/aws_light_theme_logo.svg` & `botocore-a-la-carte-1.34.9/docs/source/_static/logos/aws_light_theme_logo.svg`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_static/shortbreadv1.js` & `botocore-a-la-carte-1.34.9/docs/source/_static/shortbreadv1.js`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/_templates/page.html` & `botocore-a-la-carte-1.34.9/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/client_upgrades.rst` & `botocore-a-la-carte-1.34.9/docs/source/client_upgrades.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/conf.py` & `botocore-a-la-carte-1.34.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '1.34'
 # The full version, including alpha/beta/rc tags.
-release = '1.34.8'
+release = '1.34.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `botocore-a-la-carte-1.34.8/docs/source/development/designnotes.rst` & `botocore-a-la-carte-1.34.9/docs/source/development/designnotes.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/index.rst` & `botocore-a-la-carte-1.34.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/topics/events.rst` & `botocore-a-la-carte-1.34.9/docs/source/topics/events.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/topics/paginators.rst` & `botocore-a-la-carte-1.34.9/docs/source/topics/paginators.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/docs/source/tutorial/index.rst` & `botocore-a-la-carte-1.34.9/docs/source/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/setup.cfg` & `botocore-a-la-carte-1.34.9/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -6,390 +6,390 @@
 	jmespath>=0.7.1,<2.0.0
 	python-dateutil>=2.1,<3.0.0
 	urllib3>=1.25.4,<1.27; python_version<"3.10"
 	urllib3>=1.25.4,<2.1; python_version>="3.10"
 
 [options.extras_require]
 crt = awscrt==0.19.19
-accessanalyzer = botocore-a-la-carte-accessanalyzer==1.34.8
-account = botocore-a-la-carte-account==1.34.8
-acm = botocore-a-la-carte-acm==1.34.8
-acm-pca = botocore-a-la-carte-acm-pca==1.34.8
-alexaforbusiness = botocore-a-la-carte-alexaforbusiness==1.34.8
-amp = botocore-a-la-carte-amp==1.34.8
-amplify = botocore-a-la-carte-amplify==1.34.8
-amplifybackend = botocore-a-la-carte-amplifybackend==1.34.8
-amplifyuibuilder = botocore-a-la-carte-amplifyuibuilder==1.34.8
-apigateway = botocore-a-la-carte-apigateway==1.34.8
-apigatewaymanagementapi = botocore-a-la-carte-apigatewaymanagementapi==1.34.8
-apigatewayv2 = botocore-a-la-carte-apigatewayv2==1.34.8
-appconfig = botocore-a-la-carte-appconfig==1.34.8
-appconfigdata = botocore-a-la-carte-appconfigdata==1.34.8
-appfabric = botocore-a-la-carte-appfabric==1.34.8
-appflow = botocore-a-la-carte-appflow==1.34.8
-appintegrations = botocore-a-la-carte-appintegrations==1.34.8
-application-autoscaling = botocore-a-la-carte-application-autoscaling==1.34.8
-application-insights = botocore-a-la-carte-application-insights==1.34.8
-applicationcostprofiler = botocore-a-la-carte-applicationcostprofiler==1.34.8
-appmesh = botocore-a-la-carte-appmesh==1.34.8
-apprunner = botocore-a-la-carte-apprunner==1.34.8
-appstream = botocore-a-la-carte-appstream==1.34.8
-appsync = botocore-a-la-carte-appsync==1.34.8
-arc-zonal-shift = botocore-a-la-carte-arc-zonal-shift==1.34.8
-athena = botocore-a-la-carte-athena==1.34.8
-auditmanager = botocore-a-la-carte-auditmanager==1.34.8
-autoscaling = botocore-a-la-carte-autoscaling==1.34.8
-autoscaling-plans = botocore-a-la-carte-autoscaling-plans==1.34.8
-b2bi = botocore-a-la-carte-b2bi==1.34.8
-backup = botocore-a-la-carte-backup==1.34.8
-backup-gateway = botocore-a-la-carte-backup-gateway==1.34.8
-backupstorage = botocore-a-la-carte-backupstorage==1.34.8
-batch = botocore-a-la-carte-batch==1.34.8
-bcm-data-exports = botocore-a-la-carte-bcm-data-exports==1.34.8
-bedrock = botocore-a-la-carte-bedrock==1.34.8
-bedrock-agent = botocore-a-la-carte-bedrock-agent==1.34.8
-bedrock-agent-runtime = botocore-a-la-carte-bedrock-agent-runtime==1.34.8
-bedrock-runtime = botocore-a-la-carte-bedrock-runtime==1.34.8
-billingconductor = botocore-a-la-carte-billingconductor==1.34.8
-braket = botocore-a-la-carte-braket==1.34.8
-budgets = botocore-a-la-carte-budgets==1.34.8
-ce = botocore-a-la-carte-ce==1.34.8
-chime = botocore-a-la-carte-chime==1.34.8
-chime-sdk-identity = botocore-a-la-carte-chime-sdk-identity==1.34.8
-chime-sdk-media-pipelines = botocore-a-la-carte-chime-sdk-media-pipelines==1.34.8
-chime-sdk-meetings = botocore-a-la-carte-chime-sdk-meetings==1.34.8
-chime-sdk-messaging = botocore-a-la-carte-chime-sdk-messaging==1.34.8
-chime-sdk-voice = botocore-a-la-carte-chime-sdk-voice==1.34.8
-cleanrooms = botocore-a-la-carte-cleanrooms==1.34.8
-cleanroomsml = botocore-a-la-carte-cleanroomsml==1.34.8
-cloud9 = botocore-a-la-carte-cloud9==1.34.8
-cloudcontrol = botocore-a-la-carte-cloudcontrol==1.34.8
-clouddirectory = botocore-a-la-carte-clouddirectory==1.34.8
-cloudformation = botocore-a-la-carte-cloudformation==1.34.8
-cloudfront = botocore-a-la-carte-cloudfront==1.34.8
-cloudfront-keyvaluestore = botocore-a-la-carte-cloudfront-keyvaluestore==1.34.8
-cloudhsm = botocore-a-la-carte-cloudhsm==1.34.8
-cloudhsmv2 = botocore-a-la-carte-cloudhsmv2==1.34.8
-cloudsearch = botocore-a-la-carte-cloudsearch==1.34.8
-cloudsearchdomain = botocore-a-la-carte-cloudsearchdomain==1.34.8
-cloudtrail = botocore-a-la-carte-cloudtrail==1.34.8
-cloudtrail-data = botocore-a-la-carte-cloudtrail-data==1.34.8
-cloudwatch = botocore-a-la-carte-cloudwatch==1.34.8
-codeartifact = botocore-a-la-carte-codeartifact==1.34.8
-codebuild = botocore-a-la-carte-codebuild==1.34.8
-codecatalyst = botocore-a-la-carte-codecatalyst==1.34.8
-codecommit = botocore-a-la-carte-codecommit==1.34.8
-codedeploy = botocore-a-la-carte-codedeploy==1.34.8
-codeguru-reviewer = botocore-a-la-carte-codeguru-reviewer==1.34.8
-codeguru-security = botocore-a-la-carte-codeguru-security==1.34.8
-codeguruprofiler = botocore-a-la-carte-codeguruprofiler==1.34.8
-codepipeline = botocore-a-la-carte-codepipeline==1.34.8
-codestar = botocore-a-la-carte-codestar==1.34.8
-codestar-connections = botocore-a-la-carte-codestar-connections==1.34.8
-codestar-notifications = botocore-a-la-carte-codestar-notifications==1.34.8
-cognito-identity = botocore-a-la-carte-cognito-identity==1.34.8
-cognito-idp = botocore-a-la-carte-cognito-idp==1.34.8
-cognito-sync = botocore-a-la-carte-cognito-sync==1.34.8
-comprehend = botocore-a-la-carte-comprehend==1.34.8
-comprehendmedical = botocore-a-la-carte-comprehendmedical==1.34.8
-compute-optimizer = botocore-a-la-carte-compute-optimizer==1.34.8
-config = botocore-a-la-carte-config==1.34.8
-connect = botocore-a-la-carte-connect==1.34.8
-connect-contact-lens = botocore-a-la-carte-connect-contact-lens==1.34.8
-connectcampaigns = botocore-a-la-carte-connectcampaigns==1.34.8
-connectcases = botocore-a-la-carte-connectcases==1.34.8
-connectparticipant = botocore-a-la-carte-connectparticipant==1.34.8
-controltower = botocore-a-la-carte-controltower==1.34.8
-cost-optimization-hub = botocore-a-la-carte-cost-optimization-hub==1.34.8
-cur = botocore-a-la-carte-cur==1.34.8
-customer-profiles = botocore-a-la-carte-customer-profiles==1.34.8
-databrew = botocore-a-la-carte-databrew==1.34.8
-dataexchange = botocore-a-la-carte-dataexchange==1.34.8
-datapipeline = botocore-a-la-carte-datapipeline==1.34.8
-datasync = botocore-a-la-carte-datasync==1.34.8
-datazone = botocore-a-la-carte-datazone==1.34.8
-dax = botocore-a-la-carte-dax==1.34.8
-detective = botocore-a-la-carte-detective==1.34.8
-devicefarm = botocore-a-la-carte-devicefarm==1.34.8
-devops-guru = botocore-a-la-carte-devops-guru==1.34.8
-directconnect = botocore-a-la-carte-directconnect==1.34.8
-discovery = botocore-a-la-carte-discovery==1.34.8
-dlm = botocore-a-la-carte-dlm==1.34.8
-dms = botocore-a-la-carte-dms==1.34.8
-docdb = botocore-a-la-carte-docdb==1.34.8
-docdb-elastic = botocore-a-la-carte-docdb-elastic==1.34.8
-drs = botocore-a-la-carte-drs==1.34.8
-ds = botocore-a-la-carte-ds==1.34.8
-dynamodb = botocore-a-la-carte-dynamodb==1.34.8
-dynamodbstreams = botocore-a-la-carte-dynamodbstreams==1.34.8
-ebs = botocore-a-la-carte-ebs==1.34.8
-ec2 = botocore-a-la-carte-ec2==1.34.8
-ec2-instance-connect = botocore-a-la-carte-ec2-instance-connect==1.34.8
-ecr = botocore-a-la-carte-ecr==1.34.8
-ecr-public = botocore-a-la-carte-ecr-public==1.34.8
-ecs = botocore-a-la-carte-ecs==1.34.8
-efs = botocore-a-la-carte-efs==1.34.8
-eks = botocore-a-la-carte-eks==1.34.8
-eks-auth = botocore-a-la-carte-eks-auth==1.34.8
-elastic-inference = botocore-a-la-carte-elastic-inference==1.34.8
-elasticache = botocore-a-la-carte-elasticache==1.34.8
-elasticbeanstalk = botocore-a-la-carte-elasticbeanstalk==1.34.8
-elastictranscoder = botocore-a-la-carte-elastictranscoder==1.34.8
-elb = botocore-a-la-carte-elb==1.34.8
-elbv2 = botocore-a-la-carte-elbv2==1.34.8
-emr = botocore-a-la-carte-emr==1.34.8
-emr-containers = botocore-a-la-carte-emr-containers==1.34.8
-emr-serverless = botocore-a-la-carte-emr-serverless==1.34.8
-entityresolution = botocore-a-la-carte-entityresolution==1.34.8
-es = botocore-a-la-carte-es==1.34.8
-events = botocore-a-la-carte-events==1.34.8
-evidently = botocore-a-la-carte-evidently==1.34.8
-finspace = botocore-a-la-carte-finspace==1.34.8
-finspace-data = botocore-a-la-carte-finspace-data==1.34.8
-firehose = botocore-a-la-carte-firehose==1.34.8
-fis = botocore-a-la-carte-fis==1.34.8
-fms = botocore-a-la-carte-fms==1.34.8
-forecast = botocore-a-la-carte-forecast==1.34.8
-forecastquery = botocore-a-la-carte-forecastquery==1.34.8
-frauddetector = botocore-a-la-carte-frauddetector==1.34.8
-freetier = botocore-a-la-carte-freetier==1.34.8
-fsx = botocore-a-la-carte-fsx==1.34.8
-gamelift = botocore-a-la-carte-gamelift==1.34.8
-glacier = botocore-a-la-carte-glacier==1.34.8
-globalaccelerator = botocore-a-la-carte-globalaccelerator==1.34.8
-glue = botocore-a-la-carte-glue==1.34.8
-grafana = botocore-a-la-carte-grafana==1.34.8
-greengrass = botocore-a-la-carte-greengrass==1.34.8
-greengrassv2 = botocore-a-la-carte-greengrassv2==1.34.8
-groundstation = botocore-a-la-carte-groundstation==1.34.8
-guardduty = botocore-a-la-carte-guardduty==1.34.8
-health = botocore-a-la-carte-health==1.34.8
-healthlake = botocore-a-la-carte-healthlake==1.34.8
-honeycode = botocore-a-la-carte-honeycode==1.34.8
-iam = botocore-a-la-carte-iam==1.34.8
-identitystore = botocore-a-la-carte-identitystore==1.34.8
-imagebuilder = botocore-a-la-carte-imagebuilder==1.34.8
-importexport = botocore-a-la-carte-importexport==1.34.8
-inspector = botocore-a-la-carte-inspector==1.34.8
-inspector-scan = botocore-a-la-carte-inspector-scan==1.34.8
-inspector2 = botocore-a-la-carte-inspector2==1.34.8
-internetmonitor = botocore-a-la-carte-internetmonitor==1.34.8
-iot = botocore-a-la-carte-iot==1.34.8
-iot-data = botocore-a-la-carte-iot-data==1.34.8
-iot-jobs-data = botocore-a-la-carte-iot-jobs-data==1.34.8
-iot-roborunner = botocore-a-la-carte-iot-roborunner==1.34.8
-iot1click-devices = botocore-a-la-carte-iot1click-devices==1.34.8
-iot1click-projects = botocore-a-la-carte-iot1click-projects==1.34.8
-iotanalytics = botocore-a-la-carte-iotanalytics==1.34.8
-iotdeviceadvisor = botocore-a-la-carte-iotdeviceadvisor==1.34.8
-iotevents = botocore-a-la-carte-iotevents==1.34.8
-iotevents-data = botocore-a-la-carte-iotevents-data==1.34.8
-iotfleethub = botocore-a-la-carte-iotfleethub==1.34.8
-iotfleetwise = botocore-a-la-carte-iotfleetwise==1.34.8
-iotsecuretunneling = botocore-a-la-carte-iotsecuretunneling==1.34.8
-iotsitewise = botocore-a-la-carte-iotsitewise==1.34.8
-iotthingsgraph = botocore-a-la-carte-iotthingsgraph==1.34.8
-iottwinmaker = botocore-a-la-carte-iottwinmaker==1.34.8
-iotwireless = botocore-a-la-carte-iotwireless==1.34.8
-ivs = botocore-a-la-carte-ivs==1.34.8
-ivs-realtime = botocore-a-la-carte-ivs-realtime==1.34.8
-ivschat = botocore-a-la-carte-ivschat==1.34.8
-kafka = botocore-a-la-carte-kafka==1.34.8
-kafkaconnect = botocore-a-la-carte-kafkaconnect==1.34.8
-kendra = botocore-a-la-carte-kendra==1.34.8
-kendra-ranking = botocore-a-la-carte-kendra-ranking==1.34.8
-keyspaces = botocore-a-la-carte-keyspaces==1.34.8
-kinesis = botocore-a-la-carte-kinesis==1.34.8
-kinesis-video-archived-media = botocore-a-la-carte-kinesis-video-archived-media==1.34.8
-kinesis-video-media = botocore-a-la-carte-kinesis-video-media==1.34.8
-kinesis-video-signaling = botocore-a-la-carte-kinesis-video-signaling==1.34.8
-kinesis-video-webrtc-storage = botocore-a-la-carte-kinesis-video-webrtc-storage==1.34.8
-kinesisanalytics = botocore-a-la-carte-kinesisanalytics==1.34.8
-kinesisanalyticsv2 = botocore-a-la-carte-kinesisanalyticsv2==1.34.8
-kinesisvideo = botocore-a-la-carte-kinesisvideo==1.34.8
-kms = botocore-a-la-carte-kms==1.34.8
-lakeformation = botocore-a-la-carte-lakeformation==1.34.8
-lambda = botocore-a-la-carte-lambda==1.34.8
-launch-wizard = botocore-a-la-carte-launch-wizard==1.34.8
-lex-models = botocore-a-la-carte-lex-models==1.34.8
-lex-runtime = botocore-a-la-carte-lex-runtime==1.34.8
-lexv2-models = botocore-a-la-carte-lexv2-models==1.34.8
-lexv2-runtime = botocore-a-la-carte-lexv2-runtime==1.34.8
-license-manager = botocore-a-la-carte-license-manager==1.34.8
-license-manager-linux-subscriptions = botocore-a-la-carte-license-manager-linux-subscriptions==1.34.8
-license-manager-user-subscriptions = botocore-a-la-carte-license-manager-user-subscriptions==1.34.8
-lightsail = botocore-a-la-carte-lightsail==1.34.8
-location = botocore-a-la-carte-location==1.34.8
-logs = botocore-a-la-carte-logs==1.34.8
-lookoutequipment = botocore-a-la-carte-lookoutequipment==1.34.8
-lookoutmetrics = botocore-a-la-carte-lookoutmetrics==1.34.8
-lookoutvision = botocore-a-la-carte-lookoutvision==1.34.8
-m2 = botocore-a-la-carte-m2==1.34.8
-machinelearning = botocore-a-la-carte-machinelearning==1.34.8
-macie2 = botocore-a-la-carte-macie2==1.34.8
-managedblockchain = botocore-a-la-carte-managedblockchain==1.34.8
-managedblockchain-query = botocore-a-la-carte-managedblockchain-query==1.34.8
-marketplace-agreement = botocore-a-la-carte-marketplace-agreement==1.34.8
-marketplace-catalog = botocore-a-la-carte-marketplace-catalog==1.34.8
-marketplace-deployment = botocore-a-la-carte-marketplace-deployment==1.34.8
-marketplace-entitlement = botocore-a-la-carte-marketplace-entitlement==1.34.8
-marketplacecommerceanalytics = botocore-a-la-carte-marketplacecommerceanalytics==1.34.8
-mediaconnect = botocore-a-la-carte-mediaconnect==1.34.8
-mediaconvert = botocore-a-la-carte-mediaconvert==1.34.8
-medialive = botocore-a-la-carte-medialive==1.34.8
-mediapackage = botocore-a-la-carte-mediapackage==1.34.8
-mediapackage-vod = botocore-a-la-carte-mediapackage-vod==1.34.8
-mediapackagev2 = botocore-a-la-carte-mediapackagev2==1.34.8
-mediastore = botocore-a-la-carte-mediastore==1.34.8
-mediastore-data = botocore-a-la-carte-mediastore-data==1.34.8
-mediatailor = botocore-a-la-carte-mediatailor==1.34.8
-medical-imaging = botocore-a-la-carte-medical-imaging==1.34.8
-memorydb = botocore-a-la-carte-memorydb==1.34.8
-meteringmarketplace = botocore-a-la-carte-meteringmarketplace==1.34.8
-mgh = botocore-a-la-carte-mgh==1.34.8
-mgn = botocore-a-la-carte-mgn==1.34.8
-migration-hub-refactor-spaces = botocore-a-la-carte-migration-hub-refactor-spaces==1.34.8
-migrationhub-config = botocore-a-la-carte-migrationhub-config==1.34.8
-migrationhuborchestrator = botocore-a-la-carte-migrationhuborchestrator==1.34.8
-migrationhubstrategy = botocore-a-la-carte-migrationhubstrategy==1.34.8
-mobile = botocore-a-la-carte-mobile==1.34.8
-mq = botocore-a-la-carte-mq==1.34.8
-mturk = botocore-a-la-carte-mturk==1.34.8
-mwaa = botocore-a-la-carte-mwaa==1.34.8
-neptune = botocore-a-la-carte-neptune==1.34.8
-neptune-graph = botocore-a-la-carte-neptune-graph==1.34.8
-neptunedata = botocore-a-la-carte-neptunedata==1.34.8
-network-firewall = botocore-a-la-carte-network-firewall==1.34.8
-networkmanager = botocore-a-la-carte-networkmanager==1.34.8
-networkmonitor = botocore-a-la-carte-networkmonitor==1.34.8
-nimble = botocore-a-la-carte-nimble==1.34.8
-oam = botocore-a-la-carte-oam==1.34.8
-omics = botocore-a-la-carte-omics==1.34.8
-opensearch = botocore-a-la-carte-opensearch==1.34.8
-opensearchserverless = botocore-a-la-carte-opensearchserverless==1.34.8
-opsworks = botocore-a-la-carte-opsworks==1.34.8
-opsworkscm = botocore-a-la-carte-opsworkscm==1.34.8
-organizations = botocore-a-la-carte-organizations==1.34.8
-osis = botocore-a-la-carte-osis==1.34.8
-outposts = botocore-a-la-carte-outposts==1.34.8
-panorama = botocore-a-la-carte-panorama==1.34.8
-payment-cryptography = botocore-a-la-carte-payment-cryptography==1.34.8
-payment-cryptography-data = botocore-a-la-carte-payment-cryptography-data==1.34.8
-pca-connector-ad = botocore-a-la-carte-pca-connector-ad==1.34.8
-personalize = botocore-a-la-carte-personalize==1.34.8
-personalize-events = botocore-a-la-carte-personalize-events==1.34.8
-personalize-runtime = botocore-a-la-carte-personalize-runtime==1.34.8
-pi = botocore-a-la-carte-pi==1.34.8
-pinpoint = botocore-a-la-carte-pinpoint==1.34.8
-pinpoint-email = botocore-a-la-carte-pinpoint-email==1.34.8
-pinpoint-sms-voice = botocore-a-la-carte-pinpoint-sms-voice==1.34.8
-pinpoint-sms-voice-v2 = botocore-a-la-carte-pinpoint-sms-voice-v2==1.34.8
-pipes = botocore-a-la-carte-pipes==1.34.8
-polly = botocore-a-la-carte-polly==1.34.8
-pricing = botocore-a-la-carte-pricing==1.34.8
-privatenetworks = botocore-a-la-carte-privatenetworks==1.34.8
-proton = botocore-a-la-carte-proton==1.34.8
-qbusiness = botocore-a-la-carte-qbusiness==1.34.8
-qconnect = botocore-a-la-carte-qconnect==1.34.8
-qldb = botocore-a-la-carte-qldb==1.34.8
-qldb-session = botocore-a-la-carte-qldb-session==1.34.8
-quicksight = botocore-a-la-carte-quicksight==1.34.8
-ram = botocore-a-la-carte-ram==1.34.8
-rbin = botocore-a-la-carte-rbin==1.34.8
-rds = botocore-a-la-carte-rds==1.34.8
-rds-data = botocore-a-la-carte-rds-data==1.34.8
-redshift = botocore-a-la-carte-redshift==1.34.8
-redshift-data = botocore-a-la-carte-redshift-data==1.34.8
-redshift-serverless = botocore-a-la-carte-redshift-serverless==1.34.8
-rekognition = botocore-a-la-carte-rekognition==1.34.8
-repostspace = botocore-a-la-carte-repostspace==1.34.8
-resiliencehub = botocore-a-la-carte-resiliencehub==1.34.8
-resource-explorer-2 = botocore-a-la-carte-resource-explorer-2==1.34.8
-resource-groups = botocore-a-la-carte-resource-groups==1.34.8
-resourcegroupstaggingapi = botocore-a-la-carte-resourcegroupstaggingapi==1.34.8
-robomaker = botocore-a-la-carte-robomaker==1.34.8
-rolesanywhere = botocore-a-la-carte-rolesanywhere==1.34.8
-route53 = botocore-a-la-carte-route53==1.34.8
-route53-recovery-cluster = botocore-a-la-carte-route53-recovery-cluster==1.34.8
-route53-recovery-control-config = botocore-a-la-carte-route53-recovery-control-config==1.34.8
-route53-recovery-readiness = botocore-a-la-carte-route53-recovery-readiness==1.34.8
-route53domains = botocore-a-la-carte-route53domains==1.34.8
-route53resolver = botocore-a-la-carte-route53resolver==1.34.8
-rum = botocore-a-la-carte-rum==1.34.8
-s3 = botocore-a-la-carte-s3==1.34.8
-s3control = botocore-a-la-carte-s3control==1.34.8
-s3outposts = botocore-a-la-carte-s3outposts==1.34.8
-sagemaker = botocore-a-la-carte-sagemaker==1.34.8
-sagemaker-a2i-runtime = botocore-a-la-carte-sagemaker-a2i-runtime==1.34.8
-sagemaker-edge = botocore-a-la-carte-sagemaker-edge==1.34.8
-sagemaker-featurestore-runtime = botocore-a-la-carte-sagemaker-featurestore-runtime==1.34.8
-sagemaker-geospatial = botocore-a-la-carte-sagemaker-geospatial==1.34.8
-sagemaker-metrics = botocore-a-la-carte-sagemaker-metrics==1.34.8
-sagemaker-runtime = botocore-a-la-carte-sagemaker-runtime==1.34.8
-savingsplans = botocore-a-la-carte-savingsplans==1.34.8
-scheduler = botocore-a-la-carte-scheduler==1.34.8
-schemas = botocore-a-la-carte-schemas==1.34.8
-sdb = botocore-a-la-carte-sdb==1.34.8
-secretsmanager = botocore-a-la-carte-secretsmanager==1.34.8
-securityhub = botocore-a-la-carte-securityhub==1.34.8
-securitylake = botocore-a-la-carte-securitylake==1.34.8
-serverlessrepo = botocore-a-la-carte-serverlessrepo==1.34.8
-service-quotas = botocore-a-la-carte-service-quotas==1.34.8
-servicecatalog = botocore-a-la-carte-servicecatalog==1.34.8
-servicecatalog-appregistry = botocore-a-la-carte-servicecatalog-appregistry==1.34.8
-servicediscovery = botocore-a-la-carte-servicediscovery==1.34.8
-ses = botocore-a-la-carte-ses==1.34.8
-sesv2 = botocore-a-la-carte-sesv2==1.34.8
-shield = botocore-a-la-carte-shield==1.34.8
-signer = botocore-a-la-carte-signer==1.34.8
-simspaceweaver = botocore-a-la-carte-simspaceweaver==1.34.8
-sms = botocore-a-la-carte-sms==1.34.8
-sms-voice = botocore-a-la-carte-sms-voice==1.34.8
-snow-device-management = botocore-a-la-carte-snow-device-management==1.34.8
-snowball = botocore-a-la-carte-snowball==1.34.8
-sns = botocore-a-la-carte-sns==1.34.8
-sqs = botocore-a-la-carte-sqs==1.34.8
-ssm = botocore-a-la-carte-ssm==1.34.8
-ssm-contacts = botocore-a-la-carte-ssm-contacts==1.34.8
-ssm-incidents = botocore-a-la-carte-ssm-incidents==1.34.8
-ssm-sap = botocore-a-la-carte-ssm-sap==1.34.8
-sso = botocore-a-la-carte-sso==1.34.8
-sso-admin = botocore-a-la-carte-sso-admin==1.34.8
-sso-oidc = botocore-a-la-carte-sso-oidc==1.34.8
-stepfunctions = botocore-a-la-carte-stepfunctions==1.34.8
-storagegateway = botocore-a-la-carte-storagegateway==1.34.8
-sts = botocore-a-la-carte-sts==1.34.8
-support = botocore-a-la-carte-support==1.34.8
-support-app = botocore-a-la-carte-support-app==1.34.8
-swf = botocore-a-la-carte-swf==1.34.8
-synthetics = botocore-a-la-carte-synthetics==1.34.8
-textract = botocore-a-la-carte-textract==1.34.8
-timestream-query = botocore-a-la-carte-timestream-query==1.34.8
-timestream-write = botocore-a-la-carte-timestream-write==1.34.8
-tnb = botocore-a-la-carte-tnb==1.34.8
-transcribe = botocore-a-la-carte-transcribe==1.34.8
-transfer = botocore-a-la-carte-transfer==1.34.8
-translate = botocore-a-la-carte-translate==1.34.8
-trustedadvisor = botocore-a-la-carte-trustedadvisor==1.34.8
-verifiedpermissions = botocore-a-la-carte-verifiedpermissions==1.34.8
-voice-id = botocore-a-la-carte-voice-id==1.34.8
-vpc-lattice = botocore-a-la-carte-vpc-lattice==1.34.8
-waf = botocore-a-la-carte-waf==1.34.8
-waf-regional = botocore-a-la-carte-waf-regional==1.34.8
-wafv2 = botocore-a-la-carte-wafv2==1.34.8
-wellarchitected = botocore-a-la-carte-wellarchitected==1.34.8
-wisdom = botocore-a-la-carte-wisdom==1.34.8
-workdocs = botocore-a-la-carte-workdocs==1.34.8
-worklink = botocore-a-la-carte-worklink==1.34.8
-workmail = botocore-a-la-carte-workmail==1.34.8
-workmailmessageflow = botocore-a-la-carte-workmailmessageflow==1.34.8
-workspaces = botocore-a-la-carte-workspaces==1.34.8
-workspaces-thin-client = botocore-a-la-carte-workspaces-thin-client==1.34.8
-workspaces-web = botocore-a-la-carte-workspaces-web==1.34.8
-xray = botocore-a-la-carte-xray==1.34.8
+accessanalyzer = botocore-a-la-carte-accessanalyzer==1.34.9
+account = botocore-a-la-carte-account==1.34.9
+acm = botocore-a-la-carte-acm==1.34.9
+acm-pca = botocore-a-la-carte-acm-pca==1.34.9
+alexaforbusiness = botocore-a-la-carte-alexaforbusiness==1.34.9
+amp = botocore-a-la-carte-amp==1.34.9
+amplify = botocore-a-la-carte-amplify==1.34.9
+amplifybackend = botocore-a-la-carte-amplifybackend==1.34.9
+amplifyuibuilder = botocore-a-la-carte-amplifyuibuilder==1.34.9
+apigateway = botocore-a-la-carte-apigateway==1.34.9
+apigatewaymanagementapi = botocore-a-la-carte-apigatewaymanagementapi==1.34.9
+apigatewayv2 = botocore-a-la-carte-apigatewayv2==1.34.9
+appconfig = botocore-a-la-carte-appconfig==1.34.9
+appconfigdata = botocore-a-la-carte-appconfigdata==1.34.9
+appfabric = botocore-a-la-carte-appfabric==1.34.9
+appflow = botocore-a-la-carte-appflow==1.34.9
+appintegrations = botocore-a-la-carte-appintegrations==1.34.9
+application-autoscaling = botocore-a-la-carte-application-autoscaling==1.34.9
+application-insights = botocore-a-la-carte-application-insights==1.34.9
+applicationcostprofiler = botocore-a-la-carte-applicationcostprofiler==1.34.9
+appmesh = botocore-a-la-carte-appmesh==1.34.9
+apprunner = botocore-a-la-carte-apprunner==1.34.9
+appstream = botocore-a-la-carte-appstream==1.34.9
+appsync = botocore-a-la-carte-appsync==1.34.9
+arc-zonal-shift = botocore-a-la-carte-arc-zonal-shift==1.34.9
+athena = botocore-a-la-carte-athena==1.34.9
+auditmanager = botocore-a-la-carte-auditmanager==1.34.9
+autoscaling = botocore-a-la-carte-autoscaling==1.34.9
+autoscaling-plans = botocore-a-la-carte-autoscaling-plans==1.34.9
+b2bi = botocore-a-la-carte-b2bi==1.34.9
+backup = botocore-a-la-carte-backup==1.34.9
+backup-gateway = botocore-a-la-carte-backup-gateway==1.34.9
+backupstorage = botocore-a-la-carte-backupstorage==1.34.9
+batch = botocore-a-la-carte-batch==1.34.9
+bcm-data-exports = botocore-a-la-carte-bcm-data-exports==1.34.9
+bedrock = botocore-a-la-carte-bedrock==1.34.9
+bedrock-agent = botocore-a-la-carte-bedrock-agent==1.34.9
+bedrock-agent-runtime = botocore-a-la-carte-bedrock-agent-runtime==1.34.9
+bedrock-runtime = botocore-a-la-carte-bedrock-runtime==1.34.9
+billingconductor = botocore-a-la-carte-billingconductor==1.34.9
+braket = botocore-a-la-carte-braket==1.34.9
+budgets = botocore-a-la-carte-budgets==1.34.9
+ce = botocore-a-la-carte-ce==1.34.9
+chime = botocore-a-la-carte-chime==1.34.9
+chime-sdk-identity = botocore-a-la-carte-chime-sdk-identity==1.34.9
+chime-sdk-media-pipelines = botocore-a-la-carte-chime-sdk-media-pipelines==1.34.9
+chime-sdk-meetings = botocore-a-la-carte-chime-sdk-meetings==1.34.9
+chime-sdk-messaging = botocore-a-la-carte-chime-sdk-messaging==1.34.9
+chime-sdk-voice = botocore-a-la-carte-chime-sdk-voice==1.34.9
+cleanrooms = botocore-a-la-carte-cleanrooms==1.34.9
+cleanroomsml = botocore-a-la-carte-cleanroomsml==1.34.9
+cloud9 = botocore-a-la-carte-cloud9==1.34.9
+cloudcontrol = botocore-a-la-carte-cloudcontrol==1.34.9
+clouddirectory = botocore-a-la-carte-clouddirectory==1.34.9
+cloudformation = botocore-a-la-carte-cloudformation==1.34.9
+cloudfront = botocore-a-la-carte-cloudfront==1.34.9
+cloudfront-keyvaluestore = botocore-a-la-carte-cloudfront-keyvaluestore==1.34.9
+cloudhsm = botocore-a-la-carte-cloudhsm==1.34.9
+cloudhsmv2 = botocore-a-la-carte-cloudhsmv2==1.34.9
+cloudsearch = botocore-a-la-carte-cloudsearch==1.34.9
+cloudsearchdomain = botocore-a-la-carte-cloudsearchdomain==1.34.9
+cloudtrail = botocore-a-la-carte-cloudtrail==1.34.9
+cloudtrail-data = botocore-a-la-carte-cloudtrail-data==1.34.9
+cloudwatch = botocore-a-la-carte-cloudwatch==1.34.9
+codeartifact = botocore-a-la-carte-codeartifact==1.34.9
+codebuild = botocore-a-la-carte-codebuild==1.34.9
+codecatalyst = botocore-a-la-carte-codecatalyst==1.34.9
+codecommit = botocore-a-la-carte-codecommit==1.34.9
+codedeploy = botocore-a-la-carte-codedeploy==1.34.9
+codeguru-reviewer = botocore-a-la-carte-codeguru-reviewer==1.34.9
+codeguru-security = botocore-a-la-carte-codeguru-security==1.34.9
+codeguruprofiler = botocore-a-la-carte-codeguruprofiler==1.34.9
+codepipeline = botocore-a-la-carte-codepipeline==1.34.9
+codestar = botocore-a-la-carte-codestar==1.34.9
+codestar-connections = botocore-a-la-carte-codestar-connections==1.34.9
+codestar-notifications = botocore-a-la-carte-codestar-notifications==1.34.9
+cognito-identity = botocore-a-la-carte-cognito-identity==1.34.9
+cognito-idp = botocore-a-la-carte-cognito-idp==1.34.9
+cognito-sync = botocore-a-la-carte-cognito-sync==1.34.9
+comprehend = botocore-a-la-carte-comprehend==1.34.9
+comprehendmedical = botocore-a-la-carte-comprehendmedical==1.34.9
+compute-optimizer = botocore-a-la-carte-compute-optimizer==1.34.9
+config = botocore-a-la-carte-config==1.34.9
+connect = botocore-a-la-carte-connect==1.34.9
+connect-contact-lens = botocore-a-la-carte-connect-contact-lens==1.34.9
+connectcampaigns = botocore-a-la-carte-connectcampaigns==1.34.9
+connectcases = botocore-a-la-carte-connectcases==1.34.9
+connectparticipant = botocore-a-la-carte-connectparticipant==1.34.9
+controltower = botocore-a-la-carte-controltower==1.34.9
+cost-optimization-hub = botocore-a-la-carte-cost-optimization-hub==1.34.9
+cur = botocore-a-la-carte-cur==1.34.9
+customer-profiles = botocore-a-la-carte-customer-profiles==1.34.9
+databrew = botocore-a-la-carte-databrew==1.34.9
+dataexchange = botocore-a-la-carte-dataexchange==1.34.9
+datapipeline = botocore-a-la-carte-datapipeline==1.34.9
+datasync = botocore-a-la-carte-datasync==1.34.9
+datazone = botocore-a-la-carte-datazone==1.34.9
+dax = botocore-a-la-carte-dax==1.34.9
+detective = botocore-a-la-carte-detective==1.34.9
+devicefarm = botocore-a-la-carte-devicefarm==1.34.9
+devops-guru = botocore-a-la-carte-devops-guru==1.34.9
+directconnect = botocore-a-la-carte-directconnect==1.34.9
+discovery = botocore-a-la-carte-discovery==1.34.9
+dlm = botocore-a-la-carte-dlm==1.34.9
+dms = botocore-a-la-carte-dms==1.34.9
+docdb = botocore-a-la-carte-docdb==1.34.9
+docdb-elastic = botocore-a-la-carte-docdb-elastic==1.34.9
+drs = botocore-a-la-carte-drs==1.34.9
+ds = botocore-a-la-carte-ds==1.34.9
+dynamodb = botocore-a-la-carte-dynamodb==1.34.9
+dynamodbstreams = botocore-a-la-carte-dynamodbstreams==1.34.9
+ebs = botocore-a-la-carte-ebs==1.34.9
+ec2 = botocore-a-la-carte-ec2==1.34.9
+ec2-instance-connect = botocore-a-la-carte-ec2-instance-connect==1.34.9
+ecr = botocore-a-la-carte-ecr==1.34.9
+ecr-public = botocore-a-la-carte-ecr-public==1.34.9
+ecs = botocore-a-la-carte-ecs==1.34.9
+efs = botocore-a-la-carte-efs==1.34.9
+eks = botocore-a-la-carte-eks==1.34.9
+eks-auth = botocore-a-la-carte-eks-auth==1.34.9
+elastic-inference = botocore-a-la-carte-elastic-inference==1.34.9
+elasticache = botocore-a-la-carte-elasticache==1.34.9
+elasticbeanstalk = botocore-a-la-carte-elasticbeanstalk==1.34.9
+elastictranscoder = botocore-a-la-carte-elastictranscoder==1.34.9
+elb = botocore-a-la-carte-elb==1.34.9
+elbv2 = botocore-a-la-carte-elbv2==1.34.9
+emr = botocore-a-la-carte-emr==1.34.9
+emr-containers = botocore-a-la-carte-emr-containers==1.34.9
+emr-serverless = botocore-a-la-carte-emr-serverless==1.34.9
+entityresolution = botocore-a-la-carte-entityresolution==1.34.9
+es = botocore-a-la-carte-es==1.34.9
+events = botocore-a-la-carte-events==1.34.9
+evidently = botocore-a-la-carte-evidently==1.34.9
+finspace = botocore-a-la-carte-finspace==1.34.9
+finspace-data = botocore-a-la-carte-finspace-data==1.34.9
+firehose = botocore-a-la-carte-firehose==1.34.9
+fis = botocore-a-la-carte-fis==1.34.9
+fms = botocore-a-la-carte-fms==1.34.9
+forecast = botocore-a-la-carte-forecast==1.34.9
+forecastquery = botocore-a-la-carte-forecastquery==1.34.9
+frauddetector = botocore-a-la-carte-frauddetector==1.34.9
+freetier = botocore-a-la-carte-freetier==1.34.9
+fsx = botocore-a-la-carte-fsx==1.34.9
+gamelift = botocore-a-la-carte-gamelift==1.34.9
+glacier = botocore-a-la-carte-glacier==1.34.9
+globalaccelerator = botocore-a-la-carte-globalaccelerator==1.34.9
+glue = botocore-a-la-carte-glue==1.34.9
+grafana = botocore-a-la-carte-grafana==1.34.9
+greengrass = botocore-a-la-carte-greengrass==1.34.9
+greengrassv2 = botocore-a-la-carte-greengrassv2==1.34.9
+groundstation = botocore-a-la-carte-groundstation==1.34.9
+guardduty = botocore-a-la-carte-guardduty==1.34.9
+health = botocore-a-la-carte-health==1.34.9
+healthlake = botocore-a-la-carte-healthlake==1.34.9
+honeycode = botocore-a-la-carte-honeycode==1.34.9
+iam = botocore-a-la-carte-iam==1.34.9
+identitystore = botocore-a-la-carte-identitystore==1.34.9
+imagebuilder = botocore-a-la-carte-imagebuilder==1.34.9
+importexport = botocore-a-la-carte-importexport==1.34.9
+inspector = botocore-a-la-carte-inspector==1.34.9
+inspector-scan = botocore-a-la-carte-inspector-scan==1.34.9
+inspector2 = botocore-a-la-carte-inspector2==1.34.9
+internetmonitor = botocore-a-la-carte-internetmonitor==1.34.9
+iot = botocore-a-la-carte-iot==1.34.9
+iot-data = botocore-a-la-carte-iot-data==1.34.9
+iot-jobs-data = botocore-a-la-carte-iot-jobs-data==1.34.9
+iot-roborunner = botocore-a-la-carte-iot-roborunner==1.34.9
+iot1click-devices = botocore-a-la-carte-iot1click-devices==1.34.9
+iot1click-projects = botocore-a-la-carte-iot1click-projects==1.34.9
+iotanalytics = botocore-a-la-carte-iotanalytics==1.34.9
+iotdeviceadvisor = botocore-a-la-carte-iotdeviceadvisor==1.34.9
+iotevents = botocore-a-la-carte-iotevents==1.34.9
+iotevents-data = botocore-a-la-carte-iotevents-data==1.34.9
+iotfleethub = botocore-a-la-carte-iotfleethub==1.34.9
+iotfleetwise = botocore-a-la-carte-iotfleetwise==1.34.9
+iotsecuretunneling = botocore-a-la-carte-iotsecuretunneling==1.34.9
+iotsitewise = botocore-a-la-carte-iotsitewise==1.34.9
+iotthingsgraph = botocore-a-la-carte-iotthingsgraph==1.34.9
+iottwinmaker = botocore-a-la-carte-iottwinmaker==1.34.9
+iotwireless = botocore-a-la-carte-iotwireless==1.34.9
+ivs = botocore-a-la-carte-ivs==1.34.9
+ivs-realtime = botocore-a-la-carte-ivs-realtime==1.34.9
+ivschat = botocore-a-la-carte-ivschat==1.34.9
+kafka = botocore-a-la-carte-kafka==1.34.9
+kafkaconnect = botocore-a-la-carte-kafkaconnect==1.34.9
+kendra = botocore-a-la-carte-kendra==1.34.9
+kendra-ranking = botocore-a-la-carte-kendra-ranking==1.34.9
+keyspaces = botocore-a-la-carte-keyspaces==1.34.9
+kinesis = botocore-a-la-carte-kinesis==1.34.9
+kinesis-video-archived-media = botocore-a-la-carte-kinesis-video-archived-media==1.34.9
+kinesis-video-media = botocore-a-la-carte-kinesis-video-media==1.34.9
+kinesis-video-signaling = botocore-a-la-carte-kinesis-video-signaling==1.34.9
+kinesis-video-webrtc-storage = botocore-a-la-carte-kinesis-video-webrtc-storage==1.34.9
+kinesisanalytics = botocore-a-la-carte-kinesisanalytics==1.34.9
+kinesisanalyticsv2 = botocore-a-la-carte-kinesisanalyticsv2==1.34.9
+kinesisvideo = botocore-a-la-carte-kinesisvideo==1.34.9
+kms = botocore-a-la-carte-kms==1.34.9
+lakeformation = botocore-a-la-carte-lakeformation==1.34.9
+lambda = botocore-a-la-carte-lambda==1.34.9
+launch-wizard = botocore-a-la-carte-launch-wizard==1.34.9
+lex-models = botocore-a-la-carte-lex-models==1.34.9
+lex-runtime = botocore-a-la-carte-lex-runtime==1.34.9
+lexv2-models = botocore-a-la-carte-lexv2-models==1.34.9
+lexv2-runtime = botocore-a-la-carte-lexv2-runtime==1.34.9
+license-manager = botocore-a-la-carte-license-manager==1.34.9
+license-manager-linux-subscriptions = botocore-a-la-carte-license-manager-linux-subscriptions==1.34.9
+license-manager-user-subscriptions = botocore-a-la-carte-license-manager-user-subscriptions==1.34.9
+lightsail = botocore-a-la-carte-lightsail==1.34.9
+location = botocore-a-la-carte-location==1.34.9
+logs = botocore-a-la-carte-logs==1.34.9
+lookoutequipment = botocore-a-la-carte-lookoutequipment==1.34.9
+lookoutmetrics = botocore-a-la-carte-lookoutmetrics==1.34.9
+lookoutvision = botocore-a-la-carte-lookoutvision==1.34.9
+m2 = botocore-a-la-carte-m2==1.34.9
+machinelearning = botocore-a-la-carte-machinelearning==1.34.9
+macie2 = botocore-a-la-carte-macie2==1.34.9
+managedblockchain = botocore-a-la-carte-managedblockchain==1.34.9
+managedblockchain-query = botocore-a-la-carte-managedblockchain-query==1.34.9
+marketplace-agreement = botocore-a-la-carte-marketplace-agreement==1.34.9
+marketplace-catalog = botocore-a-la-carte-marketplace-catalog==1.34.9
+marketplace-deployment = botocore-a-la-carte-marketplace-deployment==1.34.9
+marketplace-entitlement = botocore-a-la-carte-marketplace-entitlement==1.34.9
+marketplacecommerceanalytics = botocore-a-la-carte-marketplacecommerceanalytics==1.34.9
+mediaconnect = botocore-a-la-carte-mediaconnect==1.34.9
+mediaconvert = botocore-a-la-carte-mediaconvert==1.34.9
+medialive = botocore-a-la-carte-medialive==1.34.9
+mediapackage = botocore-a-la-carte-mediapackage==1.34.9
+mediapackage-vod = botocore-a-la-carte-mediapackage-vod==1.34.9
+mediapackagev2 = botocore-a-la-carte-mediapackagev2==1.34.9
+mediastore = botocore-a-la-carte-mediastore==1.34.9
+mediastore-data = botocore-a-la-carte-mediastore-data==1.34.9
+mediatailor = botocore-a-la-carte-mediatailor==1.34.9
+medical-imaging = botocore-a-la-carte-medical-imaging==1.34.9
+memorydb = botocore-a-la-carte-memorydb==1.34.9
+meteringmarketplace = botocore-a-la-carte-meteringmarketplace==1.34.9
+mgh = botocore-a-la-carte-mgh==1.34.9
+mgn = botocore-a-la-carte-mgn==1.34.9
+migration-hub-refactor-spaces = botocore-a-la-carte-migration-hub-refactor-spaces==1.34.9
+migrationhub-config = botocore-a-la-carte-migrationhub-config==1.34.9
+migrationhuborchestrator = botocore-a-la-carte-migrationhuborchestrator==1.34.9
+migrationhubstrategy = botocore-a-la-carte-migrationhubstrategy==1.34.9
+mobile = botocore-a-la-carte-mobile==1.34.9
+mq = botocore-a-la-carte-mq==1.34.9
+mturk = botocore-a-la-carte-mturk==1.34.9
+mwaa = botocore-a-la-carte-mwaa==1.34.9
+neptune = botocore-a-la-carte-neptune==1.34.9
+neptune-graph = botocore-a-la-carte-neptune-graph==1.34.9
+neptunedata = botocore-a-la-carte-neptunedata==1.34.9
+network-firewall = botocore-a-la-carte-network-firewall==1.34.9
+networkmanager = botocore-a-la-carte-networkmanager==1.34.9
+networkmonitor = botocore-a-la-carte-networkmonitor==1.34.9
+nimble = botocore-a-la-carte-nimble==1.34.9
+oam = botocore-a-la-carte-oam==1.34.9
+omics = botocore-a-la-carte-omics==1.34.9
+opensearch = botocore-a-la-carte-opensearch==1.34.9
+opensearchserverless = botocore-a-la-carte-opensearchserverless==1.34.9
+opsworks = botocore-a-la-carte-opsworks==1.34.9
+opsworkscm = botocore-a-la-carte-opsworkscm==1.34.9
+organizations = botocore-a-la-carte-organizations==1.34.9
+osis = botocore-a-la-carte-osis==1.34.9
+outposts = botocore-a-la-carte-outposts==1.34.9
+panorama = botocore-a-la-carte-panorama==1.34.9
+payment-cryptography = botocore-a-la-carte-payment-cryptography==1.34.9
+payment-cryptography-data = botocore-a-la-carte-payment-cryptography-data==1.34.9
+pca-connector-ad = botocore-a-la-carte-pca-connector-ad==1.34.9
+personalize = botocore-a-la-carte-personalize==1.34.9
+personalize-events = botocore-a-la-carte-personalize-events==1.34.9
+personalize-runtime = botocore-a-la-carte-personalize-runtime==1.34.9
+pi = botocore-a-la-carte-pi==1.34.9
+pinpoint = botocore-a-la-carte-pinpoint==1.34.9
+pinpoint-email = botocore-a-la-carte-pinpoint-email==1.34.9
+pinpoint-sms-voice = botocore-a-la-carte-pinpoint-sms-voice==1.34.9
+pinpoint-sms-voice-v2 = botocore-a-la-carte-pinpoint-sms-voice-v2==1.34.9
+pipes = botocore-a-la-carte-pipes==1.34.9
+polly = botocore-a-la-carte-polly==1.34.9
+pricing = botocore-a-la-carte-pricing==1.34.9
+privatenetworks = botocore-a-la-carte-privatenetworks==1.34.9
+proton = botocore-a-la-carte-proton==1.34.9
+qbusiness = botocore-a-la-carte-qbusiness==1.34.9
+qconnect = botocore-a-la-carte-qconnect==1.34.9
+qldb = botocore-a-la-carte-qldb==1.34.9
+qldb-session = botocore-a-la-carte-qldb-session==1.34.9
+quicksight = botocore-a-la-carte-quicksight==1.34.9
+ram = botocore-a-la-carte-ram==1.34.9
+rbin = botocore-a-la-carte-rbin==1.34.9
+rds = botocore-a-la-carte-rds==1.34.9
+rds-data = botocore-a-la-carte-rds-data==1.34.9
+redshift = botocore-a-la-carte-redshift==1.34.9
+redshift-data = botocore-a-la-carte-redshift-data==1.34.9
+redshift-serverless = botocore-a-la-carte-redshift-serverless==1.34.9
+rekognition = botocore-a-la-carte-rekognition==1.34.9
+repostspace = botocore-a-la-carte-repostspace==1.34.9
+resiliencehub = botocore-a-la-carte-resiliencehub==1.34.9
+resource-explorer-2 = botocore-a-la-carte-resource-explorer-2==1.34.9
+resource-groups = botocore-a-la-carte-resource-groups==1.34.9
+resourcegroupstaggingapi = botocore-a-la-carte-resourcegroupstaggingapi==1.34.9
+robomaker = botocore-a-la-carte-robomaker==1.34.9
+rolesanywhere = botocore-a-la-carte-rolesanywhere==1.34.9
+route53 = botocore-a-la-carte-route53==1.34.9
+route53-recovery-cluster = botocore-a-la-carte-route53-recovery-cluster==1.34.9
+route53-recovery-control-config = botocore-a-la-carte-route53-recovery-control-config==1.34.9
+route53-recovery-readiness = botocore-a-la-carte-route53-recovery-readiness==1.34.9
+route53domains = botocore-a-la-carte-route53domains==1.34.9
+route53resolver = botocore-a-la-carte-route53resolver==1.34.9
+rum = botocore-a-la-carte-rum==1.34.9
+s3 = botocore-a-la-carte-s3==1.34.9
+s3control = botocore-a-la-carte-s3control==1.34.9
+s3outposts = botocore-a-la-carte-s3outposts==1.34.9
+sagemaker = botocore-a-la-carte-sagemaker==1.34.9
+sagemaker-a2i-runtime = botocore-a-la-carte-sagemaker-a2i-runtime==1.34.9
+sagemaker-edge = botocore-a-la-carte-sagemaker-edge==1.34.9
+sagemaker-featurestore-runtime = botocore-a-la-carte-sagemaker-featurestore-runtime==1.34.9
+sagemaker-geospatial = botocore-a-la-carte-sagemaker-geospatial==1.34.9
+sagemaker-metrics = botocore-a-la-carte-sagemaker-metrics==1.34.9
+sagemaker-runtime = botocore-a-la-carte-sagemaker-runtime==1.34.9
+savingsplans = botocore-a-la-carte-savingsplans==1.34.9
+scheduler = botocore-a-la-carte-scheduler==1.34.9
+schemas = botocore-a-la-carte-schemas==1.34.9
+sdb = botocore-a-la-carte-sdb==1.34.9
+secretsmanager = botocore-a-la-carte-secretsmanager==1.34.9
+securityhub = botocore-a-la-carte-securityhub==1.34.9
+securitylake = botocore-a-la-carte-securitylake==1.34.9
+serverlessrepo = botocore-a-la-carte-serverlessrepo==1.34.9
+service-quotas = botocore-a-la-carte-service-quotas==1.34.9
+servicecatalog = botocore-a-la-carte-servicecatalog==1.34.9
+servicecatalog-appregistry = botocore-a-la-carte-servicecatalog-appregistry==1.34.9
+servicediscovery = botocore-a-la-carte-servicediscovery==1.34.9
+ses = botocore-a-la-carte-ses==1.34.9
+sesv2 = botocore-a-la-carte-sesv2==1.34.9
+shield = botocore-a-la-carte-shield==1.34.9
+signer = botocore-a-la-carte-signer==1.34.9
+simspaceweaver = botocore-a-la-carte-simspaceweaver==1.34.9
+sms = botocore-a-la-carte-sms==1.34.9
+sms-voice = botocore-a-la-carte-sms-voice==1.34.9
+snow-device-management = botocore-a-la-carte-snow-device-management==1.34.9
+snowball = botocore-a-la-carte-snowball==1.34.9
+sns = botocore-a-la-carte-sns==1.34.9
+sqs = botocore-a-la-carte-sqs==1.34.9
+ssm = botocore-a-la-carte-ssm==1.34.9
+ssm-contacts = botocore-a-la-carte-ssm-contacts==1.34.9
+ssm-incidents = botocore-a-la-carte-ssm-incidents==1.34.9
+ssm-sap = botocore-a-la-carte-ssm-sap==1.34.9
+sso = botocore-a-la-carte-sso==1.34.9
+sso-admin = botocore-a-la-carte-sso-admin==1.34.9
+sso-oidc = botocore-a-la-carte-sso-oidc==1.34.9
+stepfunctions = botocore-a-la-carte-stepfunctions==1.34.9
+storagegateway = botocore-a-la-carte-storagegateway==1.34.9
+sts = botocore-a-la-carte-sts==1.34.9
+support = botocore-a-la-carte-support==1.34.9
+support-app = botocore-a-la-carte-support-app==1.34.9
+swf = botocore-a-la-carte-swf==1.34.9
+synthetics = botocore-a-la-carte-synthetics==1.34.9
+textract = botocore-a-la-carte-textract==1.34.9
+timestream-query = botocore-a-la-carte-timestream-query==1.34.9
+timestream-write = botocore-a-la-carte-timestream-write==1.34.9
+tnb = botocore-a-la-carte-tnb==1.34.9
+transcribe = botocore-a-la-carte-transcribe==1.34.9
+transfer = botocore-a-la-carte-transfer==1.34.9
+translate = botocore-a-la-carte-translate==1.34.9
+trustedadvisor = botocore-a-la-carte-trustedadvisor==1.34.9
+verifiedpermissions = botocore-a-la-carte-verifiedpermissions==1.34.9
+voice-id = botocore-a-la-carte-voice-id==1.34.9
+vpc-lattice = botocore-a-la-carte-vpc-lattice==1.34.9
+waf = botocore-a-la-carte-waf==1.34.9
+waf-regional = botocore-a-la-carte-waf-regional==1.34.9
+wafv2 = botocore-a-la-carte-wafv2==1.34.9
+wellarchitected = botocore-a-la-carte-wellarchitected==1.34.9
+wisdom = botocore-a-la-carte-wisdom==1.34.9
+workdocs = botocore-a-la-carte-workdocs==1.34.9
+worklink = botocore-a-la-carte-worklink==1.34.9
+workmail = botocore-a-la-carte-workmail==1.34.9
+workmailmessageflow = botocore-a-la-carte-workmailmessageflow==1.34.9
+workspaces = botocore-a-la-carte-workspaces==1.34.9
+workspaces-thin-client = botocore-a-la-carte-workspaces-thin-client==1.34.9
+workspaces-web = botocore-a-la-carte-workspaces-web==1.34.9
+xray = botocore-a-la-carte-xray==1.34.9
 
 [flake8]
 ignore = E203,E226,E501,E731,W503,W504
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `botocore-a-la-carte-1.34.8/setup.py` & `botocore-a-la-carte-1.34.9/setup.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/__init__.py` & `botocore-a-la-carte-1.34.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/acceptance/features/environment.py` & `botocore-a-la-carte-1.34.9/tests/acceptance/features/environment.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/autoscaling/autoscaling.feature` & `botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/autoscaling/autoscaling.feature`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature` & `botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/cognitoidentity/cognitoidentity.feature`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/acceptance/features/smoke/support/support.feature` & `botocore-a-la-carte-1.34.9/tests/acceptance/features/smoke/support/support.feature`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/acceptance/features/steps/base.py` & `botocore-a-la-carte-1.34.9/tests/acceptance/features/steps/base.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/cmd-runner` & `botocore-a-la-carte-1.34.9/tests/cmd-runner`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/__init__.py` & `botocore-a-la-carte-1.34.9/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/__init__.py` & `botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/profile-tests.json` & `botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/profile-tests.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py` & `botocore-a-la-carte-1.34.9/tests/functional/configured_endpoint_urls/test_configured_endpoint_url.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/conftest.py` & `botocore-a-la-carte-1.34.9/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/csm/__init__.py` & `botocore-a-la-carte-1.34.9/tests/functional/csm/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/csm/cases.json` & `botocore-a-la-carte-1.34.9/tests/functional/csm/cases.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/csm/data/csmtest/2018-06-19/service-2.json` & `botocore-a-la-carte-1.34.9/tests/functional/csm/data/csmtest/2018-06-19/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/csm/test_monitoring.py` & `botocore-a-la-carte-1.34.9/tests/functional/csm/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/__init__.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_alias.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_autoscaling.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_ec2.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_ec2.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_glacier.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_glacier.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_lex.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_lex.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_s3.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_s3.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_secretsmanager.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_shared_example_config.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_shared_example_config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/docs/test_streaming_body.py` & `botocore-a-la-carte-1.34.9/tests/functional/docs/test_streaming_body.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/accessanalyzer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/account/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/account/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/acm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/acm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/acm-pca/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/alexaforbusiness/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amp/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amp/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplify/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplifybackend/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/amplifyuibuilder/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigateway/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigatewaymanagementapi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apigatewayv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appconfig/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appconfigdata/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appfabric/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appflow/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appintegrations/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/application-autoscaling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/application-insights/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/applicationcostprofiler/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appmesh/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/apprunner/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appstream/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/appsync/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/arc-zonal-shift/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/athena/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/athena/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/auditmanager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/autoscaling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/autoscaling-plans/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/b2bi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backup/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backup/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backup-gateway/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/backupstorage/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/batch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/batch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bcm-data-exports/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-agent/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-agent-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/bedrock-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/billingconductor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/braket/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/braket/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/budgets/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ce/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ce/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-identity/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-media-pipelines/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-meetings/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-messaging/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/chime-sdk-voice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cleanrooms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cleanroomsml/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloud9/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudcontrol/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/clouddirectory/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudformation/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudfront/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudfront-keyvaluestore/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudhsm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudhsmv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudsearch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudsearchdomain/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudtrail/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudtrail-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cloudwatch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeartifact/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codebuild/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codecatalyst/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codecommit/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codedeploy/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguru-reviewer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguru-security/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codeguruprofiler/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codepipeline/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar-connections/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/codestar-notifications/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-identity/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-idp/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cognito-sync/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/comprehend/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/comprehendmedical/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/compute-optimizer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/config/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/config/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connect-contact-lens/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectcampaigns/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectcases/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/connectparticipant/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/controltower/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cost-optimization-hub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/cur/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/cur/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/customer-profiles/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/databrew/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dataexchange/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datapipeline/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datasync/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/datazone/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dax/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dax/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/detective/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/detective/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/devicefarm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/devops-guru/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/directconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/discovery/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dlm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/docdb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/docdb-elastic/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/drs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/drs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ds/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ds/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dynamodb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/dynamodbstreams/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ebs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ec2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ec2-instance-connect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecr/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecr-public/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ecs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/efs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/efs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/eks/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/eks/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/eks-auth/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elastic-inference/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elasticache/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elasticbeanstalk/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elastictranscoder/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/elbv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr-containers/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/emr-serverless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/entityresolution/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/es/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/es/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/events/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/events/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/evidently/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/finspace/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/finspace-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/firehose/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fis/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fis/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/forecast/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/forecastquery/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/frauddetector/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/freetier/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/fsx/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/gamelift/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/glacier/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/globalaccelerator/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/glue/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/glue/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/grafana/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/greengrass/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/greengrassv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/groundstation/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/guardduty/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/health/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/health/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/healthlake/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/honeycode/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iam/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iam/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/identitystore/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/imagebuilder/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/importexport/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector-scan/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/inspector2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/internetmonitor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-jobs-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot-roborunner/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot-roborunner/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot1click-devices/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iot1click-projects/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotanalytics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotdeviceadvisor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotevents/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotevents-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotfleethub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotfleetwise/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotsecuretunneling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotsitewise/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotthingsgraph/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iottwinmaker/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/iotwireless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivs-realtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ivschat/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kafka/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kafkaconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kendra/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kendra-ranking/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/keyspaces/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-archived-media/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-media/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-signaling/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesis-video-webrtc-storage/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisanalytics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisanalyticsv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kinesisvideo/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/kms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/kms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lakeformation/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lambda/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/launch-wizard/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lex-models/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lex-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lexv2-models/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lexv2-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager-linux-subscriptions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/license-manager-user-subscriptions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lightsail/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/location/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/location/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/logs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/logs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutequipment/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutmetrics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/lookoutvision/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/m2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/m2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/machinelearning/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/macie2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/managedblockchain/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/managedblockchain-query/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-agreement/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-catalog/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-deployment/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplace-entitlement/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/marketplacecommerceanalytics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediaconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediaconvert/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/medialive/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackage/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackage-vod/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediapackagev2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediastore/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediastore-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mediatailor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/medical-imaging/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/memorydb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/meteringmarketplace/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mgh/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mgn/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migration-hub-refactor-spaces/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhub-config/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhuborchestrator/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/migrationhubstrategy/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mobile/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mq/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mq/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mturk/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/mwaa/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptune/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptune-graph/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/neptunedata/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/network-firewall/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/networkmanager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/networkmonitor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/nimble/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/oam/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/oam/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/omics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/omics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opensearch/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opensearchserverless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opsworks/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/opsworkscm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/organizations/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/osis/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/osis/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/outposts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/panorama/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/payment-cryptography/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/payment-cryptography-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pca-connector-ad/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize-events/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/personalize-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-email/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-sms-voice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pinpoint-sms-voice-v2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pipes/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/polly/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/polly/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/pricing/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/privatenetworks/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/proton/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/proton/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qbusiness/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qconnect/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qldb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/qldb-session/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/quicksight/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ram/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ram/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rbin/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rds/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rds/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rds-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift-data/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/redshift-serverless/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rekognition/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/repostspace/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resiliencehub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resource-explorer-2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resource-groups/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/resourcegroupstaggingapi/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/robomaker/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rolesanywhere/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-cluster/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-control-config/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53-recovery-readiness/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53domains/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/route53resolver/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/rum/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/rum/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3control/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/s3outposts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-a2i-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-edge/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-featurestore-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-geospatial/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-metrics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sagemaker-runtime/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/savingsplans/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/scheduler/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/schemas/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sdb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/secretsmanager/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/securityhub/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/securitylake/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/serverlessrepo/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/service-quotas/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicecatalog/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicecatalog-appregistry/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/servicediscovery/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ses/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ses/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sesv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/shield/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/shield/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/signer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/signer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/simspaceweaver/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sms/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sms/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sms-voice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/snow-device-management/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/snowball/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sns/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sns/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sqs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-contacts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-incidents/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/ssm-sap/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso-admin/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sso-oidc/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/stepfunctions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/storagegateway/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/sts/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/sts/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/support/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/support/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/support-app/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/swf/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/swf/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/synthetics/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/textract/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/textract/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/timestream-query/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/timestream-write/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/tnb/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/transcribe/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/transfer/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/translate/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/translate/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/trustedadvisor/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/verifiedpermissions/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/voice-id/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/vpc-lattice/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/waf/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/waf/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/waf-regional/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wafv2/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wellarchitected/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/wisdom/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workdocs/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/worklink/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workmail/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workmailmessageflow/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces-thin-client/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/workspaces-web/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/endpoint-rules/xray/endpoint-tests-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/endpoint-rules/xray/endpoint-tests-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/leak/__init__.py` & `botocore-a-la-carte-1.34.9/tests/functional/leak/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/leak/test_resource_leaks.py` & `botocore-a-la-carte-1.34.9/tests/functional/leak/test_resource_leaks.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json` & `botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/service-2.json` & `botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/models/custom-acm/2015-12-08/waiters-2.json` & `botocore-a-la-carte-1.34.9/tests/functional/models/custom-acm/2015-12-08/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/models/endpoints.json` & `botocore-a-la-carte-1.34.9/tests/functional/models/endpoints.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/models/sdk-default-configuration.json` & `botocore-a-la-carte-1.34.9/tests/functional/models/sdk-default-configuration.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json` & `botocore-a-la-carte-1.34.9/tests/functional/models/test-discovery-endpoint/2020-08-20/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/retries/test_bucket.py` & `botocore-a-la-carte-1.34.9/tests/functional/retries/test_bucket.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/retries/test_quota.py` & `botocore-a-la-carte-1.34.9/tests/functional/retries/test_quota.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_alias.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_apigateway.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_client.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_client_class_names.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_client_class_names.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_client_metadata.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_client_metadata.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_cloudformation.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_cloudsearchdomain.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_cloudsearchdomain.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_cognito_idp.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_cognito_idp.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_compress.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_compress.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_config_provider.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_config_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_context_params.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_context_params.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_credentials.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_discovery.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_discovery.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_docdb.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_docdb.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_dynamodb.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_ec2.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_ec2.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_endpoint_rulesets.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_endpoint_rulesets.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_endpoints.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_event_alias.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_event_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_eventbridge.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_eventbridge.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_events.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_events.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_h2_required.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_h2_required.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_history.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_history.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_importexport.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_importexport.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_iot_data.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_iot_data.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_kinesis.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_lex.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_lex.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_loaders.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_machinelearning.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_machinelearning.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_model_backcompat.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_model_backcompat.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_model_completeness.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_model_completeness.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_modeled_exceptions.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_modeled_exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_mturk.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_mturk.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_neptune.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_neptune.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_paginate.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_paginate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_paginator_config.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_paginator_config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_public_apis.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_public_apis.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_rds.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_rds.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_regions.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_regions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_response_shadowing.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_response_shadowing.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_retry.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_retry.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_route53.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_route53.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_s3.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_s3.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_s3_control.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_s3_control.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_s3_control_redirects.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_s3_control_redirects.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_s3express.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_s3express.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_sagemaker.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_sagemaker.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_service_alias.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_service_alias.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_service_names.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_service_names.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_session.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_six_imports.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_six_imports.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_six_threading.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_six_threading.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_sts.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_sts.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_stub.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_stub.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_tagged_unions_unknown.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_tagged_unions_unknown.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_useragent.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_useragent.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_utils.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/test_waiter_config.py` & `botocore-a-la-carte-1.34.9/tests/functional/test_waiter_config.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/utils/__init__.py` & `botocore-a-la-carte-1.34.9/tests/functional/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/functional/utils/credentialprocess.py` & `botocore-a-la-carte-1.34.9/tests/functional/utils/credentialprocess.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/__init__.py` & `botocore-a-la-carte-1.34.9/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_apigateway.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_client.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_client_http.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_client_http.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_cloudformation.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_cloudformation.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_cognito_identity.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_cognito_identity.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_credentials.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_ec2.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_ec2.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_elastictranscoder.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_elastictranscoder.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_emr.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_emr.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_glacier.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_glacier.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_loaders.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_rds.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_rds.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_route53.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_route53.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_s3.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_s3.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_session.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_smoke.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_smoke.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_sts.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_sts.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_utils.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/integration/test_waiters.py` & `botocore-a-la-carte-1.34.9/tests/integration/test_waiters.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/__init__.py` & `botocore-a-la-carte-1.34.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/__init__.py` & `botocore-a-la-carte-1.34.9/tests/unit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/LICENSE` & `botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/LICENSE`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt` & `botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/normalize-path/normalize-path.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq` & `botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-after/post-sts-header-after.sreq`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq` & `botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.creq`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq` & `botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/post-sts-header-before/post-sts-header-before.sreq`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt` & `botocore-a-la-carte-1.34.9/tests/unit/auth/aws4_testsuite/post-sts-token/readme.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/test_signers.py` & `botocore-a-la-carte-1.34.9/tests/unit/auth/test_signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/auth/test_sigv4.py` & `botocore-a-la-carte-1.34.9/tests/unit/auth/test_sigv4.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/cfg/aws_config_badbytes` & `botocore-a-la-carte-1.34.9/tests/unit/cfg/aws_config_badbytes`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/crt/auth/test_crt_signers.py` & `botocore-a-la-carte-1.34.9/tests/unit/crt/auth/test_crt_signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/crt/auth/test_crt_sigv4.py` & `botocore-a-la-carte-1.34.9/tests/unit/crt/auth/test_crt_sigv4.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/aws-region.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/aws-region.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/default-values.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/default-values.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/eventbridge.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/eventbridge.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/fns.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/fns.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/is-virtual-hostable-s3-bucket.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/parse-arn.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/parse-arn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/parse-url.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/parse-url.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/partition-fn.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/partition-fn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/substring.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/substring.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/uri-encode.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/uri-encode.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/test-cases/valid-hostlabel.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/test-cases/valid-hostlabel.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/aws-region.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/aws-region.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/default-values.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/default-values.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/deprecated-param.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/deprecated-param.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/eventbridge.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/eventbridge.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/fns.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/fns.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/get-attr-type-inference.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/headers.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/headers.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/is-virtual-hostable-s3-bucket.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/local-region-override.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/local-region-override.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/minimal-ruleset.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/parse-arn.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/parse-arn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/parse-url.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/parse-url.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/partition-fn.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/partition-fn.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/substring.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/substring.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/uri-encode.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/uri-encode.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json` & `botocore-a-la-carte-1.34.9/tests/unit/data/endpoints/valid-rules/valid-hostlabel.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/__init__.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/__init__.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/test_docstringparser.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/test_docstringparser.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/test_document.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/test_document.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/bcdoc/test_style.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/bcdoc/test_style.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_client.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_docs.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_docs.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_docstring.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_docstring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_example.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_example.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_method.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_method.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_paginator.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_paginator.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_params.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_params.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_service.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_service.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_sharedexample.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_sharedexample.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_utils.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/docs/test_waiter.py` & `botocore-a-la-carte-1.34.9/tests/unit/docs/test_waiter.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/input/ec2.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/input/ec2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/input/json.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/input/json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/input/query.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/input/query.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/input/rest-json.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/input/rest-json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/input/rest-xml.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/input/rest-xml.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/output/ec2.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/output/ec2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/output/json.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/output/json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/output/query.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/output/query.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/output/rest-json.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/output/rest-json.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/protocols/output/rest-xml.json` & `botocore-a-la-carte-1.34.9/tests/unit/protocols/output/rest-xml.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/README.rst` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/README.rst`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/__init__.py` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/json/expected/elastictranscoder-list-pipelines.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/test_response_parsing.py` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/test_response_parsing.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-adjustment-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-auto-scaling-notification-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-metric-collection-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-scaling-process-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/autoscaling-describe-termination-policy-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-get-template.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudformation-get-template.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-distribution.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-invalidation.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-get-streaming-distribution.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-cloud-front-origin-access-identities.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-distributions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-invalidations.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudfront-list-streaming-distributions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/cloudwatch-list-metrics.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-bundle-instance.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-bundle-task.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-cancel-reserved-instances-listing.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-dhcp-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-instance-export-task.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-key-pair.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-acl.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-network-interface.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-reserved-instances-listing.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-create-route-table.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-account-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-addresses.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-availability-zones.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-bundle-tasks.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-dhcp-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-export-tasks.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instance-status.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-internet-gateways.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-acls.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-network-interfaces.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-regions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-regions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances-offerings.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-reserved-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-route-tables.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-security-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-snapshots.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-instance-requests.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-spot-price-history.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-subnets.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volume-status.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-volumes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpcs.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-connections.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-describe-vpn-gateways.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-instance.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-instance.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-instance.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-volume.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-volume.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-import-volume.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-request-spot-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-run-instances.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-run-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-run-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ec2-unmonitor-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application-version.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-application.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-configuration-template.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-create-environment.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-application-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-applications.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-configuration-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-environments.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-describe-events.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-list-available-solution-stacks.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-retrieve-environment-info.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-terminate-environment.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application-version.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elasticbeanstalk-update-application.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policies.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/elb-describe-load-balancer-policy-types.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-create-virtual-mfa-device.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-account-summary.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-account-summary.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-group.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-group.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-group.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-user-policy.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-get-user-policy.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-access-keys.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-groups.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-instance-profiles.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-roles.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-roles.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-roles.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-roles.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-server-certificates.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-signing-certificates.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-users.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-users.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-users.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-users.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/iam-list-virtual-mfa-devices.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/importexport-list-jobs.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-engine-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-parameter-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-security-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-snapshots.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-db-subnet-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-event-categories.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-events.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-events.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-events.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-events.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-option-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances-offerings.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/rds-describe-reserved-db-instances.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-authorize-cluster-security-group-ingress.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-copy-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-parameter-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-security-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster-subnet-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-create-cluster.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-delete-cluster.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameter-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-parameters.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-security-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-snapshots.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-subnet-groups.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-cluster-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-clusters.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-events.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-orderable-cluster-options.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-node-offerings.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-describe-reserved-nodes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-modify-cluster-parameter-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-purchase-reserved-node-offering.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reboot-cluster.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-reset-cluster-parameter-group.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-restore-from-cluster-snapshot.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/redshift-revoke-cluster-security-group-ingress.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-acl.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-get-bucket-logging.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-buckets.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-buckets.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-buckets.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads#2.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-multipart-uploads.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-object-versions.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-object-versions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-objects.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-objects.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/s3-list-objects.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/s3-list-objects.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-dkim-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-notification-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-identity-verification-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/ses-get-send-statistics.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-subscription-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-get-topic-attributes.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-subscriptions-by-topic.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sns-list-subscriptions.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-get-queue-attributes.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sqs-receive-message.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sqs-receive-message.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sts-get-session-token.json` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sts-get-session-token.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml` & `botocore-a-la-carte-1.34.9/tests/unit/response_parsing/xml/responses/sts-get-session-token.xml`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/retries/test_adaptive.py` & `botocore-a-la-carte-1.34.9/tests/unit/retries/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/retries/test_bucket.py` & `botocore-a-la-carte-1.34.9/tests/unit/retries/test_bucket.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/retries/test_quota.py` & `botocore-a-la-carte-1.34.9/tests/unit/retries/test_quota.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/retries/test_special.py` & `botocore-a-la-carte-1.34.9/tests/unit/retries/test_special.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/retries/test_standard.py` & `botocore-a-la-carte-1.34.9/tests/unit/retries/test_standard.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/retries/test_throttling.py` & `botocore-a-la-carte-1.34.9/tests/unit/retries/test_throttling.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_args.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_args.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_auth_bearer.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_auth_bearer.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_auth_sigv4.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_auth_sigv4.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_awsrequest.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_awsrequest.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_client.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_compat.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_compress.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_compress.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_config_provider.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_config_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_configloader.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_configloader.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_credentials.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_discovery.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_endpoint.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_endpoint_provider.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_endpoint_provider.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_errorfactory.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_errorfactory.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_eventstream.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_eventstream.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_exceptions.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_handlers.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_handlers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_history.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_hooks.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_hooks.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_http_client_exception_mapping.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_http_client_exception_mapping.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_http_session.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_http_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_httpchecksum.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_httpchecksum.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_idempotency.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_idempotency.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_loaders.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_model.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_monitoring.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_paginate.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_parsers.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_protocols.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_protocols.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_regions.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_regions.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_response.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_retryhandler.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_s3_addressing.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_s3_addressing.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_serialize.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_serialize.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_session.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_session_legacy.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_session_legacy.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_signers.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_stub.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_stub.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_tokens.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_tokens.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_translate.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_translate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_useragent.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_useragent.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_utils.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_validate.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-1.34.8/tests/unit/test_waiters.py` & `botocore-a-la-carte-1.34.9/tests/unit/test_waiters.py`

 * *Files identical despite different names*

