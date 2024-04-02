# Comparing `tmp/speakeasy-client-sdk-python-5.5.0.tar.gz` & `tmp/speakeasy-client-sdk-python-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.5.0.tar", last modified: Wed Mar 27 00:12:13 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.5.1.tar", last modified: Tue Apr  2 00:12:11 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.5.0.tar` & `speakeasy-client-sdk-python-5.5.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.076290 speakeasy-client-sdk-python-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-03-27 00:12:13.076290 speakeasy-client-sdk-python-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 00:12:13.076290 speakeasy-client-sdk-python-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.060290 speakeasy-client-sdk-python-5.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.064290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.064290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28386 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.064290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.064290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.072290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.076290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.076290 speakeasy-client-sdk-python-5.5.0/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-03-27 00:11:59.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:12:13.076290 speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-03-27 00:12:12.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-27 00:12:13.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 00:12:12.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 00:12:12.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 00:12:12.000000 speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.400406 speakeasy-client-sdk-python-5.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-04-02 00:12:11.400406 speakeasy-client-sdk-python-5.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:12:11.400406 speakeasy-client-sdk-python-5.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.384406 speakeasy-client-sdk-python-5.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.388406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.388406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28386 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.388406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.388406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.392406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.396406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.396406 speakeasy-client-sdk-python-5.5.1/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-02 00:11:56.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:12:11.400406 speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-04-02 00:12:10.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-02 00:12:11.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:12:10.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-02 00:12:10.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 00:12:10.000000 speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.5.0/PKG-INFO` & `speakeasy-client-sdk-python-5.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.5.0
+Version: 5.5.1
 Summary: Speakeasy API Client SDK for Python
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -122,15 +122,15 @@
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object     | Status Code      | Content Type     |
         | ---------------- | ---------------- | ---------------- |
         | errors.Error     | 5XX              | application/json |
-        | errors.SDKError  | 4x-5xx           | */*              |
+        | errors.SDKError  | 4xx-5xx          | */*              |
         
         ### Example
         
         ```python
         import speakeasy
         from speakeasy.models import errors, operations, shared
```

### Comparing `speakeasy-client-sdk-python-5.5.0/README.md` & `speakeasy-client-sdk-python-5.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object     | Status Code      | Content Type     |
 | ---------------- | ---------------- | ---------------- |
 | errors.Error     | 5XX              | application/json |
-| errors.SDKError  | 4x-5xx           | */*              |
+| errors.SDKError  | 4xx-5xx          | */*              |
 
 ### Example
 
 ```python
 import speakeasy
 from speakeasy.models import errors, operations, shared
```

### Comparing `speakeasy-client-sdk-python-5.5.0/setup.py` & `speakeasy-client-sdk-python-5.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="speakeasy-client-sdk-python",
-    version="5.5.0",
+    version="5.5.1",
     author="Speakeasy",
     description="Speakeasy API Client SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
```

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/auth.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/events.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getworkspaceevents.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/sdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/sdkconfiguration.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: str = ''
     server: str = ''
     globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.4.0'
-    sdk_version: str = '5.5.0'
-    gen_version: str = '2.291.0'
-    user_agent: str = 'speakeasy-sdk/python 5.5.0 2.291.0 0.4.0 speakeasy-client-sdk-python'
+    sdk_version: str = '5.5.1'
+    gen_version: str = '2.295.1'
+    user_agent: str = 'speakeasy-sdk/python 5.5.1 2.295.1 0.4.0 speakeasy-client-sdk-python'
     retry_config: RetryConfig = None
     _hooks: SDKHooks = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url:
             return utils.remove_suffix(self.server_url, '/'), {}
         if not self.server:
```

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.5.0
+Version: 5.5.1
 Summary: Speakeasy API Client SDK for Python
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -122,15 +122,15 @@
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object     | Status Code      | Content Type     |
         | ---------------- | ---------------- | ---------------- |
         | errors.Error     | 5XX              | application/json |
-        | errors.SDKError  | 4x-5xx           | */*              |
+        | errors.SDKError  | 4xx-5xx          | */*              |
         
         ### Example
         
         ```python
         import speakeasy
         from speakeasy.models import errors, operations, shared
```

### Comparing `speakeasy-client-sdk-python-5.5.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.5.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

