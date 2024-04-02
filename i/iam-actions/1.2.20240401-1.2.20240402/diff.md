# Comparing `tmp/iam_actions-1.2.20240401.tar.gz` & `tmp/iam_actions-1.2.20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240401.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240402.tar", max compression
```

## Comparing `iam_actions-1.2.20240401.tar` & `iam_actions-1.2.20240402.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-01 02:23:08.119806 iam_actions-1.2.20240401/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-01 02:23:08.119806 iam_actions-1.2.20240401/README.md
--rw-r--r--   0        0        0      228 2024-04-01 02:23:08.119806 iam_actions-1.2.20240401/iam_actions/__init__.py
--rw-r--r--   0        0        0  4759201 2024-04-01 02:25:30.009644 iam_actions-1.2.20240401/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-01 02:23:08.119806 iam_actions-1.2.20240401/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-01 02:23:08.119806 iam_actions-1.2.20240401/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-01 02:23:08.123806 iam_actions-1.2.20240401/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-01 02:23:08.123806 iam_actions-1.2.20240401/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-01 02:23:08.123806 iam_actions-1.2.20240401/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-01 02:23:08.123806 iam_actions-1.2.20240401/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-01 02:23:08.123806 iam_actions-1.2.20240401/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-01 02:23:08.123806 iam_actions-1.2.20240401/iam_actions/generate/services.py
--rw-r--r--   0        0        0   617975 2024-04-01 02:25:30.009644 iam_actions-1.2.20240401/iam_actions/policies.json
--rw-r--r--   0        0        0   207182 2024-04-01 02:25:30.009644 iam_actions-1.2.20240401/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   599513 2024-04-01 02:25:30.009644 iam_actions-1.2.20240401/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-01 02:25:30.693653 iam_actions-1.2.20240401/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240401/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240401/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/README.md
+-rw-r--r--   0        0        0      228 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4779698 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-02 02:17:46.735590 iam_actions-1.2.20240402/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   621280 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/policies.json
+-rw-r--r--   0        0        0   207224 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   602719 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-02 02:19:54.688534 iam_actions-1.2.20240402/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240402/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240402/PKG-INFO
```

### Comparing `iam_actions-1.2.20240401/LICENSE` & `iam_actions-1.2.20240402/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/README.md` & `iam_actions-1.2.20240402/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/actions.json` & `iam_actions-1.2.20240402/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972738237706008%*

 * *Differences: {"'cloudformation'": "{'ListStackSetAutoDeploymentTargets': OrderedDict([('access_level', "*

 * *                     "'Undocumented'), ('action', 'ListStackSetAutoDeploymentTargets'), "*

 * *                     "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *                     "False), ('resources', [])])}",*

 * * "'codecatalyst'": "{'AssociateIdentityCenterApplicationToSpace': {'condition_keys': "*

 * *                   "['aws:ResourceTag/${TagKey}']}, "*

 * *                   "'AssociateIdent […]*

```diff
@@ -22045,14 +22045,22 @@
             "condition_keys": [],
             "description": "Grants permission to return descriptions of all resources of the specified stack",
             "orphan": false,
             "resources": [
                 "stack"
             ]
         },
+        "ListStackSetAutoDeploymentTargets": {
+            "access_level": "Undocumented",
+            "action": "ListStackSetAutoDeploymentTargets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListStackSetOperationResults": {
             "access_level": "List",
             "action": "ListStackSetOperationResults",
             "condition_keys": [],
             "description": "Grants permission to return summary information about the results of a stack set operation",
             "orphan": false,
             "resources": [
@@ -26374,55 +26382,66 @@
             "resources": [
                 "connections"
             ]
         },
         "AssociateIdentityCenterApplicationToSpace": {
             "access_level": "Write",
             "action": "AssociateIdentityCenterApplicationToSpace",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to associate an IAM Identity Center application with an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "AssociateIdentityToIdentityCenterApplication": {
             "access_level": "Write",
             "action": "AssociateIdentityToIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to associate an identity with an IAM Identity Center application for an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "BatchAssociateIdentitiesToIdentityCenterApplication": {
             "access_level": "Write",
             "action": "BatchAssociateIdentitiesToIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to associate multiple identities with an IAM Identity Center application for an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "BatchDisassociateIdentitiesFromIdentityCenterApplication": {
             "access_level": "Write",
             "action": "BatchDisassociateIdentitiesFromIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to disassociate multiple identities from an IAM Identity Center application for an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "CreateIdentityCenterApplication": {
             "access_level": "Write",
             "action": "CreateIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to create an IAM Identity Center application",
             "orphan": false,
             "resources": []
         },
         "CreateSpace": {
             "access_level": "Write",
             "action": "CreateSpace",
@@ -26433,15 +26452,17 @@
             "description": "Grants permission to create an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": []
         },
         "CreateSpaceAdminRoleAssignment": {
             "access_level": "Write",
             "action": "CreateSpaceAdminRoleAssignment",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to create an administrator role assignment for a given Amazon CodeCatalyst space and IAM Identity Center application",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "DeleteConnection": {
@@ -26455,15 +26476,17 @@
             "resources": [
                 "connections"
             ]
         },
         "DeleteIdentityCenterApplication": {
             "access_level": "Write",
             "action": "DeleteIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete an IAM Identity Center application",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "DisassociateIamRoleFromConnection": {
@@ -26477,25 +26500,29 @@
             "resources": [
                 "connections"
             ]
         },
         "DisassociateIdentityCenterApplicationFromSpace": {
             "access_level": "Write",
             "action": "DisassociateIdentityCenterApplicationFromSpace",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to disassociate an IAM Identity Center application from an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "DisassociateIdentityFromIdentityCenterApplication": {
             "access_level": "Write",
             "action": "DisassociateIdentityFromIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to disassociate an identity from an IAM Identity Center application for an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "GetBillingAuthorization": {
@@ -26521,15 +26548,17 @@
             "resources": [
                 "connections"
             ]
         },
         "GetIdentityCenterApplication": {
             "access_level": "Read",
             "action": "GetIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to get information about an IAM Identity Center application",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "GetPendingConnection": {
@@ -26575,15 +26604,17 @@
             "description": "Grants permission to view a list of IAM Identity Center applications by Amazon CodeCatalyst space",
             "orphan": false,
             "resources": []
         },
         "ListSpacesForIdentityCenterApplication": {
             "access_level": "List",
             "action": "ListSpacesForIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to view a list of Amazon CodeCatalyst spaces by IAM Identity Center application",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "ListTagsForResource": {
@@ -26591,15 +26622,16 @@
             "action": "ListTagsForResource",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to list tags for an Amazon CodeCatalyst resource",
             "orphan": false,
             "resources": [
-                "connections"
+                "connections",
+                "identity-center-applications"
             ]
         },
         "PutBillingAuthorization": {
             "access_level": "Write",
             "action": "PutBillingAuthorization",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
@@ -26617,15 +26649,17 @@
             "description": "Grants permission to reject a request to connect this account to an Amazon CodeCatalyst space",
             "orphan": false,
             "resources": []
         },
         "SynchronizeIdentityCenterApplication": {
             "access_level": "Write",
             "action": "SynchronizeIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to synchronize an IAM Identity Center application with the backing identity store",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         },
         "TagResource": {
@@ -26635,34 +26669,38 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to tag an Amazon CodeCatalyst resource",
             "orphan": false,
             "resources": [
-                "connections"
+                "connections",
+                "identity-center-applications"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to untag an Amazon CodeCatalyst resource",
             "orphan": false,
             "resources": [
-                "connections"
+                "connections",
+                "identity-center-applications"
             ]
         },
         "UpdateIdentityCenterApplication": {
             "access_level": "Write",
             "action": "UpdateIdentityCenterApplication",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to update an IAM Identity Center application",
             "orphan": false,
             "resources": [
                 "identity-center-applications"
             ]
         }
     },
@@ -40242,14 +40280,22 @@
             "access_level": "Undocumented",
             "action": "DeleteSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "DeleteTimeSeriesDataPoints": {
+            "access_level": "Undocumented",
+            "action": "DeleteTimeSeriesDataPoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetAsset": {
             "access_level": "Undocumented",
             "action": "GetAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -40442,14 +40488,22 @@
             "access_level": "Undocumented",
             "action": "GetSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetTimeSeriesDataPoint": {
+            "access_level": "Undocumented",
+            "action": "GetTimeSeriesDataPoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetUserProfile": {
             "access_level": "Undocumented",
             "action": "GetUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -40618,22 +40672,38 @@
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListTimeSeriesDataPoints": {
+            "access_level": "Undocumented",
+            "action": "ListTimeSeriesDataPoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListWarehouseMetadata": {
             "access_level": "Undocumented",
             "action": "ListWarehouseMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "PostTimeSeriesDataPoints": {
+            "access_level": "Undocumented",
+            "action": "PostTimeSeriesDataPoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ProvisionDomain": {
             "access_level": "Undocumented",
             "action": "ProvisionDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -41301,14 +41371,840 @@
             "action": "UpdateTab",
             "condition_keys": [],
             "description": "Grants permission to update query tab",
             "orphan": false,
             "resources": []
         }
     },
+    "deadline": {
+        "AssociateMemberToFarm": {
+            "access_level": "Undocumented",
+            "action": "AssociateMemberToFarm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssociateMemberToFleet": {
+            "access_level": "Undocumented",
+            "action": "AssociateMemberToFleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssociateMemberToJob": {
+            "access_level": "Undocumented",
+            "action": "AssociateMemberToJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssociateMemberToQueue": {
+            "access_level": "Undocumented",
+            "action": "AssociateMemberToQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssumeFleetRoleForRead": {
+            "access_level": "Undocumented",
+            "action": "AssumeFleetRoleForRead",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssumeFleetRoleForWorker": {
+            "access_level": "Undocumented",
+            "action": "AssumeFleetRoleForWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssumeQueueRoleForRead": {
+            "access_level": "Undocumented",
+            "action": "AssumeQueueRoleForRead",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssumeQueueRoleForUser": {
+            "access_level": "Undocumented",
+            "action": "AssumeQueueRoleForUser",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssumeQueueRoleForWorker": {
+            "access_level": "Undocumented",
+            "action": "AssumeQueueRoleForWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "BatchGetJobEntity": {
+            "access_level": "Undocumented",
+            "action": "BatchGetJobEntity",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CopyJobTemplate": {
+            "access_level": "Undocumented",
+            "action": "CopyJobTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateBudget": {
+            "access_level": "Undocumented",
+            "action": "CreateBudget",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateFarm": {
+            "access_level": "Undocumented",
+            "action": "CreateFarm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateFleet": {
+            "access_level": "Undocumented",
+            "action": "CreateFleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateJob": {
+            "access_level": "Undocumented",
+            "action": "CreateJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateLicenseEndpoint": {
+            "access_level": "Undocumented",
+            "action": "CreateLicenseEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateMonitor": {
+            "access_level": "Undocumented",
+            "action": "CreateMonitor",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateQueue": {
+            "access_level": "Undocumented",
+            "action": "CreateQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateQueueEnvironment": {
+            "access_level": "Undocumented",
+            "action": "CreateQueueEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateQueueFleetAssociation": {
+            "access_level": "Undocumented",
+            "action": "CreateQueueFleetAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateStorageProfile": {
+            "access_level": "Undocumented",
+            "action": "CreateStorageProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateWorker": {
+            "access_level": "Undocumented",
+            "action": "CreateWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteBudget": {
+            "access_level": "Undocumented",
+            "action": "DeleteBudget",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteFarm": {
+            "access_level": "Undocumented",
+            "action": "DeleteFarm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteFleet": {
+            "access_level": "Undocumented",
+            "action": "DeleteFleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteLicenseEndpoint": {
+            "access_level": "Undocumented",
+            "action": "DeleteLicenseEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteMeteredProduct": {
+            "access_level": "Undocumented",
+            "action": "DeleteMeteredProduct",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteMonitor": {
+            "access_level": "Undocumented",
+            "action": "DeleteMonitor",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteQueue": {
+            "access_level": "Undocumented",
+            "action": "DeleteQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteQueueEnvironment": {
+            "access_level": "Undocumented",
+            "action": "DeleteQueueEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteQueueFleetAssociation": {
+            "access_level": "Undocumented",
+            "action": "DeleteQueueFleetAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteStorageProfile": {
+            "access_level": "Undocumented",
+            "action": "DeleteStorageProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteWorker": {
+            "access_level": "Undocumented",
+            "action": "DeleteWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateMemberFromFarm": {
+            "access_level": "Undocumented",
+            "action": "DisassociateMemberFromFarm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateMemberFromFleet": {
+            "access_level": "Undocumented",
+            "action": "DisassociateMemberFromFleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateMemberFromJob": {
+            "access_level": "Undocumented",
+            "action": "DisassociateMemberFromJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateMemberFromQueue": {
+            "access_level": "Undocumented",
+            "action": "DisassociateMemberFromQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetApplicationVersion": {
+            "access_level": "Undocumented",
+            "action": "GetApplicationVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetBudget": {
+            "access_level": "Undocumented",
+            "action": "GetBudget",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetFarm": {
+            "access_level": "Undocumented",
+            "action": "GetFarm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetFleet": {
+            "access_level": "Undocumented",
+            "action": "GetFleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetJob": {
+            "access_level": "Undocumented",
+            "action": "GetJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetLicenseEndpoint": {
+            "access_level": "Undocumented",
+            "action": "GetLicenseEndpoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetMonitor": {
+            "access_level": "Undocumented",
+            "action": "GetMonitor",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetQueue": {
+            "access_level": "Undocumented",
+            "action": "GetQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetQueueEnvironment": {
+            "access_level": "Undocumented",
+            "action": "GetQueueEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetQueueFleetAssociation": {
+            "access_level": "Undocumented",
+            "action": "GetQueueFleetAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSession": {
+            "access_level": "Undocumented",
+            "action": "GetSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSessionAction": {
+            "access_level": "Undocumented",
+            "action": "GetSessionAction",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSessionsStatisticsAggregation": {
+            "access_level": "Undocumented",
+            "action": "GetSessionsStatisticsAggregation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStep": {
+            "access_level": "Undocumented",
+            "action": "GetStep",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStorageProfile": {
+            "access_level": "Undocumented",
+            "action": "GetStorageProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetStorageProfileForQueue": {
+            "access_level": "Undocumented",
+            "action": "GetStorageProfileForQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetTask": {
+            "access_level": "Undocumented",
+            "action": "GetTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetWorker": {
+            "access_level": "Undocumented",
+            "action": "GetWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListAvailableMeteredProducts": {
+            "access_level": "Undocumented",
+            "action": "ListAvailableMeteredProducts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListBudgets": {
+            "access_level": "Undocumented",
+            "action": "ListBudgets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListFarmMembers": {
+            "access_level": "Undocumented",
+            "action": "ListFarmMembers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListFarms": {
+            "access_level": "Undocumented",
+            "action": "ListFarms",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListFleetMembers": {
+            "access_level": "Undocumented",
+            "action": "ListFleetMembers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListFleets": {
+            "access_level": "Undocumented",
+            "action": "ListFleets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListJobMembers": {
+            "access_level": "Undocumented",
+            "action": "ListJobMembers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListJobs": {
+            "access_level": "Undocumented",
+            "action": "ListJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListLicenseEndpoints": {
+            "access_level": "Undocumented",
+            "action": "ListLicenseEndpoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListMeteredProducts": {
+            "access_level": "Undocumented",
+            "action": "ListMeteredProducts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListMonitors": {
+            "access_level": "Undocumented",
+            "action": "ListMonitors",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListQueueEnvironments": {
+            "access_level": "Undocumented",
+            "action": "ListQueueEnvironments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListQueueFleetAssociations": {
+            "access_level": "Undocumented",
+            "action": "ListQueueFleetAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListQueueMembers": {
+            "access_level": "Undocumented",
+            "action": "ListQueueMembers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListQueues": {
+            "access_level": "Undocumented",
+            "action": "ListQueues",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSessionActions": {
+            "access_level": "Undocumented",
+            "action": "ListSessionActions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSessions": {
+            "access_level": "Undocumented",
+            "action": "ListSessions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSessionsForWorker": {
+            "access_level": "Undocumented",
+            "action": "ListSessionsForWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListStepConsumers": {
+            "access_level": "Undocumented",
+            "action": "ListStepConsumers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListStepDependencies": {
+            "access_level": "Undocumented",
+            "action": "ListStepDependencies",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListSteps": {
+            "access_level": "Undocumented",
+            "action": "ListSteps",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListStorageProfiles": {
+            "access_level": "Undocumented",
+            "action": "ListStorageProfiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListStorageProfilesForQueue": {
+            "access_level": "Undocumented",
+            "action": "ListStorageProfilesForQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTasks": {
+            "access_level": "Undocumented",
+            "action": "ListTasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListWorkers": {
+            "access_level": "Undocumented",
+            "action": "ListWorkers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "PutMeteredProduct": {
+            "access_level": "Undocumented",
+            "action": "PutMeteredProduct",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchJobs": {
+            "access_level": "Undocumented",
+            "action": "SearchJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchSteps": {
+            "access_level": "Undocumented",
+            "action": "SearchSteps",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchTasks": {
+            "access_level": "Undocumented",
+            "action": "SearchTasks",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchWorkers": {
+            "access_level": "Undocumented",
+            "action": "SearchWorkers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartSessionsStatisticsAggregation": {
+            "access_level": "Undocumented",
+            "action": "StartSessionsStatisticsAggregation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateBudget": {
+            "access_level": "Undocumented",
+            "action": "UpdateBudget",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateFarm": {
+            "access_level": "Undocumented",
+            "action": "UpdateFarm",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateFleet": {
+            "access_level": "Undocumented",
+            "action": "UpdateFleet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateJob": {
+            "access_level": "Undocumented",
+            "action": "UpdateJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateMonitor": {
+            "access_level": "Undocumented",
+            "action": "UpdateMonitor",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateQueue": {
+            "access_level": "Undocumented",
+            "action": "UpdateQueue",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateQueueEnvironment": {
+            "access_level": "Undocumented",
+            "action": "UpdateQueueEnvironment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateQueueFleetAssociation": {
+            "access_level": "Undocumented",
+            "action": "UpdateQueueFleetAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateSession": {
+            "access_level": "Undocumented",
+            "action": "UpdateSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateStep": {
+            "access_level": "Undocumented",
+            "action": "UpdateStep",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateStorageProfile": {
+            "access_level": "Undocumented",
+            "action": "UpdateStorageProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateTask": {
+            "access_level": "Undocumented",
+            "action": "UpdateTask",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateWorker": {
+            "access_level": "Undocumented",
+            "action": "UpdateWorker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateWorkerSchedule": {
+            "access_level": "Undocumented",
+            "action": "UpdateWorkerSchedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "deepcomposer": {
         "AssociateCoupon": {
             "access_level": "Write",
             "action": "AssociateCoupon",
             "condition_keys": [],
             "description": "Grants permission to associate a DeepComposer coupon (or DSN) with the account associated with the sender of the request",
             "orphan": false,
@@ -167716,24 +168612,14 @@
             "condition_keys": [],
             "description": "Grants permission to create a mail domain",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "CreateMailUser": {
-            "access_level": "Write",
-            "action": "CreateMailUser",
-            "condition_keys": [],
-            "description": "Grants permission to create a user in the directory",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "CreateMobileDeviceAccessRule": {
             "access_level": "Write",
             "action": "CreateMobileDeviceAccessRule",
             "condition_keys": [],
             "description": "Grants permission to create a new mobile device access rule",
             "orphan": false,
             "resources": [
@@ -168148,34 +169034,14 @@
             "condition_keys": [],
             "description": "Grants permission to read details for a user",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "DisableMailGroups": {
-            "access_level": "Write",
-            "action": "DisableMailGroups",
-            "condition_keys": [],
-            "description": "Grants permission to disable a mail group when it is not being used, in order to allow it to be deleted",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
-        "DisableMailUsers": {
-            "access_level": "Write",
-            "action": "DisableMailUsers",
-            "condition_keys": [],
-            "description": "Grants permission to disable a user mailbox when it is no longer being used, in order to allow it to be deleted",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "DisassociateDelegateFromResource": {
             "access_level": "Write",
             "action": "DisassociateDelegateFromResource",
             "condition_keys": [],
             "description": "Grants permission to remove a member from the resource's set of delegates",
             "orphan": false,
             "resources": [
@@ -168198,34 +169064,14 @@
             "condition_keys": [],
             "description": "Grants permission to enable a mail domain in the organization",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "EnableMailGroups": {
-            "access_level": "Write",
-            "action": "EnableMailGroups",
-            "condition_keys": [],
-            "description": "Grants permission to enable a mail group after it has been created to allow it to receive mail",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
-        "EnableMailUsers": {
-            "access_level": "Write",
-            "action": "EnableMailUsers",
-            "condition_keys": [],
-            "description": "Grants permission to enable a user's mailbox after it has been created to allow it to receive mail",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "GetAccessControlEffect": {
             "access_level": "Read",
             "action": "GetAccessControlEffect",
             "condition_keys": [],
             "description": "Grants permission to get the effects of access control rules as they apply to a specified IPv4 address, access protocol action, or user ID",
             "orphan": false,
             "resources": [
@@ -168298,24 +169144,14 @@
             "condition_keys": [],
             "description": "Grants permission to get the details of the mail group",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "GetMailUserDetails": {
-            "access_level": "Read",
-            "action": "GetMailUserDetails",
-            "condition_keys": [],
-            "description": "Grants permission to get the details of the user's mailbox and account",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "GetMailboxDetails": {
             "access_level": "Read",
             "action": "GetMailboxDetails",
             "condition_keys": [],
             "description": "Grants permission to read the details of the user's mailbox",
             "orphan": false,
             "resources": [
@@ -168729,34 +169565,14 @@
             "condition_keys": [],
             "description": "Grants permission to set journaling and fallback email addresses for email journaling",
             "orphan": false,
             "resources": [
                 "organization"
             ]
         },
-        "SetMailGroupDetails": {
-            "access_level": "Write",
-            "action": "SetMailGroupDetails",
-            "condition_keys": [],
-            "description": "Grants permission to set the details of the mail group which has just been created",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
-        "SetMailUserDetails": {
-            "access_level": "Write",
-            "action": "SetMailUserDetails",
-            "condition_keys": [],
-            "description": "Grants permission to set the details for the user account which has just been created",
-            "orphan": false,
-            "resources": [
-                "organization"
-            ]
-        },
         "SetMobilePolicyDetails": {
             "access_level": "Write",
             "action": "SetMobilePolicyDetails",
             "condition_keys": [],
             "description": "Grants permission to set the details of a mobile policy associated with the organization",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20240401/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240402/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240402/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/generate/generate.py` & `iam_actions-1.2.20240402/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240402/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240402/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/generate/services.py` & `iam_actions-1.2.20240402/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240401/iam_actions/policies.json` & `iam_actions-1.2.20240402/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997538593908079%*

 * *Differences: {"'serviceMap'": "{'Amazon DataZone': {'Actions': {insert: [(41, 'DeleteTimeSeriesDataPoints'), "*

 * *                 "(67, 'GetTimeSeriesDataPoint'), (90, 'ListTimeSeriesDataPoints'), (92, "*

 * *                 "'PostTimeSeriesDataPoints')]}}, 'AWS CloudFormation': {'Actions': {insert: [(57, "*

 * *                 "'ListStackSetAutoDeploymentTargets')]}}, 'AWS Deadline Cloud': "*

 * *                 "OrderedDict([('StringPrefix', 'deadline'), ('Actions', ['AssociateMemberToFarm', "*

 * *                 "'AssociateMemberToFl […]*

```diff
@@ -1775,14 +1775,15 @@
                 "ListImports",
                 "ListResourceScanRelatedResources",
                 "ListResourceScanResources",
                 "ListResourceScans",
                 "ListStackInstanceResourceDrifts",
                 "ListStackInstances",
                 "ListStackResources",
+                "ListStackSetAutoDeploymentTargets",
                 "ListStackSetOperationResults",
                 "ListStackSetOperations",
                 "ListStackSets",
                 "ListStacks",
                 "ListTypeRegistrations",
                 "ListTypeVersions",
                 "ListTypes",
@@ -3213,14 +3214,138 @@
                 "dms:rep-tag/${TagKey}",
                 "dms:replication-config-tag/${TagKey}",
                 "dms:req-tag/${TagKey}",
                 "dms:subgrp-tag/${TagKey}",
                 "dms:task-tag/${TagKey}"
             ]
         },
+        "AWS Deadline Cloud": {
+            "ARNFormat": "arn:aws:deadline:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:deadline:.+:.+:.+",
+            "Actions": [
+                "AssociateMemberToFarm",
+                "AssociateMemberToFleet",
+                "AssociateMemberToJob",
+                "AssociateMemberToQueue",
+                "AssumeFleetRoleForRead",
+                "AssumeFleetRoleForWorker",
+                "AssumeQueueRoleForRead",
+                "AssumeQueueRoleForUser",
+                "AssumeQueueRoleForWorker",
+                "BatchGetJobEntity",
+                "CopyJobTemplate",
+                "CreateBudget",
+                "CreateFarm",
+                "CreateFleet",
+                "CreateJob",
+                "CreateLicenseEndpoint",
+                "CreateMonitor",
+                "CreateQueue",
+                "CreateQueueEnvironment",
+                "CreateQueueFleetAssociation",
+                "CreateStorageProfile",
+                "CreateWorker",
+                "DeleteBudget",
+                "DeleteFarm",
+                "DeleteFleet",
+                "DeleteLicenseEndpoint",
+                "DeleteMeteredProduct",
+                "DeleteMonitor",
+                "DeleteQueue",
+                "DeleteQueueEnvironment",
+                "DeleteQueueFleetAssociation",
+                "DeleteStorageProfile",
+                "DeleteWorker",
+                "DisassociateMemberFromFarm",
+                "DisassociateMemberFromFleet",
+                "DisassociateMemberFromJob",
+                "DisassociateMemberFromQueue",
+                "GetApplicationVersion",
+                "GetBudget",
+                "GetFarm",
+                "GetFleet",
+                "GetJob",
+                "GetLicenseEndpoint",
+                "GetMonitor",
+                "GetQueue",
+                "GetQueueEnvironment",
+                "GetQueueFleetAssociation",
+                "GetSession",
+                "GetSessionAction",
+                "GetSessionsStatisticsAggregation",
+                "GetStep",
+                "GetStorageProfile",
+                "GetStorageProfileForQueue",
+                "GetTask",
+                "GetWorker",
+                "ListAvailableMeteredProducts",
+                "ListBudgets",
+                "ListFarmMembers",
+                "ListFarms",
+                "ListFleetMembers",
+                "ListFleets",
+                "ListJobMembers",
+                "ListJobs",
+                "ListLicenseEndpoints",
+                "ListMeteredProducts",
+                "ListMonitors",
+                "ListQueueEnvironments",
+                "ListQueueFleetAssociations",
+                "ListQueueMembers",
+                "ListQueues",
+                "ListSessionActions",
+                "ListSessions",
+                "ListSessionsForWorker",
+                "ListStepConsumers",
+                "ListStepDependencies",
+                "ListSteps",
+                "ListStorageProfiles",
+                "ListStorageProfilesForQueue",
+                "ListTagsForResource",
+                "ListTasks",
+                "ListWorkers",
+                "PutMeteredProduct",
+                "SearchJobs",
+                "SearchSteps",
+                "SearchTasks",
+                "SearchWorkers",
+                "StartSessionsStatisticsAggregation",
+                "TagResource",
+                "UntagResource",
+                "UpdateBudget",
+                "UpdateFarm",
+                "UpdateFleet",
+                "UpdateJob",
+                "UpdateMonitor",
+                "UpdateQueue",
+                "UpdateQueueEnvironment",
+                "UpdateQueueFleetAssociation",
+                "UpdateSession",
+                "UpdateStep",
+                "UpdateStorageProfile",
+                "UpdateTask",
+                "UpdateWorker",
+                "UpdateWorkerSchedule"
+            ],
+            "HasResource": true,
+            "StringPrefix": "deadline",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "deadline:AssociatedMembershipLevel",
+                "deadline:FarmMembershipLevels",
+                "deadline:FleetMembershipLevels",
+                "deadline:JobMembershipLevels",
+                "deadline:MembershipLevel",
+                "deadline:PrincipalId",
+                "deadline:QueueMembershipLevels",
+                "deadline:RequesterPrincipalId"
+            ]
+        },
         "AWS DeepComposer": {
             "ARNFormat": "arn:aws:deepcomposer:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:deepcomposer:.+:.+:.+",
             "Actions": [
                 "AssociateCoupon",
                 "CreateAudio",
                 "CreateComposition",
@@ -13288,14 +13413,15 @@
                 "DeleteGlossaryTerm",
                 "DeleteListing",
                 "DeleteProject",
                 "DeleteProjectMembership",
                 "DeleteSubscriptionGrant",
                 "DeleteSubscriptionRequest",
                 "DeleteSubscriptionTarget",
+                "DeleteTimeSeriesDataPoints",
                 "GetAsset",
                 "GetAssetType",
                 "GetDataSource",
                 "GetDataSourceRun",
                 "GetDomain",
                 "GetDomainSharingPolicy",
                 "GetEnvironment",
@@ -13313,14 +13439,15 @@
                 "GetMetadataGenerationRun",
                 "GetProject",
                 "GetSubscription",
                 "GetSubscriptionEligibility",
                 "GetSubscriptionGrant",
                 "GetSubscriptionRequestDetails",
                 "GetSubscriptionTarget",
+                "GetTimeSeriesDataPoint",
                 "GetUserProfile",
                 "ListAccountEnvironments",
                 "ListAssetRevisions",
                 "ListDataSourceRunActivities",
                 "ListDataSourceRuns",
                 "ListDataSources",
                 "ListDomains",
@@ -13335,15 +13462,17 @@
                 "ListProjectMemberships",
                 "ListProjects",
                 "ListSubscriptionGrants",
                 "ListSubscriptionRequests",
                 "ListSubscriptionTargets",
                 "ListSubscriptions",
                 "ListTagsForResource",
+                "ListTimeSeriesDataPoints",
                 "ListWarehouseMetadata",
+                "PostTimeSeriesDataPoints",
                 "ProvisionDomain",
                 "PutDomainSharingPolicy",
                 "PutEnvironmentBlueprintConfiguration",
                 "RefreshToken",
                 "RejectPredictions",
                 "RejectSubscriptionRequest",
                 "RevokeSubscription",
```

### Comparing `iam_actions-1.2.20240401/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240402/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997348971722365%*

 * *Differences: {"'artifact'": "{'report': {'arn_pattern': 'arn:*:artifact:*::report/*:*'}}",*

 * * "'codecatalyst'": "{'identity-center-applications': {'condition_keys': "*

 * *                   "'aws:ResourceTag/${TagKey}'}}",*

 * * "'deadline'": 'OrderedDict()'}*

```diff
@@ -696,15 +696,15 @@
             "condition_keys": null
         },
         "customer-agreement": {
             "arn_pattern": "arn:*:artifact::*:customer-agreement/*",
             "condition_keys": null
         },
         "report": {
-            "arn_pattern": "arn:*:artifact:*::report/*",
+            "arn_pattern": "arn:*:artifact:*::report/*:*",
             "condition_keys": null
         },
         "report-package": {
             "arn_pattern": "arn:*:artifact:::report-package/*",
             "condition_keys": null
         }
     },
@@ -1218,15 +1218,15 @@
     "codecatalyst": {
         "connections": {
             "arn_pattern": "arn:*:codecatalyst:*:*:/connections/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "identity-center-applications": {
             "arn_pattern": "arn:*:codecatalyst:*:*:/identity-center-applications/*",
-            "condition_keys": null
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "project": {
             "arn_pattern": "arn:*:codecatalyst:::space/*/project/*",
             "condition_keys": null
         },
         "space": {
             "arn_pattern": "arn:*:codecatalyst:::space/*",
@@ -1735,14 +1735,15 @@
     "dax": {
         "application": {
             "arn_pattern": "arn:*:dax:*:*:cache/*",
             "condition_keys": null
         }
     },
     "dbqms": {},
+    "deadline": {},
     "deepcomposer": {
         "audio": {
             "arn_pattern": "arn:*:deepcomposer:*:*:audio/*",
             "condition_keys": null
         },
         "composition": {
             "arn_pattern": "arn:*:deepcomposer:*:*:composition/*",
```

### Comparing `iam_actions-1.2.20240401/iam_actions/services.json` & `iam_actions-1.2.20240402/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974248069100073%*

 * *Differences: {"'cloudformation'": "{'Actions': {insert: [(64, 'ListStackSetAutoDeploymentTargets')]}}",*

 * * "'datazone'": "{'Actions': {insert: [(41, 'DeleteTimeSeriesDataPoints'), (67, "*

 * *               "'GetTimeSeriesDataPoint'), (90, 'ListTimeSeriesDataPoints'), (92, "*

 * *               "'PostTimeSeriesDataPoints')]}}",*

 * * "'deadline'": "OrderedDict([('Actions', ['AssociateMemberToFarm', 'AssociateMemberToFleet', "*

 * *               "'AssociateMemberToJob', 'AssociateMemberToQueue', 'AssumeFleetRoleForRead', "*

 * *               "'A […]*

```diff
@@ -3372,14 +3372,15 @@
             "ListResourceScanRelatedResources",
             "ListResourceScanResources",
             "ListResourceScans",
             "ListResources",
             "ListStackInstanceResourceDrifts",
             "ListStackInstances",
             "ListStackResources",
+            "ListStackSetAutoDeploymentTargets",
             "ListStackSetOperationResults",
             "ListStackSetOperations",
             "ListStackSets",
             "ListStacks",
             "ListTypeRegistrations",
             "ListTypeVersions",
             "ListTypes",
@@ -5972,14 +5973,15 @@
             "DeleteGlossaryTerm",
             "DeleteListing",
             "DeleteProject",
             "DeleteProjectMembership",
             "DeleteSubscriptionGrant",
             "DeleteSubscriptionRequest",
             "DeleteSubscriptionTarget",
+            "DeleteTimeSeriesDataPoints",
             "GetAsset",
             "GetAssetType",
             "GetDataSource",
             "GetDataSourceRun",
             "GetDomain",
             "GetDomainSharingPolicy",
             "GetEnvironment",
@@ -5997,14 +5999,15 @@
             "GetMetadataGenerationRun",
             "GetProject",
             "GetSubscription",
             "GetSubscriptionEligibility",
             "GetSubscriptionGrant",
             "GetSubscriptionRequestDetails",
             "GetSubscriptionTarget",
+            "GetTimeSeriesDataPoint",
             "GetUserProfile",
             "ListAccountEnvironments",
             "ListAssetRevisions",
             "ListDataSourceRunActivities",
             "ListDataSourceRuns",
             "ListDataSources",
             "ListDomains",
@@ -6019,15 +6022,17 @@
             "ListProjectMemberships",
             "ListProjects",
             "ListSubscriptionGrants",
             "ListSubscriptionRequests",
             "ListSubscriptionTargets",
             "ListSubscriptions",
             "ListTagsForResource",
+            "ListTimeSeriesDataPoints",
             "ListWarehouseMetadata",
+            "PostTimeSeriesDataPoints",
             "ProvisionDomain",
             "PutDomainSharingPolicy",
             "PutEnvironmentBlueprintConfiguration",
             "RefreshToken",
             "RejectPredictions",
             "RejectSubscriptionRequest",
             "RevokeSubscription",
@@ -6141,14 +6146,144 @@
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "Database Query Metadata Service"
         ]
     },
+    "deadline": {
+        "ARNFormats": [
+            "arn:aws:deadline:${Region}:${Account}:${ResourceType}/${ResourcePath}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:deadline:.+:.+:.+"
+        ],
+        "Actions": [
+            "AssociateMemberToFarm",
+            "AssociateMemberToFleet",
+            "AssociateMemberToJob",
+            "AssociateMemberToQueue",
+            "AssumeFleetRoleForRead",
+            "AssumeFleetRoleForWorker",
+            "AssumeQueueRoleForRead",
+            "AssumeQueueRoleForUser",
+            "AssumeQueueRoleForWorker",
+            "BatchGetJobEntity",
+            "CopyJobTemplate",
+            "CreateBudget",
+            "CreateFarm",
+            "CreateFleet",
+            "CreateJob",
+            "CreateLicenseEndpoint",
+            "CreateMonitor",
+            "CreateQueue",
+            "CreateQueueEnvironment",
+            "CreateQueueFleetAssociation",
+            "CreateStorageProfile",
+            "CreateWorker",
+            "DeleteBudget",
+            "DeleteFarm",
+            "DeleteFleet",
+            "DeleteLicenseEndpoint",
+            "DeleteMeteredProduct",
+            "DeleteMonitor",
+            "DeleteQueue",
+            "DeleteQueueEnvironment",
+            "DeleteQueueFleetAssociation",
+            "DeleteStorageProfile",
+            "DeleteWorker",
+            "DisassociateMemberFromFarm",
+            "DisassociateMemberFromFleet",
+            "DisassociateMemberFromJob",
+            "DisassociateMemberFromQueue",
+            "GetApplicationVersion",
+            "GetBudget",
+            "GetFarm",
+            "GetFleet",
+            "GetJob",
+            "GetLicenseEndpoint",
+            "GetMonitor",
+            "GetQueue",
+            "GetQueueEnvironment",
+            "GetQueueFleetAssociation",
+            "GetSession",
+            "GetSessionAction",
+            "GetSessionsStatisticsAggregation",
+            "GetStep",
+            "GetStorageProfile",
+            "GetStorageProfileForQueue",
+            "GetTask",
+            "GetWorker",
+            "ListAvailableMeteredProducts",
+            "ListBudgets",
+            "ListFarmMembers",
+            "ListFarms",
+            "ListFleetMembers",
+            "ListFleets",
+            "ListJobMembers",
+            "ListJobs",
+            "ListLicenseEndpoints",
+            "ListMeteredProducts",
+            "ListMonitors",
+            "ListQueueEnvironments",
+            "ListQueueFleetAssociations",
+            "ListQueueMembers",
+            "ListQueues",
+            "ListSessionActions",
+            "ListSessions",
+            "ListSessionsForWorker",
+            "ListStepConsumers",
+            "ListStepDependencies",
+            "ListSteps",
+            "ListStorageProfiles",
+            "ListStorageProfilesForQueue",
+            "ListTagsForResource",
+            "ListTasks",
+            "ListWorkers",
+            "PutMeteredProduct",
+            "SearchJobs",
+            "SearchSteps",
+            "SearchTasks",
+            "SearchWorkers",
+            "StartSessionsStatisticsAggregation",
+            "TagResource",
+            "UntagResource",
+            "UpdateBudget",
+            "UpdateFarm",
+            "UpdateFleet",
+            "UpdateJob",
+            "UpdateMonitor",
+            "UpdateQueue",
+            "UpdateQueueEnvironment",
+            "UpdateQueueFleetAssociation",
+            "UpdateSession",
+            "UpdateStep",
+            "UpdateStorageProfile",
+            "UpdateTask",
+            "UpdateWorker",
+            "UpdateWorkerSchedule"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys",
+            "deadline:AssociatedMembershipLevel",
+            "deadline:FarmMembershipLevels",
+            "deadline:FleetMembershipLevels",
+            "deadline:JobMembershipLevels",
+            "deadline:MembershipLevel",
+            "deadline:PrincipalId",
+            "deadline:QueueMembershipLevels",
+            "deadline:RequesterPrincipalId"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "AWS Deadline Cloud"
+        ]
+    },
     "deepcomposer": {
         "ARNFormats": [
             "arn:aws:deepcomposer:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:deepcomposer:.+:.+:.+"
         ],
```

### Comparing `iam_actions-1.2.20240401/pyproject.toml` & `iam_actions-1.2.20240402/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240401"
+version = "1.2.20240402"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240401/setup.py` & `iam_actions-1.2.20240402/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240401',
+    'version': '1.2.20240402',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240401/PKG-INFO` & `iam_actions-1.2.20240402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240401
+Version: 1.2.20240402
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

