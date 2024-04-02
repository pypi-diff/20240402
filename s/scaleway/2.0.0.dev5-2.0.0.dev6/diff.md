# Comparing `tmp/scaleway-2.0.0.dev5.tar.gz` & `tmp/scaleway-2.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway-2.0.0.dev5.tar", max compression
+gzip compressed data, was "scaleway-2.0.0.dev6.tar", max compression
```

## Comparing `scaleway-2.0.0.dev5.tar` & `scaleway-2.0.0.dev6.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0        0        0       76 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/README.md
--rw-r--r--   0        0        0     1132 2023-11-27 13:24:59.339475 scaleway-2.0.0.dev5/pyproject.toml
--rw-r--r--   0        0        0      905 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/__init__.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/__init__.py
--rw-r--r--   0        0        0      714 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v2/__init__.py
--rw-r--r--   0        0        0     8456 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v2/api.py
--rw-r--r--   0        0        0     2514 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v2/marshalling.py
--rw-r--r--   0        0        0     2638 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v2/types.py
--rw-r--r--   0        0        0      828 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v3/__init__.py
--rw-r--r--   0        0        0     8180 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v3/api.py
--rw-r--r--   0        0        0     2574 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v3/marshalling.py
--rw-r--r--   0        0        0     2678 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/account/v3/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/applesilicon/__init__.py
--rw-r--r--   0        0        0     1674 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18185 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/api.py
--rw-r--r--   0        0        0      496 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/content.py
--rw-r--r--   0        0        0     6476 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7171 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/baremetal/__init__.py
--rw-r--r--   0        0        0     5332 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/baremetal/v1/__init__.py
--rw-r--r--   0        0        0    52790 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/baremetal/v1/api.py
--rw-r--r--   0        0        0     1060 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/baremetal/v1/content.py
--rw-r--r--   0        0        0    26268 2023-11-27 13:24:43.891617 scaleway-2.0.0.dev5/scaleway/baremetal/v1/marshalling.py
--rw-r--r--   0        0        0    27983 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/baremetal/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/billing/__init__.py
--rw-r--r--   0        0        0     1414 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/__init__.py
--rw-r--r--   0        0        0     9098 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/api.py
--rw-r--r--   0        0        0     6100 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/marshalling.py
--rw-r--r--   0        0        0     7103 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/block/__init__.py
--rw-r--r--   0        0        0     2456 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/block/v1alpha1/__init__.py
--rw-r--r--   0        0        0    26281 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/block/v1alpha1/api.py
--rw-r--r--   0        0        0      926 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/block/v1alpha1/content.py
--rw-r--r--   0        0        0    12137 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/block/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    13735 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/block/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/cockpit/__init__.py
--rw-r--r--   0        0        0     3684 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/__init__.py
--rw-r--r--   0        0        0    34543 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/api.py
--rw-r--r--   0        0        0      418 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/content.py
--rw-r--r--   0        0        0    19017 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/marshalling.py
--rw-r--r--   0        0        0    15156 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/container/__init__.py
--rw-r--r--   0        0        0     5370 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/container/v1beta1/__init__.py
--rw-r--r--   0        0        0    65173 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/container/v1beta1/api.py
--rw-r--r--   0        0        0     1581 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/container/v1beta1/content.py
--rw-r--r--   0        0        0    25088 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/container/v1beta1/marshalling.py
--rw-r--r--   0        0        0    28544 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/container/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/document_db/__init__.py
--rw-r--r--   0        0        0     9020 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/__init__.py
--rw-r--r--   0        0        0   100490 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/api.py
--rw-r--r--   0        0        0     1612 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/content.py
--rw-r--r--   0        0        0    43777 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/marshalling.py
--rw-r--r--   0        0        0    41184 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/domain/__init__.py
--rw-r--r--   0        0        0    13030 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/domain/v2beta1/__init__.py
--rw-r--r--   0        0        0    87761 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/domain/v2beta1/api.py
--rw-r--r--   0        0        0     1942 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/domain/v2beta1/content.py
--rw-r--r--   0        0        0    78660 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/domain/v2beta1/marshalling.py
--rw-r--r--   0        0        0    34374 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/domain/v2beta1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/flexibleip/__init__.py
--rw-r--r--   0        0        0     1762 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20505 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/api.py
--rw-r--r--   0        0        0      647 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/content.py
--rw-r--r--   0        0        0     7007 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8804 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/function/__init__.py
--rw-r--r--   0        0        0     5864 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/function/v1beta1/__init__.py
--rw-r--r--   0        0        0    67235 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/function/v1beta1/api.py
--rw-r--r--   0        0        0     1573 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/function/v1beta1/content.py
--rw-r--r--   0        0        0    26889 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/function/v1beta1/marshalling.py
--rw-r--r--   0        0        0    30250 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/function/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/iam/__init__.py
--rw-r--r--   0        0        0     5416 2023-11-27 13:24:43.895617 scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/__init__.py
--rw-r--r--   0        0        0    79405 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/api.py
--rw-r--r--   0        0        0    26720 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    29209 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/__init__.py
--rw-r--r--   0        0        0    13232 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/__init__.py
--rw-r--r--   0        0        0   139528 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/api.py
--rw-r--r--   0        0        0     2660 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/api_utils.py
--rw-r--r--   0        0        0     2384 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/content.py
--rw-r--r--   0        0        0    96533 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/marshalling.py
--rw-r--r--   0        0        0      712 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/marshalling_utils.py
--rw-r--r--   0        0        0    66625 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/types.py
--rw-r--r--   0        0        0    11110 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/instance/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iot/__init__.py
--rw-r--r--   0        0        0     5818 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iot/v1/__init__.py
--rw-r--r--   0        0        0    61461 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iot/v1/api.py
--rw-r--r--   0        0        0      363 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iot/v1/content.py
--rw-r--r--   0        0        0    29667 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iot/v1/marshalling.py
--rw-r--r--   0        0        0    29997 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/iot/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipam/__init__.py
--rw-r--r--   0        0        0      762 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipam/v1/__init__.py
--rw-r--r--   0        0        0    13026 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipam/v1/api.py
--rw-r--r--   0        0        0     4324 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipam/v1/marshalling.py
--rw-r--r--   0        0        0     6040 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipam/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipfs/__init__.py
--rw-r--r--   0        0        0     2572 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/__init__.py
--rw-r--r--   0        0        0    33644 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/api.py
--rw-r--r--   0        0        0      552 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/content.py
--rw-r--r--   0        0        0    10996 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    11507 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/jobs/__init__.py
--rw-r--r--   0        0        0     1464 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/__init__.py
--rw-r--r--   0        0        0    14617 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/api.py
--rw-r--r--   0        0        0      401 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/content.py
--rw-r--r--   0        0        0     5997 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     4756 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/__init__.py
--rw-r--r--   0        0        0     5312 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/v1/__init__.py
--rw-r--r--   0        0        0    58714 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/v1/api.py
--rw-r--r--   0        0        0      934 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/v1/content.py
--rw-r--r--   0        0        0    34608 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/v1/marshalling.py
--rw-r--r--   0        0        0    45094 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/v1/types.py
--rw-r--r--   0        0        0      540 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/k8s/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/lb/__init__.py
--rw-r--r--   0        0        0    13054 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/lb/v1/__init__.py
--rw-r--r--   0        0        0   221979 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/lb/v1/api.py
--rw-r--r--   0        0        0     1106 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/lb/v1/content.py
--rw-r--r--   0        0        0    72789 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/lb/v1/marshalling.py
--rw-r--r--   0        0        0    88883 2023-11-27 13:24:43.899617 scaleway-2.0.0.dev5/scaleway/lb/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/__init__.py
--rw-r--r--   0        0        0      884 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/v1/__init__.py
--rw-r--r--   0        0        0     4428 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/v1/api.py
--rw-r--r--   0        0        0     5343 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/v1/marshalling.py
--rw-r--r--   0        0        0     3014 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/v1/types.py
--rw-r--r--   0        0        0     1470 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/v2/__init__.py
--rw-r--r--   0        0        0    14335 2023-11-27 13:24:43.903617 scaleway-2.0.0.dev5/scaleway/marketplace/v2/api.py
--rw-r--r--   0        0        0     5429 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/marketplace/v2/marshalling.py
--rw-r--r--   0        0        0     5135 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/marketplace/v2/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/mnq/__init__.py
--rw-r--r--   0        0        0     3766 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/__init__.py
--rw-r--r--   0        0        0    42072 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/api.py
--rw-r--r--   0        0        0    15225 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/marshalling.py
--rw-r--r--   0        0        0    16867 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/types.py
--rw-r--r--   0        0        0        0 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/py.typed
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/qaas/__init__.py
--rw-r--r--   0        0        0     1994 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/__init__.py
--rw-r--r--   0        0        0    21731 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/api.py
--rw-r--r--   0        0        0      600 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/content.py
--rw-r--r--   0        0        0     8552 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     9916 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/rdb/__init__.py
--rw-r--r--   0        0        0    10286 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/rdb/v1/__init__.py
--rw-r--r--   0        0        0   117249 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/rdb/v1/api.py
--rw-r--r--   0        0        0     1947 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/rdb/v1/content.py
--rw-r--r--   0        0        0    48994 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/rdb/v1/marshalling.py
--rw-r--r--   0        0        0    47933 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/rdb/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/redis/__init__.py
--rw-r--r--   0        0        0     3760 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/redis/v1/__init__.py
--rw-r--r--   0        0        0    43927 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/redis/v1/api.py
--rw-r--r--   0        0        0      488 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/redis/v1/content.py
--rw-r--r--   0        0        0    19329 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/redis/v1/marshalling.py
--rw-r--r--   0        0        0    17769 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/redis/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/registry/__init__.py
--rw-r--r--   0        0        0     1962 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/registry/v1/__init__.py
--rw-r--r--   0        0        0    29003 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/registry/v1/api.py
--rw-r--r--   0        0        0      710 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/registry/v1/content.py
--rw-r--r--   0        0        0     6741 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/registry/v1/marshalling.py
--rw-r--r--   0        0        0    11276 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/registry/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/secret/__init__.py
--rw-r--r--   0        0        0     3036 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/__init__.py
--rw-r--r--   0        0        0    50497 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/api.py
--rw-r--r--   0        0        0    11199 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    20064 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/types.py
--rw-r--r--   0        0        0      194 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/std/__init__.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/std/api.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/std/marshalling.py
--rw-r--r--   0        0        0      469 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/std/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/tem/__init__.py
--rw-r--r--   0        0        0     2370 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/__init__.py
--rw-r--r--   0        0        0    25780 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/api.py
--rw-r--r--   0        0        0      549 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/content.py
--rw-r--r--   0        0        0    12392 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    15311 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/test/__init__.py
--rw-r--r--   0        0        0     1088 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/test/v1/__init__.py
--rw-r--r--   0        0        0    11504 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/test/v1/api.py
--rw-r--r--   0        0        0      349 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/test/v1/content.py
--rw-r--r--   0        0        0     5549 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/test/v1/marshalling.py
--rw-r--r--   0        0        0     3231 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/test/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/testinternal/__init__.py
--rw-r--r--   0        0        0     5394 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/testinternal/v1/__init__.py
--rw-r--r--   0        0        0    61934 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/testinternal/v1/api.py
--rw-r--r--   0        0        0      373 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/testinternal/v1/content.py
--rw-r--r--   0        0        0    77739 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/testinternal/v1/marshalling.py
--rw-r--r--   0        0        0    23543 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/testinternal/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/__init__.py
--rw-r--r--   0        0        0      818 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v1/__init__.py
--rw-r--r--   0        0        0    11732 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v1/api.py
--rw-r--r--   0        0        0     2912 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v1/marshalling.py
--rw-r--r--   0        0        0     4368 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v1/types.py
--rw-r--r--   0        0        0     1864 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v2/__init__.py
--rw-r--r--   0        0        0    29237 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v2/api.py
--rw-r--r--   0        0        0     9014 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v2/marshalling.py
--rw-r--r--   0        0        0    10131 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpc/v2/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpcgw/__init__.py
--rw-r--r--   0        0        0     4770 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpcgw/v1/__init__.py
--rw-r--r--   0        0        0    79566 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpcgw/v1/api.py
--rw-r--r--   0        0        0      754 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpcgw/v1/content.py
--rw-r--r--   0        0        0    26355 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpcgw/v1/marshalling.py
--rw-r--r--   0        0        0    35147 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/vpcgw/v1/types.py
--rw-r--r--   0        0        0      127 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/webhosting/__init__.py
--rw-r--r--   0        0        0     2128 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20047 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/api.py
--rw-r--r--   0        0        0      421 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/content.py
--rw-r--r--   0        0        0    10319 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    12583 2023-11-27 13:24:43.907617 scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/types.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 scaleway-2.0.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/README.md
+-rw-r--r--   0        0        0     1132 2023-11-28 15:51:56.846307 scaleway-2.0.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0      905 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/__init__.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/__init__.py
+-rw-r--r--   0        0        0      714 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v2/__init__.py
+-rw-r--r--   0        0        0     8456 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v2/api.py
+-rw-r--r--   0        0        0     2762 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v2/marshalling.py
+-rw-r--r--   0        0        0     2638 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v2/types.py
+-rw-r--r--   0        0        0      828 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v3/__init__.py
+-rw-r--r--   0        0        0     8180 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v3/api.py
+-rw-r--r--   0        0        0     2822 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v3/marshalling.py
+-rw-r--r--   0        0        0     2678 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/account/v3/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/applesilicon/__init__.py
+-rw-r--r--   0        0        0     1674 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18185 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/api.py
+-rw-r--r--   0        0        0      496 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/content.py
+-rw-r--r--   0        0        0     7536 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     7171 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/baremetal/__init__.py
+-rw-r--r--   0        0        0     5332 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/baremetal/v1/__init__.py
+-rw-r--r--   0        0        0    52790 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/baremetal/v1/api.py
+-rw-r--r--   0        0        0     1060 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/baremetal/v1/content.py
+-rw-r--r--   0        0        0    30608 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/baremetal/v1/marshalling.py
+-rw-r--r--   0        0        0    27983 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/baremetal/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/billing/__init__.py
+-rw-r--r--   0        0        0     1414 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/__init__.py
+-rw-r--r--   0        0        0     9098 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/api.py
+-rw-r--r--   0        0        0     7208 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/marshalling.py
+-rw-r--r--   0        0        0     7103 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/block/__init__.py
+-rw-r--r--   0        0        0     2456 2023-11-28 15:51:38.522460 scaleway-2.0.0.dev6/scaleway/block/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    26281 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/block/v1alpha1/api.py
+-rw-r--r--   0        0        0      926 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/block/v1alpha1/content.py
+-rw-r--r--   0        0        0    13955 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/block/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    13735 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/block/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/cockpit/__init__.py
+-rw-r--r--   0        0        0     3684 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/__init__.py
+-rw-r--r--   0        0        0    34543 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/api.py
+-rw-r--r--   0        0        0      418 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/content.py
+-rw-r--r--   0        0        0    21183 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    15156 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/container/__init__.py
+-rw-r--r--   0        0        0     5370 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/container/v1beta1/__init__.py
+-rw-r--r--   0        0        0    65173 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/container/v1beta1/api.py
+-rw-r--r--   0        0        0     1581 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/container/v1beta1/content.py
+-rw-r--r--   0        0        0    28232 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/container/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    28544 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/container/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/document_db/__init__.py
+-rw-r--r--   0        0        0     9020 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/__init__.py
+-rw-r--r--   0        0        0   100490 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/api.py
+-rw-r--r--   0        0        0     1612 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/content.py
+-rw-r--r--   0        0        0    49031 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    41184 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/domain/__init__.py
+-rw-r--r--   0        0        0    13030 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/domain/v2beta1/__init__.py
+-rw-r--r--   0        0        0    87761 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/domain/v2beta1/api.py
+-rw-r--r--   0        0        0     1942 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/domain/v2beta1/content.py
+-rw-r--r--   0        0        0    86406 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/domain/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    34374 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/domain/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/flexibleip/__init__.py
+-rw-r--r--   0        0        0     1762 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20505 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/api.py
+-rw-r--r--   0        0        0      647 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/content.py
+-rw-r--r--   0        0        0     7811 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8804 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/function/__init__.py
+-rw-r--r--   0        0        0     5864 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/function/v1beta1/__init__.py
+-rw-r--r--   0        0        0    67235 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/function/v1beta1/api.py
+-rw-r--r--   0        0        0     1573 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/function/v1beta1/content.py
+-rw-r--r--   0        0        0    30521 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/function/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    30250 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/function/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/iam/__init__.py
+-rw-r--r--   0        0        0     5416 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    79405 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/api.py
+-rw-r--r--   0        0        0    30504 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    29209 2023-11-28 15:51:38.526460 scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/__init__.py
+-rw-r--r--   0        0        0    13232 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/__init__.py
+-rw-r--r--   0        0        0   139528 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/api.py
+-rw-r--r--   0        0        0     2660 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/api_utils.py
+-rw-r--r--   0        0        0     2384 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/content.py
+-rw-r--r--   0        0        0   106377 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/marshalling.py
+-rw-r--r--   0        0        0      712 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/marshalling_utils.py
+-rw-r--r--   0        0        0    66625 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/types.py
+-rw-r--r--   0        0        0    11110 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/instance/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/iot/__init__.py
+-rw-r--r--   0        0        0     5818 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/iot/v1/__init__.py
+-rw-r--r--   0        0        0    61461 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/iot/v1/api.py
+-rw-r--r--   0        0        0      363 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/iot/v1/content.py
+-rw-r--r--   0        0        0    32821 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/iot/v1/marshalling.py
+-rw-r--r--   0        0        0    29997 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/iot/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipam/__init__.py
+-rw-r--r--   0        0        0      762 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipam/v1/__init__.py
+-rw-r--r--   0        0        0    13026 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipam/v1/api.py
+-rw-r--r--   0        0        0     4924 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipam/v1/marshalling.py
+-rw-r--r--   0        0        0     6040 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipam/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipfs/__init__.py
+-rw-r--r--   0        0        0     2572 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    33644 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/api.py
+-rw-r--r--   0        0        0      552 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/content.py
+-rw-r--r--   0        0        0    12468 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    11507 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/jobs/__init__.py
+-rw-r--r--   0        0        0     1464 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    14617 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/api.py
+-rw-r--r--   0        0        0      401 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/content.py
+-rw-r--r--   0        0        0     6847 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     4756 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/__init__.py
+-rw-r--r--   0        0        0     5312 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/v1/__init__.py
+-rw-r--r--   0        0        0    58714 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/v1/api.py
+-rw-r--r--   0        0        0      934 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/v1/content.py
+-rw-r--r--   0        0        0    38380 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/v1/marshalling.py
+-rw-r--r--   0        0        0    45094 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/v1/types.py
+-rw-r--r--   0        0        0      540 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/k8s/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/lb/__init__.py
+-rw-r--r--   0        0        0    13054 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/lb/v1/__init__.py
+-rw-r--r--   0        0        0   221979 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/lb/v1/api.py
+-rw-r--r--   0        0        0     1106 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/lb/v1/content.py
+-rw-r--r--   0        0        0    78597 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/lb/v1/marshalling.py
+-rw-r--r--   0        0        0    88883 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/lb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/marketplace/__init__.py
+-rw-r--r--   0        0        0      884 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/marketplace/v1/__init__.py
+-rw-r--r--   0        0        0     4428 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/marketplace/v1/api.py
+-rw-r--r--   0        0        0     6349 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/marketplace/v1/marshalling.py
+-rw-r--r--   0        0        0     3014 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/marketplace/v1/types.py
+-rw-r--r--   0        0        0     1470 2023-11-28 15:51:38.530460 scaleway-2.0.0.dev6/scaleway/marketplace/v2/__init__.py
+-rw-r--r--   0        0        0    14335 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/marketplace/v2/api.py
+-rw-r--r--   0        0        0     6455 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/marketplace/v2/marshalling.py
+-rw-r--r--   0        0        0     5135 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/marketplace/v2/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/mnq/__init__.py
+-rw-r--r--   0        0        0     3766 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/__init__.py
+-rw-r--r--   0        0        0    42072 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/api.py
+-rw-r--r--   0        0        0    17117 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    16867 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/types.py
+-rw-r--r--   0        0        0        0 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/py.typed
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/qaas/__init__.py
+-rw-r--r--   0        0        0     1994 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    21731 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/api.py
+-rw-r--r--   0        0        0      600 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/content.py
+-rw-r--r--   0        0        0     9768 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9916 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/rdb/__init__.py
+-rw-r--r--   0        0        0    10286 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/rdb/v1/__init__.py
+-rw-r--r--   0        0        0   117249 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/rdb/v1/api.py
+-rw-r--r--   0        0        0     1947 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/rdb/v1/content.py
+-rw-r--r--   0        0        0    54842 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/rdb/v1/marshalling.py
+-rw-r--r--   0        0        0    47933 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/rdb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/redis/__init__.py
+-rw-r--r--   0        0        0     3760 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/redis/v1/__init__.py
+-rw-r--r--   0        0        0    43927 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/redis/v1/api.py
+-rw-r--r--   0        0        0      488 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/redis/v1/content.py
+-rw-r--r--   0        0        0    21445 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/redis/v1/marshalling.py
+-rw-r--r--   0        0        0    17769 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/redis/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/registry/__init__.py
+-rw-r--r--   0        0        0     1962 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/registry/v1/__init__.py
+-rw-r--r--   0        0        0    29003 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/registry/v1/api.py
+-rw-r--r--   0        0        0      710 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/registry/v1/content.py
+-rw-r--r--   0        0        0     7883 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/registry/v1/marshalling.py
+-rw-r--r--   0        0        0    11276 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/registry/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/secret/__init__.py
+-rw-r--r--   0        0        0     3036 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    50497 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/api.py
+-rw-r--r--   0        0        0    12453 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    20064 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/types.py
+-rw-r--r--   0        0        0      194 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/std/__init__.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/std/api.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/std/marshalling.py
+-rw-r--r--   0        0        0      469 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/std/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/tem/__init__.py
+-rw-r--r--   0        0        0     2370 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    25780 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/api.py
+-rw-r--r--   0        0        0      549 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/content.py
+-rw-r--r--   0        0        0    14480 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    15311 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/test/__init__.py
+-rw-r--r--   0        0        0     1088 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/test/v1/__init__.py
+-rw-r--r--   0        0        0    11504 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/test/v1/api.py
+-rw-r--r--   0        0        0      349 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/test/v1/content.py
+-rw-r--r--   0        0        0     6143 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/test/v1/marshalling.py
+-rw-r--r--   0        0        0     3231 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/test/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/testinternal/__init__.py
+-rw-r--r--   0        0        0     5394 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/testinternal/v1/__init__.py
+-rw-r--r--   0        0        0    61934 2023-11-28 15:51:38.534459 scaleway-2.0.0.dev6/scaleway/testinternal/v1/api.py
+-rw-r--r--   0        0        0      373 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/testinternal/v1/content.py
+-rw-r--r--   0        0        0    84969 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/testinternal/v1/marshalling.py
+-rw-r--r--   0        0        0    23543 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/testinternal/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/__init__.py
+-rw-r--r--   0        0        0      818 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v1/__init__.py
+-rw-r--r--   0        0        0    11732 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v1/api.py
+-rw-r--r--   0        0        0     3250 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v1/marshalling.py
+-rw-r--r--   0        0        0     4368 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v1/types.py
+-rw-r--r--   0        0        0     1864 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v2/__init__.py
+-rw-r--r--   0        0        0    29237 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v2/api.py
+-rw-r--r--   0        0        0     9990 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v2/marshalling.py
+-rw-r--r--   0        0        0    10131 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpc/v2/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpcgw/__init__.py
+-rw-r--r--   0        0        0     4770 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpcgw/v1/__init__.py
+-rw-r--r--   0        0        0    79566 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpcgw/v1/api.py
+-rw-r--r--   0        0        0      754 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpcgw/v1/content.py
+-rw-r--r--   0        0        0    29413 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpcgw/v1/marshalling.py
+-rw-r--r--   0        0        0    35147 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/vpcgw/v1/types.py
+-rw-r--r--   0        0        0      127 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/webhosting/__init__.py
+-rw-r--r--   0        0        0     2128 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20047 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/api.py
+-rw-r--r--   0        0        0      421 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/content.py
+-rw-r--r--   0        0        0    12221 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    12583 2023-11-28 15:51:38.538459 scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/types.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 scaleway-2.0.0.dev6/PKG-INFO
```

### Comparing `scaleway-2.0.0.dev5/pyproject.toml` & `scaleway-2.0.0.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway"
-version = "2.0.0.dev5"
+version = "2.0.0.dev6"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-scaleway-core = "2.0.0.dev5"
+scaleway-core = "2.0.0.dev6"
 
 [tool.poetry.group.dev.dependencies]
 scaleway-core = { path = "../scaleway-core", develop = true }
 ruff = "^0.0.286"
 mypy = "^1.5.1"
 black = "^23.7.0"
```

### Comparing `scaleway-2.0.0.dev5/scaleway/__init__.py` & `scaleway-2.0.0.dev6/scaleway/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v2/__init__.py` & `scaleway-2.0.0.dev6/scaleway/account/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v2/api.py` & `scaleway-2.0.0.dev6/scaleway/account/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v2/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/account/v3/marshalling.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,89 +4,97 @@
 from typing import Any, Dict
 from dateutil import parser
 
 from scaleway_core.profile import ProfileDefaults
 from .types import (
     Project,
     ListProjectsResponse,
-    CreateProjectRequest,
-    UpdateProjectRequest,
+    ProjectApiCreateProjectRequest,
+    ProjectApiUpdateProjectRequest,
 )
 
 
 def unmarshal_Project(data: Any) -> Project:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Project' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Project(**args)
 
 
 def unmarshal_ListProjectsResponse(data: Any) -> ListProjectsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListProjectsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("projects", None)
-    args["projects"] = (
-        [unmarshal_Project(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["projects"] = (
+            [unmarshal_Project(v) for v in field] if field is not None else None
+        )
 
     return ListProjectsResponse(**args)
 
 
-def marshal_CreateProjectRequest(
-    request: CreateProjectRequest,
+def marshal_ProjectApiCreateProjectRequest(
+    request: ProjectApiCreateProjectRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
+    if request.description is not None:
+        output["description"] = request.description
+
     if request.name is not None:
         output["name"] = request.name
 
     if request.organization_id is not None:
         output["organization_id"] = (
             request.organization_id or defaults.default_organization_id
         )
 
-    if request.description is not None:
-        output["description"] = request.description
-
     return output
 
 
-def marshal_UpdateProjectRequest(
-    request: UpdateProjectRequest,
+def marshal_ProjectApiUpdateProjectRequest(
+    request: ProjectApiUpdateProjectRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
```

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v2/types.py` & `scaleway-2.0.0.dev6/scaleway/account/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v3/__init__.py` & `scaleway-2.0.0.dev6/scaleway/account/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v3/api.py` & `scaleway-2.0.0.dev6/scaleway/account/v3/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v3/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/account/v2/marshalling.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,89 +4,97 @@
 from typing import Any, Dict
 from dateutil import parser
 
 from scaleway_core.profile import ProfileDefaults
 from .types import (
     Project,
     ListProjectsResponse,
-    ProjectApiCreateProjectRequest,
-    ProjectApiUpdateProjectRequest,
+    CreateProjectRequest,
+    UpdateProjectRequest,
 )
 
 
 def unmarshal_Project(data: Any) -> Project:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Project' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Project(**args)
 
 
 def unmarshal_ListProjectsResponse(data: Any) -> ListProjectsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListProjectsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("projects", None)
-    args["projects"] = (
-        [unmarshal_Project(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["projects"] = (
+            [unmarshal_Project(v) for v in field] if field is not None else None
+        )
 
     return ListProjectsResponse(**args)
 
 
-def marshal_ProjectApiCreateProjectRequest(
-    request: ProjectApiCreateProjectRequest,
+def marshal_CreateProjectRequest(
+    request: CreateProjectRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.description is not None:
-        output["description"] = request.description
-
     if request.name is not None:
         output["name"] = request.name
 
     if request.organization_id is not None:
         output["organization_id"] = (
             request.organization_id or defaults.default_organization_id
         )
 
+    if request.description is not None:
+        output["description"] = request.description
+
     return output
 
 
-def marshal_ProjectApiUpdateProjectRequest(
-    request: ProjectApiUpdateProjectRequest,
+def marshal_UpdateProjectRequest(
+    request: UpdateProjectRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
```

### Comparing `scaleway-2.0.0.dev5/scaleway/account/v3/types.py` & `scaleway-2.0.0.dev6/scaleway/account/v3/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/marshalling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,255 +1,259 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 
 from typing import Any, Dict
 from dateutil import parser
 
-from scaleway_core.profile import ProfileDefaults
+from scaleway_core.bridge import (
+    unmarshal_Money,
+)
 from .types import (
-    OS,
-    ServerTypeCPU,
-    ServerTypeDisk,
-    ServerTypeMemory,
-    ServerType,
-    Server,
-    ListOSResponse,
-    ListServerTypesResponse,
-    ListServersResponse,
-    CreateServerRequest,
-    UpdateServerRequest,
+    GetConsumptionResponseConsumption,
+    GetConsumptionResponse,
+    DiscountCoupon,
+    DiscountFilter,
+    Discount,
+    ListDiscountsResponse,
+    Invoice,
+    ListInvoicesResponse,
 )
 
 
-def unmarshal_OS(data: Any) -> OS:
+def unmarshal_GetConsumptionResponseConsumption(
+    data: Any,
+) -> GetConsumptionResponseConsumption:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'OS' failed as data isn't a dictionary."
+            "Unmarshalling the type 'GetConsumptionResponseConsumption' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
 
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
-    field = data.get("label", None)
-    args["label"] = field
+    field = data.get("category", None)
+    if field is not None:
+        args["category"] = field
 
-    field = data.get("image_url", None)
-    args["image_url"] = field
+    field = data.get("operation_path", None)
+    if field is not None:
+        args["operation_path"] = field
 
-    field = data.get("compatible_server_types", None)
-    args["compatible_server_types"] = field
+    field = data.get("value", None)
+    if field is not None:
+        args["value"] = unmarshal_Money(field)
 
-    return OS(**args)
+    return GetConsumptionResponseConsumption(**args)
 
 
-def unmarshal_ServerTypeCPU(data: Any) -> ServerTypeCPU:
+def unmarshal_GetConsumptionResponse(data: Any) -> GetConsumptionResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerTypeCPU' failed as data isn't a dictionary."
+            "Unmarshalling the type 'GetConsumptionResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("core_count", None)
-    args["core_count"] = field
-
-    return ServerTypeCPU(**args)
-
-
-def unmarshal_ServerTypeDisk(data: Any) -> ServerTypeDisk:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ServerTypeDisk' failed as data isn't a dictionary."
+    field = data.get("consumptions", None)
+    if field is not None:
+        args["consumptions"] = (
+            [unmarshal_GetConsumptionResponseConsumption(v) for v in field]
+            if field is not None
+            else None
         )
 
-    args: Dict[str, Any] = {}
-
-    field = data.get("capacity", None)
-    args["capacity"] = field
-
-    field = data.get("type_", None)
-    args["type_"] = field
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return ServerTypeDisk(**args)
+    return GetConsumptionResponse(**args)
 
 
-def unmarshal_ServerTypeMemory(data: Any) -> ServerTypeMemory:
+def unmarshal_DiscountCoupon(data: Any) -> DiscountCoupon:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerTypeMemory' failed as data isn't a dictionary."
+            "Unmarshalling the type 'DiscountCoupon' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("capacity", None)
-    args["capacity"] = field
-
-    field = data.get("type_", None)
-    args["type_"] = field
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
 
-    return ServerTypeMemory(**args)
+    return DiscountCoupon(**args)
 
 
-def unmarshal_ServerType(data: Any) -> ServerType:
+def unmarshal_DiscountFilter(data: Any) -> DiscountFilter:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerType' failed as data isn't a dictionary."
+            "Unmarshalling the type 'DiscountFilter' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("stock", None)
-    args["stock"] = field
-
-    field = data.get("cpu", None)
-    args["cpu"] = unmarshal_ServerTypeCPU(field)
-
-    field = data.get("disk", None)
-    args["disk"] = unmarshal_ServerTypeDisk(field)
-
-    field = data.get("memory", None)
-    args["memory"] = unmarshal_ServerTypeMemory(field)
+    field = data.get("type_", None)
+    if field is not None:
+        args["type_"] = field
 
-    field = data.get("minimum_lease_duration", None)
-    args["minimum_lease_duration"] = field
+    field = data.get("value", None)
+    if field is not None:
+        args["value"] = field
 
-    return ServerType(**args)
+    return DiscountFilter(**args)
 
 
-def unmarshal_Server(data: Any) -> Server:
+def unmarshal_Discount(data: Any) -> Discount:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Server' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Discount' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("type_", None)
-    args["type_"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
-
-    field = data.get("ip", None)
-    args["ip"] = field
-
-    field = data.get("vnc_url", None)
-    args["vnc_url"] = field
+    if field is not None:
+        args["organization_id"] = field
 
-    field = data.get("status", None)
-    args["status"] = field
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
+
+    field = data.get("value", None)
+    if field is not None:
+        args["value"] = field
+
+    field = data.get("value_used", None)
+    if field is not None:
+        args["value_used"] = field
+
+    field = data.get("value_remaining", None)
+    if field is not None:
+        args["value_remaining"] = field
+
+    field = data.get("mode", None)
+    if field is not None:
+        args["mode"] = field
+
+    field = data.get("filters", None)
+    if field is not None:
+        args["filters"] = (
+            [unmarshal_DiscountFilter(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("creation_date", None)
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("start_date", None)
+    if field is not None:
+        args["start_date"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("stop_date", None)
+    if field is not None:
+        args["stop_date"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("deletable_at", None)
-    args["deletable_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("coupon", None)
+    if field is not None:
+        args["coupon"] = unmarshal_DiscountCoupon(field)
 
-    return Server(**args)
+    return Discount(**args)
 
 
-def unmarshal_ListOSResponse(data: Any) -> ListOSResponse:
+def unmarshal_ListDiscountsResponse(data: Any) -> ListDiscountsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListOSResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListDiscountsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    field = data.get("os", None)
-    args["os"] = [unmarshal_OS(v) for v in field] if field is not None else None
-
-    return ListOSResponse(**args)
-
-
-def unmarshal_ListServerTypesResponse(data: Any) -> ListServerTypesResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListServerTypesResponse' failed as data isn't a dictionary."
+    field = data.get("discounts", None)
+    if field is not None:
+        args["discounts"] = (
+            [unmarshal_Discount(v) for v in field] if field is not None else None
         )
 
-    args: Dict[str, Any] = {}
-
-    field = data.get("server_types", None)
-    args["server_types"] = (
-        [unmarshal_ServerType(v) for v in field] if field is not None else None
-    )
-
-    return ListServerTypesResponse(**args)
+    return ListDiscountsResponse(**args)
 
 
-def unmarshal_ListServersResponse(data: Any) -> ListServersResponse:
+def unmarshal_Invoice(data: Any) -> Invoice:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListServersResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Invoice' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
-
-    field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_Server(v) for v in field] if field is not None else None
-    )
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-    return ListServersResponse(**args)
+    field = data.get("invoice_type", None)
+    if field is not None:
+        args["invoice_type"] = field
+
+    field = data.get("number", None)
+    if field is not None:
+        args["number"] = field
+
+    field = data.get("start_date", None)
+    if field is not None:
+        args["start_date"] = parser.isoparse(field) if isinstance(field, str) else field
+
+    field = data.get("issued_date", None)
+    if field is not None:
+        args["issued_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
+    field = data.get("due_date", None)
+    if field is not None:
+        args["due_date"] = parser.isoparse(field) if isinstance(field, str) else field
 
-def marshal_CreateServerRequest(
-    request: CreateServerRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
+    field = data.get("total_untaxed", None)
+    if field is not None:
+        args["total_untaxed"] = unmarshal_Money(field)
 
-    if request.type_ is not None:
-        output["type"] = request.type_
+    field = data.get("total_taxed", None)
+    if field is not None:
+        args["total_taxed"] = unmarshal_Money(field)
 
-    if request.name is not None:
-        output["name"] = request.name
+    return Invoice(**args)
 
-    if request.project_id is not None:
-        output["project_id"] = request.project_id or defaults.default_project_id
 
-    return output
+def unmarshal_ListInvoicesResponse(data: Any) -> ListInvoicesResponse:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ListInvoicesResponse' failed as data isn't a dictionary."
+        )
 
+    args: Dict[str, Any] = {}
 
-def marshal_UpdateServerRequest(
-    request: UpdateServerRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    if request.name is not None:
-        output["name"] = request.name
+    field = data.get("invoices", None)
+    if field is not None:
+        args["invoices"] = (
+            [unmarshal_Invoice(v) for v in field] if field is not None else None
+        )
 
-    return output
+    return ListInvoicesResponse(**args)
```

### Comparing `scaleway-2.0.0.dev5/scaleway/applesilicon/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/baremetal/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/baremetal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/baremetal/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/baremetal/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/baremetal/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/baremetal/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/baremetal/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/vpcgw/v1/marshalling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1026 +1,1075 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 
 from typing import Any, Dict
 from dateutil import parser
 
 from scaleway_core.profile import ProfileDefaults
-from scaleway_core.bridge import (
-    unmarshal_Money,
-    unmarshal_TimeSeries,
-)
 from scaleway_core.utils import (
     OneOfPossibility,
     resolve_one_of,
 )
 from .types import (
+    DHCP,
+    IpamConfig,
+    GatewayNetwork,
     IP,
-    OSOSField,
-    OS,
-    CPU,
-    Disk,
-    Memory,
-    OfferOptionOffer,
-    PersistentMemory,
-    RaidController,
-    Offer,
-    Option,
-    ServerPrivateNetwork,
-    ServerInstall,
-    ServerOption,
-    ServerRescueServer,
-    Server,
-    Setting,
-    BMCAccess,
-    GetServerMetricsResponse,
-    ListOSResponse,
-    ListOffersResponse,
-    ListOptionsResponse,
-    ServerEvent,
-    ListServerEventsResponse,
-    ListServerPrivateNetworksResponse,
-    ListServersResponse,
-    ListSettingsResponse,
-    SetServerPrivateNetworksResponse,
-    AddOptionServerRequest,
-    CreateServerRequestInstall,
-    CreateServerRequest,
-    InstallServerRequest,
-    PrivateNetworkApiAddServerPrivateNetworkRequest,
-    PrivateNetworkApiSetServerPrivateNetworksRequest,
-    RebootServerRequest,
-    StartBMCAccessRequest,
-    StartServerRequest,
+    DHCPEntry,
+    GatewayType,
+    Gateway,
+    PATRule,
+    ListDHCPEntriesResponse,
+    ListDHCPsResponse,
+    ListGatewayNetworksResponse,
+    ListGatewayTypesResponse,
+    ListGatewaysResponse,
+    ListIPsResponse,
+    ListPATRulesResponse,
+    SetDHCPEntriesResponse,
+    SetPATRulesResponse,
+    CreateDHCPRequest,
+    CreateDHCPEntryRequest,
+    CreateGatewayNetworkRequestIpamConfig,
+    CreateGatewayNetworkRequest,
+    CreateGatewayRequest,
+    CreateIPRequest,
+    CreatePATRuleRequest,
+    SetDHCPEntriesRequestEntry,
+    SetDHCPEntriesRequest,
+    SetPATRulesRequestRule,
+    SetPATRulesRequest,
+    UpdateDHCPEntryRequest,
+    UpdateDHCPRequest,
+    UpdateGatewayNetworkRequestIpamConfig,
+    UpdateGatewayNetworkRequest,
+    UpdateGatewayRequest,
     UpdateIPRequest,
-    UpdateServerRequest,
-    UpdateSettingRequest,
+    UpdatePATRuleRequest,
 )
 
 
-def unmarshal_IP(data: Any) -> IP:
+def unmarshal_DHCP(data: Any) -> DHCP:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'IP' failed as data isn't a dictionary."
+            "Unmarshalling the type 'DHCP' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("address", None)
-    args["address"] = field
+    field = data.get("organization_id", None)
+    if field is not None:
+        args["organization_id"] = field
 
-    field = data.get("reverse", None)
-    args["reverse"] = field
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
-    field = data.get("version", None)
-    args["version"] = field
+    field = data.get("subnet", None)
+    if field is not None:
+        args["subnet"] = field
 
-    field = data.get("reverse_status", None)
-    args["reverse_status"] = field
+    field = data.get("address", None)
+    if field is not None:
+        args["address"] = field
 
-    field = data.get("reverse_status_message", None)
-    args["reverse_status_message"] = field
+    field = data.get("pool_low", None)
+    if field is not None:
+        args["pool_low"] = field
 
-    return IP(**args)
+    field = data.get("created_at", None)
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-def unmarshal_OSOSField(data: Any) -> OSOSField:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'OSOSField' failed as data isn't a dictionary."
-        )
+    field = data.get("pool_high", None)
+    if field is not None:
+        args["pool_high"] = field
+
+    field = data.get("enable_dynamic", None)
+    if field is not None:
+        args["enable_dynamic"] = field
+
+    field = data.get("push_default_route", None)
+    if field is not None:
+        args["push_default_route"] = field
+
+    field = data.get("push_dns_server", None)
+    if field is not None:
+        args["push_dns_server"] = field
+
+    field = data.get("dns_servers_override", None)
+    if field is not None:
+        args["dns_servers_override"] = field
+
+    field = data.get("dns_search", None)
+    if field is not None:
+        args["dns_search"] = field
+
+    field = data.get("dns_local_name", None)
+    if field is not None:
+        args["dns_local_name"] = field
 
-    args: Dict[str, Any] = {}
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
-    field = data.get("editable", None)
-    args["editable"] = field
+    field = data.get("valid_lifetime", None)
+    if field is not None:
+        args["valid_lifetime"] = field
 
-    field = data.get("required", None)
-    args["required"] = field
+    field = data.get("renew_timer", None)
+    if field is not None:
+        args["renew_timer"] = field
 
-    field = data.get("default_value", None)
-    args["default_value"] = field
+    field = data.get("rebind_timer", None)
+    if field is not None:
+        args["rebind_timer"] = field
 
-    return OSOSField(**args)
+    return DHCP(**args)
 
 
-def unmarshal_OS(data: Any) -> OS:
+def unmarshal_IpamConfig(data: Any) -> IpamConfig:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'OS' failed as data isn't a dictionary."
+            "Unmarshalling the type 'IpamConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("version", None)
-    args["version"] = field
+    field = data.get("push_default_route", None)
+    if field is not None:
+        args["push_default_route"] = field
 
-    field = data.get("logo_url", None)
-    args["logo_url"] = field
+    field = data.get("ipam_ip_id", None)
+    if field is not None:
+        args["ipam_ip_id"] = field
 
-    field = data.get("enabled", None)
-    args["enabled"] = field
+    return IpamConfig(**args)
 
-    field = data.get("license_required", None)
-    args["license_required"] = field
 
-    field = data.get("allowed", None)
-    args["allowed"] = field
+def unmarshal_GatewayNetwork(data: Any) -> GatewayNetwork:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'GatewayNetwork' failed as data isn't a dictionary."
+        )
 
-    field = data.get("ssh", None)
-    args["ssh"] = unmarshal_OSOSField(field)
+    args: Dict[str, Any] = {}
 
-    field = data.get("user", None)
-    args["user"] = unmarshal_OSOSField(field)
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("password", None)
-    args["password"] = unmarshal_OSOSField(field)
+    field = data.get("gateway_id", None)
+    if field is not None:
+        args["gateway_id"] = field
 
-    field = data.get("service_user", None)
-    args["service_user"] = unmarshal_OSOSField(field)
+    field = data.get("private_network_id", None)
+    if field is not None:
+        args["private_network_id"] = field
 
-    field = data.get("service_password", None)
-    args["service_password"] = unmarshal_OSOSField(field)
+    field = data.get("created_at", None)
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return OS(**args)
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
+    field = data.get("mac_address", None)
+    if field is not None:
+        args["mac_address"] = field
+
+    field = data.get("enable_masquerade", None)
+    if field is not None:
+        args["enable_masquerade"] = field
 
-def unmarshal_CPU(data: Any) -> CPU:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'CPU' failed as data isn't a dictionary."
-        )
-
-    args: Dict[str, Any] = {}
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("enable_dhcp", None)
+    if field is not None:
+        args["enable_dhcp"] = field
 
-    field = data.get("core_count", None)
-    args["core_count"] = field
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
-    field = data.get("thread_count", None)
-    args["thread_count"] = field
+    field = data.get("dhcp", None)
+    if field is not None:
+        args["dhcp"] = unmarshal_DHCP(field)
 
-    field = data.get("frequency", None)
-    args["frequency"] = field
+    field = data.get("address", None)
+    if field is not None:
+        args["address"] = field
 
-    field = data.get("benchmark", None)
-    args["benchmark"] = field
+    field = data.get("ipam_config", None)
+    if field is not None:
+        args["ipam_config"] = unmarshal_IpamConfig(field)
 
-    return CPU(**args)
+    return GatewayNetwork(**args)
 
 
-def unmarshal_Disk(data: Any) -> Disk:
+def unmarshal_IP(data: Any) -> IP:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Disk' failed as data isn't a dictionary."
+            "Unmarshalling the type 'IP' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("capacity", None)
-    args["capacity"] = field
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("type_", None)
-    args["type_"] = field
+    field = data.get("organization_id", None)
+    if field is not None:
+        args["organization_id"] = field
 
-    return Disk(**args)
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
+    field = data.get("tags", None)
+    if field is not None:
+        args["tags"] = field
 
-def unmarshal_Memory(data: Any) -> Memory:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'Memory' failed as data isn't a dictionary."
-        )
+    field = data.get("address", None)
+    if field is not None:
+        args["address"] = field
 
-    args: Dict[str, Any] = {}
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
-    field = data.get("capacity", None)
-    args["capacity"] = field
+    field = data.get("created_at", None)
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("type_", None)
-    args["type_"] = field
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("frequency", None)
-    args["frequency"] = field
+    field = data.get("reverse", None)
+    if field is not None:
+        args["reverse"] = field
 
-    field = data.get("is_ecc", None)
-    args["is_ecc"] = field
+    field = data.get("gateway_id", None)
+    if field is not None:
+        args["gateway_id"] = field
 
-    return Memory(**args)
+    return IP(**args)
 
 
-def unmarshal_OfferOptionOffer(data: Any) -> OfferOptionOffer:
+def unmarshal_DHCPEntry(data: Any) -> DHCPEntry:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'OfferOptionOffer' failed as data isn't a dictionary."
+            "Unmarshalling the type 'DHCPEntry' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("gateway_network_id", None)
+    if field is not None:
+        args["gateway_network_id"] = field
+
+    field = data.get("mac_address", None)
+    if field is not None:
+        args["mac_address"] = field
+
+    field = data.get("ip_address", None)
+    if field is not None:
+        args["ip_address"] = field
 
-    field = data.get("enabled", None)
-    args["enabled"] = field
+    field = data.get("hostname", None)
+    if field is not None:
+        args["hostname"] = field
 
-    field = data.get("subscription_period", None)
-    args["subscription_period"] = field
+    field = data.get("type_", None)
+    if field is not None:
+        args["type_"] = field
 
-    field = data.get("manageable", None)
-    args["manageable"] = field
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
-    field = data.get("price", None)
-    args["price"] = unmarshal_Money(field)
+    field = data.get("created_at", None)
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("os_id", None)
-    args["os_id"] = field
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return OfferOptionOffer(**args)
+    return DHCPEntry(**args)
 
 
-def unmarshal_PersistentMemory(data: Any) -> PersistentMemory:
+def unmarshal_GatewayType(data: Any) -> GatewayType:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'PersistentMemory' failed as data isn't a dictionary."
+            "Unmarshalling the type 'GatewayType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("capacity", None)
-    args["capacity"] = field
-
-    field = data.get("type_", None)
-    args["type_"] = field
-
-    field = data.get("frequency", None)
-    args["frequency"] = field
-
-    return PersistentMemory(**args)
-
-
-def unmarshal_RaidController(data: Any) -> RaidController:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'RaidController' failed as data isn't a dictionary."
-        )
-
-    args: Dict[str, Any] = {}
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("model", None)
-    args["model"] = field
+    field = data.get("bandwidth", None)
+    if field is not None:
+        args["bandwidth"] = field
 
-    field = data.get("raid_level", None)
-    args["raid_level"] = field
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
-    return RaidController(**args)
+    return GatewayType(**args)
 
 
-def unmarshal_Offer(data: Any) -> Offer:
+def unmarshal_Gateway(data: Any) -> Gateway:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Offer' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Gateway' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("stock", None)
-    args["stock"] = field
-
-    field = data.get("bandwidth", None)
-    args["bandwidth"] = field
-
-    field = data.get("commercial_range", None)
-    args["commercial_range"] = field
-
-    field = data.get("disks", None)
-    args["disks"] = [unmarshal_Disk(v) for v in field] if field is not None else None
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("enable", None)
-    args["enable"] = field
-
-    field = data.get("price_per_hour", None)
-    args["price_per_hour"] = unmarshal_Money(field)
-
-    field = data.get("price_per_month", None)
-    args["price_per_month"] = unmarshal_Money(field)
-
-    field = data.get("cpus", None)
-    args["cpus"] = [unmarshal_CPU(v) for v in field] if field is not None else None
-
-    field = data.get("memories", None)
-    args["memories"] = (
-        [unmarshal_Memory(v) for v in field] if field is not None else None
-    )
-
-    field = data.get("quota_name", None)
-    args["quota_name"] = field
-
-    field = data.get("persistent_memories", None)
-    args["persistent_memories"] = (
-        [unmarshal_PersistentMemory(v) for v in field] if field is not None else None
-    )
-
-    field = data.get("raid_controllers", None)
-    args["raid_controllers"] = (
-        [unmarshal_RaidController(v) for v in field] if field is not None else None
-    )
+    field = data.get("organization_id", None)
+    if field is not None:
+        args["organization_id"] = field
 
-    field = data.get("incompatible_os_ids", None)
-    args["incompatible_os_ids"] = field
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
-    field = data.get("subscription_period", None)
-    args["subscription_period"] = field
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("operation_path", None)
-    args["operation_path"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("options", None)
-    args["options"] = (
-        [unmarshal_OfferOptionOffer(v) for v in field] if field is not None else None
-    )
+    field = data.get("created_at", None)
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("private_bandwidth", None)
-    args["private_bandwidth"] = field
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("shared_bandwidth", None)
-    args["shared_bandwidth"] = field
+    field = data.get("type_", None)
+    if field is not None:
+        args["type_"] = unmarshal_GatewayType(field)
 
     field = data.get("tags", None)
-    args["tags"] = field
-
-    field = data.get("fee", None)
-    args["fee"] = unmarshal_Money(field)
-
-    return Offer(**args)
-
+    if field is not None:
+        args["tags"] = field
 
-def unmarshal_Option(data: Any) -> Option:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'Option' failed as data isn't a dictionary."
-        )
+    field = data.get("gateway_networks", None)
+    if field is not None:
+        args["gateway_networks"] = (
+            [unmarshal_GatewayNetwork(v) for v in field] if field is not None else None
+        )
+
+    field = data.get("upstream_dns_servers", None)
+    if field is not None:
+        args["upstream_dns_servers"] = field
+
+    field = data.get("bastion_enabled", None)
+    if field is not None:
+        args["bastion_enabled"] = field
+
+    field = data.get("bastion_port", None)
+    if field is not None:
+        args["bastion_port"] = field
+
+    field = data.get("smtp_enabled", None)
+    if field is not None:
+        args["smtp_enabled"] = field
+
+    field = data.get("is_legacy", None)
+    if field is not None:
+        args["is_legacy"] = field
 
-    args: Dict[str, Any] = {}
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
-    field = data.get("id", None)
-    args["id"] = field
+    field = data.get("ip", None)
+    if field is not None:
+        args["ip"] = unmarshal_IP(field)
 
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("version", None)
+    if field is not None:
+        args["version"] = field
 
-    field = data.get("manageable", None)
-    args["manageable"] = field
+    field = data.get("can_upgrade_to", None)
+    if field is not None:
+        args["can_upgrade_to"] = field
 
-    return Option(**args)
+    return Gateway(**args)
 
 
-def unmarshal_ServerPrivateNetwork(data: Any) -> ServerPrivateNetwork:
+def unmarshal_PATRule(data: Any) -> PATRule:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerPrivateNetwork' failed as data isn't a dictionary."
+            "Unmarshalling the type 'PATRule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("project_id", None)
-    args["project_id"] = field
+    field = data.get("gateway_id", None)
+    if field is not None:
+        args["gateway_id"] = field
+
+    field = data.get("public_port", None)
+    if field is not None:
+        args["public_port"] = field
+
+    field = data.get("private_ip", None)
+    if field is not None:
+        args["private_ip"] = field
+
+    field = data.get("private_port", None)
+    if field is not None:
+        args["private_port"] = field
+
+    field = data.get("protocol", None)
+    if field is not None:
+        args["protocol"] = field
 
-    field = data.get("server_id", None)
-    args["server_id"] = field
-
-    field = data.get("private_network_id", None)
-    args["private_network_id"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("vlan", None)
-    args["vlan"] = field
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return ServerPrivateNetwork(**args)
+    return PATRule(**args)
 
 
-def unmarshal_ServerInstall(data: Any) -> ServerInstall:
+def unmarshal_ListDHCPEntriesResponse(data: Any) -> ListDHCPEntriesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerInstall' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListDHCPEntriesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("os_id", None)
-    args["os_id"] = field
-
-    field = data.get("hostname", None)
-    args["hostname"] = field
-
-    field = data.get("ssh_key_ids", None)
-    args["ssh_key_ids"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("user", None)
-    args["user"] = field
-
-    field = data.get("service_user", None)
-    args["service_user"] = field
+    field = data.get("dhcp_entries", None)
+    if field is not None:
+        args["dhcp_entries"] = (
+            [unmarshal_DHCPEntry(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("service_url", None)
-    args["service_url"] = field
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return ServerInstall(**args)
+    return ListDHCPEntriesResponse(**args)
 
 
-def unmarshal_ServerOption(data: Any) -> ServerOption:
+def unmarshal_ListDHCPsResponse(data: Any) -> ListDHCPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerOption' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListDHCPsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("manageable", None)
-    args["manageable"] = field
+    field = data.get("dhcps", None)
+    if field is not None:
+        args["dhcps"] = (
+            [unmarshal_DHCP(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return ServerOption(**args)
+    return ListDHCPsResponse(**args)
 
 
-def unmarshal_ServerRescueServer(data: Any) -> ServerRescueServer:
+def unmarshal_ListGatewayNetworksResponse(data: Any) -> ListGatewayNetworksResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ServerRescueServer' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListGatewayNetworksResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("user", None)
-    args["user"] = field
+    field = data.get("gateway_networks", None)
+    if field is not None:
+        args["gateway_networks"] = (
+            [unmarshal_GatewayNetwork(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("password", None)
-    args["password"] = field
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return ServerRescueServer(**args)
+    return ListGatewayNetworksResponse(**args)
 
 
-def unmarshal_Server(data: Any) -> Server:
+def unmarshal_ListGatewayTypesResponse(data: Any) -> ListGatewayTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Server' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListGatewayTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("organization_id", None)
-    args["organization_id"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("description", None)
-    args["description"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("offer_id", None)
-    args["offer_id"] = field
-
-    field = data.get("offer_name", None)
-    args["offer_name"] = field
-
-    field = data.get("tags", None)
-    args["tags"] = field
-
-    field = data.get("ips", None)
-    args["ips"] = [unmarshal_IP(v) for v in field] if field is not None else None
+    field = data.get("types", None)
+    if field is not None:
+        args["types"] = (
+            [unmarshal_GatewayType(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("domain", None)
-    args["domain"] = field
+    return ListGatewayTypesResponse(**args)
 
-    field = data.get("boot_type", None)
-    args["boot_type"] = field
 
-    field = data.get("zone", None)
-    args["zone"] = field
-
-    field = data.get("ping_status", None)
-    args["ping_status"] = field
+def unmarshal_ListGatewaysResponse(data: Any) -> ListGatewaysResponse:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ListGatewaysResponse' failed as data isn't a dictionary."
+        )
 
-    field = data.get("options", None)
-    args["options"] = (
-        [unmarshal_ServerOption(v) for v in field] if field is not None else None
-    )
+    args: Dict[str, Any] = {}
 
-    field = data.get("install", None)
-    args["install"] = unmarshal_ServerInstall(field)
+    field = data.get("gateways", None)
+    if field is not None:
+        args["gateways"] = (
+            [unmarshal_Gateway(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("rescue_server", None)
-    args["rescue_server"] = unmarshal_ServerRescueServer(field)
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return Server(**args)
+    return ListGatewaysResponse(**args)
 
 
-def unmarshal_Setting(data: Any) -> Setting:
+def unmarshal_ListIPsResponse(data: Any) -> ListIPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Setting' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListIPsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("type_", None)
-    args["type_"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
+    field = data.get("ips", None)
+    if field is not None:
+        args["ips"] = [unmarshal_IP(v) for v in field] if field is not None else None
 
-    field = data.get("enabled", None)
-    args["enabled"] = field
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return Setting(**args)
+    return ListIPsResponse(**args)
 
 
-def unmarshal_BMCAccess(data: Any) -> BMCAccess:
+def unmarshal_ListPATRulesResponse(data: Any) -> ListPATRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'BMCAccess' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListPATRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("url", None)
-    args["url"] = field
-
-    field = data.get("login", None)
-    args["login"] = field
-
-    field = data.get("password", None)
-    args["password"] = field
+    field = data.get("pat_rules", None)
+    if field is not None:
+        args["pat_rules"] = (
+            [unmarshal_PATRule(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return BMCAccess(**args)
+    return ListPATRulesResponse(**args)
 
 
-def unmarshal_GetServerMetricsResponse(data: Any) -> GetServerMetricsResponse:
+def unmarshal_SetDHCPEntriesResponse(data: Any) -> SetDHCPEntriesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'GetServerMetricsResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'SetDHCPEntriesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("pings", None)
-    args["pings"] = unmarshal_TimeSeries(field)
+    field = data.get("dhcp_entries", None)
+    if field is not None:
+        args["dhcp_entries"] = (
+            [unmarshal_DHCPEntry(v) for v in field] if field is not None else None
+        )
 
-    return GetServerMetricsResponse(**args)
+    return SetDHCPEntriesResponse(**args)
 
 
-def unmarshal_ListOSResponse(data: Any) -> ListOSResponse:
+def unmarshal_SetPATRulesResponse(data: Any) -> SetPATRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListOSResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'SetPATRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
-
-    field = data.get("os", None)
-    args["os"] = [unmarshal_OS(v) for v in field] if field is not None else None
+    field = data.get("pat_rules", None)
+    if field is not None:
+        args["pat_rules"] = (
+            [unmarshal_PATRule(v) for v in field] if field is not None else None
+        )
 
-    return ListOSResponse(**args)
+    return SetPATRulesResponse(**args)
 
 
-def unmarshal_ListOffersResponse(data: Any) -> ListOffersResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListOffersResponse' failed as data isn't a dictionary."
-        )
+def marshal_CreateDHCPRequest(
+    request: CreateDHCPRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-    args: Dict[str, Any] = {}
+    if request.subnet is not None:
+        output["subnet"] = request.subnet
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
 
-    field = data.get("offers", None)
-    args["offers"] = [unmarshal_Offer(v) for v in field] if field is not None else None
+    if request.address is not None:
+        output["address"] = request.address
 
-    return ListOffersResponse(**args)
+    if request.pool_low is not None:
+        output["pool_low"] = request.pool_low
 
+    if request.pool_high is not None:
+        output["pool_high"] = request.pool_high
 
-def unmarshal_ListOptionsResponse(data: Any) -> ListOptionsResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListOptionsResponse' failed as data isn't a dictionary."
-        )
+    if request.enable_dynamic is not None:
+        output["enable_dynamic"] = request.enable_dynamic
 
-    args: Dict[str, Any] = {}
+    if request.valid_lifetime is not None:
+        output["valid_lifetime"] = request.valid_lifetime
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    if request.renew_timer is not None:
+        output["renew_timer"] = request.renew_timer
 
-    field = data.get("options", None)
-    args["options"] = (
-        [unmarshal_Option(v) for v in field] if field is not None else None
-    )
+    if request.rebind_timer is not None:
+        output["rebind_timer"] = request.rebind_timer
 
-    return ListOptionsResponse(**args)
+    if request.push_default_route is not None:
+        output["push_default_route"] = request.push_default_route
 
+    if request.push_dns_server is not None:
+        output["push_dns_server"] = request.push_dns_server
 
-def unmarshal_ServerEvent(data: Any) -> ServerEvent:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ServerEvent' failed as data isn't a dictionary."
-        )
+    if request.dns_servers_override is not None:
+        output["dns_servers_override"] = request.dns_servers_override
 
-    args: Dict[str, Any] = {}
+    if request.dns_search is not None:
+        output["dns_search"] = request.dns_search
 
-    field = data.get("id", None)
-    args["id"] = field
+    if request.dns_local_name is not None:
+        output["dns_local_name"] = request.dns_local_name
 
-    field = data.get("action", None)
-    args["action"] = field
+    return output
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+def marshal_CreateDHCPEntryRequest(
+    request: CreateDHCPEntryRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-    return ServerEvent(**args)
+    if request.gateway_network_id is not None:
+        output["gateway_network_id"] = request.gateway_network_id
 
+    if request.mac_address is not None:
+        output["mac_address"] = request.mac_address
 
-def unmarshal_ListServerEventsResponse(data: Any) -> ListServerEventsResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListServerEventsResponse' failed as data isn't a dictionary."
-        )
+    if request.ip_address is not None:
+        output["ip_address"] = request.ip_address
 
-    args: Dict[str, Any] = {}
+    return output
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
 
-    field = data.get("events", None)
-    args["events"] = (
-        [unmarshal_ServerEvent(v) for v in field] if field is not None else None
-    )
+def marshal_CreateGatewayNetworkRequestIpamConfig(
+    request: CreateGatewayNetworkRequestIpamConfig,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-    return ListServerEventsResponse(**args)
+    if request.push_default_route is not None:
+        output["push_default_route"] = request.push_default_route
 
+    if request.ipam_ip_id is not None:
+        output["ipam_ip_id"] = request.ipam_ip_id
 
-def unmarshal_ListServerPrivateNetworksResponse(
-    data: Any,
-) -> ListServerPrivateNetworksResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListServerPrivateNetworksResponse' failed as data isn't a dictionary."
-        )
+    return output
 
-    args: Dict[str, Any] = {}
 
-    field = data.get("server_private_networks", None)
-    args["server_private_networks"] = (
-        [unmarshal_ServerPrivateNetwork(v) for v in field]
-        if field is not None
-        else None
+def marshal_CreateGatewayNetworkRequest(
+    request: CreateGatewayNetworkRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
+    output.update(
+        resolve_one_of(
+            [
+                OneOfPossibility("dhcp_id", request.dhcp_id),
+                OneOfPossibility("dhcp", request.dhcp),
+                OneOfPossibility("address", request.address),
+                OneOfPossibility("ipam_config", request.ipam_config),
+            ]
+        ),
     )
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
-
-    return ListServerPrivateNetworksResponse(**args)
+    if request.gateway_id is not None:
+        output["gateway_id"] = request.gateway_id
 
+    if request.private_network_id is not None:
+        output["private_network_id"] = request.private_network_id
 
-def unmarshal_ListServersResponse(data: Any) -> ListServersResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListServersResponse' failed as data isn't a dictionary."
-        )
-
-    args: Dict[str, Any] = {}
+    if request.enable_masquerade is not None:
+        output["enable_masquerade"] = request.enable_masquerade
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    if request.enable_dhcp is not None:
+        output["enable_dhcp"] = request.enable_dhcp
 
-    field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_Server(v) for v in field] if field is not None else None
-    )
+    return output
 
-    return ListServersResponse(**args)
 
+def marshal_CreateGatewayRequest(
+    request: CreateGatewayRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-def unmarshal_ListSettingsResponse(data: Any) -> ListSettingsResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListSettingsResponse' failed as data isn't a dictionary."
-        )
+    if request.type_ is not None:
+        output["type"] = request.type_
 
-    args: Dict[str, Any] = {}
+    if request.enable_smtp is not None:
+        output["enable_smtp"] = request.enable_smtp
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    if request.enable_bastion is not None:
+        output["enable_bastion"] = request.enable_bastion
 
-    field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_Setting(v) for v in field] if field is not None else None
-    )
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
 
-    return ListSettingsResponse(**args)
+    if request.name is not None:
+        output["name"] = request.name
 
+    if request.tags is not None:
+        output["tags"] = request.tags
 
-def unmarshal_SetServerPrivateNetworksResponse(
-    data: Any,
-) -> SetServerPrivateNetworksResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'SetServerPrivateNetworksResponse' failed as data isn't a dictionary."
-        )
+    if request.upstream_dns_servers is not None:
+        output["upstream_dns_servers"] = request.upstream_dns_servers
 
-    args: Dict[str, Any] = {}
+    if request.ip_id is not None:
+        output["ip_id"] = request.ip_id
 
-    field = data.get("server_private_networks", None)
-    args["server_private_networks"] = (
-        [unmarshal_ServerPrivateNetwork(v) for v in field]
-        if field is not None
-        else None
-    )
+    if request.bastion_port is not None:
+        output["bastion_port"] = request.bastion_port
 
-    return SetServerPrivateNetworksResponse(**args)
+    return output
 
 
-def marshal_AddOptionServerRequest(
-    request: AddOptionServerRequest,
+def marshal_CreateIPRequest(
+    request: CreateIPRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.expires_at is not None:
-        output["expires_at"] = request.expires_at
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
+
+    if request.tags is not None:
+        output["tags"] = request.tags
 
     return output
 
 
-def marshal_CreateServerRequestInstall(
-    request: CreateServerRequestInstall,
+def marshal_CreatePATRuleRequest(
+    request: CreatePATRuleRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.os_id is not None:
-        output["os_id"] = request.os_id
-
-    if request.hostname is not None:
-        output["hostname"] = request.hostname
-
-    if request.ssh_key_ids is not None:
-        output["ssh_key_ids"] = request.ssh_key_ids
+    if request.gateway_id is not None:
+        output["gateway_id"] = request.gateway_id
 
-    if request.user is not None:
-        output["user"] = request.user
+    if request.public_port is not None:
+        output["public_port"] = request.public_port
 
-    if request.password is not None:
-        output["password"] = request.password
+    if request.private_ip is not None:
+        output["private_ip"] = request.private_ip
 
-    if request.service_user is not None:
-        output["service_user"] = request.service_user
+    if request.private_port is not None:
+        output["private_port"] = request.private_port
 
-    if request.service_password is not None:
-        output["service_password"] = request.service_password
+    if request.protocol is not None:
+        output["protocol"] = str(request.protocol)
 
     return output
 
 
-def marshal_CreateServerRequest(
-    request: CreateServerRequest,
+def marshal_SetDHCPEntriesRequestEntry(
+    request: SetDHCPEntriesRequestEntry,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
-    output.update(
-        resolve_one_of(
-            [
-                OneOfPossibility(
-                    "project_id", request.project_id, defaults.default_project_id
-                ),
-                OneOfPossibility(
-                    "organization_id",
-                    request.organization_id,
-                    defaults.default_organization_id,
-                ),
-            ]
-        ),
-    )
 
-    if request.offer_id is not None:
-        output["offer_id"] = request.offer_id
+    if request.mac_address is not None:
+        output["mac_address"] = request.mac_address
 
-    if request.name is not None:
-        output["name"] = request.name
+    if request.ip_address is not None:
+        output["ip_address"] = request.ip_address
 
-    if request.description is not None:
-        output["description"] = request.description
+    return output
 
-    if request.tags is not None:
-        output["tags"] = request.tags
 
-    if request.install is not None:
-        output["install"] = (
-            marshal_CreateServerRequestInstall(request.install, defaults),
-        )
+def marshal_SetDHCPEntriesRequest(
+    request: SetDHCPEntriesRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
+
+    if request.gateway_network_id is not None:
+        output["gateway_network_id"] = request.gateway_network_id
 
-    if request.option_ids is not None:
-        output["option_ids"] = request.option_ids
+    if request.dhcp_entries is not None:
+        output["dhcp_entries"] = [
+            marshal_SetDHCPEntriesRequestEntry(item, defaults)
+            for item in request.dhcp_entries
+        ]
 
     return output
 
 
-def marshal_InstallServerRequest(
-    request: InstallServerRequest,
+def marshal_SetPATRulesRequestRule(
+    request: SetPATRulesRequestRule,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.os_id is not None:
-        output["os_id"] = request.os_id
+    if request.public_port is not None:
+        output["public_port"] = request.public_port
 
-    if request.hostname is not None:
-        output["hostname"] = request.hostname
+    if request.private_ip is not None:
+        output["private_ip"] = request.private_ip
 
-    if request.ssh_key_ids is not None:
-        output["ssh_key_ids"] = request.ssh_key_ids
+    if request.private_port is not None:
+        output["private_port"] = request.private_port
 
-    if request.user is not None:
-        output["user"] = request.user
-
-    if request.password is not None:
-        output["password"] = request.password
-
-    if request.service_user is not None:
-        output["service_user"] = request.service_user
-
-    if request.service_password is not None:
-        output["service_password"] = request.service_password
+    if request.protocol is not None:
+        output["protocol"] = str(request.protocol)
 
     return output
 
 
-def marshal_PrivateNetworkApiAddServerPrivateNetworkRequest(
-    request: PrivateNetworkApiAddServerPrivateNetworkRequest,
+def marshal_SetPATRulesRequest(
+    request: SetPATRulesRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.private_network_id is not None:
-        output["private_network_id"] = request.private_network_id
+    if request.gateway_id is not None:
+        output["gateway_id"] = request.gateway_id
+
+    if request.pat_rules is not None:
+        output["pat_rules"] = [
+            marshal_SetPATRulesRequestRule(item, defaults) for item in request.pat_rules
+        ]
 
     return output
 
 
-def marshal_PrivateNetworkApiSetServerPrivateNetworksRequest(
-    request: PrivateNetworkApiSetServerPrivateNetworksRequest,
+def marshal_UpdateDHCPEntryRequest(
+    request: UpdateDHCPEntryRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.private_network_ids is not None:
-        output["private_network_ids"] = request.private_network_ids
+    if request.ip_address is not None:
+        output["ip_address"] = request.ip_address
 
     return output
 
 
-def marshal_RebootServerRequest(
-    request: RebootServerRequest,
+def marshal_UpdateDHCPRequest(
+    request: UpdateDHCPRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.boot_type is not None:
-        output["boot_type"] = str(request.boot_type)
+    if request.subnet is not None:
+        output["subnet"] = request.subnet
 
-    return output
+    if request.address is not None:
+        output["address"] = request.address
 
+    if request.pool_low is not None:
+        output["pool_low"] = request.pool_low
 
-def marshal_StartBMCAccessRequest(
-    request: StartBMCAccessRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
+    if request.pool_high is not None:
+        output["pool_high"] = request.pool_high
 
-    if request.ip is not None:
-        output["ip"] = request.ip
+    if request.enable_dynamic is not None:
+        output["enable_dynamic"] = request.enable_dynamic
+
+    if request.valid_lifetime is not None:
+        output["valid_lifetime"] = request.valid_lifetime
+
+    if request.renew_timer is not None:
+        output["renew_timer"] = request.renew_timer
+
+    if request.rebind_timer is not None:
+        output["rebind_timer"] = request.rebind_timer
+
+    if request.push_default_route is not None:
+        output["push_default_route"] = request.push_default_route
+
+    if request.push_dns_server is not None:
+        output["push_dns_server"] = request.push_dns_server
+
+    if request.dns_servers_override is not None:
+        output["dns_servers_override"] = request.dns_servers_override
+
+    if request.dns_search is not None:
+        output["dns_search"] = request.dns_search
+
+    if request.dns_local_name is not None:
+        output["dns_local_name"] = request.dns_local_name
 
     return output
 
 
-def marshal_StartServerRequest(
-    request: StartServerRequest,
+def marshal_UpdateGatewayNetworkRequestIpamConfig(
+    request: UpdateGatewayNetworkRequestIpamConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.boot_type is not None:
-        output["boot_type"] = str(request.boot_type)
+    if request.push_default_route is not None:
+        output["push_default_route"] = request.push_default_route
+
+    if request.ipam_ip_id is not None:
+        output["ipam_ip_id"] = request.ipam_ip_id
 
     return output
 
 
-def marshal_UpdateIPRequest(
-    request: UpdateIPRequest,
+def marshal_UpdateGatewayNetworkRequest(
+    request: UpdateGatewayNetworkRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
+    output.update(
+        resolve_one_of(
+            [
+                OneOfPossibility("dhcp_id", request.dhcp_id),
+                OneOfPossibility("address", request.address),
+                OneOfPossibility("ipam_config", request.ipam_config),
+            ]
+        ),
+    )
 
-    if request.reverse is not None:
-        output["reverse"] = request.reverse
+    if request.enable_masquerade is not None:
+        output["enable_masquerade"] = request.enable_masquerade
+
+    if request.enable_dhcp is not None:
+        output["enable_dhcp"] = request.enable_dhcp
 
     return output
 
 
-def marshal_UpdateServerRequest(
-    request: UpdateServerRequest,
+def marshal_UpdateGatewayRequest(
+    request: UpdateGatewayRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
 
-    if request.description is not None:
-        output["description"] = request.description
+    if request.tags is not None:
+        output["tags"] = request.tags
+
+    if request.upstream_dns_servers is not None:
+        output["upstream_dns_servers"] = request.upstream_dns_servers
+
+    if request.enable_bastion is not None:
+        output["enable_bastion"] = request.enable_bastion
+
+    if request.bastion_port is not None:
+        output["bastion_port"] = request.bastion_port
+
+    if request.enable_smtp is not None:
+        output["enable_smtp"] = request.enable_smtp
+
+    return output
+
+
+def marshal_UpdateIPRequest(
+    request: UpdateIPRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
     if request.tags is not None:
         output["tags"] = request.tags
 
+    if request.reverse is not None:
+        output["reverse"] = request.reverse
+
+    if request.gateway_id is not None:
+        output["gateway_id"] = request.gateway_id
+
     return output
 
 
-def marshal_UpdateSettingRequest(
-    request: UpdateSettingRequest,
+def marshal_UpdatePATRuleRequest(
+    request: UpdatePATRuleRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.enabled is not None:
-        output["enabled"] = request.enabled
+    if request.public_port is not None:
+        output["public_port"] = request.public_port
+
+    if request.private_ip is not None:
+        output["private_ip"] = request.private_ip
+
+    if request.private_port is not None:
+        output["private_port"] = request.private_port
+
+    if request.protocol is not None:
+        output["protocol"] = str(request.protocol)
 
     return output
```

### Comparing `scaleway-2.0.0.dev5/scaleway/baremetal/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/baremetal/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/applesilicon/v1alpha1/marshalling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,291 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 
 from typing import Any, Dict
 from dateutil import parser
 
-from scaleway_core.bridge import (
-    unmarshal_Money,
-)
+from scaleway_core.profile import ProfileDefaults
 from .types import (
-    GetConsumptionResponseConsumption,
-    GetConsumptionResponse,
-    DiscountCoupon,
-    DiscountFilter,
-    Discount,
-    ListDiscountsResponse,
-    Invoice,
-    ListInvoicesResponse,
+    OS,
+    ServerTypeCPU,
+    ServerTypeDisk,
+    ServerTypeMemory,
+    ServerType,
+    Server,
+    ListOSResponse,
+    ListServerTypesResponse,
+    ListServersResponse,
+    CreateServerRequest,
+    UpdateServerRequest,
 )
 
 
-def unmarshal_GetConsumptionResponseConsumption(
-    data: Any,
-) -> GetConsumptionResponseConsumption:
+def unmarshal_OS(data: Any) -> OS:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'GetConsumptionResponseConsumption' failed as data isn't a dictionary."
+            "Unmarshalling the type 'OS' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("description", None)
-    args["description"] = field
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("project_id", None)
-    args["project_id"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("category", None)
-    args["category"] = field
+    field = data.get("label", None)
+    if field is not None:
+        args["label"] = field
 
-    field = data.get("operation_path", None)
-    args["operation_path"] = field
+    field = data.get("image_url", None)
+    if field is not None:
+        args["image_url"] = field
 
-    field = data.get("value", None)
-    args["value"] = unmarshal_Money(field)
+    field = data.get("compatible_server_types", None)
+    if field is not None:
+        args["compatible_server_types"] = field
 
-    return GetConsumptionResponseConsumption(**args)
+    return OS(**args)
 
 
-def unmarshal_GetConsumptionResponse(data: Any) -> GetConsumptionResponse:
+def unmarshal_ServerTypeCPU(data: Any) -> ServerTypeCPU:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'GetConsumptionResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ServerTypeCPU' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("consumptions", None)
-    args["consumptions"] = (
-        [unmarshal_GetConsumptionResponseConsumption(v) for v in field]
-        if field is not None
-        else None
-    )
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("core_count", None)
+    if field is not None:
+        args["core_count"] = field
 
-    return GetConsumptionResponse(**args)
+    return ServerTypeCPU(**args)
 
 
-def unmarshal_DiscountCoupon(data: Any) -> DiscountCoupon:
+def unmarshal_ServerTypeDisk(data: Any) -> ServerTypeDisk:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'DiscountCoupon' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ServerTypeDisk' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("description", None)
-    args["description"] = field
+    field = data.get("capacity", None)
+    if field is not None:
+        args["capacity"] = field
+
+    field = data.get("type_", None)
+    if field is not None:
+        args["type_"] = field
 
-    return DiscountCoupon(**args)
+    return ServerTypeDisk(**args)
 
 
-def unmarshal_DiscountFilter(data: Any) -> DiscountFilter:
+def unmarshal_ServerTypeMemory(data: Any) -> ServerTypeMemory:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'DiscountFilter' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ServerTypeMemory' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("type_", None)
-    args["type_"] = field
+    field = data.get("capacity", None)
+    if field is not None:
+        args["capacity"] = field
 
-    field = data.get("value", None)
-    args["value"] = field
+    field = data.get("type_", None)
+    if field is not None:
+        args["type_"] = field
 
-    return DiscountFilter(**args)
+    return ServerTypeMemory(**args)
 
 
-def unmarshal_Discount(data: Any) -> Discount:
+def unmarshal_ServerType(data: Any) -> ServerType:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Discount' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ServerType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("organization_id", None)
-    args["organization_id"] = field
+    field = data.get("stock", None)
+    if field is not None:
+        args["stock"] = field
+
+    field = data.get("cpu", None)
+    if field is not None:
+        args["cpu"] = unmarshal_ServerTypeCPU(field)
 
-    field = data.get("description", None)
-    args["description"] = field
+    field = data.get("disk", None)
+    if field is not None:
+        args["disk"] = unmarshal_ServerTypeDisk(field)
 
-    field = data.get("value", None)
-    args["value"] = field
+    field = data.get("memory", None)
+    if field is not None:
+        args["memory"] = unmarshal_ServerTypeMemory(field)
 
-    field = data.get("value_used", None)
-    args["value_used"] = field
+    field = data.get("minimum_lease_duration", None)
+    if field is not None:
+        args["minimum_lease_duration"] = field
+
+    return ServerType(**args)
+
+
+def unmarshal_Server(data: Any) -> Server:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'Server' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("value_remaining", None)
-    args["value_remaining"] = field
+    field = data.get("type_", None)
+    if field is not None:
+        args["type_"] = field
 
-    field = data.get("mode", None)
-    args["mode"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("filters", None)
-    args["filters"] = (
-        [unmarshal_DiscountFilter(v) for v in field] if field is not None else None
-    )
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
-    field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("organization_id", None)
+    if field is not None:
+        args["organization_id"] = field
 
-    field = data.get("start_date", None)
-    args["start_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("ip", None)
+    if field is not None:
+        args["ip"] = field
+
+    field = data.get("vnc_url", None)
+    if field is not None:
+        args["vnc_url"] = field
+
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
+
+    field = data.get("zone", None)
+    if field is not None:
+        args["zone"] = field
+
+    field = data.get("created_at", None)
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("stop_date", None)
-    args["stop_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("updated_at", None)
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("coupon", None)
-    args["coupon"] = unmarshal_DiscountCoupon(field)
+    field = data.get("deletable_at", None)
+    if field is not None:
+        args["deletable_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
-    return Discount(**args)
+    return Server(**args)
 
 
-def unmarshal_ListDiscountsResponse(data: Any) -> ListDiscountsResponse:
+def unmarshal_ListOSResponse(data: Any) -> ListOSResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListDiscountsResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListOSResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    field = data.get("discounts", None)
-    args["discounts"] = (
-        [unmarshal_Discount(v) for v in field] if field is not None else None
-    )
+    field = data.get("os", None)
+    if field is not None:
+        args["os"] = [unmarshal_OS(v) for v in field] if field is not None else None
 
-    return ListDiscountsResponse(**args)
+    return ListOSResponse(**args)
 
 
-def unmarshal_Invoice(data: Any) -> Invoice:
+def unmarshal_ListServerTypesResponse(data: Any) -> ListServerTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Invoice' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListServerTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
+    field = data.get("server_types", None)
+    if field is not None:
+        args["server_types"] = (
+            [unmarshal_ServerType(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("invoice_type", None)
-    args["invoice_type"] = field
+    return ListServerTypesResponse(**args)
 
-    field = data.get("number", None)
-    args["number"] = field
 
-    field = data.get("start_date", None)
-    args["start_date"] = parser.isoparse(field) if isinstance(field, str) else field
+def unmarshal_ListServersResponse(data: Any) -> ListServersResponse:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ListServersResponse' failed as data isn't a dictionary."
+        )
 
-    field = data.get("issued_date", None)
-    args["issued_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    args: Dict[str, Any] = {}
 
-    field = data.get("due_date", None)
-    args["due_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    field = data.get("total_untaxed", None)
-    args["total_untaxed"] = unmarshal_Money(field)
+    field = data.get("servers", None)
+    if field is not None:
+        args["servers"] = (
+            [unmarshal_Server(v) for v in field] if field is not None else None
+        )
 
-    field = data.get("total_taxed", None)
-    args["total_taxed"] = unmarshal_Money(field)
+    return ListServersResponse(**args)
 
-    return Invoice(**args)
 
+def marshal_CreateServerRequest(
+    request: CreateServerRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-def unmarshal_ListInvoicesResponse(data: Any) -> ListInvoicesResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListInvoicesResponse' failed as data isn't a dictionary."
-        )
+    if request.type_ is not None:
+        output["type"] = request.type_
 
-    args: Dict[str, Any] = {}
+    if request.name is not None:
+        output["name"] = request.name
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
+
+    return output
+
+
+def marshal_UpdateServerRequest(
+    request: UpdateServerRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-    field = data.get("invoices", None)
-    args["invoices"] = (
-        [unmarshal_Invoice(v) for v in field] if field is not None else None
-    )
+    if request.name is not None:
+        output["name"] = request.name
 
-    return ListInvoicesResponse(**args)
+    return output
```

### Comparing `scaleway-2.0.0.dev5/scaleway/billing/v2alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/billing/v2alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/block/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/block/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/block/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/block/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/block/v1alpha1/content.py` & `scaleway-2.0.0.dev6/scaleway/block/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/block/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/block/v1alpha1/marshalling.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,300 +38,359 @@
         raise TypeError(
             "Unmarshalling the type 'Reference' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("product_resource_type", None)
-    args["product_resource_type"] = field
+    if field is not None:
+        args["product_resource_type"] = field
 
     field = data.get("product_resource_id", None)
-    args["product_resource_id"] = field
+    if field is not None:
+        args["product_resource_id"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Reference(**args)
 
 
 def unmarshal_VolumeSpecifications(data: Any) -> VolumeSpecifications:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeSpecifications' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("class_", None)
-    args["class_"] = field
+    if field is not None:
+        args["class_"] = field
 
     field = data.get("perf_iops", None)
-    args["perf_iops"] = field
+    if field is not None:
+        args["perf_iops"] = field
 
     return VolumeSpecifications(**args)
 
 
 def unmarshal_Volume(data: Any) -> Volume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Volume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("references", None)
-    args["references"] = (
-        [unmarshal_Reference(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["references"] = (
+            [unmarshal_Reference(v) for v in field] if field is not None else None
+        )
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("parent_snapshot_id", None)
-    args["parent_snapshot_id"] = field
+    if field is not None:
+        args["parent_snapshot_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("specs", None)
-    args["specs"] = unmarshal_VolumeSpecifications(field)
+    if field is not None:
+        args["specs"] = unmarshal_VolumeSpecifications(field)
 
     field = data.get("last_detached_at", None)
-    args["last_detached_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["last_detached_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return Volume(**args)
 
 
 def unmarshal_SnapshotParentVolume(data: Any) -> SnapshotParentVolume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SnapshotParentVolume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     return SnapshotParentVolume(**args)
 
 
 def unmarshal_SnapshotSummary(data: Any) -> SnapshotSummary:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SnapshotSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("class_", None)
-    args["class_"] = field
+    if field is not None:
+        args["class_"] = field
 
     field = data.get("parent_volume", None)
-    args["parent_volume"] = unmarshal_SnapshotParentVolume(field)
+    if field is not None:
+        args["parent_volume"] = unmarshal_SnapshotParentVolume(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return SnapshotSummary(**args)
 
 
 def unmarshal_ListSnapshotsResponse(data: Any) -> ListSnapshotsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSnapshotsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshots", None)
-    args["snapshots"] = (
-        [unmarshal_SnapshotSummary(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["snapshots"] = (
+            [unmarshal_SnapshotSummary(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSnapshotsResponse(**args)
 
 
 def unmarshal_VolumeType(data: Any) -> VolumeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("pricing", None)
-    args["pricing"] = unmarshal_Money(field)
+    if field is not None:
+        args["pricing"] = unmarshal_Money(field)
 
     field = data.get("snapshot_pricing", None)
-    args["snapshot_pricing"] = unmarshal_Money(field)
+    if field is not None:
+        args["snapshot_pricing"] = unmarshal_Money(field)
 
     field = data.get("specs", None)
-    args["specs"] = unmarshal_VolumeSpecifications(field)
+    if field is not None:
+        args["specs"] = unmarshal_VolumeSpecifications(field)
 
     return VolumeType(**args)
 
 
 def unmarshal_ListVolumeTypesResponse(data: Any) -> ListVolumeTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVolumeTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volume_types", None)
-    args["volume_types"] = (
-        [unmarshal_VolumeType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["volume_types"] = (
+            [unmarshal_VolumeType(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListVolumeTypesResponse(**args)
 
 
 def unmarshal_ListVolumesResponse(data: Any) -> ListVolumesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVolumesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volumes", None)
-    args["volumes"] = (
-        [unmarshal_Volume(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["volumes"] = (
+            [unmarshal_Volume(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListVolumesResponse(**args)
 
 
 def unmarshal_Snapshot(data: Any) -> Snapshot:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Snapshot' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("references", None)
-    args["references"] = (
-        [unmarshal_Reference(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["references"] = (
+            [unmarshal_Reference(v) for v in field] if field is not None else None
+        )
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("class_", None)
-    args["class_"] = field
+    if field is not None:
+        args["class_"] = field
 
     field = data.get("parent_volume", None)
-    args["parent_volume"] = unmarshal_SnapshotParentVolume(field)
+    if field is not None:
+        args["parent_volume"] = unmarshal_SnapshotParentVolume(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Snapshot(**args)
 
 
 def marshal_CreateSnapshotRequest(
     request: CreateSnapshotRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/block/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/block/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/api.py` & `scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/marshalling.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,333 +52,394 @@
         raise TypeError(
             "Unmarshalling the type 'ContactPointEmail' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("to", None)
-    args["to"] = field
+    if field is not None:
+        args["to"] = field
 
     return ContactPointEmail(**args)
 
 
 def unmarshal_ContactPoint(data: Any) -> ContactPoint:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactPoint' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("email", None)
-    args["email"] = unmarshal_ContactPointEmail(field)
+    if field is not None:
+        args["email"] = unmarshal_ContactPointEmail(field)
 
     return ContactPoint(**args)
 
 
 def unmarshal_Datasource(data: Any) -> Datasource:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Datasource' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("is_managed_by_scaleway", None)
-    args["is_managed_by_scaleway"] = field
+    if field is not None:
+        args["is_managed_by_scaleway"] = field
 
     return Datasource(**args)
 
 
 def unmarshal_GrafanaProductDashboard(data: Any) -> GrafanaProductDashboard:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GrafanaProductDashboard' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("dashboard_name", None)
-    args["dashboard_name"] = field
+    if field is not None:
+        args["dashboard_name"] = field
 
     field = data.get("title", None)
-    args["title"] = field
+    if field is not None:
+        args["title"] = field
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("variables", None)
-    args["variables"] = field
+    if field is not None:
+        args["variables"] = field
 
     return GrafanaProductDashboard(**args)
 
 
 def unmarshal_GrafanaUser(data: Any) -> GrafanaUser:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GrafanaUser' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("login", None)
-    args["login"] = field
+    if field is not None:
+        args["login"] = field
 
     field = data.get("role", None)
-    args["role"] = field
+    if field is not None:
+        args["role"] = field
 
     field = data.get("password", None)
-    args["password"] = field
+    if field is not None:
+        args["password"] = field
 
     return GrafanaUser(**args)
 
 
 def unmarshal_TokenScopes(data: Any) -> TokenScopes:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'TokenScopes' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("query_metrics", None)
-    args["query_metrics"] = field
+    if field is not None:
+        args["query_metrics"] = field
 
     field = data.get("write_metrics", None)
-    args["write_metrics"] = field
+    if field is not None:
+        args["write_metrics"] = field
 
     field = data.get("setup_metrics_rules", None)
-    args["setup_metrics_rules"] = field
+    if field is not None:
+        args["setup_metrics_rules"] = field
 
     field = data.get("query_logs", None)
-    args["query_logs"] = field
+    if field is not None:
+        args["query_logs"] = field
 
     field = data.get("write_logs", None)
-    args["write_logs"] = field
+    if field is not None:
+        args["write_logs"] = field
 
     field = data.get("setup_logs_rules", None)
-    args["setup_logs_rules"] = field
+    if field is not None:
+        args["setup_logs_rules"] = field
 
     field = data.get("setup_alerts", None)
-    args["setup_alerts"] = field
+    if field is not None:
+        args["setup_alerts"] = field
 
     field = data.get("query_traces", None)
-    args["query_traces"] = field
+    if field is not None:
+        args["query_traces"] = field
 
     field = data.get("write_traces", None)
-    args["write_traces"] = field
+    if field is not None:
+        args["write_traces"] = field
 
     return TokenScopes(**args)
 
 
 def unmarshal_Token(data: Any) -> Token:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Token' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("scopes", None)
-    args["scopes"] = unmarshal_TokenScopes(field)
+    if field is not None:
+        args["scopes"] = unmarshal_TokenScopes(field)
 
     field = data.get("secret_key", None)
-    args["secret_key"] = field
+    if field is not None:
+        args["secret_key"] = field
 
     return Token(**args)
 
 
 def unmarshal_CockpitEndpoints(data: Any) -> CockpitEndpoints:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CockpitEndpoints' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("metrics_url", None)
-    args["metrics_url"] = field
+    if field is not None:
+        args["metrics_url"] = field
 
     field = data.get("logs_url", None)
-    args["logs_url"] = field
+    if field is not None:
+        args["logs_url"] = field
 
     field = data.get("traces_url", None)
-    args["traces_url"] = field
+    if field is not None:
+        args["traces_url"] = field
 
     field = data.get("alertmanager_url", None)
-    args["alertmanager_url"] = field
+    if field is not None:
+        args["alertmanager_url"] = field
 
     field = data.get("grafana_url", None)
-    args["grafana_url"] = field
+    if field is not None:
+        args["grafana_url"] = field
 
     return CockpitEndpoints(**args)
 
 
 def unmarshal_Plan(data: Any) -> Plan:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Plan' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("sample_ingestion_price", None)
-    args["sample_ingestion_price"] = field
+    if field is not None:
+        args["sample_ingestion_price"] = field
 
     field = data.get("logs_ingestion_price", None)
-    args["logs_ingestion_price"] = field
+    if field is not None:
+        args["logs_ingestion_price"] = field
 
     field = data.get("traces_ingestion_price", None)
-    args["traces_ingestion_price"] = field
+    if field is not None:
+        args["traces_ingestion_price"] = field
 
     field = data.get("retention_price", None)
-    args["retention_price"] = field
+    if field is not None:
+        args["retention_price"] = field
 
     field = data.get("retention_metrics_interval", None)
-    args["retention_metrics_interval"] = field
+    if field is not None:
+        args["retention_metrics_interval"] = field
 
     field = data.get("retention_logs_interval", None)
-    args["retention_logs_interval"] = field
+    if field is not None:
+        args["retention_logs_interval"] = field
 
     field = data.get("retention_traces_interval", None)
-    args["retention_traces_interval"] = field
+    if field is not None:
+        args["retention_traces_interval"] = field
 
     return Plan(**args)
 
 
 def unmarshal_Cockpit(data: Any) -> Cockpit:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Cockpit' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("managed_alerts_enabled", None)
-    args["managed_alerts_enabled"] = field
+    if field is not None:
+        args["managed_alerts_enabled"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("endpoints", None)
-    args["endpoints"] = unmarshal_CockpitEndpoints(field)
+    if field is not None:
+        args["endpoints"] = unmarshal_CockpitEndpoints(field)
 
     field = data.get("plan", None)
-    args["plan"] = unmarshal_Plan(field)
+    if field is not None:
+        args["plan"] = unmarshal_Plan(field)
 
     return Cockpit(**args)
 
 
 def unmarshal_CockpitMetrics(data: Any) -> CockpitMetrics:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CockpitMetrics' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("timeseries", None)
-    args["timeseries"] = (
-        [unmarshal_TimeSeries(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["timeseries"] = (
+            [unmarshal_TimeSeries(v) for v in field] if field is not None else None
+        )
 
     return CockpitMetrics(**args)
 
 
 def unmarshal_ListContactPointsResponse(data: Any) -> ListContactPointsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListContactPointsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("contact_points", None)
-    args["contact_points"] = (
-        [unmarshal_ContactPoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["contact_points"] = (
+            [unmarshal_ContactPoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("has_additional_receivers", None)
-    args["has_additional_receivers"] = field
+    if field is not None:
+        args["has_additional_receivers"] = field
 
     field = data.get("has_additional_contact_points", None)
-    args["has_additional_contact_points"] = field
+    if field is not None:
+        args["has_additional_contact_points"] = field
 
     return ListContactPointsResponse(**args)
 
 
 def unmarshal_ListDatasourcesResponse(data: Any) -> ListDatasourcesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDatasourcesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("datasources", None)
-    args["datasources"] = (
-        [unmarshal_Datasource(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["datasources"] = (
+            [unmarshal_Datasource(v) for v in field] if field is not None else None
+        )
 
     return ListDatasourcesResponse(**args)
 
 
 def unmarshal_ListGrafanaProductDashboardsResponse(
     data: Any,
 ) -> ListGrafanaProductDashboardsResponse:
@@ -386,75 +447,87 @@
         raise TypeError(
             "Unmarshalling the type 'ListGrafanaProductDashboardsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("dashboards", None)
-    args["dashboards"] = (
-        [unmarshal_GrafanaProductDashboard(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["dashboards"] = (
+            [unmarshal_GrafanaProductDashboard(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return ListGrafanaProductDashboardsResponse(**args)
 
 
 def unmarshal_ListGrafanaUsersResponse(data: Any) -> ListGrafanaUsersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListGrafanaUsersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("grafana_users", None)
-    args["grafana_users"] = (
-        [unmarshal_GrafanaUser(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["grafana_users"] = (
+            [unmarshal_GrafanaUser(v) for v in field] if field is not None else None
+        )
 
     return ListGrafanaUsersResponse(**args)
 
 
 def unmarshal_ListPlansResponse(data: Any) -> ListPlansResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPlansResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("plans", None)
-    args["plans"] = [unmarshal_Plan(v) for v in field] if field is not None else None
+    if field is not None:
+        args["plans"] = (
+            [unmarshal_Plan(v) for v in field] if field is not None else None
+        )
 
     return ListPlansResponse(**args)
 
 
 def unmarshal_ListTokensResponse(data: Any) -> ListTokensResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTokensResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("tokens", None)
-    args["tokens"] = [unmarshal_Token(v) for v in field] if field is not None else None
+    if field is not None:
+        args["tokens"] = (
+            [unmarshal_Token(v) for v in field] if field is not None else None
+        )
 
     return ListTokensResponse(**args)
 
 
 def unmarshal_SelectPlanResponse(data: Any) -> SelectPlanResponse:
     if not isinstance(data, dict):
         raise TypeError(
```

### Comparing `scaleway-2.0.0.dev5/scaleway/cockpit/v1beta1/types.py` & `scaleway-2.0.0.dev6/scaleway/cockpit/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/container/v1beta1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/container/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/container/v1beta1/api.py` & `scaleway-2.0.0.dev6/scaleway/container/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/container/v1beta1/content.py` & `scaleway-2.0.0.dev6/scaleway/container/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/container/v1beta1/types.py` & `scaleway-2.0.0.dev6/scaleway/container/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/api.py` & `scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/content.py` & `scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/marshalling.py`

 * *Files 18% similar despite different names*

```diff
@@ -116,491 +116,589 @@
         raise TypeError(
             "Unmarshalling the type 'EndpointPrivateNetworkDetails' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_network_id", None)
-    args["private_network_id"] = field
+    if field is not None:
+        args["private_network_id"] = field
 
     field = data.get("service_ip", None)
-    args["service_ip"] = field
+    if field is not None:
+        args["service_ip"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return EndpointPrivateNetworkDetails(**args)
 
 
 def unmarshal_Endpoint(data: Any) -> Endpoint:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Endpoint' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("private_network", None)
-    args["private_network"] = unmarshal_EndpointPrivateNetworkDetails(field)
+    if field is not None:
+        args["private_network"] = unmarshal_EndpointPrivateNetworkDetails(field)
 
     field = data.get("load_balancer", None)
-    args["load_balancer"] = unmarshal_EndpointLoadBalancerDetails(field)
+    if field is not None:
+        args["load_balancer"] = unmarshal_EndpointLoadBalancerDetails(field)
 
     field = data.get("direct_access", None)
-    args["direct_access"] = unmarshal_EndpointDirectAccessDetails(field)
+    if field is not None:
+        args["direct_access"] = unmarshal_EndpointDirectAccessDetails(field)
 
     field = data.get("hostname", None)
-    args["hostname"] = field
+    if field is not None:
+        args["hostname"] = field
 
     return Endpoint(**args)
 
 
 def unmarshal_ReadReplica(data: Any) -> ReadReplica:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ReadReplica' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("same_zone", None)
-    args["same_zone"] = field
+    if field is not None:
+        args["same_zone"] = field
 
     return ReadReplica(**args)
 
 
 def unmarshal_Database(data: Any) -> Database:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Database' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("owner", None)
-    args["owner"] = field
+    if field is not None:
+        args["owner"] = field
 
     field = data.get("managed", None)
-    args["managed"] = field
+    if field is not None:
+        args["managed"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     return Database(**args)
 
 
 def unmarshal_InstanceLog(data: Any) -> InstanceLog:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceLog' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("node_name", None)
-    args["node_name"] = field
+    if field is not None:
+        args["node_name"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("download_url", None)
-    args["download_url"] = field
+    if field is not None:
+        args["download_url"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return InstanceLog(**args)
 
 
 def unmarshal_BackupSchedule(data: Any) -> BackupSchedule:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'BackupSchedule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("frequency", None)
-    args["frequency"] = field
+    if field is not None:
+        args["frequency"] = field
 
     field = data.get("retention", None)
-    args["retention"] = field
+    if field is not None:
+        args["retention"] = field
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("next_run_at", None)
-    args["next_run_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["next_run_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return BackupSchedule(**args)
 
 
 def unmarshal_InstanceSetting(data: Any) -> InstanceSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("value", None)
-    args["value"] = field
+    if field is not None:
+        args["value"] = field
 
     return InstanceSetting(**args)
 
 
 def unmarshal_LogsPolicy(data: Any) -> LogsPolicy:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'LogsPolicy' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("max_age_retention", None)
-    args["max_age_retention"] = field
+    if field is not None:
+        args["max_age_retention"] = field
 
     field = data.get("total_disk_retention", None)
-    args["total_disk_retention"] = field
+    if field is not None:
+        args["total_disk_retention"] = field
 
     return LogsPolicy(**args)
 
 
 def unmarshal_Maintenance(data: Any) -> Maintenance:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Maintenance' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("reason", None)
-    args["reason"] = field
+    if field is not None:
+        args["reason"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("starts_at", None)
-    args["starts_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["starts_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("stops_at", None)
-    args["stops_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["stops_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("closed_at", None)
-    args["closed_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["closed_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Maintenance(**args)
 
 
 def unmarshal_UpgradableVersion(data: Any) -> UpgradableVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpgradableVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("minor_version", None)
-    args["minor_version"] = field
+    if field is not None:
+        args["minor_version"] = field
 
     return UpgradableVersion(**args)
 
 
 def unmarshal_Volume(data: Any) -> Volume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Volume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     return Volume(**args)
 
 
 def unmarshal_Instance(data: Any) -> Instance:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Instance' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("volume", None)
-    args["volume"] = unmarshal_Volume(field)
+    if field is not None:
+        args["volume"] = unmarshal_Volume(field)
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("engine", None)
-    args["engine"] = field
+    if field is not None:
+        args["engine"] = field
 
     field = data.get("upgradable_version", None)
-    args["upgradable_version"] = (
-        [unmarshal_UpgradableVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["upgradable_version"] = (
+            [unmarshal_UpgradableVersion(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("is_ha_cluster", None)
-    args["is_ha_cluster"] = field
+    if field is not None:
+        args["is_ha_cluster"] = field
 
     field = data.get("endpoint", None)
-    args["endpoint"] = unmarshal_Endpoint(field)
+    if field is not None:
+        args["endpoint"] = unmarshal_Endpoint(field)
 
     field = data.get("backup_schedule", None)
-    args["backup_schedule"] = unmarshal_BackupSchedule(field)
+    if field is not None:
+        args["backup_schedule"] = unmarshal_BackupSchedule(field)
 
     field = data.get("read_replicas", None)
-    args["read_replicas"] = (
-        [unmarshal_ReadReplica(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["read_replicas"] = (
+            [unmarshal_ReadReplica(v) for v in field] if field is not None else None
+        )
 
     field = data.get("node_type", None)
-    args["node_type"] = field
+    if field is not None:
+        args["node_type"] = field
 
     field = data.get("init_settings", None)
-    args["init_settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["init_settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("backup_same_region", None)
-    args["backup_same_region"] = field
+    if field is not None:
+        args["backup_same_region"] = field
 
     field = data.get("maintenances", None)
-    args["maintenances"] = (
-        [unmarshal_Maintenance(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["maintenances"] = (
+            [unmarshal_Maintenance(v) for v in field] if field is not None else None
+        )
 
     field = data.get("logs_policy", None)
-    args["logs_policy"] = unmarshal_LogsPolicy(field)
+    if field is not None:
+        args["logs_policy"] = unmarshal_LogsPolicy(field)
 
     return Instance(**args)
 
 
 def unmarshal_Privilege(data: Any) -> Privilege:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Privilege' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("permission", None)
-    args["permission"] = field
+    if field is not None:
+        args["permission"] = field
 
     field = data.get("database_name", None)
-    args["database_name"] = field
+    if field is not None:
+        args["database_name"] = field
 
     field = data.get("user_name", None)
-    args["user_name"] = field
+    if field is not None:
+        args["user_name"] = field
 
     return Privilege(**args)
 
 
 def unmarshal_Snapshot(data: Any) -> Snapshot:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Snapshot' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("instance_id", None)
-    args["instance_id"] = field
+    if field is not None:
+        args["instance_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("instance_name", None)
-    args["instance_name"] = field
+    if field is not None:
+        args["instance_name"] = field
 
     field = data.get("node_type", None)
-    args["node_type"] = field
+    if field is not None:
+        args["node_type"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Snapshot(**args)
 
 
 def unmarshal_User(data: Any) -> User:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'User' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("is_admin", None)
-    args["is_admin"] = field
+    if field is not None:
+        args["is_admin"] = field
 
     return User(**args)
 
 
 def unmarshal_ACLRule(data: Any) -> ACLRule:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ACLRule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("protocol", None)
-    args["protocol"] = field
+    if field is not None:
+        args["protocol"] = field
 
     field = data.get("direction", None)
-    args["direction"] = field
+    if field is not None:
+        args["direction"] = field
 
     field = data.get("action", None)
-    args["action"] = field
+    if field is not None:
+        args["action"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     return ACLRule(**args)
 
 
 def unmarshal_AddInstanceACLRulesResponse(data: Any) -> AddInstanceACLRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return AddInstanceACLRulesResponse(**args)
 
 
 def unmarshal_AddInstanceSettingsResponse(data: Any) -> AddInstanceSettingsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddInstanceSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     return AddInstanceSettingsResponse(**args)
 
 
 def unmarshal_DeleteInstanceACLRulesResponse(
     data: Any,
 ) -> DeleteInstanceACLRulesResponse:
@@ -608,15 +706,18 @@
         raise TypeError(
             "Unmarshalling the type 'DeleteInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return DeleteInstanceACLRulesResponse(**args)
 
 
 def unmarshal_DeleteInstanceSettingsResponse(
     data: Any,
 ) -> DeleteInstanceSettingsResponse:
@@ -624,193 +725,227 @@
         raise TypeError(
             "Unmarshalling the type 'DeleteInstanceSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     return DeleteInstanceSettingsResponse(**args)
 
 
 def unmarshal_InstanceMetrics(data: Any) -> InstanceMetrics:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceMetrics' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("timeseries", None)
-    args["timeseries"] = (
-        [unmarshal_TimeSeries(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["timeseries"] = (
+            [unmarshal_TimeSeries(v) for v in field] if field is not None else None
+        )
 
     return InstanceMetrics(**args)
 
 
 def unmarshal_EngineSetting(data: Any) -> EngineSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'EngineSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("default_value", None)
-    args["default_value"] = field
+    if field is not None:
+        args["default_value"] = field
 
     field = data.get("hot_configurable", None)
-    args["hot_configurable"] = field
+    if field is not None:
+        args["hot_configurable"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("property_type", None)
-    args["property_type"] = field
+    if field is not None:
+        args["property_type"] = field
 
     field = data.get("unit", None)
-    args["unit"] = field
+    if field is not None:
+        args["unit"] = field
 
     field = data.get("string_constraint", None)
-    args["string_constraint"] = field
+    if field is not None:
+        args["string_constraint"] = field
 
     field = data.get("int_min", None)
-    args["int_min"] = field
+    if field is not None:
+        args["int_min"] = field
 
     field = data.get("int_max", None)
-    args["int_max"] = field
+    if field is not None:
+        args["int_max"] = field
 
     field = data.get("float_min", None)
-    args["float_min"] = field
+    if field is not None:
+        args["float_min"] = field
 
     field = data.get("float_max", None)
-    args["float_max"] = field
+    if field is not None:
+        args["float_max"] = field
 
     return EngineSetting(**args)
 
 
 def unmarshal_EngineVersion(data: Any) -> EngineVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'EngineVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("available_settings", None)
-    args["available_settings"] = (
-        [unmarshal_EngineSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_settings"] = (
+            [unmarshal_EngineSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("beta", None)
-    args["beta"] = field
+    if field is not None:
+        args["beta"] = field
 
     field = data.get("available_init_settings", None)
-    args["available_init_settings"] = (
-        [unmarshal_EngineSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_init_settings"] = (
+            [unmarshal_EngineSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("end_of_life", None)
-    args["end_of_life"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["end_of_life"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return EngineVersion(**args)
 
 
 def unmarshal_DatabaseEngine(data: Any) -> DatabaseEngine:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DatabaseEngine' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("logo_url", None)
-    args["logo_url"] = field
+    if field is not None:
+        args["logo_url"] = field
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_EngineVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_EngineVersion(v) for v in field] if field is not None else None
+        )
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return DatabaseEngine(**args)
 
 
 def unmarshal_ListDatabaseEnginesResponse(data: Any) -> ListDatabaseEnginesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDatabaseEnginesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("engines", None)
-    args["engines"] = (
-        [unmarshal_DatabaseEngine(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["engines"] = (
+            [unmarshal_DatabaseEngine(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListDatabaseEnginesResponse(**args)
 
 
 def unmarshal_ListDatabasesResponse(data: Any) -> ListDatabasesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDatabasesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("databases", None)
-    args["databases"] = (
-        [unmarshal_Database(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["databases"] = (
+            [unmarshal_Database(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListDatabasesResponse(**args)
 
 
 def unmarshal_ListInstanceACLRulesResponse(data: Any) -> ListInstanceACLRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListInstanceACLRulesResponse(**args)
 
 
 def unmarshal_ListInstanceLogsDetailsResponseInstanceLogDetail(
     data: Any,
 ) -> ListInstanceLogsDetailsResponseInstanceLogDetail:
@@ -818,18 +953,20 @@
         raise TypeError(
             "Unmarshalling the type 'ListInstanceLogsDetailsResponseInstanceLogDetail' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("log_name", None)
-    args["log_name"] = field
+    if field is not None:
+        args["log_name"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     return ListInstanceLogsDetailsResponseInstanceLogDetail(**args)
 
 
 def unmarshal_ListInstanceLogsDetailsResponse(
     data: Any,
 ) -> ListInstanceLogsDetailsResponse:
@@ -837,256 +974,300 @@
         raise TypeError(
             "Unmarshalling the type 'ListInstanceLogsDetailsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("details", None)
-    args["details"] = (
-        [unmarshal_ListInstanceLogsDetailsResponseInstanceLogDetail(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["details"] = (
+            [
+                unmarshal_ListInstanceLogsDetailsResponseInstanceLogDetail(v)
+                for v in field
+            ]
+            if field is not None
+            else None
+        )
 
     return ListInstanceLogsDetailsResponse(**args)
 
 
 def unmarshal_ListInstanceLogsResponse(data: Any) -> ListInstanceLogsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListInstanceLogsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("instance_logs", None)
-    args["instance_logs"] = (
-        [unmarshal_InstanceLog(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["instance_logs"] = (
+            [unmarshal_InstanceLog(v) for v in field] if field is not None else None
+        )
 
     return ListInstanceLogsResponse(**args)
 
 
 def unmarshal_ListInstancesResponse(data: Any) -> ListInstancesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListInstancesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("instances", None)
-    args["instances"] = (
-        [unmarshal_Instance(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["instances"] = (
+            [unmarshal_Instance(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListInstancesResponse(**args)
 
 
 def unmarshal_NodeTypeVolumeConstraintSizes(data: Any) -> NodeTypeVolumeConstraintSizes:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeTypeVolumeConstraintSizes' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("min_size", None)
-    args["min_size"] = field
+    if field is not None:
+        args["min_size"] = field
 
     field = data.get("max_size", None)
-    args["max_size"] = field
+    if field is not None:
+        args["max_size"] = field
 
     return NodeTypeVolumeConstraintSizes(**args)
 
 
 def unmarshal_NodeTypeVolumeType(data: Any) -> NodeTypeVolumeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeTypeVolumeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("min_size", None)
-    args["min_size"] = field
+    if field is not None:
+        args["min_size"] = field
 
     field = data.get("max_size", None)
-    args["max_size"] = field
+    if field is not None:
+        args["max_size"] = field
 
     field = data.get("chunk_size", None)
-    args["chunk_size"] = field
+    if field is not None:
+        args["chunk_size"] = field
 
     return NodeTypeVolumeType(**args)
 
 
 def unmarshal_NodeType(data: Any) -> NodeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("stock_status", None)
-    args["stock_status"] = field
+    if field is not None:
+        args["stock_status"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("vcpus", None)
-    args["vcpus"] = field
+    if field is not None:
+        args["vcpus"] = field
 
     field = data.get("memory", None)
-    args["memory"] = field
+    if field is not None:
+        args["memory"] = field
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("beta", None)
-    args["beta"] = field
+    if field is not None:
+        args["beta"] = field
 
     field = data.get("volume_constraint", None)
-    args["volume_constraint"] = unmarshal_NodeTypeVolumeConstraintSizes(field)
+    if field is not None:
+        args["volume_constraint"] = unmarshal_NodeTypeVolumeConstraintSizes(field)
 
     field = data.get("is_bssd_compatible", None)
-    args["is_bssd_compatible"] = field
+    if field is not None:
+        args["is_bssd_compatible"] = field
 
     field = data.get("available_volume_types", None)
-    args["available_volume_types"] = (
-        [unmarshal_NodeTypeVolumeType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_volume_types"] = (
+            [unmarshal_NodeTypeVolumeType(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("is_ha_required", None)
-    args["is_ha_required"] = field
+    if field is not None:
+        args["is_ha_required"] = field
 
     field = data.get("generation", None)
-    args["generation"] = field
+    if field is not None:
+        args["generation"] = field
 
     field = data.get("instance_range", None)
-    args["instance_range"] = field
+    if field is not None:
+        args["instance_range"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return NodeType(**args)
 
 
 def unmarshal_ListNodeTypesResponse(data: Any) -> ListNodeTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNodeTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("node_types", None)
-    args["node_types"] = (
-        [unmarshal_NodeType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["node_types"] = (
+            [unmarshal_NodeType(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListNodeTypesResponse(**args)
 
 
 def unmarshal_ListPrivilegesResponse(data: Any) -> ListPrivilegesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPrivilegesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("privileges", None)
-    args["privileges"] = (
-        [unmarshal_Privilege(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["privileges"] = (
+            [unmarshal_Privilege(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPrivilegesResponse(**args)
 
 
 def unmarshal_ListSnapshotsResponse(data: Any) -> ListSnapshotsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSnapshotsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshots", None)
-    args["snapshots"] = (
-        [unmarshal_Snapshot(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["snapshots"] = (
+            [unmarshal_Snapshot(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSnapshotsResponse(**args)
 
 
 def unmarshal_ListUsersResponse(data: Any) -> ListUsersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListUsersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("users", None)
-    args["users"] = [unmarshal_User(v) for v in field] if field is not None else None
+    if field is not None:
+        args["users"] = (
+            [unmarshal_User(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListUsersResponse(**args)
 
 
 def unmarshal_SetInstanceACLRulesResponse(data: Any) -> SetInstanceACLRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return SetInstanceACLRulesResponse(**args)
 
 
 def unmarshal_SetInstanceSettingsResponse(data: Any) -> SetInstanceSettingsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetInstanceSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     return SetInstanceSettingsResponse(**args)
 
 
 def marshal_ACLRuleRequest(
     request: ACLRuleRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/document_db/v1beta1/types.py` & `scaleway-2.0.0.dev6/scaleway/document_db/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/domain/v2beta1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/domain/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/domain/v2beta1/api.py` & `scaleway-2.0.0.dev6/scaleway/domain/v2beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/domain/v2beta1/content.py` & `scaleway-2.0.0.dev6/scaleway/domain/v2beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/domain/v2beta1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/domain/v2beta1/marshalling.py`

 * *Files 13% similar despite different names*

```diff
@@ -125,18 +125,22 @@
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionFRAssociationInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("publication_jo_page", None)
-    args["publication_jo_page"] = field
+    if field is not None:
+        args["publication_jo_page"] = field
 
     field = data.get("publication_jo", None)
-    args["publication_jo"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["publication_jo"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return ContactExtensionFRAssociationInfo(**args)
 
 
 def unmarshal_ContactExtensionFRCodeAuthAfnicInfo(
     data: Any,
 ) -> ContactExtensionFRCodeAuthAfnicInfo:
@@ -144,32 +148,35 @@
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionFRCodeAuthAfnicInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("code_auth_afnic", None)
-    args["code_auth_afnic"] = field
+    if field is not None:
+        args["code_auth_afnic"] = field
 
     return ContactExtensionFRCodeAuthAfnicInfo(**args)
 
 
 def unmarshal_ContactExtensionFRDunsInfo(data: Any) -> ContactExtensionFRDunsInfo:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionFRDunsInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("duns_id", None)
-    args["duns_id"] = field
+    if field is not None:
+        args["duns_id"] = field
 
     field = data.get("local_id", None)
-    args["local_id"] = field
+    if field is not None:
+        args["local_id"] = field
 
     return ContactExtensionFRDunsInfo(**args)
 
 
 def unmarshal_ContactExtensionFRIndividualInfo(
     data: Any,
 ) -> ContactExtensionFRIndividualInfo:
@@ -177,15 +184,16 @@
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionFRIndividualInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("whois_opt_in", None)
-    args["whois_opt_in"] = field
+    if field is not None:
+        args["whois_opt_in"] = field
 
     return ContactExtensionFRIndividualInfo(**args)
 
 
 def unmarshal_ContactExtensionFRTrademarkInfo(
     data: Any,
 ) -> ContactExtensionFRTrademarkInfo:
@@ -193,278 +201,338 @@
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionFRTrademarkInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("trademark_inpi", None)
-    args["trademark_inpi"] = field
+    if field is not None:
+        args["trademark_inpi"] = field
 
     return ContactExtensionFRTrademarkInfo(**args)
 
 
 def unmarshal_ContactExtensionEU(data: Any) -> ContactExtensionEU:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionEU' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("european_citizenship", None)
-    args["european_citizenship"] = field
+    if field is not None:
+        args["european_citizenship"] = field
 
     return ContactExtensionEU(**args)
 
 
 def unmarshal_ContactExtensionFR(data: Any) -> ContactExtensionFR:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionFR' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("mode", None)
-    args["mode"] = field
+    if field is not None:
+        args["mode"] = field
 
     field = data.get("individual_info", None)
-    args["individual_info"] = unmarshal_ContactExtensionFRIndividualInfo(field)
+    if field is not None:
+        args["individual_info"] = unmarshal_ContactExtensionFRIndividualInfo(field)
 
     field = data.get("duns_info", None)
-    args["duns_info"] = unmarshal_ContactExtensionFRDunsInfo(field)
+    if field is not None:
+        args["duns_info"] = unmarshal_ContactExtensionFRDunsInfo(field)
 
     field = data.get("association_info", None)
-    args["association_info"] = unmarshal_ContactExtensionFRAssociationInfo(field)
+    if field is not None:
+        args["association_info"] = unmarshal_ContactExtensionFRAssociationInfo(field)
 
     field = data.get("trademark_info", None)
-    args["trademark_info"] = unmarshal_ContactExtensionFRTrademarkInfo(field)
+    if field is not None:
+        args["trademark_info"] = unmarshal_ContactExtensionFRTrademarkInfo(field)
 
     field = data.get("code_auth_afnic_info", None)
-    args["code_auth_afnic_info"] = unmarshal_ContactExtensionFRCodeAuthAfnicInfo(field)
+    if field is not None:
+        args["code_auth_afnic_info"] = unmarshal_ContactExtensionFRCodeAuthAfnicInfo(
+            field
+        )
 
     return ContactExtensionFR(**args)
 
 
 def unmarshal_ContactExtensionNL(data: Any) -> ContactExtensionNL:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactExtensionNL' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("legal_form", None)
-    args["legal_form"] = field
+    if field is not None:
+        args["legal_form"] = field
 
     field = data.get("legal_form_registration_number", None)
-    args["legal_form_registration_number"] = field
+    if field is not None:
+        args["legal_form_registration_number"] = field
 
     return ContactExtensionNL(**args)
 
 
 def unmarshal_ContactQuestion(data: Any) -> ContactQuestion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactQuestion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("question", None)
-    args["question"] = field
+    if field is not None:
+        args["question"] = field
 
     field = data.get("answer", None)
-    args["answer"] = field
+    if field is not None:
+        args["answer"] = field
 
     return ContactQuestion(**args)
 
 
 def unmarshal_Contact(data: Any) -> Contact:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Contact' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("legal_form", None)
-    args["legal_form"] = field
+    if field is not None:
+        args["legal_form"] = field
 
     field = data.get("firstname", None)
-    args["firstname"] = field
+    if field is not None:
+        args["firstname"] = field
 
     field = data.get("lastname", None)
-    args["lastname"] = field
+    if field is not None:
+        args["lastname"] = field
 
     field = data.get("company_name", None)
-    args["company_name"] = field
+    if field is not None:
+        args["company_name"] = field
 
     field = data.get("email", None)
-    args["email"] = field
+    if field is not None:
+        args["email"] = field
 
     field = data.get("email_alt", None)
-    args["email_alt"] = field
+    if field is not None:
+        args["email_alt"] = field
 
     field = data.get("phone_number", None)
-    args["phone_number"] = field
+    if field is not None:
+        args["phone_number"] = field
 
     field = data.get("fax_number", None)
-    args["fax_number"] = field
+    if field is not None:
+        args["fax_number"] = field
 
     field = data.get("address_line_1", None)
-    args["address_line_1"] = field
+    if field is not None:
+        args["address_line_1"] = field
 
     field = data.get("address_line_2", None)
-    args["address_line_2"] = field
+    if field is not None:
+        args["address_line_2"] = field
 
     field = data.get("zip", None)
-    args["zip"] = field
+    if field is not None:
+        args["zip"] = field
 
     field = data.get("city", None)
-    args["city"] = field
+    if field is not None:
+        args["city"] = field
 
     field = data.get("country", None)
-    args["country"] = field
+    if field is not None:
+        args["country"] = field
 
     field = data.get("vat_identification_code", None)
-    args["vat_identification_code"] = field
+    if field is not None:
+        args["vat_identification_code"] = field
 
     field = data.get("company_identification_code", None)
-    args["company_identification_code"] = field
+    if field is not None:
+        args["company_identification_code"] = field
 
     field = data.get("lang", None)
-    args["lang"] = field
+    if field is not None:
+        args["lang"] = field
 
     field = data.get("resale", None)
-    args["resale"] = field
+    if field is not None:
+        args["resale"] = field
 
     field = data.get("whois_opt_in", None)
-    args["whois_opt_in"] = field
+    if field is not None:
+        args["whois_opt_in"] = field
 
     field = data.get("email_status", None)
-    args["email_status"] = field
+    if field is not None:
+        args["email_status"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("questions", None)
-    args["questions"] = (
-        [unmarshal_ContactQuestion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["questions"] = (
+            [unmarshal_ContactQuestion(v) for v in field] if field is not None else None
+        )
 
     field = data.get("extension_fr", None)
-    args["extension_fr"] = unmarshal_ContactExtensionFR(field)
+    if field is not None:
+        args["extension_fr"] = unmarshal_ContactExtensionFR(field)
 
     field = data.get("extension_eu", None)
-    args["extension_eu"] = unmarshal_ContactExtensionEU(field)
+    if field is not None:
+        args["extension_eu"] = unmarshal_ContactExtensionEU(field)
 
     field = data.get("extension_nl", None)
-    args["extension_nl"] = unmarshal_ContactExtensionNL(field)
+    if field is not None:
+        args["extension_nl"] = unmarshal_ContactExtensionNL(field)
 
     return Contact(**args)
 
 
 def unmarshal_DNSZone(data: Any) -> DNSZone:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DNSZone' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("subdomain", None)
-    args["subdomain"] = field
+    if field is not None:
+        args["subdomain"] = field
 
     field = data.get("ns", None)
-    args["ns"] = field
+    if field is not None:
+        args["ns"] = field
 
     field = data.get("ns_default", None)
-    args["ns_default"] = field
+    if field is not None:
+        args["ns_default"] = field
 
     field = data.get("ns_master", None)
-    args["ns_master"] = field
+    if field is not None:
+        args["ns_master"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("linked_products", None)
-    args["linked_products"] = (
-        [LinkedProduct(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["linked_products"] = (
+            [LinkedProduct(v) for v in field] if field is not None else None
+        )
 
     field = data.get("message", None)
-    args["message"] = field
+    if field is not None:
+        args["message"] = field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return DNSZone(**args)
 
 
 def unmarshal_Host(data: Any) -> Host:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Host' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("ips", None)
-    args["ips"] = field
+    if field is not None:
+        args["ips"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     return Host(**args)
 
 
 def unmarshal_SSLCertificate(data: Any) -> SSLCertificate:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SSLCertificate' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("dns_zone", None)
-    args["dns_zone"] = field
+    if field is not None:
+        args["dns_zone"] = field
 
     field = data.get("alternative_dns_zones", None)
-    args["alternative_dns_zones"] = field
+    if field is not None:
+        args["alternative_dns_zones"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("private_key", None)
-    args["private_key"] = field
+    if field is not None:
+        args["private_key"] = field
 
     field = data.get("certificate_chain", None)
-    args["certificate_chain"] = field
+    if field is not None:
+        args["certificate_chain"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("expired_at", None)
-    args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return SSLCertificate(**args)
 
 
 def unmarshal_CheckContactsCompatibilityResponseContactCheckResult(
     data: Any,
 ) -> CheckContactsCompatibilityResponseContactCheckResult:
@@ -472,18 +540,20 @@
         raise TypeError(
             "Unmarshalling the type 'CheckContactsCompatibilityResponseContactCheckResult' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("compatible", None)
-    args["compatible"] = field
+    if field is not None:
+        args["compatible"] = field
 
     field = data.get("error_message", None)
-    args["error_message"] = field
+    if field is not None:
+        args["error_message"] = field
 
     return CheckContactsCompatibilityResponseContactCheckResult(**args)
 
 
 def unmarshal_CheckContactsCompatibilityResponse(
     data: Any,
 ) -> CheckContactsCompatibilityResponse:
@@ -491,30 +561,34 @@
         raise TypeError(
             "Unmarshalling the type 'CheckContactsCompatibilityResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("compatible", None)
-    args["compatible"] = field
+    if field is not None:
+        args["compatible"] = field
 
     field = data.get("owner_check_result", None)
-    args[
-        "owner_check_result"
-    ] = unmarshal_CheckContactsCompatibilityResponseContactCheckResult(field)
+    if field is not None:
+        args[
+            "owner_check_result"
+        ] = unmarshal_CheckContactsCompatibilityResponseContactCheckResult(field)
 
     field = data.get("administrative_check_result", None)
-    args[
-        "administrative_check_result"
-    ] = unmarshal_CheckContactsCompatibilityResponseContactCheckResult(field)
+    if field is not None:
+        args[
+            "administrative_check_result"
+        ] = unmarshal_CheckContactsCompatibilityResponseContactCheckResult(field)
 
     field = data.get("technical_check_result", None)
-    args[
-        "technical_check_result"
-    ] = unmarshal_CheckContactsCompatibilityResponseContactCheckResult(field)
+    if field is not None:
+        args[
+            "technical_check_result"
+        ] = unmarshal_CheckContactsCompatibilityResponseContactCheckResult(field)
 
     return CheckContactsCompatibilityResponse(**args)
 
 
 def unmarshal_ClearDNSZoneRecordsResponse(data: Any) -> ClearDNSZoneRecordsResponse:
     if not isinstance(data, dict):
         raise TypeError(
@@ -564,97 +638,110 @@
         raise TypeError(
             "Unmarshalling the type 'DSRecordPublicKey' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("key", None)
-    args["key"] = field
+    if field is not None:
+        args["key"] = field
 
     return DSRecordPublicKey(**args)
 
 
 def unmarshal_DSRecordDigest(data: Any) -> DSRecordDigest:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DSRecordDigest' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("digest", None)
-    args["digest"] = field
+    if field is not None:
+        args["digest"] = field
 
     field = data.get("public_key", None)
-    args["public_key"] = unmarshal_DSRecordPublicKey(field)
+    if field is not None:
+        args["public_key"] = unmarshal_DSRecordPublicKey(field)
 
     return DSRecordDigest(**args)
 
 
 def unmarshal_DSRecord(data: Any) -> DSRecord:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DSRecord' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("key_id", None)
-    args["key_id"] = field
+    if field is not None:
+        args["key_id"] = field
 
     field = data.get("algorithm", None)
-    args["algorithm"] = field
+    if field is not None:
+        args["algorithm"] = field
 
     field = data.get("digest", None)
-    args["digest"] = unmarshal_DSRecordDigest(field)
+    if field is not None:
+        args["digest"] = unmarshal_DSRecordDigest(field)
 
     field = data.get("public_key", None)
-    args["public_key"] = unmarshal_DSRecordPublicKey(field)
+    if field is not None:
+        args["public_key"] = unmarshal_DSRecordPublicKey(field)
 
     return DSRecord(**args)
 
 
 def unmarshal_TldOffer(data: Any) -> TldOffer:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'TldOffer' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("action", None)
-    args["action"] = field
+    if field is not None:
+        args["action"] = field
 
     field = data.get("operation_path", None)
-    args["operation_path"] = field
+    if field is not None:
+        args["operation_path"] = field
 
     field = data.get("price", None)
-    args["price"] = unmarshal_Money(field)
+    if field is not None:
+        args["price"] = unmarshal_Money(field)
 
     return TldOffer(**args)
 
 
 def unmarshal_DomainDNSSEC(data: Any) -> DomainDNSSEC:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainDNSSEC' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("ds_records", None)
-    args["ds_records"] = (
-        [unmarshal_DSRecord(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["ds_records"] = (
+            [unmarshal_DSRecord(v) for v in field] if field is not None else None
+        )
 
     return DomainDNSSEC(**args)
 
 
 def unmarshal_DomainRegistrationStatusExternalDomain(
     data: Any,
 ) -> DomainRegistrationStatusExternalDomain:
@@ -662,15 +749,16 @@
         raise TypeError(
             "Unmarshalling the type 'DomainRegistrationStatusExternalDomain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("validation_token", None)
-    args["validation_token"] = field
+    if field is not None:
+        args["validation_token"] = field
 
     return DomainRegistrationStatusExternalDomain(**args)
 
 
 def unmarshal_DomainRegistrationStatusTransfer(
     data: Any,
 ) -> DomainRegistrationStatusTransfer:
@@ -678,190 +766,227 @@
         raise TypeError(
             "Unmarshalling the type 'DomainRegistrationStatusTransfer' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("vote_current_owner", None)
-    args["vote_current_owner"] = field
+    if field is not None:
+        args["vote_current_owner"] = field
 
     field = data.get("vote_new_owner", None)
-    args["vote_new_owner"] = field
+    if field is not None:
+        args["vote_new_owner"] = field
 
     return DomainRegistrationStatusTransfer(**args)
 
 
 def unmarshal_Tld(data: Any) -> Tld:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Tld' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("dnssec_support", None)
-    args["dnssec_support"] = field
+    if field is not None:
+        args["dnssec_support"] = field
 
     field = data.get("duration_in_years_min", None)
-    args["duration_in_years_min"] = field
+    if field is not None:
+        args["duration_in_years_min"] = field
 
     field = data.get("duration_in_years_max", None)
-    args["duration_in_years_max"] = field
+    if field is not None:
+        args["duration_in_years_max"] = field
 
     field = data.get("idn_support", None)
-    args["idn_support"] = field
+    if field is not None:
+        args["idn_support"] = field
 
     field = data.get("offers", None)
-    args["offers"] = (
-        {key: unmarshal_TldOffer(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["offers"] = (
+            {key: unmarshal_TldOffer(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     field = data.get("specifications", None)
-    args["specifications"] = field
+    if field is not None:
+        args["specifications"] = field
 
     return Tld(**args)
 
 
 def unmarshal_Domain(data: Any) -> Domain:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Domain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("auto_renew_status", None)
-    args["auto_renew_status"] = field
+    if field is not None:
+        args["auto_renew_status"] = field
 
     field = data.get("epp_code", None)
-    args["epp_code"] = field
+    if field is not None:
+        args["epp_code"] = field
 
     field = data.get("dnssec", None)
-    args["dnssec"] = unmarshal_DomainDNSSEC(field)
+    if field is not None:
+        args["dnssec"] = unmarshal_DomainDNSSEC(field)
 
     field = data.get("expired_at", None)
-    args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("registrar", None)
-    args["registrar"] = field
+    if field is not None:
+        args["registrar"] = field
 
     field = data.get("is_external", None)
-    args["is_external"] = field
+    if field is not None:
+        args["is_external"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("dns_zones", None)
-    args["dns_zones"] = (
-        [unmarshal_DNSZone(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["dns_zones"] = (
+            [unmarshal_DNSZone(v) for v in field] if field is not None else None
+        )
 
     field = data.get("linked_products", None)
-    args["linked_products"] = (
-        [LinkedProduct(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["linked_products"] = (
+            [LinkedProduct(v) for v in field] if field is not None else None
+        )
 
     field = data.get("owner_contact", None)
-    args["owner_contact"] = unmarshal_Contact(field)
+    if field is not None:
+        args["owner_contact"] = unmarshal_Contact(field)
 
     field = data.get("technical_contact", None)
-    args["technical_contact"] = unmarshal_Contact(field)
+    if field is not None:
+        args["technical_contact"] = unmarshal_Contact(field)
 
     field = data.get("administrative_contact", None)
-    args["administrative_contact"] = unmarshal_Contact(field)
+    if field is not None:
+        args["administrative_contact"] = unmarshal_Contact(field)
 
     field = data.get("external_domain_registration_status", None)
-    args[
-        "external_domain_registration_status"
-    ] = unmarshal_DomainRegistrationStatusExternalDomain(field)
+    if field is not None:
+        args[
+            "external_domain_registration_status"
+        ] = unmarshal_DomainRegistrationStatusExternalDomain(field)
 
     field = data.get("transfer_registration_status", None)
-    args["transfer_registration_status"] = unmarshal_DomainRegistrationStatusTransfer(
-        field
-    )
+    if field is not None:
+        args[
+            "transfer_registration_status"
+        ] = unmarshal_DomainRegistrationStatusTransfer(field)
 
     field = data.get("tld", None)
-    args["tld"] = unmarshal_Tld(field)
+    if field is not None:
+        args["tld"] = unmarshal_Tld(field)
 
     return Domain(**args)
 
 
 def unmarshal_GetDNSZoneTsigKeyResponse(data: Any) -> GetDNSZoneTsigKeyResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetDNSZoneTsigKeyResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("key", None)
-    args["key"] = field
+    if field is not None:
+        args["key"] = field
 
     field = data.get("algorithm", None)
-    args["algorithm"] = field
+    if field is not None:
+        args["algorithm"] = field
 
     return GetDNSZoneTsigKeyResponse(**args)
 
 
 def unmarshal_RecordGeoIPConfigMatch(data: Any) -> RecordGeoIPConfigMatch:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordGeoIPConfigMatch' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("countries", None)
-    args["countries"] = field
+    if field is not None:
+        args["countries"] = field
 
     field = data.get("continents", None)
-    args["continents"] = field
+    if field is not None:
+        args["continents"] = field
 
     field = data.get("data", None)
-    args["data"] = field
+    if field is not None:
+        args["data"] = field
 
     return RecordGeoIPConfigMatch(**args)
 
 
 def unmarshal_RecordViewConfigView(data: Any) -> RecordViewConfigView:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordViewConfigView' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("subnet", None)
-    args["subnet"] = field
+    if field is not None:
+        args["subnet"] = field
 
     field = data.get("data", None)
-    args["data"] = field
+    if field is not None:
+        args["data"] = field
 
     return RecordViewConfigView(**args)
 
 
 def unmarshal_RecordWeightedConfigWeightedIP(
     data: Any,
 ) -> RecordWeightedConfigWeightedIP:
@@ -869,184 +994,211 @@
         raise TypeError(
             "Unmarshalling the type 'RecordWeightedConfigWeightedIP' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("weight", None)
-    args["weight"] = field
+    if field is not None:
+        args["weight"] = field
 
     return RecordWeightedConfigWeightedIP(**args)
 
 
 def unmarshal_RecordGeoIPConfig(data: Any) -> RecordGeoIPConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordGeoIPConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("matches", None)
-    args["matches"] = (
-        [unmarshal_RecordGeoIPConfigMatch(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["matches"] = (
+            [unmarshal_RecordGeoIPConfigMatch(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("default", None)
-    args["default"] = field
+    if field is not None:
+        args["default"] = field
 
     return RecordGeoIPConfig(**args)
 
 
 def unmarshal_RecordHTTPServiceConfig(data: Any) -> RecordHTTPServiceConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordHTTPServiceConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ips", None)
-    args["ips"] = field
+    if field is not None:
+        args["ips"] = field
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("strategy", None)
-    args["strategy"] = field
+    if field is not None:
+        args["strategy"] = field
 
     field = data.get("must_contain", None)
-    args["must_contain"] = field
+    if field is not None:
+        args["must_contain"] = field
 
     field = data.get("user_agent", None)
-    args["user_agent"] = field
+    if field is not None:
+        args["user_agent"] = field
 
     return RecordHTTPServiceConfig(**args)
 
 
 def unmarshal_RecordViewConfig(data: Any) -> RecordViewConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordViewConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("views", None)
-    args["views"] = (
-        [unmarshal_RecordViewConfigView(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["views"] = (
+            [unmarshal_RecordViewConfigView(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return RecordViewConfig(**args)
 
 
 def unmarshal_RecordWeightedConfig(data: Any) -> RecordWeightedConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordWeightedConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("weighted_ips", None)
-    args["weighted_ips"] = (
-        [unmarshal_RecordWeightedConfigWeightedIP(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["weighted_ips"] = (
+            [unmarshal_RecordWeightedConfigWeightedIP(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return RecordWeightedConfig(**args)
 
 
 def unmarshal_Record(data: Any) -> Record:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Record' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("data", None)
-    args["data"] = field
+    if field is not None:
+        args["data"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("priority", None)
-    args["priority"] = field
+    if field is not None:
+        args["priority"] = field
 
     field = data.get("ttl", None)
-    args["ttl"] = field
+    if field is not None:
+        args["ttl"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("comment", None)
-    args["comment"] = field
+    if field is not None:
+        args["comment"] = field
 
     field = data.get("geo_ip_config", None)
-    args["geo_ip_config"] = unmarshal_RecordGeoIPConfig(field)
+    if field is not None:
+        args["geo_ip_config"] = unmarshal_RecordGeoIPConfig(field)
 
     field = data.get("http_service_config", None)
-    args["http_service_config"] = unmarshal_RecordHTTPServiceConfig(field)
+    if field is not None:
+        args["http_service_config"] = unmarshal_RecordHTTPServiceConfig(field)
 
     field = data.get("weighted_config", None)
-    args["weighted_config"] = unmarshal_RecordWeightedConfig(field)
+    if field is not None:
+        args["weighted_config"] = unmarshal_RecordWeightedConfig(field)
 
     field = data.get("view_config", None)
-    args["view_config"] = unmarshal_RecordViewConfig(field)
+    if field is not None:
+        args["view_config"] = unmarshal_RecordViewConfig(field)
 
     return Record(**args)
 
 
 def unmarshal_RecordIdentifier(data: Any) -> RecordIdentifier:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordIdentifier' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("data", None)
-    args["data"] = field
+    if field is not None:
+        args["data"] = field
 
     field = data.get("ttl", None)
-    args["ttl"] = field
+    if field is not None:
+        args["ttl"] = field
 
     return RecordIdentifier(**args)
 
 
 def unmarshal_RecordChangeAdd(data: Any) -> RecordChangeAdd:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordChangeAdd' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     return RecordChangeAdd(**args)
 
 
 def unmarshal_RecordChangeClear(data: Any) -> RecordChangeClear:
     if not isinstance(data, dict):
         raise TypeError(
@@ -1063,202 +1215,224 @@
         raise TypeError(
             "Unmarshalling the type 'RecordChangeDelete' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("id_fields", None)
-    args["id_fields"] = unmarshal_RecordIdentifier(field)
+    if field is not None:
+        args["id_fields"] = unmarshal_RecordIdentifier(field)
 
     return RecordChangeDelete(**args)
 
 
 def unmarshal_RecordChangeSet(data: Any) -> RecordChangeSet:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordChangeSet' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("id_fields", None)
-    args["id_fields"] = unmarshal_RecordIdentifier(field)
+    if field is not None:
+        args["id_fields"] = unmarshal_RecordIdentifier(field)
 
     return RecordChangeSet(**args)
 
 
 def unmarshal_RecordChange(data: Any) -> RecordChange:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RecordChange' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("add", None)
-    args["add"] = unmarshal_RecordChangeAdd(field)
+    if field is not None:
+        args["add"] = unmarshal_RecordChangeAdd(field)
 
     field = data.get("set_", None)
-    args["set_"] = unmarshal_RecordChangeSet(field)
+    if field is not None:
+        args["set_"] = unmarshal_RecordChangeSet(field)
 
     field = data.get("delete", None)
-    args["delete"] = unmarshal_RecordChangeDelete(field)
+    if field is not None:
+        args["delete"] = unmarshal_RecordChangeDelete(field)
 
     field = data.get("clear", None)
-    args["clear"] = unmarshal_RecordChangeClear(field)
+    if field is not None:
+        args["clear"] = unmarshal_RecordChangeClear(field)
 
     return RecordChange(**args)
 
 
 def unmarshal_GetDNSZoneVersionDiffResponse(data: Any) -> GetDNSZoneVersionDiffResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetDNSZoneVersionDiffResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("changes", None)
-    args["changes"] = (
-        [unmarshal_RecordChange(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["changes"] = (
+            [unmarshal_RecordChange(v) for v in field] if field is not None else None
+        )
 
     return GetDNSZoneVersionDiffResponse(**args)
 
 
 def unmarshal_GetDomainAuthCodeResponse(data: Any) -> GetDomainAuthCodeResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetDomainAuthCodeResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("auth_code", None)
-    args["auth_code"] = field
+    if field is not None:
+        args["auth_code"] = field
 
     return GetDomainAuthCodeResponse(**args)
 
 
 def unmarshal_ImportProviderDNSZoneResponse(data: Any) -> ImportProviderDNSZoneResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ImportProviderDNSZoneResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     return ImportProviderDNSZoneResponse(**args)
 
 
 def unmarshal_ImportRawDNSZoneResponse(data: Any) -> ImportRawDNSZoneResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ImportRawDNSZoneResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     return ImportRawDNSZoneResponse(**args)
 
 
 def unmarshal_ContactRolesRoles(data: Any) -> ContactRolesRoles:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactRolesRoles' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("is_owner", None)
-    args["is_owner"] = field
+    if field is not None:
+        args["is_owner"] = field
 
     field = data.get("is_administrative", None)
-    args["is_administrative"] = field
+    if field is not None:
+        args["is_administrative"] = field
 
     field = data.get("is_technical", None)
-    args["is_technical"] = field
+    if field is not None:
+        args["is_technical"] = field
 
     return ContactRolesRoles(**args)
 
 
 def unmarshal_ContactRoles(data: Any) -> ContactRoles:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ContactRoles' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("roles", None)
-    args["roles"] = (
-        {key: unmarshal_ContactRolesRoles(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["roles"] = (
+            {key: unmarshal_ContactRolesRoles(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     field = data.get("contact", None)
-    args["contact"] = unmarshal_Contact(field)
+    if field is not None:
+        args["contact"] = unmarshal_Contact(field)
 
     return ContactRoles(**args)
 
 
 def unmarshal_ListContactsResponse(data: Any) -> ListContactsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListContactsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("contacts", None)
-    args["contacts"] = (
-        [unmarshal_ContactRoles(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["contacts"] = (
+            [unmarshal_ContactRoles(v) for v in field] if field is not None else None
+        )
 
     return ListContactsResponse(**args)
 
 
 def unmarshal_Nameserver(data: Any) -> Nameserver:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Nameserver' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     return Nameserver(**args)
 
 
 def unmarshal_ListDNSZoneNameserversResponse(
     data: Any,
 ) -> ListDNSZoneNameserversResponse:
@@ -1266,34 +1440,39 @@
         raise TypeError(
             "Unmarshalling the type 'ListDNSZoneNameserversResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ns", None)
-    args["ns"] = [unmarshal_Nameserver(v) for v in field] if field is not None else None
+    if field is not None:
+        args["ns"] = (
+            [unmarshal_Nameserver(v) for v in field] if field is not None else None
+        )
 
     return ListDNSZoneNameserversResponse(**args)
 
 
 def unmarshal_ListDNSZoneRecordsResponse(data: Any) -> ListDNSZoneRecordsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDNSZoneRecordsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     return ListDNSZoneRecordsResponse(**args)
 
 
 def unmarshal_ListDNSZoneVersionRecordsResponse(
     data: Any,
 ) -> ListDNSZoneVersionRecordsResponse:
@@ -1301,362 +1480,426 @@
         raise TypeError(
             "Unmarshalling the type 'ListDNSZoneVersionRecordsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     return ListDNSZoneVersionRecordsResponse(**args)
 
 
 def unmarshal_DNSZoneVersion(data: Any) -> DNSZoneVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DNSZoneVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return DNSZoneVersion(**args)
 
 
 def unmarshal_ListDNSZoneVersionsResponse(data: Any) -> ListDNSZoneVersionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDNSZoneVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_DNSZoneVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_DNSZoneVersion(v) for v in field] if field is not None else None
+        )
 
     return ListDNSZoneVersionsResponse(**args)
 
 
 def unmarshal_ListDNSZonesResponse(data: Any) -> ListDNSZonesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDNSZonesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("dns_zones", None)
-    args["dns_zones"] = (
-        [unmarshal_DNSZone(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["dns_zones"] = (
+            [unmarshal_DNSZone(v) for v in field] if field is not None else None
+        )
 
     return ListDNSZonesResponse(**args)
 
 
 def unmarshal_ListDomainHostsResponse(data: Any) -> ListDomainHostsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDomainHostsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("hosts", None)
-    args["hosts"] = [unmarshal_Host(v) for v in field] if field is not None else None
+    if field is not None:
+        args["hosts"] = (
+            [unmarshal_Host(v) for v in field] if field is not None else None
+        )
 
     return ListDomainHostsResponse(**args)
 
 
 def unmarshal_DomainSummary(data: Any) -> DomainSummary:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("auto_renew_status", None)
-    args["auto_renew_status"] = field
+    if field is not None:
+        args["auto_renew_status"] = field
 
     field = data.get("dnssec_status", None)
-    args["dnssec_status"] = field
+    if field is not None:
+        args["dnssec_status"] = field
 
     field = data.get("epp_code", None)
-    args["epp_code"] = field
+    if field is not None:
+        args["epp_code"] = field
 
     field = data.get("registrar", None)
-    args["registrar"] = field
+    if field is not None:
+        args["registrar"] = field
 
     field = data.get("is_external", None)
-    args["is_external"] = field
+    if field is not None:
+        args["is_external"] = field
 
     field = data.get("expired_at", None)
-    args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("external_domain_registration_status", None)
-    args[
-        "external_domain_registration_status"
-    ] = unmarshal_DomainRegistrationStatusExternalDomain(field)
+    if field is not None:
+        args[
+            "external_domain_registration_status"
+        ] = unmarshal_DomainRegistrationStatusExternalDomain(field)
 
     field = data.get("transfer_registration_status", None)
-    args["transfer_registration_status"] = unmarshal_DomainRegistrationStatusTransfer(
-        field
-    )
+    if field is not None:
+        args[
+            "transfer_registration_status"
+        ] = unmarshal_DomainRegistrationStatusTransfer(field)
 
     return DomainSummary(**args)
 
 
 def unmarshal_ListDomainsResponse(data: Any) -> ListDomainsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDomainsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("domains", None)
-    args["domains"] = (
-        [unmarshal_DomainSummary(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["domains"] = (
+            [unmarshal_DomainSummary(v) for v in field] if field is not None else None
+        )
 
     return ListDomainsResponse(**args)
 
 
 def unmarshal_RenewableDomain(data: Any) -> RenewableDomain:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RenewableDomain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("renewable_duration_in_years", None)
-    args["renewable_duration_in_years"] = field
+    if field is not None:
+        args["renewable_duration_in_years"] = field
 
     field = data.get("expired_at", None)
-    args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expired_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("limit_renew_at", None)
-    args["limit_renew_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["limit_renew_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("limit_redemption_at", None)
-    args["limit_redemption_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["limit_redemption_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("estimated_delete_at", None)
-    args["estimated_delete_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["estimated_delete_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("tld", None)
-    args["tld"] = unmarshal_Tld(field)
+    if field is not None:
+        args["tld"] = unmarshal_Tld(field)
 
     return RenewableDomain(**args)
 
 
 def unmarshal_ListRenewableDomainsResponse(data: Any) -> ListRenewableDomainsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListRenewableDomainsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("domains", None)
-    args["domains"] = (
-        [unmarshal_RenewableDomain(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["domains"] = (
+            [unmarshal_RenewableDomain(v) for v in field] if field is not None else None
+        )
 
     return ListRenewableDomainsResponse(**args)
 
 
 def unmarshal_ListSSLCertificatesResponse(data: Any) -> ListSSLCertificatesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSSLCertificatesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("certificates", None)
-    args["certificates"] = (
-        [unmarshal_SSLCertificate(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["certificates"] = (
+            [unmarshal_SSLCertificate(v) for v in field] if field is not None else None
+        )
 
     return ListSSLCertificatesResponse(**args)
 
 
 def unmarshal_Task(data: Any) -> Task:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Task' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("started_at", None)
-    args["started_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["started_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("message", None)
-    args["message"] = field
+    if field is not None:
+        args["message"] = field
 
     return Task(**args)
 
 
 def unmarshal_ListTasksResponse(data: Any) -> ListTasksResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTasksResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("tasks", None)
-    args["tasks"] = [unmarshal_Task(v) for v in field] if field is not None else None
+    if field is not None:
+        args["tasks"] = (
+            [unmarshal_Task(v) for v in field] if field is not None else None
+        )
 
     return ListTasksResponse(**args)
 
 
 def unmarshal_ListTldsResponse(data: Any) -> ListTldsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTldsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("tlds", None)
-    args["tlds"] = [unmarshal_Tld(v) for v in field] if field is not None else None
+    if field is not None:
+        args["tlds"] = [unmarshal_Tld(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListTldsResponse(**args)
 
 
 def unmarshal_OrderResponse(data: Any) -> OrderResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'OrderResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domains", None)
-    args["domains"] = field
+    if field is not None:
+        args["domains"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("task_id", None)
-    args["task_id"] = field
+    if field is not None:
+        args["task_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return OrderResponse(**args)
 
 
 def unmarshal_RefreshDNSZoneResponse(data: Any) -> RefreshDNSZoneResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RefreshDNSZoneResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("dns_zones", None)
-    args["dns_zones"] = (
-        [unmarshal_DNSZone(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["dns_zones"] = (
+            [unmarshal_DNSZone(v) for v in field] if field is not None else None
+        )
 
     return RefreshDNSZoneResponse(**args)
 
 
 def unmarshal_RegisterExternalDomainResponse(
     data: Any,
 ) -> RegisterExternalDomainResponse:
@@ -1664,27 +1907,32 @@
         raise TypeError(
             "Unmarshalling the type 'RegisterExternalDomainResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("validation_token", None)
-    args["validation_token"] = field
+    if field is not None:
+        args["validation_token"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return RegisterExternalDomainResponse(**args)
 
 
 def unmarshal_RestoreDNSZoneVersionResponse(data: Any) -> RestoreDNSZoneVersionResponse:
     if not isinstance(data, dict):
         raise TypeError(
@@ -1701,21 +1949,24 @@
         raise TypeError(
             "Unmarshalling the type 'AvailableDomain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("available", None)
-    args["available"] = field
+    if field is not None:
+        args["available"] = field
 
     field = data.get("tld", None)
-    args["tld"] = unmarshal_Tld(field)
+    if field is not None:
+        args["tld"] = unmarshal_Tld(field)
 
     return AvailableDomain(**args)
 
 
 def unmarshal_SearchAvailableDomainsResponse(
     data: Any,
 ) -> SearchAvailableDomainsResponse:
@@ -1723,17 +1974,18 @@
         raise TypeError(
             "Unmarshalling the type 'SearchAvailableDomainsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("available_domains", None)
-    args["available_domains"] = (
-        [unmarshal_AvailableDomain(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_domains"] = (
+            [unmarshal_AvailableDomain(v) for v in field] if field is not None else None
+        )
 
     return SearchAvailableDomainsResponse(**args)
 
 
 def unmarshal_UpdateDNSZoneNameserversResponse(
     data: Any,
 ) -> UpdateDNSZoneNameserversResponse:
@@ -1741,31 +1993,35 @@
         raise TypeError(
             "Unmarshalling the type 'UpdateDNSZoneNameserversResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ns", None)
-    args["ns"] = [unmarshal_Nameserver(v) for v in field] if field is not None else None
+    if field is not None:
+        args["ns"] = (
+            [unmarshal_Nameserver(v) for v in field] if field is not None else None
+        )
 
     return UpdateDNSZoneNameserversResponse(**args)
 
 
 def unmarshal_UpdateDNSZoneRecordsResponse(data: Any) -> UpdateDNSZoneRecordsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpdateDNSZoneRecordsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_Record(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_Record(v) for v in field] if field is not None else None
+        )
 
     return UpdateDNSZoneRecordsResponse(**args)
 
 
 def marshal_CloneDNSZoneRequest(
     request: CloneDNSZoneRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/domain/v2beta1/types.py` & `scaleway-2.0.0.dev6/scaleway/domain/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/content.py` & `scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/marshalling.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,140 +26,166 @@
         raise TypeError(
             "Unmarshalling the type 'MACAddress' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("mac_address", None)
-    args["mac_address"] = field
+    if field is not None:
+        args["mac_address"] = field
 
     field = data.get("mac_type", None)
-    args["mac_type"] = field
+    if field is not None:
+        args["mac_type"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return MACAddress(**args)
 
 
 def unmarshal_FlexibleIP(data: Any) -> FlexibleIP:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'FlexibleIP' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("ip_address", None)
-    args["ip_address"] = field
+    if field is not None:
+        args["ip_address"] = field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("reverse", None)
-    args["reverse"] = field
+    if field is not None:
+        args["reverse"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("mac_address", None)
-    args["mac_address"] = unmarshal_MACAddress(field)
+    if field is not None:
+        args["mac_address"] = unmarshal_MACAddress(field)
 
     field = data.get("server_id", None)
-    args["server_id"] = field
+    if field is not None:
+        args["server_id"] = field
 
     return FlexibleIP(**args)
 
 
 def unmarshal_AttachFlexibleIPsResponse(data: Any) -> AttachFlexibleIPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AttachFlexibleIPsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("flexible_ips", None)
-    args["flexible_ips"] = (
-        [unmarshal_FlexibleIP(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["flexible_ips"] = (
+            [unmarshal_FlexibleIP(v) for v in field] if field is not None else None
+        )
 
     return AttachFlexibleIPsResponse(**args)
 
 
 def unmarshal_DetachFlexibleIPsResponse(data: Any) -> DetachFlexibleIPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DetachFlexibleIPsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("flexible_ips", None)
-    args["flexible_ips"] = (
-        [unmarshal_FlexibleIP(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["flexible_ips"] = (
+            [unmarshal_FlexibleIP(v) for v in field] if field is not None else None
+        )
 
     return DetachFlexibleIPsResponse(**args)
 
 
 def unmarshal_ListFlexibleIPsResponse(data: Any) -> ListFlexibleIPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListFlexibleIPsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("flexible_ips", None)
-    args["flexible_ips"] = (
-        [unmarshal_FlexibleIP(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["flexible_ips"] = (
+            [unmarshal_FlexibleIP(v) for v in field] if field is not None else None
+        )
 
     return ListFlexibleIPsResponse(**args)
 
 
 def marshal_AttachFlexibleIPRequest(
     request: AttachFlexibleIPRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/flexibleip/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/flexibleip/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/function/v1beta1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/function/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/function/v1beta1/api.py` & `scaleway-2.0.0.dev6/scaleway/function/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/function/v1beta1/content.py` & `scaleway-2.0.0.dev6/scaleway/function/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/function/v1beta1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/function/v1beta1/marshalling.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,605 +55,729 @@
         raise TypeError(
             "Unmarshalling the type 'Cron' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("function_id", None)
-    args["function_id"] = field
+    if field is not None:
+        args["function_id"] = field
 
     field = data.get("schedule", None)
-    args["schedule"] = field
+    if field is not None:
+        args["schedule"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("args", None)
-    args["args"] = field
+    if field is not None:
+        args["args"] = field
 
     return Cron(**args)
 
 
 def unmarshal_Domain(data: Any) -> Domain:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Domain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("hostname", None)
-    args["hostname"] = field
+    if field is not None:
+        args["hostname"] = field
 
     field = data.get("function_id", None)
-    args["function_id"] = field
+    if field is not None:
+        args["function_id"] = field
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("error_message", None)
-    args["error_message"] = field
+    if field is not None:
+        args["error_message"] = field
 
     return Domain(**args)
 
 
 def unmarshal_SecretHashedValue(data: Any) -> SecretHashedValue:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SecretHashedValue' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("key", None)
-    args["key"] = field
+    if field is not None:
+        args["key"] = field
 
     field = data.get("hashed_value", None)
-    args["hashed_value"] = field
+    if field is not None:
+        args["hashed_value"] = field
 
     return SecretHashedValue(**args)
 
 
 def unmarshal_Function(data: Any) -> Function:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Function' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("namespace_id", None)
-    args["namespace_id"] = field
+    if field is not None:
+        args["namespace_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("environment_variables", None)
-    args["environment_variables"] = field
+    if field is not None:
+        args["environment_variables"] = field
 
     field = data.get("min_scale", None)
-    args["min_scale"] = field
+    if field is not None:
+        args["min_scale"] = field
 
     field = data.get("max_scale", None)
-    args["max_scale"] = field
+    if field is not None:
+        args["max_scale"] = field
 
     field = data.get("runtime", None)
-    args["runtime"] = field
+    if field is not None:
+        args["runtime"] = field
 
     field = data.get("memory_limit", None)
-    args["memory_limit"] = field
+    if field is not None:
+        args["memory_limit"] = field
 
     field = data.get("cpu_limit", None)
-    args["cpu_limit"] = field
+    if field is not None:
+        args["cpu_limit"] = field
 
     field = data.get("handler", None)
-    args["handler"] = field
+    if field is not None:
+        args["handler"] = field
 
     field = data.get("privacy", None)
-    args["privacy"] = field
+    if field is not None:
+        args["privacy"] = field
 
     field = data.get("domain_name", None)
-    args["domain_name"] = field
+    if field is not None:
+        args["domain_name"] = field
 
     field = data.get("secret_environment_variables", None)
-    args["secret_environment_variables"] = (
-        [unmarshal_SecretHashedValue(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["secret_environment_variables"] = (
+            [unmarshal_SecretHashedValue(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("http_option", None)
-    args["http_option"] = field
+    if field is not None:
+        args["http_option"] = field
 
     field = data.get("runtime_message", None)
-    args["runtime_message"] = field
+    if field is not None:
+        args["runtime_message"] = field
 
     field = data.get("timeout", None)
-    args["timeout"] = field
+    if field is not None:
+        args["timeout"] = field
 
     field = data.get("error_message", None)
-    args["error_message"] = field
+    if field is not None:
+        args["error_message"] = field
 
     field = data.get("build_message", None)
-    args["build_message"] = field
+    if field is not None:
+        args["build_message"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     return Function(**args)
 
 
 def unmarshal_Namespace(data: Any) -> Namespace:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Namespace' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("environment_variables", None)
-    args["environment_variables"] = field
+    if field is not None:
+        args["environment_variables"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("registry_namespace_id", None)
-    args["registry_namespace_id"] = field
+    if field is not None:
+        args["registry_namespace_id"] = field
 
     field = data.get("registry_endpoint", None)
-    args["registry_endpoint"] = field
+    if field is not None:
+        args["registry_endpoint"] = field
 
     field = data.get("secret_environment_variables", None)
-    args["secret_environment_variables"] = (
-        [unmarshal_SecretHashedValue(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["secret_environment_variables"] = (
+            [unmarshal_SecretHashedValue(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("error_message", None)
-    args["error_message"] = field
+    if field is not None:
+        args["error_message"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     return Namespace(**args)
 
 
 def unmarshal_Token(data: Any) -> Token:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Token' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("token", None)
-    args["token"] = field
+    if field is not None:
+        args["token"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("function_id", None)
-    args["function_id"] = field
+    if field is not None:
+        args["function_id"] = field
 
     field = data.get("namespace_id", None)
-    args["namespace_id"] = field
+    if field is not None:
+        args["namespace_id"] = field
 
     field = data.get("public_key", None)
-    args["public_key"] = field
+    if field is not None:
+        args["public_key"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Token(**args)
 
 
 def unmarshal_TriggerMnqNatsClientConfig(data: Any) -> TriggerMnqNatsClientConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'TriggerMnqNatsClientConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("subject", None)
-    args["subject"] = field
+    if field is not None:
+        args["subject"] = field
 
     field = data.get("mnq_nats_account_id", None)
-    args["mnq_nats_account_id"] = field
+    if field is not None:
+        args["mnq_nats_account_id"] = field
 
     field = data.get("mnq_project_id", None)
-    args["mnq_project_id"] = field
+    if field is not None:
+        args["mnq_project_id"] = field
 
     field = data.get("mnq_region", None)
-    args["mnq_region"] = field
+    if field is not None:
+        args["mnq_region"] = field
 
     field = data.get("mnq_namespace_id", None)
-    args["mnq_namespace_id"] = field
+    if field is not None:
+        args["mnq_namespace_id"] = field
 
     field = data.get("mnq_credential_id", None)
-    args["mnq_credential_id"] = field
+    if field is not None:
+        args["mnq_credential_id"] = field
 
     return TriggerMnqNatsClientConfig(**args)
 
 
 def unmarshal_TriggerMnqSqsClientConfig(data: Any) -> TriggerMnqSqsClientConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'TriggerMnqSqsClientConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("queue", None)
-    args["queue"] = field
+    if field is not None:
+        args["queue"] = field
 
     field = data.get("mnq_project_id", None)
-    args["mnq_project_id"] = field
+    if field is not None:
+        args["mnq_project_id"] = field
 
     field = data.get("mnq_region", None)
-    args["mnq_region"] = field
+    if field is not None:
+        args["mnq_region"] = field
 
     field = data.get("mnq_namespace_id", None)
-    args["mnq_namespace_id"] = field
+    if field is not None:
+        args["mnq_namespace_id"] = field
 
     field = data.get("mnq_credential_id", None)
-    args["mnq_credential_id"] = field
+    if field is not None:
+        args["mnq_credential_id"] = field
 
     return TriggerMnqSqsClientConfig(**args)
 
 
 def unmarshal_TriggerSqsClientConfig(data: Any) -> TriggerSqsClientConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'TriggerSqsClientConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("endpoint", None)
-    args["endpoint"] = field
+    if field is not None:
+        args["endpoint"] = field
 
     field = data.get("queue_url", None)
-    args["queue_url"] = field
+    if field is not None:
+        args["queue_url"] = field
 
     field = data.get("access_key", None)
-    args["access_key"] = field
+    if field is not None:
+        args["access_key"] = field
 
     field = data.get("secret_key", None)
-    args["secret_key"] = field
+    if field is not None:
+        args["secret_key"] = field
 
     return TriggerSqsClientConfig(**args)
 
 
 def unmarshal_Trigger(data: Any) -> Trigger:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Trigger' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("function_id", None)
-    args["function_id"] = field
+    if field is not None:
+        args["function_id"] = field
 
     field = data.get("input_type", None)
-    args["input_type"] = field
+    if field is not None:
+        args["input_type"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("error_message", None)
-    args["error_message"] = field
+    if field is not None:
+        args["error_message"] = field
 
     field = data.get("scw_sqs_config", None)
-    args["scw_sqs_config"] = unmarshal_TriggerMnqSqsClientConfig(field)
+    if field is not None:
+        args["scw_sqs_config"] = unmarshal_TriggerMnqSqsClientConfig(field)
 
     field = data.get("scw_nats_config", None)
-    args["scw_nats_config"] = unmarshal_TriggerMnqNatsClientConfig(field)
+    if field is not None:
+        args["scw_nats_config"] = unmarshal_TriggerMnqNatsClientConfig(field)
 
     field = data.get("sqs_config", None)
-    args["sqs_config"] = unmarshal_TriggerSqsClientConfig(field)
+    if field is not None:
+        args["sqs_config"] = unmarshal_TriggerSqsClientConfig(field)
 
     return Trigger(**args)
 
 
 def unmarshal_DownloadURL(data: Any) -> DownloadURL:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DownloadURL' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("headers", None)
-    args["headers"] = field
+    if field is not None:
+        args["headers"] = field
 
     return DownloadURL(**args)
 
 
 def unmarshal_ListCronsResponse(data: Any) -> ListCronsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListCronsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("crons", None)
-    args["crons"] = [unmarshal_Cron(v) for v in field] if field is not None else None
+    if field is not None:
+        args["crons"] = (
+            [unmarshal_Cron(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListCronsResponse(**args)
 
 
 def unmarshal_ListDomainsResponse(data: Any) -> ListDomainsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDomainsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domains", None)
-    args["domains"] = (
-        [unmarshal_Domain(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["domains"] = (
+            [unmarshal_Domain(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListDomainsResponse(**args)
 
 
 def unmarshal_Runtime(data: Any) -> Runtime:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Runtime' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("language", None)
-    args["language"] = field
+    if field is not None:
+        args["language"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("default_handler", None)
-    args["default_handler"] = field
+    if field is not None:
+        args["default_handler"] = field
 
     field = data.get("code_sample", None)
-    args["code_sample"] = field
+    if field is not None:
+        args["code_sample"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("status_message", None)
-    args["status_message"] = field
+    if field is not None:
+        args["status_message"] = field
 
     field = data.get("extension", None)
-    args["extension"] = field
+    if field is not None:
+        args["extension"] = field
 
     field = data.get("implementation", None)
-    args["implementation"] = field
+    if field is not None:
+        args["implementation"] = field
 
     field = data.get("logo_url", None)
-    args["logo_url"] = field
+    if field is not None:
+        args["logo_url"] = field
 
     return Runtime(**args)
 
 
 def unmarshal_ListFunctionRuntimesResponse(data: Any) -> ListFunctionRuntimesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListFunctionRuntimesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("runtimes", None)
-    args["runtimes"] = (
-        [unmarshal_Runtime(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["runtimes"] = (
+            [unmarshal_Runtime(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListFunctionRuntimesResponse(**args)
 
 
 def unmarshal_ListFunctionsResponse(data: Any) -> ListFunctionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListFunctionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("functions", None)
-    args["functions"] = (
-        [unmarshal_Function(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["functions"] = (
+            [unmarshal_Function(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListFunctionsResponse(**args)
 
 
 def unmarshal_Log(data: Any) -> Log:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Log' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("message", None)
-    args["message"] = field
+    if field is not None:
+        args["message"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("level", None)
-    args["level"] = field
+    if field is not None:
+        args["level"] = field
 
     field = data.get("source", None)
-    args["source"] = field
+    if field is not None:
+        args["source"] = field
 
     field = data.get("stream", None)
-    args["stream"] = field
+    if field is not None:
+        args["stream"] = field
 
     field = data.get("timestamp", None)
-    args["timestamp"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["timestamp"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Log(**args)
 
 
 def unmarshal_ListLogsResponse(data: Any) -> ListLogsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListLogsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("logs", None)
-    args["logs"] = [unmarshal_Log(v) for v in field] if field is not None else None
+    if field is not None:
+        args["logs"] = [unmarshal_Log(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListLogsResponse(**args)
 
 
 def unmarshal_ListNamespacesResponse(data: Any) -> ListNamespacesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNamespacesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("namespaces", None)
-    args["namespaces"] = (
-        [unmarshal_Namespace(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["namespaces"] = (
+            [unmarshal_Namespace(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListNamespacesResponse(**args)
 
 
 def unmarshal_ListTokensResponse(data: Any) -> ListTokensResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTokensResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("tokens", None)
-    args["tokens"] = [unmarshal_Token(v) for v in field] if field is not None else None
+    if field is not None:
+        args["tokens"] = (
+            [unmarshal_Token(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListTokensResponse(**args)
 
 
 def unmarshal_ListTriggersResponse(data: Any) -> ListTriggersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTriggersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("triggers", None)
-    args["triggers"] = (
-        [unmarshal_Trigger(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["triggers"] = (
+            [unmarshal_Trigger(v) for v in field] if field is not None else None
+        )
 
     return ListTriggersResponse(**args)
 
 
 def unmarshal_UploadURL(data: Any) -> UploadURL:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UploadURL' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("headers", None)
-    args["headers"] = field
+    if field is not None:
+        args["headers"] = field
 
     return UploadURL(**args)
 
 
 def marshal_CreateCronRequest(
     request: CreateCronRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/function/v1beta1/types.py` & `scaleway-2.0.0.dev6/scaleway/function/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/marshalling.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,624 +58,756 @@
         raise TypeError(
             "Unmarshalling the type 'JWT' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("jti", None)
-    args["jti"] = field
+    if field is not None:
+        args["jti"] = field
 
     field = data.get("issuer_id", None)
-    args["issuer_id"] = field
+    if field is not None:
+        args["issuer_id"] = field
 
     field = data.get("audience_id", None)
-    args["audience_id"] = field
+    if field is not None:
+        args["audience_id"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("user_agent", None)
-    args["user_agent"] = field
+    if field is not None:
+        args["user_agent"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return JWT(**args)
 
 
 def unmarshal_APIKey(data: Any) -> APIKey:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'APIKey' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("access_key", None)
-    args["access_key"] = field
+    if field is not None:
+        args["access_key"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("default_project_id", None)
-    args["default_project_id"] = field
+    if field is not None:
+        args["default_project_id"] = field
 
     field = data.get("editable", None)
-    args["editable"] = field
+    if field is not None:
+        args["editable"] = field
 
     field = data.get("creation_ip", None)
-    args["creation_ip"] = field
+    if field is not None:
+        args["creation_ip"] = field
 
     field = data.get("secret_key", None)
-    args["secret_key"] = field
+    if field is not None:
+        args["secret_key"] = field
 
     field = data.get("application_id", None)
-    args["application_id"] = field
+    if field is not None:
+        args["application_id"] = field
 
     field = data.get("user_id", None)
-    args["user_id"] = field
+    if field is not None:
+        args["user_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return APIKey(**args)
 
 
 def unmarshal_Application(data: Any) -> Application:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Application' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("editable", None)
-    args["editable"] = field
+    if field is not None:
+        args["editable"] = field
 
     field = data.get("nb_api_keys", None)
-    args["nb_api_keys"] = field
+    if field is not None:
+        args["nb_api_keys"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Application(**args)
 
 
 def unmarshal_Group(data: Any) -> Group:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Group' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("user_ids", None)
-    args["user_ids"] = field
+    if field is not None:
+        args["user_ids"] = field
 
     field = data.get("application_ids", None)
-    args["application_ids"] = field
+    if field is not None:
+        args["application_ids"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Group(**args)
 
 
 def unmarshal_Log(data: Any) -> Log:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Log' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("user_agent", None)
-    args["user_agent"] = field
+    if field is not None:
+        args["user_agent"] = field
 
     field = data.get("action", None)
-    args["action"] = field
+    if field is not None:
+        args["action"] = field
 
     field = data.get("bearer_id", None)
-    args["bearer_id"] = field
+    if field is not None:
+        args["bearer_id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("resource_type", None)
-    args["resource_type"] = field
+    if field is not None:
+        args["resource_type"] = field
 
     field = data.get("resource_id", None)
-    args["resource_id"] = field
+    if field is not None:
+        args["resource_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Log(**args)
 
 
 def unmarshal_Policy(data: Any) -> Policy:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Policy' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("editable", None)
-    args["editable"] = field
+    if field is not None:
+        args["editable"] = field
 
     field = data.get("nb_rules", None)
-    args["nb_rules"] = field
+    if field is not None:
+        args["nb_rules"] = field
 
     field = data.get("nb_scopes", None)
-    args["nb_scopes"] = field
+    if field is not None:
+        args["nb_scopes"] = field
 
     field = data.get("nb_permission_sets", None)
-    args["nb_permission_sets"] = field
+    if field is not None:
+        args["nb_permission_sets"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("user_id", None)
-    args["user_id"] = field
+    if field is not None:
+        args["user_id"] = field
 
     field = data.get("group_id", None)
-    args["group_id"] = field
+    if field is not None:
+        args["group_id"] = field
 
     field = data.get("application_id", None)
-    args["application_id"] = field
+    if field is not None:
+        args["application_id"] = field
 
     field = data.get("no_principal", None)
-    args["no_principal"] = field
+    if field is not None:
+        args["no_principal"] = field
 
     return Policy(**args)
 
 
 def unmarshal_Quotum(data: Any) -> Quotum:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Quotum' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("limit", None)
-    args["limit"] = field
+    if field is not None:
+        args["limit"] = field
 
     field = data.get("unlimited", None)
-    args["unlimited"] = field
+    if field is not None:
+        args["unlimited"] = field
 
     return Quotum(**args)
 
 
 def unmarshal_SSHKey(data: Any) -> SSHKey:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SSHKey' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("public_key", None)
-    args["public_key"] = field
+    if field is not None:
+        args["public_key"] = field
 
     field = data.get("fingerprint", None)
-    args["fingerprint"] = field
+    if field is not None:
+        args["fingerprint"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return SSHKey(**args)
 
 
 def unmarshal_User(data: Any) -> User:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'User' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("email", None)
-    args["email"] = field
+    if field is not None:
+        args["email"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("deletable", None)
-    args["deletable"] = field
+    if field is not None:
+        args["deletable"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("mfa", None)
-    args["mfa"] = field
+    if field is not None:
+        args["mfa"] = field
 
     field = data.get("account_root_user_id", None)
-    args["account_root_user_id"] = field
+    if field is not None:
+        args["account_root_user_id"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("last_login_at", None)
-    args["last_login_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["last_login_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("two_factor_enabled", None)
-    args["two_factor_enabled"] = field
+    if field is not None:
+        args["two_factor_enabled"] = field
 
     return User(**args)
 
 
 def unmarshal_ListAPIKeysResponse(data: Any) -> ListAPIKeysResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListAPIKeysResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("api_keys", None)
-    args["api_keys"] = (
-        [unmarshal_APIKey(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["api_keys"] = (
+            [unmarshal_APIKey(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListAPIKeysResponse(**args)
 
 
 def unmarshal_ListApplicationsResponse(data: Any) -> ListApplicationsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListApplicationsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("applications", None)
-    args["applications"] = (
-        [unmarshal_Application(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["applications"] = (
+            [unmarshal_Application(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListApplicationsResponse(**args)
 
 
 def unmarshal_ListGroupsResponse(data: Any) -> ListGroupsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListGroupsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("groups", None)
-    args["groups"] = [unmarshal_Group(v) for v in field] if field is not None else None
+    if field is not None:
+        args["groups"] = (
+            [unmarshal_Group(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListGroupsResponse(**args)
 
 
 def unmarshal_ListJWTsResponse(data: Any) -> ListJWTsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListJWTsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("jwts", None)
-    args["jwts"] = [unmarshal_JWT(v) for v in field] if field is not None else None
+    if field is not None:
+        args["jwts"] = [unmarshal_JWT(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListJWTsResponse(**args)
 
 
 def unmarshal_ListLogsResponse(data: Any) -> ListLogsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListLogsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("logs", None)
-    args["logs"] = [unmarshal_Log(v) for v in field] if field is not None else None
+    if field is not None:
+        args["logs"] = [unmarshal_Log(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListLogsResponse(**args)
 
 
 def unmarshal_PermissionSet(data: Any) -> PermissionSet:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PermissionSet' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("scope_type", None)
-    args["scope_type"] = field
+    if field is not None:
+        args["scope_type"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("categories", None)
-    args["categories"] = field
+    if field is not None:
+        args["categories"] = field
 
     return PermissionSet(**args)
 
 
 def unmarshal_ListPermissionSetsResponse(data: Any) -> ListPermissionSetsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPermissionSetsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("permission_sets", None)
-    args["permission_sets"] = (
-        [unmarshal_PermissionSet(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["permission_sets"] = (
+            [unmarshal_PermissionSet(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPermissionSetsResponse(**args)
 
 
 def unmarshal_ListPoliciesResponse(data: Any) -> ListPoliciesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPoliciesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("policies", None)
-    args["policies"] = (
-        [unmarshal_Policy(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["policies"] = (
+            [unmarshal_Policy(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPoliciesResponse(**args)
 
 
 def unmarshal_ListQuotaResponse(data: Any) -> ListQuotaResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListQuotaResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("quota", None)
-    args["quota"] = [unmarshal_Quotum(v) for v in field] if field is not None else None
+    if field is not None:
+        args["quota"] = (
+            [unmarshal_Quotum(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListQuotaResponse(**args)
 
 
 def unmarshal_Rule(data: Any) -> Rule:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Rule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("permission_sets_scope_type", None)
-    args["permission_sets_scope_type"] = field
+    if field is not None:
+        args["permission_sets_scope_type"] = field
 
     field = data.get("permission_set_names", None)
-    args["permission_set_names"] = field
+    if field is not None:
+        args["permission_set_names"] = field
 
     field = data.get("project_ids", None)
-    args["project_ids"] = field
+    if field is not None:
+        args["project_ids"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("account_root_user_id", None)
-    args["account_root_user_id"] = field
+    if field is not None:
+        args["account_root_user_id"] = field
 
     return Rule(**args)
 
 
 def unmarshal_ListRulesResponse(data: Any) -> ListRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_Rule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_Rule(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListRulesResponse(**args)
 
 
 def unmarshal_ListSSHKeysResponse(data: Any) -> ListSSHKeysResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSSHKeysResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ssh_keys", None)
-    args["ssh_keys"] = (
-        [unmarshal_SSHKey(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["ssh_keys"] = (
+            [unmarshal_SSHKey(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSSHKeysResponse(**args)
 
 
 def unmarshal_ListUsersResponse(data: Any) -> ListUsersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListUsersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("users", None)
-    args["users"] = [unmarshal_User(v) for v in field] if field is not None else None
+    if field is not None:
+        args["users"] = (
+            [unmarshal_User(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListUsersResponse(**args)
 
 
 def unmarshal_SetRulesResponse(data: Any) -> SetRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_Rule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_Rule(v) for v in field] if field is not None else None
+        )
 
     return SetRulesResponse(**args)
 
 
 def marshal_AddGroupMemberRequest(
     request: AddGroupMemberRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/iam/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/iam/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/api_utils.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/api_utils.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/marshalling.py`

 * *Files 12% similar despite different names*

```diff
@@ -140,792 +140,974 @@
         raise TypeError(
             "Unmarshalling the type 'PrivateNIC' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("server_id", None)
-    args["server_id"] = field
+    if field is not None:
+        args["server_id"] = field
 
     field = data.get("private_network_id", None)
-    args["private_network_id"] = field
+    if field is not None:
+        args["private_network_id"] = field
 
     field = data.get("mac_address", None)
-    args["mac_address"] = field
+    if field is not None:
+        args["mac_address"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     return PrivateNIC(**args)
 
 
 def unmarshal_ServerSummary(data: Any) -> ServerSummary:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return ServerSummary(**args)
 
 
 def unmarshal_Bootscript(data: Any) -> Bootscript:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Bootscript' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("bootcmdargs", None)
-    args["bootcmdargs"] = field
+    if field is not None:
+        args["bootcmdargs"] = field
 
     field = data.get("default", None)
-    args["default"] = field
+    if field is not None:
+        args["default"] = field
 
     field = data.get("dtb", None)
-    args["dtb"] = field
+    if field is not None:
+        args["dtb"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("initrd", None)
-    args["initrd"] = field
+    if field is not None:
+        args["initrd"] = field
 
     field = data.get("kernel", None)
-    args["kernel"] = field
+    if field is not None:
+        args["kernel"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("public", None)
-    args["public"] = field
+    if field is not None:
+        args["public"] = field
 
     field = data.get("title", None)
-    args["title"] = field
+    if field is not None:
+        args["title"] = field
 
     field = data.get("arch", None)
-    args["arch"] = field
+    if field is not None:
+        args["arch"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return Bootscript(**args)
 
 
 def unmarshal_Volume(data: Any) -> Volume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Volume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("volume_type", None)
-    args["volume_type"] = field
+    if field is not None:
+        args["volume_type"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("export_uri", None)
-    args["export_uri"] = field
+    if field is not None:
+        args["export_uri"] = field
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("server", None)
-    args["server"] = unmarshal_ServerSummary(field)
+    if field is not None:
+        args["server"] = unmarshal_ServerSummary(field)
 
     return Volume(**args)
 
 
 def unmarshal_VolumeSummary(data: Any) -> VolumeSummary:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("volume_type", None)
-    args["volume_type"] = field
+    if field is not None:
+        args["volume_type"] = field
 
     return VolumeSummary(**args)
 
 
 def unmarshal_Image(data: Any) -> Image:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Image' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("arch", None)
-    args["arch"] = field
+    if field is not None:
+        args["arch"] = field
 
     field = data.get("extra_volumes", None)
-    args["extra_volumes"] = (
-        {key: unmarshal_Volume(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["extra_volumes"] = (
+            {key: unmarshal_Volume(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     field = data.get("from_server", None)
-    args["from_server"] = field
+    if field is not None:
+        args["from_server"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("default_bootscript", None)
-    args["default_bootscript"] = unmarshal_Bootscript(field)
+    if field is not None:
+        args["default_bootscript"] = unmarshal_Bootscript(field)
 
     field = data.get("public", None)
-    args["public"] = field
+    if field is not None:
+        args["public"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("root_volume", None)
-    args["root_volume"] = unmarshal_VolumeSummary(field)
+    if field is not None:
+        args["root_volume"] = unmarshal_VolumeSummary(field)
 
     return Image(**args)
 
 
 def unmarshal_PlacementGroup(data: Any) -> PlacementGroup:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PlacementGroup' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("policy_mode", None)
-    args["policy_mode"] = field
+    if field is not None:
+        args["policy_mode"] = field
 
     field = data.get("policy_type", None)
-    args["policy_type"] = field
+    if field is not None:
+        args["policy_type"] = field
 
     field = data.get("policy_respected", None)
-    args["policy_respected"] = field
+    if field is not None:
+        args["policy_respected"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return PlacementGroup(**args)
 
 
 def unmarshal_SecurityGroupSummary(data: Any) -> SecurityGroupSummary:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SecurityGroupSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return SecurityGroupSummary(**args)
 
 
 def unmarshal_ServerIp(data: Any) -> ServerIp:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerIp' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("address", None)
-    args["address"] = field
+    if field is not None:
+        args["address"] = field
 
     field = data.get("gateway", None)
-    args["gateway"] = field
+    if field is not None:
+        args["gateway"] = field
 
     field = data.get("netmask", None)
-    args["netmask"] = field
+    if field is not None:
+        args["netmask"] = field
 
     field = data.get("family", None)
-    args["family"] = field
+    if field is not None:
+        args["family"] = field
 
     field = data.get("dynamic", None)
-    args["dynamic"] = field
+    if field is not None:
+        args["dynamic"] = field
 
     field = data.get("provisioning_mode", None)
-    args["provisioning_mode"] = field
+    if field is not None:
+        args["provisioning_mode"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     return ServerIp(**args)
 
 
 def unmarshal_ServerIpv6(data: Any) -> ServerIpv6:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerIpv6' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("address", None)
-    args["address"] = field
+    if field is not None:
+        args["address"] = field
 
     field = data.get("gateway", None)
-    args["gateway"] = field
+    if field is not None:
+        args["gateway"] = field
 
     field = data.get("netmask", None)
-    args["netmask"] = field
+    if field is not None:
+        args["netmask"] = field
 
     return ServerIpv6(**args)
 
 
 def unmarshal_ServerLocation(data: Any) -> ServerLocation:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerLocation' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("cluster_id", None)
-    args["cluster_id"] = field
+    if field is not None:
+        args["cluster_id"] = field
 
     field = data.get("hypervisor_id", None)
-    args["hypervisor_id"] = field
+    if field is not None:
+        args["hypervisor_id"] = field
 
     field = data.get("node_id", None)
-    args["node_id"] = field
+    if field is not None:
+        args["node_id"] = field
 
     field = data.get("platform_id", None)
-    args["platform_id"] = field
+    if field is not None:
+        args["platform_id"] = field
 
     field = data.get("zone_id", None)
-    args["zone_id"] = field
+    if field is not None:
+        args["zone_id"] = field
 
     return ServerLocation(**args)
 
 
 def unmarshal_ServerMaintenance(data: Any) -> ServerMaintenance:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerMaintenance' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("reason", None)
-    args["reason"] = field
+    if field is not None:
+        args["reason"] = field
 
     return ServerMaintenance(**args)
 
 
 def unmarshal_VolumeServer(data: Any) -> VolumeServer:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeServer' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("export_uri", None)
-    args["export_uri"] = field
+    if field is not None:
+        args["export_uri"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("server", None)
-    args["server"] = unmarshal_ServerSummary(field)
+    if field is not None:
+        args["server"] = unmarshal_ServerSummary(field)
 
     field = data.get("volume_type", None)
-    args["volume_type"] = field
+    if field is not None:
+        args["volume_type"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("boot", None)
-    args["boot"] = field
+    if field is not None:
+        args["boot"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return VolumeServer(**args)
 
 
 def unmarshal_Server(data: Any) -> Server:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Server' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("allowed_actions", None)
-    args["allowed_actions"] = (
-        [ServerAction(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["allowed_actions"] = (
+            [ServerAction(v) for v in field] if field is not None else None
+        )
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("commercial_type", None)
-    args["commercial_type"] = field
+    if field is not None:
+        args["commercial_type"] = field
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("dynamic_ip_required", None)
-    args["dynamic_ip_required"] = field
+    if field is not None:
+        args["dynamic_ip_required"] = field
 
     field = data.get("routed_ip_enabled", None)
-    args["routed_ip_enabled"] = field
+    if field is not None:
+        args["routed_ip_enabled"] = field
 
     field = data.get("enable_ipv6", None)
-    args["enable_ipv6"] = field
+    if field is not None:
+        args["enable_ipv6"] = field
 
     field = data.get("hostname", None)
-    args["hostname"] = field
+    if field is not None:
+        args["hostname"] = field
 
     field = data.get("protected", None)
-    args["protected"] = field
+    if field is not None:
+        args["protected"] = field
 
     field = data.get("image", None)
-    args["image"] = unmarshal_Image(field)
+    if field is not None:
+        args["image"] = unmarshal_Image(field)
 
     field = data.get("private_ip", None)
-    args["private_ip"] = field
+    if field is not None:
+        args["private_ip"] = field
 
     field = data.get("public_ip", None)
-    args["public_ip"] = unmarshal_ServerIp(field)
+    if field is not None:
+        args["public_ip"] = unmarshal_ServerIp(field)
 
     field = data.get("public_ips", None)
-    args["public_ips"] = (
-        [unmarshal_ServerIp(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["public_ips"] = (
+            [unmarshal_ServerIp(v) for v in field] if field is not None else None
+        )
 
     field = data.get("mac_address", None)
-    args["mac_address"] = field
+    if field is not None:
+        args["mac_address"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("boot_type", None)
-    args["boot_type"] = field
+    if field is not None:
+        args["boot_type"] = field
 
     field = data.get("volumes", None)
-    args["volumes"] = (
-        {key: unmarshal_VolumeServer(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["volumes"] = (
+            {key: unmarshal_VolumeServer(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("location", None)
-    args["location"] = unmarshal_ServerLocation(field)
+    if field is not None:
+        args["location"] = unmarshal_ServerLocation(field)
 
     field = data.get("ipv6", None)
-    args["ipv6"] = unmarshal_ServerIpv6(field)
+    if field is not None:
+        args["ipv6"] = unmarshal_ServerIpv6(field)
 
     field = data.get("bootscript", None)
-    args["bootscript"] = unmarshal_Bootscript(field)
+    if field is not None:
+        args["bootscript"] = unmarshal_Bootscript(field)
 
     field = data.get("security_group", None)
-    args["security_group"] = unmarshal_SecurityGroupSummary(field)
+    if field is not None:
+        args["security_group"] = unmarshal_SecurityGroupSummary(field)
 
     field = data.get("maintenances", None)
-    args["maintenances"] = (
-        [unmarshal_ServerMaintenance(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["maintenances"] = (
+            [unmarshal_ServerMaintenance(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("state_detail", None)
-    args["state_detail"] = field
+    if field is not None:
+        args["state_detail"] = field
 
     field = data.get("arch", None)
-    args["arch"] = field
+    if field is not None:
+        args["arch"] = field
 
     field = data.get("private_nics", None)
-    args["private_nics"] = (
-        [unmarshal_PrivateNIC(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["private_nics"] = (
+            [unmarshal_PrivateNIC(v) for v in field] if field is not None else None
+        )
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("placement_group", None)
-    args["placement_group"] = unmarshal_PlacementGroup(field)
+    if field is not None:
+        args["placement_group"] = unmarshal_PlacementGroup(field)
 
     return Server(**args)
 
 
 def unmarshal_AttachServerVolumeResponse(data: Any) -> AttachServerVolumeResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AttachServerVolumeResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("server", None)
-    args["server"] = unmarshal_Server(field)
+    if field is not None:
+        args["server"] = unmarshal_Server(field)
 
     return AttachServerVolumeResponse(**args)
 
 
 def unmarshal_CreateImageResponse(data: Any) -> CreateImageResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateImageResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("image", None)
-    args["image"] = unmarshal_Image(field)
+    if field is not None:
+        args["image"] = unmarshal_Image(field)
 
     return CreateImageResponse(**args)
 
 
 def unmarshal_Ip(data: Any) -> Ip:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Ip' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("address", None)
-    args["address"] = field
+    if field is not None:
+        args["address"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("prefix", None)
-    args["prefix"] = field
+    if field is not None:
+        args["prefix"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("reverse", None)
-    args["reverse"] = field
+    if field is not None:
+        args["reverse"] = field
 
     field = data.get("server", None)
-    args["server"] = unmarshal_ServerSummary(field)
+    if field is not None:
+        args["server"] = unmarshal_ServerSummary(field)
 
     return Ip(**args)
 
 
 def unmarshal_CreateIpResponse(data: Any) -> CreateIpResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateIpResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip", None)
-    args["ip"] = unmarshal_Ip(field)
+    if field is not None:
+        args["ip"] = unmarshal_Ip(field)
 
     return CreateIpResponse(**args)
 
 
 def unmarshal_CreatePlacementGroupResponse(data: Any) -> CreatePlacementGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreatePlacementGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("placement_group", None)
-    args["placement_group"] = unmarshal_PlacementGroup(field)
+    if field is not None:
+        args["placement_group"] = unmarshal_PlacementGroup(field)
 
     return CreatePlacementGroupResponse(**args)
 
 
 def unmarshal_CreatePrivateNICResponse(data: Any) -> CreatePrivateNICResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreatePrivateNICResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_nic", None)
-    args["private_nic"] = unmarshal_PrivateNIC(field)
+    if field is not None:
+        args["private_nic"] = unmarshal_PrivateNIC(field)
 
     return CreatePrivateNICResponse(**args)
 
 
 def unmarshal_SecurityGroup(data: Any) -> SecurityGroup:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SecurityGroup' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("enable_default_security", None)
-    args["enable_default_security"] = field
+    if field is not None:
+        args["enable_default_security"] = field
 
     field = data.get("inbound_default_policy", None)
-    args["inbound_default_policy"] = field
+    if field is not None:
+        args["inbound_default_policy"] = field
 
     field = data.get("outbound_default_policy", None)
-    args["outbound_default_policy"] = field
+    if field is not None:
+        args["outbound_default_policy"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("project_default", None)
-    args["project_default"] = field
+    if field is not None:
+        args["project_default"] = field
 
     field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_ServerSummary(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["servers"] = (
+            [unmarshal_ServerSummary(v) for v in field] if field is not None else None
+        )
 
     field = data.get("stateful", None)
-    args["stateful"] = field
+    if field is not None:
+        args["stateful"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("organization_default", None)
-    args["organization_default"] = field
+    if field is not None:
+        args["organization_default"] = field
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return SecurityGroup(**args)
 
 
 def unmarshal_CreateSecurityGroupResponse(data: Any) -> CreateSecurityGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateSecurityGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("security_group", None)
-    args["security_group"] = unmarshal_SecurityGroup(field)
+    if field is not None:
+        args["security_group"] = unmarshal_SecurityGroup(field)
 
     return CreateSecurityGroupResponse(**args)
 
 
 def unmarshal_SecurityGroupRule(data: Any) -> SecurityGroupRule:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SecurityGroupRule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("protocol", None)
-    args["protocol"] = field
+    if field is not None:
+        args["protocol"] = field
 
     field = data.get("direction", None)
-    args["direction"] = field
+    if field is not None:
+        args["direction"] = field
 
     field = data.get("action", None)
-    args["action"] = field
+    if field is not None:
+        args["action"] = field
 
     field = data.get("ip_range", None)
-    args["ip_range"] = field
+    if field is not None:
+        args["ip_range"] = field
 
     field = data.get("position", None)
-    args["position"] = field
+    if field is not None:
+        args["position"] = field
 
     field = data.get("editable", None)
-    args["editable"] = field
+    if field is not None:
+        args["editable"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("dest_port_from", None)
-    args["dest_port_from"] = field
+    if field is not None:
+        args["dest_port_from"] = field
 
     field = data.get("dest_port_to", None)
-    args["dest_port_to"] = field
+    if field is not None:
+        args["dest_port_to"] = field
 
     return SecurityGroupRule(**args)
 
 
 def unmarshal_CreateSecurityGroupRuleResponse(
     data: Any,
 ) -> CreateSecurityGroupRuleResponse:
@@ -933,341 +1115,399 @@
         raise TypeError(
             "Unmarshalling the type 'CreateSecurityGroupRuleResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rule", None)
-    args["rule"] = unmarshal_SecurityGroupRule(field)
+    if field is not None:
+        args["rule"] = unmarshal_SecurityGroupRule(field)
 
     return CreateSecurityGroupRuleResponse(**args)
 
 
 def unmarshal_CreateServerResponse(data: Any) -> CreateServerResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateServerResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("server", None)
-    args["server"] = unmarshal_Server(field)
+    if field is not None:
+        args["server"] = unmarshal_Server(field)
 
     return CreateServerResponse(**args)
 
 
 def unmarshal_SnapshotBaseVolume(data: Any) -> SnapshotBaseVolume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SnapshotBaseVolume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return SnapshotBaseVolume(**args)
 
 
 def unmarshal_Snapshot(data: Any) -> Snapshot:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Snapshot' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("volume_type", None)
-    args["volume_type"] = field
+    if field is not None:
+        args["volume_type"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("state", None)
-    args["state"] = field
+    if field is not None:
+        args["state"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("base_volume", None)
-    args["base_volume"] = unmarshal_SnapshotBaseVolume(field)
+    if field is not None:
+        args["base_volume"] = unmarshal_SnapshotBaseVolume(field)
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("error_reason", None)
-    args["error_reason"] = field
+    if field is not None:
+        args["error_reason"] = field
 
     return Snapshot(**args)
 
 
 def unmarshal_Task(data: Any) -> Task:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Task' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("progress", None)
-    args["progress"] = field
+    if field is not None:
+        args["progress"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("href_from", None)
-    args["href_from"] = field
+    if field is not None:
+        args["href_from"] = field
 
     field = data.get("href_result", None)
-    args["href_result"] = field
+    if field is not None:
+        args["href_result"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("started_at", None)
-    args["started_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["started_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("terminated_at", None)
-    args["terminated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["terminated_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return Task(**args)
 
 
 def unmarshal_CreateSnapshotResponse(data: Any) -> CreateSnapshotResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateSnapshotResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshot", None)
-    args["snapshot"] = unmarshal_Snapshot(field)
+    if field is not None:
+        args["snapshot"] = unmarshal_Snapshot(field)
 
     field = data.get("task", None)
-    args["task"] = unmarshal_Task(field)
+    if field is not None:
+        args["task"] = unmarshal_Task(field)
 
     return CreateSnapshotResponse(**args)
 
 
 def unmarshal_CreateVolumeResponse(data: Any) -> CreateVolumeResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateVolumeResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volume", None)
-    args["volume"] = unmarshal_Volume(field)
+    if field is not None:
+        args["volume"] = unmarshal_Volume(field)
 
     return CreateVolumeResponse(**args)
 
 
 def unmarshal_DetachServerVolumeResponse(data: Any) -> DetachServerVolumeResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DetachServerVolumeResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("server", None)
-    args["server"] = unmarshal_Server(field)
+    if field is not None:
+        args["server"] = unmarshal_Server(field)
 
     return DetachServerVolumeResponse(**args)
 
 
 def unmarshal_ExportSnapshotResponse(data: Any) -> ExportSnapshotResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ExportSnapshotResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("task", None)
-    args["task"] = unmarshal_Task(field)
+    if field is not None:
+        args["task"] = unmarshal_Task(field)
 
     return ExportSnapshotResponse(**args)
 
 
 def unmarshal_GetBootscriptResponse(data: Any) -> GetBootscriptResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetBootscriptResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("bootscript", None)
-    args["bootscript"] = unmarshal_Bootscript(field)
+    if field is not None:
+        args["bootscript"] = unmarshal_Bootscript(field)
 
     return GetBootscriptResponse(**args)
 
 
 def unmarshal_Dashboard(data: Any) -> Dashboard:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Dashboard' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volumes_count", None)
-    args["volumes_count"] = field
+    if field is not None:
+        args["volumes_count"] = field
 
     field = data.get("running_servers_count", None)
-    args["running_servers_count"] = field
+    if field is not None:
+        args["running_servers_count"] = field
 
     field = data.get("servers_by_types", None)
-    args["servers_by_types"] = field
+    if field is not None:
+        args["servers_by_types"] = field
 
     field = data.get("images_count", None)
-    args["images_count"] = field
+    if field is not None:
+        args["images_count"] = field
 
     field = data.get("snapshots_count", None)
-    args["snapshots_count"] = field
+    if field is not None:
+        args["snapshots_count"] = field
 
     field = data.get("servers_count", None)
-    args["servers_count"] = field
+    if field is not None:
+        args["servers_count"] = field
 
     field = data.get("ips_count", None)
-    args["ips_count"] = field
+    if field is not None:
+        args["ips_count"] = field
 
     field = data.get("security_groups_count", None)
-    args["security_groups_count"] = field
+    if field is not None:
+        args["security_groups_count"] = field
 
     field = data.get("ips_unused", None)
-    args["ips_unused"] = field
+    if field is not None:
+        args["ips_unused"] = field
 
     field = data.get("volumes_l_ssd_count", None)
-    args["volumes_l_ssd_count"] = field
+    if field is not None:
+        args["volumes_l_ssd_count"] = field
 
     field = data.get("volumes_b_ssd_count", None)
-    args["volumes_b_ssd_count"] = field
+    if field is not None:
+        args["volumes_b_ssd_count"] = field
 
     field = data.get("volumes_l_ssd_total_size", None)
-    args["volumes_l_ssd_total_size"] = field
+    if field is not None:
+        args["volumes_l_ssd_total_size"] = field
 
     field = data.get("volumes_b_ssd_total_size", None)
-    args["volumes_b_ssd_total_size"] = field
+    if field is not None:
+        args["volumes_b_ssd_total_size"] = field
 
     field = data.get("private_nics_count", None)
-    args["private_nics_count"] = field
+    if field is not None:
+        args["private_nics_count"] = field
 
     field = data.get("placement_groups_count", None)
-    args["placement_groups_count"] = field
+    if field is not None:
+        args["placement_groups_count"] = field
 
     return Dashboard(**args)
 
 
 def unmarshal_GetDashboardResponse(data: Any) -> GetDashboardResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetDashboardResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("dashboard", None)
-    args["dashboard"] = unmarshal_Dashboard(field)
+    if field is not None:
+        args["dashboard"] = unmarshal_Dashboard(field)
 
     return GetDashboardResponse(**args)
 
 
 def unmarshal_GetImageResponse(data: Any) -> GetImageResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetImageResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("image", None)
-    args["image"] = unmarshal_Image(field)
+    if field is not None:
+        args["image"] = unmarshal_Image(field)
 
     return GetImageResponse(**args)
 
 
 def unmarshal_GetIpResponse(data: Any) -> GetIpResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetIpResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip", None)
-    args["ip"] = unmarshal_Ip(field)
+    if field is not None:
+        args["ip"] = unmarshal_Ip(field)
 
     return GetIpResponse(**args)
 
 
 def unmarshal_GetPlacementGroupResponse(data: Any) -> GetPlacementGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetPlacementGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("placement_group", None)
-    args["placement_group"] = unmarshal_PlacementGroup(field)
+    if field is not None:
+        args["placement_group"] = unmarshal_PlacementGroup(field)
 
     return GetPlacementGroupResponse(**args)
 
 
 def unmarshal_PlacementGroupServer(data: Any) -> PlacementGroupServer:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PlacementGroupServer' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("policy_respected", None)
-    args["policy_respected"] = field
+    if field is not None:
+        args["policy_respected"] = field
 
     return PlacementGroupServer(**args)
 
 
 def unmarshal_GetPlacementGroupServersResponse(
     data: Any,
 ) -> GetPlacementGroupServersResponse:
@@ -1275,75 +1515,80 @@
         raise TypeError(
             "Unmarshalling the type 'GetPlacementGroupServersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_PlacementGroupServer(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["servers"] = (
+            [unmarshal_PlacementGroupServer(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return GetPlacementGroupServersResponse(**args)
 
 
 def unmarshal_GetPrivateNICResponse(data: Any) -> GetPrivateNICResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetPrivateNICResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_nic", None)
-    args["private_nic"] = unmarshal_PrivateNIC(field)
+    if field is not None:
+        args["private_nic"] = unmarshal_PrivateNIC(field)
 
     return GetPrivateNICResponse(**args)
 
 
 def unmarshal_GetSecurityGroupResponse(data: Any) -> GetSecurityGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetSecurityGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("security_group", None)
-    args["security_group"] = unmarshal_SecurityGroup(field)
+    if field is not None:
+        args["security_group"] = unmarshal_SecurityGroup(field)
 
     return GetSecurityGroupResponse(**args)
 
 
 def unmarshal_GetSecurityGroupRuleResponse(data: Any) -> GetSecurityGroupRuleResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetSecurityGroupRuleResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rule", None)
-    args["rule"] = unmarshal_SecurityGroupRule(field)
+    if field is not None:
+        args["rule"] = unmarshal_SecurityGroupRule(field)
 
     return GetSecurityGroupRuleResponse(**args)
 
 
 def unmarshal_GetServerResponse(data: Any) -> GetServerResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetServerResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("server", None)
-    args["server"] = unmarshal_Server(field)
+    if field is not None:
+        args["server"] = unmarshal_Server(field)
 
     return GetServerResponse(**args)
 
 
 def unmarshal_GetServerTypesAvailabilityResponseAvailability(
     data: Any,
 ) -> GetServerTypesAvailabilityResponseAvailability:
@@ -1351,15 +1596,16 @@
         raise TypeError(
             "Unmarshalling the type 'GetServerTypesAvailabilityResponseAvailability' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("availability", None)
-    args["availability"] = field
+    if field is not None:
+        args["availability"] = field
 
     return GetServerTypesAvailabilityResponseAvailability(**args)
 
 
 def unmarshal_GetServerTypesAvailabilityResponse(
     data: Any,
 ) -> GetServerTypesAvailabilityResponse:
@@ -1367,144 +1613,160 @@
         raise TypeError(
             "Unmarshalling the type 'GetServerTypesAvailabilityResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("servers", None)
-    args["servers"] = (
-        {
-            key: unmarshal_GetServerTypesAvailabilityResponseAvailability(value)
-            for key, value in field.items()
-        }
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["servers"] = (
+            {
+                key: unmarshal_GetServerTypesAvailabilityResponseAvailability(value)
+                for key, value in field.items()
+            }
+            if field is not None
+            else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return GetServerTypesAvailabilityResponse(**args)
 
 
 def unmarshal_GetSnapshotResponse(data: Any) -> GetSnapshotResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetSnapshotResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshot", None)
-    args["snapshot"] = unmarshal_Snapshot(field)
+    if field is not None:
+        args["snapshot"] = unmarshal_Snapshot(field)
 
     return GetSnapshotResponse(**args)
 
 
 def unmarshal_GetVolumeResponse(data: Any) -> GetVolumeResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetVolumeResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volume", None)
-    args["volume"] = unmarshal_Volume(field)
+    if field is not None:
+        args["volume"] = unmarshal_Volume(field)
 
     return GetVolumeResponse(**args)
 
 
 def unmarshal_ListBootscriptsResponse(data: Any) -> ListBootscriptsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListBootscriptsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("bootscripts", None)
-    args["bootscripts"] = (
-        [unmarshal_Bootscript(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["bootscripts"] = (
+            [unmarshal_Bootscript(v) for v in field] if field is not None else None
+        )
 
     return ListBootscriptsResponse(**args)
 
 
 def unmarshal_ListImagesResponse(data: Any) -> ListImagesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListImagesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("images", None)
-    args["images"] = [unmarshal_Image(v) for v in field] if field is not None else None
+    if field is not None:
+        args["images"] = (
+            [unmarshal_Image(v) for v in field] if field is not None else None
+        )
 
     return ListImagesResponse(**args)
 
 
 def unmarshal_ListIpsResponse(data: Any) -> ListIpsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListIpsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("ips", None)
-    args["ips"] = [unmarshal_Ip(v) for v in field] if field is not None else None
+    if field is not None:
+        args["ips"] = [unmarshal_Ip(v) for v in field] if field is not None else None
 
     return ListIpsResponse(**args)
 
 
 def unmarshal_ListPlacementGroupsResponse(data: Any) -> ListPlacementGroupsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPlacementGroupsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("placement_groups", None)
-    args["placement_groups"] = (
-        [unmarshal_PlacementGroup(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["placement_groups"] = (
+            [unmarshal_PlacementGroup(v) for v in field] if field is not None else None
+        )
 
     return ListPlacementGroupsResponse(**args)
 
 
 def unmarshal_ListPrivateNICsResponse(data: Any) -> ListPrivateNICsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPrivateNICsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_nics", None)
-    args["private_nics"] = (
-        [unmarshal_PrivateNIC(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["private_nics"] = (
+            [unmarshal_PrivateNIC(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPrivateNICsResponse(**args)
 
 
 def unmarshal_ListSecurityGroupRulesResponse(
     data: Any,
 ) -> ListSecurityGroupRulesResponse:
@@ -1512,103 +1774,117 @@
         raise TypeError(
             "Unmarshalling the type 'ListSecurityGroupRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("rules", None)
-    args["rules"] = (
-        [unmarshal_SecurityGroupRule(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_SecurityGroupRule(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return ListSecurityGroupRulesResponse(**args)
 
 
 def unmarshal_ListSecurityGroupsResponse(data: Any) -> ListSecurityGroupsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSecurityGroupsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("security_groups", None)
-    args["security_groups"] = (
-        [unmarshal_SecurityGroup(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["security_groups"] = (
+            [unmarshal_SecurityGroup(v) for v in field] if field is not None else None
+        )
 
     return ListSecurityGroupsResponse(**args)
 
 
 def unmarshal_ListServerActionsResponse(data: Any) -> ListServerActionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListServerActionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("actions", None)
-    args["actions"] = [ServerAction(v) for v in field] if field is not None else None
+    if field is not None:
+        args["actions"] = (
+            [ServerAction(v) for v in field] if field is not None else None
+        )
 
     return ListServerActionsResponse(**args)
 
 
 def unmarshal_ListServerUserDataResponse(data: Any) -> ListServerUserDataResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListServerUserDataResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("user_data", None)
-    args["user_data"] = field
+    if field is not None:
+        args["user_data"] = field
 
     return ListServerUserDataResponse(**args)
 
 
 def unmarshal_ListServersResponse(data: Any) -> ListServersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListServersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_Server(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["servers"] = (
+            [unmarshal_Server(v) for v in field] if field is not None else None
+        )
 
     return ListServersResponse(**args)
 
 
 def unmarshal_ServerTypeNetworkInterface(data: Any) -> ServerTypeNetworkInterface:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerTypeNetworkInterface' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("internal_bandwidth", None)
-    args["internal_bandwidth"] = field
+    if field is not None:
+        args["internal_bandwidth"] = field
 
     field = data.get("internet_bandwidth", None)
-    args["internet_bandwidth"] = field
+    if field is not None:
+        args["internet_bandwidth"] = field
 
     return ServerTypeNetworkInterface(**args)
 
 
 def unmarshal_ServerTypeVolumeConstraintSizes(
     data: Any,
 ) -> ServerTypeVolumeConstraintSizes:
@@ -1616,62 +1892,70 @@
         raise TypeError(
             "Unmarshalling the type 'ServerTypeVolumeConstraintSizes' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("min_size", None)
-    args["min_size"] = field
+    if field is not None:
+        args["min_size"] = field
 
     field = data.get("max_size", None)
-    args["max_size"] = field
+    if field is not None:
+        args["max_size"] = field
 
     return ServerTypeVolumeConstraintSizes(**args)
 
 
 def unmarshal_ServerTypeCapabilities(data: Any) -> ServerTypeCapabilities:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerTypeCapabilities' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("boot_types", None)
-    args["boot_types"] = [BootType(v) for v in field] if field is not None else None
+    if field is not None:
+        args["boot_types"] = [BootType(v) for v in field] if field is not None else None
 
     field = data.get("block_storage", None)
-    args["block_storage"] = field
+    if field is not None:
+        args["block_storage"] = field
 
     return ServerTypeCapabilities(**args)
 
 
 def unmarshal_ServerTypeNetwork(data: Any) -> ServerTypeNetwork:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerTypeNetwork' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("interfaces", None)
-    args["interfaces"] = (
-        [unmarshal_ServerTypeNetworkInterface(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["interfaces"] = (
+            [unmarshal_ServerTypeNetworkInterface(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("ipv6_support", None)
-    args["ipv6_support"] = field
+    if field is not None:
+        args["ipv6_support"] = field
 
     field = data.get("sum_internal_bandwidth", None)
-    args["sum_internal_bandwidth"] = field
+    if field is not None:
+        args["sum_internal_bandwidth"] = field
 
     field = data.get("sum_internet_bandwidth", None)
-    args["sum_internet_bandwidth"] = field
+    if field is not None:
+        args["sum_internet_bandwidth"] = field
 
     return ServerTypeNetwork(**args)
 
 
 def unmarshal_ServerTypeVolumeConstraintsByType(
     data: Any,
 ) -> ServerTypeVolumeConstraintsByType:
@@ -1679,246 +1963,281 @@
         raise TypeError(
             "Unmarshalling the type 'ServerTypeVolumeConstraintsByType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("l_ssd", None)
-    args["l_ssd"] = unmarshal_ServerTypeVolumeConstraintSizes(field)
+    if field is not None:
+        args["l_ssd"] = unmarshal_ServerTypeVolumeConstraintSizes(field)
 
     return ServerTypeVolumeConstraintsByType(**args)
 
 
 def unmarshal_ServerType(data: Any) -> ServerType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("monthly_price", None)
-    args["monthly_price"] = field
+    if field is not None:
+        args["monthly_price"] = field
 
     field = data.get("hourly_price", None)
-    args["hourly_price"] = field
+    if field is not None:
+        args["hourly_price"] = field
 
     field = data.get("alt_names", None)
-    args["alt_names"] = field
+    if field is not None:
+        args["alt_names"] = field
 
     field = data.get("ncpus", None)
-    args["ncpus"] = field
+    if field is not None:
+        args["ncpus"] = field
 
     field = data.get("ram", None)
-    args["ram"] = field
+    if field is not None:
+        args["ram"] = field
 
     field = data.get("arch", None)
-    args["arch"] = field
+    if field is not None:
+        args["arch"] = field
 
     field = data.get("baremetal", None)
-    args["baremetal"] = field
+    if field is not None:
+        args["baremetal"] = field
 
     field = data.get("per_volume_constraint", None)
-    args["per_volume_constraint"] = unmarshal_ServerTypeVolumeConstraintsByType(field)
+    if field is not None:
+        args["per_volume_constraint"] = unmarshal_ServerTypeVolumeConstraintsByType(
+            field
+        )
 
     field = data.get("volumes_constraint", None)
-    args["volumes_constraint"] = unmarshal_ServerTypeVolumeConstraintSizes(field)
+    if field is not None:
+        args["volumes_constraint"] = unmarshal_ServerTypeVolumeConstraintSizes(field)
 
     field = data.get("gpu", None)
-    args["gpu"] = field
+    if field is not None:
+        args["gpu"] = field
 
     field = data.get("network", None)
-    args["network"] = unmarshal_ServerTypeNetwork(field)
+    if field is not None:
+        args["network"] = unmarshal_ServerTypeNetwork(field)
 
     field = data.get("capabilities", None)
-    args["capabilities"] = unmarshal_ServerTypeCapabilities(field)
+    if field is not None:
+        args["capabilities"] = unmarshal_ServerTypeCapabilities(field)
 
     field = data.get("scratch_storage_max_size", None)
-    args["scratch_storage_max_size"] = field
+    if field is not None:
+        args["scratch_storage_max_size"] = field
 
     return ServerType(**args)
 
 
 def unmarshal_ListServersTypesResponse(data: Any) -> ListServersTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListServersTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("servers", None)
-    args["servers"] = (
-        {key: unmarshal_ServerType(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["servers"] = (
+            {key: unmarshal_ServerType(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     return ListServersTypesResponse(**args)
 
 
 def unmarshal_ListSnapshotsResponse(data: Any) -> ListSnapshotsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSnapshotsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("snapshots", None)
-    args["snapshots"] = (
-        [unmarshal_Snapshot(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["snapshots"] = (
+            [unmarshal_Snapshot(v) for v in field] if field is not None else None
+        )
 
     return ListSnapshotsResponse(**args)
 
 
 def unmarshal_ListVolumesResponse(data: Any) -> ListVolumesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVolumesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("volumes", None)
-    args["volumes"] = (
-        [unmarshal_Volume(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["volumes"] = (
+            [unmarshal_Volume(v) for v in field] if field is not None else None
+        )
 
     return ListVolumesResponse(**args)
 
 
 def unmarshal_VolumeTypeCapabilities(data: Any) -> VolumeTypeCapabilities:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeTypeCapabilities' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshot", None)
-    args["snapshot"] = field
+    if field is not None:
+        args["snapshot"] = field
 
     return VolumeTypeCapabilities(**args)
 
 
 def unmarshal_VolumeTypeConstraints(data: Any) -> VolumeTypeConstraints:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeTypeConstraints' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("min", None)
-    args["min"] = field
+    if field is not None:
+        args["min"] = field
 
     field = data.get("max", None)
-    args["max"] = field
+    if field is not None:
+        args["max"] = field
 
     return VolumeTypeConstraints(**args)
 
 
 def unmarshal_VolumeType(data: Any) -> VolumeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VolumeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("display_name", None)
-    args["display_name"] = field
+    if field is not None:
+        args["display_name"] = field
 
     field = data.get("capabilities", None)
-    args["capabilities"] = unmarshal_VolumeTypeCapabilities(field)
+    if field is not None:
+        args["capabilities"] = unmarshal_VolumeTypeCapabilities(field)
 
     field = data.get("constraints", None)
-    args["constraints"] = unmarshal_VolumeTypeConstraints(field)
+    if field is not None:
+        args["constraints"] = unmarshal_VolumeTypeConstraints(field)
 
     return VolumeType(**args)
 
 
 def unmarshal_ListVolumesTypesResponse(data: Any) -> ListVolumesTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVolumesTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("volumes", None)
-    args["volumes"] = (
-        {key: unmarshal_VolumeType(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["volumes"] = (
+            {key: unmarshal_VolumeType(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     return ListVolumesTypesResponse(**args)
 
 
 def unmarshal_MigrationPlan(data: Any) -> MigrationPlan:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'MigrationPlan' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshots", None)
-    args["snapshots"] = (
-        [unmarshal_Snapshot(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["snapshots"] = (
+            [unmarshal_Snapshot(v) for v in field] if field is not None else None
+        )
 
     field = data.get("validation_key", None)
-    args["validation_key"] = field
+    if field is not None:
+        args["validation_key"] = field
 
     field = data.get("volume", None)
-    args["volume"] = unmarshal_Volume(field)
+    if field is not None:
+        args["volume"] = unmarshal_Volume(field)
 
     return MigrationPlan(**args)
 
 
 def unmarshal_ServerActionResponse(data: Any) -> ServerActionResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerActionResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("task", None)
-    args["task"] = unmarshal_Task(field)
+    if field is not None:
+        args["task"] = unmarshal_Task(field)
 
     return ServerActionResponse(**args)
 
 
 def unmarshal_SetPlacementGroupResponse(data: Any) -> SetPlacementGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetPlacementGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("placement_group", None)
-    args["placement_group"] = unmarshal_PlacementGroup(field)
+    if field is not None:
+        args["placement_group"] = unmarshal_PlacementGroup(field)
 
     return SetPlacementGroupResponse(**args)
 
 
 def unmarshal_SetPlacementGroupServersResponse(
     data: Any,
 ) -> SetPlacementGroupServersResponse:
@@ -1926,63 +2245,69 @@
         raise TypeError(
             "Unmarshalling the type 'SetPlacementGroupServersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_PlacementGroupServer(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["servers"] = (
+            [unmarshal_PlacementGroupServer(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return SetPlacementGroupServersResponse(**args)
 
 
 def unmarshal_SetSecurityGroupRulesResponse(data: Any) -> SetSecurityGroupRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetSecurityGroupRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = (
-        [unmarshal_SecurityGroupRule(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_SecurityGroupRule(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return SetSecurityGroupRulesResponse(**args)
 
 
 def unmarshal_UpdateIpResponse(data: Any) -> UpdateIpResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpdateIpResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip", None)
-    args["ip"] = unmarshal_Ip(field)
+    if field is not None:
+        args["ip"] = unmarshal_Ip(field)
 
     return UpdateIpResponse(**args)
 
 
 def unmarshal_UpdatePlacementGroupResponse(data: Any) -> UpdatePlacementGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpdatePlacementGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("placement_group", None)
-    args["placement_group"] = unmarshal_PlacementGroup(field)
+    if field is not None:
+        args["placement_group"] = unmarshal_PlacementGroup(field)
 
     return UpdatePlacementGroupResponse(**args)
 
 
 def unmarshal_UpdatePlacementGroupServersResponse(
     data: Any,
 ) -> UpdatePlacementGroupServersResponse:
@@ -1990,117 +2315,125 @@
         raise TypeError(
             "Unmarshalling the type 'UpdatePlacementGroupServersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("servers", None)
-    args["servers"] = (
-        [unmarshal_PlacementGroupServer(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["servers"] = (
+            [unmarshal_PlacementGroupServer(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return UpdatePlacementGroupServersResponse(**args)
 
 
 def unmarshal_UpdateServerResponse(data: Any) -> UpdateServerResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpdateServerResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("server", None)
-    args["server"] = unmarshal_Server(field)
+    if field is not None:
+        args["server"] = unmarshal_Server(field)
 
     return UpdateServerResponse(**args)
 
 
 def unmarshal_UpdateVolumeResponse(data: Any) -> UpdateVolumeResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpdateVolumeResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volume", None)
-    args["volume"] = unmarshal_Volume(field)
+    if field is not None:
+        args["volume"] = unmarshal_Volume(field)
 
     return UpdateVolumeResponse(**args)
 
 
 def unmarshal__SetImageResponse(data: Any) -> _SetImageResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type '_SetImageResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("image", None)
-    args["image"] = unmarshal_Image(field)
+    if field is not None:
+        args["image"] = unmarshal_Image(field)
 
     return _SetImageResponse(**args)
 
 
 def unmarshal__SetSecurityGroupResponse(data: Any) -> _SetSecurityGroupResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type '_SetSecurityGroupResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("security_group", None)
-    args["security_group"] = unmarshal_SecurityGroup(field)
+    if field is not None:
+        args["security_group"] = unmarshal_SecurityGroup(field)
 
     return _SetSecurityGroupResponse(**args)
 
 
 def unmarshal__SetSecurityGroupRuleResponse(data: Any) -> _SetSecurityGroupRuleResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type '_SetSecurityGroupRuleResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rule", None)
-    args["rule"] = unmarshal_SecurityGroupRule(field)
+    if field is not None:
+        args["rule"] = unmarshal_SecurityGroupRule(field)
 
     return _SetSecurityGroupRuleResponse(**args)
 
 
 def unmarshal__SetServerResponse(data: Any) -> _SetServerResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type '_SetServerResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("server", None)
-    args["server"] = unmarshal_Server(field)
+    if field is not None:
+        args["server"] = unmarshal_Server(field)
 
     return _SetServerResponse(**args)
 
 
 def unmarshal__SetSnapshotResponse(data: Any) -> _SetSnapshotResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type '_SetSnapshotResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshot", None)
-    args["snapshot"] = unmarshal_Snapshot(field)
+    if field is not None:
+        args["snapshot"] = unmarshal_Snapshot(field)
 
     return _SetSnapshotResponse(**args)
 
 
 def marshal_ApplyBlockMigrationRequest(
     request: ApplyBlockMigrationRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/marshalling_utils.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/marshalling_utils.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/instance/v1/types_private.py` & `scaleway-2.0.0.dev6/scaleway/instance/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/iot/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/iot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/iot/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/iot/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/iot/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/iot/v1/marshalling.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,418 +65,487 @@
         raise TypeError(
             "Unmarshalling the type 'DeviceMessageFiltersRule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("policy", None)
-    args["policy"] = field
+    if field is not None:
+        args["policy"] = field
 
     field = data.get("topics", None)
-    args["topics"] = field
+    if field is not None:
+        args["topics"] = field
 
     return DeviceMessageFiltersRule(**args)
 
 
 def unmarshal_DeviceMessageFilters(data: Any) -> DeviceMessageFilters:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DeviceMessageFilters' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("publish", None)
-    args["publish"] = unmarshal_DeviceMessageFiltersRule(field)
+    if field is not None:
+        args["publish"] = unmarshal_DeviceMessageFiltersRule(field)
 
     field = data.get("subscribe", None)
-    args["subscribe"] = unmarshal_DeviceMessageFiltersRule(field)
+    if field is not None:
+        args["subscribe"] = unmarshal_DeviceMessageFiltersRule(field)
 
     return DeviceMessageFilters(**args)
 
 
 def unmarshal_Device(data: Any) -> Device:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Device' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("hub_id", None)
-    args["hub_id"] = field
+    if field is not None:
+        args["hub_id"] = field
 
     field = data.get("last_activity_at", None)
-    args["last_activity_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["last_activity_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("is_connected", None)
-    args["is_connected"] = field
+    if field is not None:
+        args["is_connected"] = field
 
     field = data.get("allow_insecure", None)
-    args["allow_insecure"] = field
+    if field is not None:
+        args["allow_insecure"] = field
 
     field = data.get("allow_multiple_connections", None)
-    args["allow_multiple_connections"] = field
+    if field is not None:
+        args["allow_multiple_connections"] = field
 
     field = data.get("has_custom_certificate", None)
-    args["has_custom_certificate"] = field
+    if field is not None:
+        args["has_custom_certificate"] = field
 
     field = data.get("message_filters", None)
-    args["message_filters"] = unmarshal_DeviceMessageFilters(field)
+    if field is not None:
+        args["message_filters"] = unmarshal_DeviceMessageFilters(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Device(**args)
 
 
 def unmarshal_Network(data: Any) -> Network:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Network' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("endpoint", None)
-    args["endpoint"] = field
+    if field is not None:
+        args["endpoint"] = field
 
     field = data.get("hub_id", None)
-    args["hub_id"] = field
+    if field is not None:
+        args["hub_id"] = field
 
     field = data.get("topic_prefix", None)
-    args["topic_prefix"] = field
+    if field is not None:
+        args["topic_prefix"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Network(**args)
 
 
 def unmarshal_HubTwinsGraphiteConfig(data: Any) -> HubTwinsGraphiteConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'HubTwinsGraphiteConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("push_uri", None)
-    args["push_uri"] = field
+    if field is not None:
+        args["push_uri"] = field
 
     return HubTwinsGraphiteConfig(**args)
 
 
 def unmarshal_Hub(data: Any) -> Hub:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Hub' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("product_plan", None)
-    args["product_plan"] = field
+    if field is not None:
+        args["product_plan"] = field
 
     field = data.get("enabled", None)
-    args["enabled"] = field
+    if field is not None:
+        args["enabled"] = field
 
     field = data.get("device_count", None)
-    args["device_count"] = field
+    if field is not None:
+        args["device_count"] = field
 
     field = data.get("connected_device_count", None)
-    args["connected_device_count"] = field
+    if field is not None:
+        args["connected_device_count"] = field
 
     field = data.get("endpoint", None)
-    args["endpoint"] = field
+    if field is not None:
+        args["endpoint"] = field
 
     field = data.get("disable_events", None)
-    args["disable_events"] = field
+    if field is not None:
+        args["disable_events"] = field
 
     field = data.get("events_topic_prefix", None)
-    args["events_topic_prefix"] = field
+    if field is not None:
+        args["events_topic_prefix"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("enable_device_auto_provisioning", None)
-    args["enable_device_auto_provisioning"] = field
+    if field is not None:
+        args["enable_device_auto_provisioning"] = field
 
     field = data.get("has_custom_ca", None)
-    args["has_custom_ca"] = field
+    if field is not None:
+        args["has_custom_ca"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("twins_graphite_config", None)
-    args["twins_graphite_config"] = unmarshal_HubTwinsGraphiteConfig(field)
+    if field is not None:
+        args["twins_graphite_config"] = unmarshal_HubTwinsGraphiteConfig(field)
 
     return Hub(**args)
 
 
 def unmarshal_Certificate(data: Any) -> Certificate:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Certificate' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("crt", None)
-    args["crt"] = field
+    if field is not None:
+        args["crt"] = field
 
     field = data.get("key", None)
-    args["key"] = field
+    if field is not None:
+        args["key"] = field
 
     return Certificate(**args)
 
 
 def unmarshal_CreateDeviceResponse(data: Any) -> CreateDeviceResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateDeviceResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("device", None)
-    args["device"] = unmarshal_Device(field)
+    if field is not None:
+        args["device"] = unmarshal_Device(field)
 
     field = data.get("certificate", None)
-    args["certificate"] = unmarshal_Certificate(field)
+    if field is not None:
+        args["certificate"] = unmarshal_Certificate(field)
 
     return CreateDeviceResponse(**args)
 
 
 def unmarshal_CreateNetworkResponse(data: Any) -> CreateNetworkResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateNetworkResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("secret", None)
-    args["secret"] = field
+    if field is not None:
+        args["secret"] = field
 
     field = data.get("network", None)
-    args["network"] = unmarshal_Network(field)
+    if field is not None:
+        args["network"] = unmarshal_Network(field)
 
     return CreateNetworkResponse(**args)
 
 
 def unmarshal_GetDeviceCertificateResponse(data: Any) -> GetDeviceCertificateResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetDeviceCertificateResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("certificate_pem", None)
-    args["certificate_pem"] = field
+    if field is not None:
+        args["certificate_pem"] = field
 
     field = data.get("device", None)
-    args["device"] = unmarshal_Device(field)
+    if field is not None:
+        args["device"] = unmarshal_Device(field)
 
     return GetDeviceCertificateResponse(**args)
 
 
 def unmarshal_GetDeviceMetricsResponse(data: Any) -> GetDeviceMetricsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetDeviceMetricsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("metrics", None)
-    args["metrics"] = (
-        [unmarshal_TimeSeries(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["metrics"] = (
+            [unmarshal_TimeSeries(v) for v in field] if field is not None else None
+        )
 
     return GetDeviceMetricsResponse(**args)
 
 
 def unmarshal_GetHubCAResponse(data: Any) -> GetHubCAResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetHubCAResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ca_cert_pem", None)
-    args["ca_cert_pem"] = field
+    if field is not None:
+        args["ca_cert_pem"] = field
 
     return GetHubCAResponse(**args)
 
 
 def unmarshal_GetHubMetricsResponse(data: Any) -> GetHubMetricsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetHubMetricsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("metrics", None)
-    args["metrics"] = (
-        [unmarshal_TimeSeries(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["metrics"] = (
+            [unmarshal_TimeSeries(v) for v in field] if field is not None else None
+        )
 
     return GetHubMetricsResponse(**args)
 
 
 def unmarshal_ListDevicesResponse(data: Any) -> ListDevicesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDevicesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("devices", None)
-    args["devices"] = (
-        [unmarshal_Device(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["devices"] = (
+            [unmarshal_Device(v) for v in field] if field is not None else None
+        )
 
     return ListDevicesResponse(**args)
 
 
 def unmarshal_ListHubsResponse(data: Any) -> ListHubsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListHubsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("hubs", None)
-    args["hubs"] = [unmarshal_Hub(v) for v in field] if field is not None else None
+    if field is not None:
+        args["hubs"] = [unmarshal_Hub(v) for v in field] if field is not None else None
 
     return ListHubsResponse(**args)
 
 
 def unmarshal_ListNetworksResponse(data: Any) -> ListNetworksResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNetworksResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("networks", None)
-    args["networks"] = (
-        [unmarshal_Network(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["networks"] = (
+            [unmarshal_Network(v) for v in field] if field is not None else None
+        )
 
     return ListNetworksResponse(**args)
 
 
 def unmarshal_RouteSummary(data: Any) -> RouteSummary:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RouteSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("hub_id", None)
-    args["hub_id"] = field
+    if field is not None:
+        args["hub_id"] = field
 
     field = data.get("topic", None)
-    args["topic"] = field
+    if field is not None:
+        args["topic"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return RouteSummary(**args)
 
 
 def unmarshal_ListRoutesResponse(data: Any) -> ListRoutesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListRoutesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("routes", None)
-    args["routes"] = (
-        [unmarshal_RouteSummary(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["routes"] = (
+            [unmarshal_RouteSummary(v) for v in field] if field is not None else None
+        )
 
     return ListRoutesResponse(**args)
 
 
 def unmarshal_ListTwinDocumentsResponseDocumentSummary(
     data: Any,
 ) -> ListTwinDocumentsResponseDocumentSummary:
@@ -484,33 +553,35 @@
         raise TypeError(
             "Unmarshalling the type 'ListTwinDocumentsResponseDocumentSummary' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("document_name", None)
-    args["document_name"] = field
+    if field is not None:
+        args["document_name"] = field
 
     return ListTwinDocumentsResponseDocumentSummary(**args)
 
 
 def unmarshal_ListTwinDocumentsResponse(data: Any) -> ListTwinDocumentsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTwinDocumentsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("documents", None)
-    args["documents"] = (
-        [unmarshal_ListTwinDocumentsResponseDocumentSummary(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["documents"] = (
+            [unmarshal_ListTwinDocumentsResponseDocumentSummary(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return ListTwinDocumentsResponse(**args)
 
 
 def unmarshal_RenewDeviceCertificateResponse(
     data: Any,
 ) -> RenewDeviceCertificateResponse:
@@ -518,174 +589,206 @@
         raise TypeError(
             "Unmarshalling the type 'RenewDeviceCertificateResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("device", None)
-    args["device"] = unmarshal_Device(field)
+    if field is not None:
+        args["device"] = unmarshal_Device(field)
 
     field = data.get("certificate", None)
-    args["certificate"] = unmarshal_Certificate(field)
+    if field is not None:
+        args["certificate"] = unmarshal_Certificate(field)
 
     return RenewDeviceCertificateResponse(**args)
 
 
 def unmarshal_RouteDatabaseConfig(data: Any) -> RouteDatabaseConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RouteDatabaseConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("engine", None)
-    args["engine"] = field
+    if field is not None:
+        args["engine"] = field
 
     field = data.get("host", None)
-    args["host"] = field
+    if field is not None:
+        args["host"] = field
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     field = data.get("dbname", None)
-    args["dbname"] = field
+    if field is not None:
+        args["dbname"] = field
 
     field = data.get("username", None)
-    args["username"] = field
+    if field is not None:
+        args["username"] = field
 
     field = data.get("password", None)
-    args["password"] = field
+    if field is not None:
+        args["password"] = field
 
     field = data.get("query", None)
-    args["query"] = field
+    if field is not None:
+        args["query"] = field
 
     return RouteDatabaseConfig(**args)
 
 
 def unmarshal_RouteRestConfig(data: Any) -> RouteRestConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RouteRestConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("verb", None)
-    args["verb"] = field
+    if field is not None:
+        args["verb"] = field
 
     field = data.get("uri", None)
-    args["uri"] = field
+    if field is not None:
+        args["uri"] = field
 
     field = data.get("headers", None)
-    args["headers"] = field
+    if field is not None:
+        args["headers"] = field
 
     return RouteRestConfig(**args)
 
 
 def unmarshal_RouteS3Config(data: Any) -> RouteS3Config:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RouteS3Config' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("bucket_region", None)
-    args["bucket_region"] = field
+    if field is not None:
+        args["bucket_region"] = field
 
     field = data.get("bucket_name", None)
-    args["bucket_name"] = field
+    if field is not None:
+        args["bucket_name"] = field
 
     field = data.get("object_prefix", None)
-    args["object_prefix"] = field
+    if field is not None:
+        args["object_prefix"] = field
 
     field = data.get("strategy", None)
-    args["strategy"] = field
+    if field is not None:
+        args["strategy"] = field
 
     return RouteS3Config(**args)
 
 
 def unmarshal_Route(data: Any) -> Route:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Route' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("hub_id", None)
-    args["hub_id"] = field
+    if field is not None:
+        args["hub_id"] = field
 
     field = data.get("topic", None)
-    args["topic"] = field
+    if field is not None:
+        args["topic"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("s3_config", None)
-    args["s3_config"] = unmarshal_RouteS3Config(field)
+    if field is not None:
+        args["s3_config"] = unmarshal_RouteS3Config(field)
 
     field = data.get("db_config", None)
-    args["db_config"] = unmarshal_RouteDatabaseConfig(field)
+    if field is not None:
+        args["db_config"] = unmarshal_RouteDatabaseConfig(field)
 
     field = data.get("rest_config", None)
-    args["rest_config"] = unmarshal_RouteRestConfig(field)
+    if field is not None:
+        args["rest_config"] = unmarshal_RouteRestConfig(field)
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Route(**args)
 
 
 def unmarshal_SetDeviceCertificateResponse(data: Any) -> SetDeviceCertificateResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetDeviceCertificateResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("certificate_pem", None)
-    args["certificate_pem"] = field
+    if field is not None:
+        args["certificate_pem"] = field
 
     field = data.get("device", None)
-    args["device"] = unmarshal_Device(field)
+    if field is not None:
+        args["device"] = unmarshal_Device(field)
 
     return SetDeviceCertificateResponse(**args)
 
 
 def unmarshal_TwinDocument(data: Any) -> TwinDocument:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'TwinDocument' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("twin_id", None)
-    args["twin_id"] = field
+    if field is not None:
+        args["twin_id"] = field
 
     field = data.get("document_name", None)
-    args["document_name"] = field
+    if field is not None:
+        args["document_name"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("data", None)
-    args["data"] = field
+    if field is not None:
+        args["data"] = field
 
     return TwinDocument(**args)
 
 
 def marshal_DeviceMessageFiltersRule(
     request: DeviceMessageFiltersRule,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/iot/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/iot/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipam/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/ipam/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipam/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/ipam/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipam/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/ipam/v1/marshalling.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,105 +24,125 @@
         raise TypeError(
             "Unmarshalling the type 'Resource' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("mac_address", None)
-    args["mac_address"] = field
+    if field is not None:
+        args["mac_address"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return Resource(**args)
 
 
 def unmarshal_Source(data: Any) -> Source:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Source' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("zonal", None)
-    args["zonal"] = field
+    if field is not None:
+        args["zonal"] = field
 
     field = data.get("private_network_id", None)
-    args["private_network_id"] = field
+    if field is not None:
+        args["private_network_id"] = field
 
     field = data.get("subnet_id", None)
-    args["subnet_id"] = field
+    if field is not None:
+        args["subnet_id"] = field
 
     return Source(**args)
 
 
 def unmarshal_IP(data: Any) -> IP:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'IP' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("address", None)
-    args["address"] = field
+    if field is not None:
+        args["address"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("is_ipv6", None)
-    args["is_ipv6"] = field
+    if field is not None:
+        args["is_ipv6"] = field
 
     field = data.get("source", None)
-    args["source"] = unmarshal_Source(field)
+    if field is not None:
+        args["source"] = unmarshal_Source(field)
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("resource", None)
-    args["resource"] = unmarshal_Resource(field)
+    if field is not None:
+        args["resource"] = unmarshal_Resource(field)
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return IP(**args)
 
 
 def unmarshal_ListIPsResponse(data: Any) -> ListIPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListIPsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("ips", None)
-    args["ips"] = [unmarshal_IP(v) for v in field] if field is not None else None
+    if field is not None:
+        args["ips"] = [unmarshal_IP(v) for v in field] if field is not None else None
 
     return ListIPsResponse(**args)
 
 
 def marshal_Source(
     request: Source,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/ipam/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/ipam/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/content.py` & `scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/marshalling.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,268 +33,318 @@
         raise TypeError(
             "Unmarshalling the type 'Name' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name_id", None)
-    args["name_id"] = field
+    if field is not None:
+        args["name_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("key", None)
-    args["key"] = field
+    if field is not None:
+        args["key"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("value", None)
-    args["value"] = field
+    if field is not None:
+        args["value"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Name(**args)
 
 
 def unmarshal_PinCIDMeta(data: Any) -> PinCIDMeta:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PinCIDMeta' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     return PinCIDMeta(**args)
 
 
 def unmarshal_PinCID(data: Any) -> PinCID:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PinCID' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("origins", None)
-    args["origins"] = field
+    if field is not None:
+        args["origins"] = field
 
     field = data.get("cid", None)
-    args["cid"] = field
+    if field is not None:
+        args["cid"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("meta", None)
-    args["meta"] = unmarshal_PinCIDMeta(field)
+    if field is not None:
+        args["meta"] = unmarshal_PinCIDMeta(field)
 
     return PinCID(**args)
 
 
 def unmarshal_PinInfo(data: Any) -> PinInfo:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PinInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status_details", None)
-    args["status_details"] = field
+    if field is not None:
+        args["status_details"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("url", None)
-    args["url"] = field
+    if field is not None:
+        args["url"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("progress", None)
-    args["progress"] = field
+    if field is not None:
+        args["progress"] = field
 
     return PinInfo(**args)
 
 
 def unmarshal_Pin(data: Any) -> Pin:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Pin' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("pin_id", None)
-    args["pin_id"] = field
+    if field is not None:
+        args["pin_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("delegates", None)
-    args["delegates"] = field
+    if field is not None:
+        args["delegates"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("cid", None)
-    args["cid"] = unmarshal_PinCID(field)
+    if field is not None:
+        args["cid"] = unmarshal_PinCID(field)
 
     field = data.get("info", None)
-    args["info"] = unmarshal_PinInfo(field)
+    if field is not None:
+        args["info"] = unmarshal_PinInfo(field)
 
     return Pin(**args)
 
 
 def unmarshal_Volume(data: Any) -> Volume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Volume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("count_pin", None)
-    args["count_pin"] = field
+    if field is not None:
+        args["count_pin"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     return Volume(**args)
 
 
 def unmarshal_ExportKeyNameResponse(data: Any) -> ExportKeyNameResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ExportKeyNameResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name_id", None)
-    args["name_id"] = field
+    if field is not None:
+        args["name_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("public_key", None)
-    args["public_key"] = field
+    if field is not None:
+        args["public_key"] = field
 
     field = data.get("private_key", None)
-    args["private_key"] = field
+    if field is not None:
+        args["private_key"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return ExportKeyNameResponse(**args)
 
 
 def unmarshal_ListNamesResponse(data: Any) -> ListNamesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNamesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("names", None)
-    args["names"] = [unmarshal_Name(v) for v in field] if field is not None else None
+    if field is not None:
+        args["names"] = (
+            [unmarshal_Name(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListNamesResponse(**args)
 
 
 def unmarshal_ListPinsResponse(data: Any) -> ListPinsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPinsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("pins", None)
-    args["pins"] = [unmarshal_Pin(v) for v in field] if field is not None else None
+    if field is not None:
+        args["pins"] = [unmarshal_Pin(v) for v in field] if field is not None else None
 
     return ListPinsResponse(**args)
 
 
 def unmarshal_ListVolumesResponse(data: Any) -> ListVolumesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVolumesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("volumes", None)
-    args["volumes"] = (
-        [unmarshal_Volume(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["volumes"] = (
+            [unmarshal_Volume(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListVolumesResponse(**args)
 
 
 def unmarshal_ReplacePinResponse(data: Any) -> ReplacePinResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ReplacePinResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("pin", None)
-    args["pin"] = unmarshal_Pin(field)
+    if field is not None:
+        args["pin"] = unmarshal_Pin(field)
 
     return ReplacePinResponse(**args)
 
 
 def marshal_CreatePinByCIDRequest(
     request: CreatePinByCIDRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/ipfs/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/ipfs/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/test/v1/marshalling.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,215 +1,228 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 
 from typing import Any, Dict
 from dateutil import parser
 
 from scaleway_core.profile import ProfileDefaults
+from scaleway_core.utils import (
+    OneOfPossibility,
+    resolve_one_of,
+)
 from .types import (
-    JobDefinition,
-    JobRun,
-    ListJobDefinitionsResponse,
-    ListJobRunsResponse,
-    CreateJobDefinitionRequest,
-    UpdateJobDefinitionRequest,
+    Human,
+    ListHumansResponse,
+    RegisterResponse,
+    CreateHumanRequest,
+    RegisterRequest,
+    UpdateHumanRequest,
 )
 
 
-def unmarshal_JobDefinition(data: Any) -> JobDefinition:
+def unmarshal_Human(data: Any) -> Human:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'JobDefinition' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Human' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("cpu_limit", None)
-    args["cpu_limit"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("memory_limit", None)
-    args["memory_limit"] = field
-
-    field = data.get("image_uri", None)
-    args["image_uri"] = field
-
-    field = data.get("command", None)
-    args["command"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
+    field = data.get("organization_id", None)
+    if field is not None:
+        args["organization_id"] = field
+
+    field = data.get("height", None)
+    if field is not None:
+        args["height"] = field
+
+    field = data.get("shoe_size", None)
+    if field is not None:
+        args["shoe_size"] = field
+
+    field = data.get("altitude_in_meter", None)
+    if field is not None:
+        args["altitude_in_meter"] = field
+
+    field = data.get("altitude_in_millimeter", None)
+    if field is not None:
+        args["altitude_in_millimeter"] = field
+
+    field = data.get("fingers_count", None)
+    if field is not None:
+        args["fingers_count"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("environment_variables", None)
-    args["environment_variables"] = field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("description", None)
-    args["description"] = field
+    field = data.get("hair_count", None)
+    if field is not None:
+        args["hair_count"] = field
+
+    field = data.get("is_happy", None)
+    if field is not None:
+        args["is_happy"] = field
+
+    field = data.get("eyes_color", None)
+    if field is not None:
+        args["eyes_color"] = field
+
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("region", None)
-    args["region"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("job_timeout", None)
-    args["job_timeout"] = field
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
-    return JobDefinition(**args)
+    return Human(**args)
 
 
-def unmarshal_JobRun(data: Any) -> JobRun:
+def unmarshal_ListHumansResponse(data: Any) -> ListHumansResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'JobRun' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListHumansResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("job_definition_id", None)
-    args["job_definition_id"] = field
-
-    field = data.get("state", None)
-    args["state"] = field
-
-    field = data.get("error_message", None)
-    args["error_message"] = field
-
-    field = data.get("region", None)
-    args["region"] = field
-
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("terminated_at", None)
-    args["terminated_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("exit_code", None)
-    args["exit_code"] = field
-
-    field = data.get("run_duration", None)
-    args["run_duration"] = field
-
-    return JobRun(**args)
-
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-def unmarshal_ListJobDefinitionsResponse(data: Any) -> ListJobDefinitionsResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListJobDefinitionsResponse' failed as data isn't a dictionary."
+    field = data.get("humans", None)
+    if field is not None:
+        args["humans"] = (
+            [unmarshal_Human(v) for v in field] if field is not None else None
         )
 
-    args: Dict[str, Any] = {}
+    return ListHumansResponse(**args)
 
-    field = data.get("job_definitions", None)
-    args["job_definitions"] = (
-        [unmarshal_JobDefinition(v) for v in field] if field is not None else None
-    )
-
-    field = data.get("total_count", None)
-    args["total_count"] = field
 
-    return ListJobDefinitionsResponse(**args)
-
-
-def unmarshal_ListJobRunsResponse(data: Any) -> ListJobRunsResponse:
+def unmarshal_RegisterResponse(data: Any) -> RegisterResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListJobRunsResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'RegisterResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("job_runs", None)
-    args["job_runs"] = (
-        [unmarshal_JobRun(v) for v in field] if field is not None else None
-    )
+    field = data.get("secret_key", None)
+    if field is not None:
+        args["secret_key"] = field
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    field = data.get("access_key", None)
+    if field is not None:
+        args["access_key"] = field
 
-    return ListJobRunsResponse(**args)
+    return RegisterResponse(**args)
 
 
-def marshal_CreateJobDefinitionRequest(
-    request: CreateJobDefinitionRequest,
+def marshal_CreateHumanRequest(
+    request: CreateHumanRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
+    output.update(
+        resolve_one_of(
+            [
+                OneOfPossibility(
+                    "project_id", request.project_id, defaults.default_project_id
+                ),
+                OneOfPossibility(
+                    "organization_id",
+                    request.organization_id,
+                    defaults.default_organization_id,
+                ),
+            ]
+        ),
+    )
+
+    if request.height is not None:
+        output["height"] = request.height
 
-    if request.cpu_limit is not None:
-        output["cpu_limit"] = request.cpu_limit
+    if request.shoe_size is not None:
+        output["shoe_size"] = request.shoe_size
 
-    if request.memory_limit is not None:
-        output["memory_limit"] = request.memory_limit
+    if request.altitude_in_meter is not None:
+        output["altitude_in_meter"] = request.altitude_in_meter
 
-    if request.image_uri is not None:
-        output["image_uri"] = request.image_uri
+    if request.altitude_in_millimeter is not None:
+        output["altitude_in_millimeter"] = request.altitude_in_millimeter
 
-    if request.command is not None:
-        output["command"] = request.command
+    if request.fingers_count is not None:
+        output["fingers_count"] = request.fingers_count
 
-    if request.description is not None:
-        output["description"] = request.description
+    if request.hair_count is not None:
+        output["hair_count"] = request.hair_count
+
+    if request.is_happy is not None:
+        output["is_happy"] = request.is_happy
 
     if request.name is not None:
         output["name"] = request.name
 
-    if request.project_id is not None:
-        output["project_id"] = request.project_id or defaults.default_project_id
+    if request.eyes_color is not None:
+        output["eyes_color"] = str(request.eyes_color)
+
+    return output
+
 
-    if request.environment_variables is not None:
-        output["environment_variables"] = {
-            key: value for key, value in request.environment_variables.items()
-        }
+def marshal_RegisterRequest(
+    request: RegisterRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-    if request.job_timeout is not None:
-        output["job_timeout"] = request.job_timeout
+    if request.username is not None:
+        output["username"] = request.username
 
     return output
 
 
-def marshal_UpdateJobDefinitionRequest(
-    request: UpdateJobDefinitionRequest,
+def marshal_UpdateHumanRequest(
+    request: UpdateHumanRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.name is not None:
-        output["name"] = request.name
+    if request.height is not None:
+        output["height"] = request.height
 
-    if request.cpu_limit is not None:
-        output["cpu_limit"] = request.cpu_limit
+    if request.shoe_size is not None:
+        output["shoe_size"] = request.shoe_size
 
-    if request.memory_limit is not None:
-        output["memory_limit"] = request.memory_limit
+    if request.altitude_in_meter is not None:
+        output["altitude_in_meter"] = request.altitude_in_meter
 
-    if request.image_uri is not None:
-        output["image_uri"] = request.image_uri
+    if request.altitude_in_millimeter is not None:
+        output["altitude_in_millimeter"] = request.altitude_in_millimeter
 
-    if request.command is not None:
-        output["command"] = request.command
+    if request.fingers_count is not None:
+        output["fingers_count"] = request.fingers_count
 
-    if request.environment_variables is not None:
-        output["environment_variables"] = request.environment_variables
+    if request.hair_count is not None:
+        output["hair_count"] = request.hair_count
 
-    if request.description is not None:
-        output["description"] = request.description
+    if request.is_happy is not None:
+        output["is_happy"] = request.is_happy
 
-    if request.job_timeout is not None:
-        output["job_timeout"] = request.job_timeout
+    if request.eyes_color is not None:
+        output["eyes_color"] = str(request.eyes_color)
+
+    if request.name is not None:
+        output["name"] = request.name
 
     return output
```

### Comparing `scaleway-2.0.0.dev5/scaleway/jobs/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/k8s/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/k8s/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/k8s/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/k8s/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/k8s/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/k8s/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/k8s/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/k8s/v1/marshalling.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,458 +57,568 @@
         raise TypeError(
             "Unmarshalling the type 'PoolUpgradePolicy' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("max_unavailable", None)
-    args["max_unavailable"] = field
+    if field is not None:
+        args["max_unavailable"] = field
 
     field = data.get("max_surge", None)
-    args["max_surge"] = field
+    if field is not None:
+        args["max_surge"] = field
 
     return PoolUpgradePolicy(**args)
 
 
 def unmarshal_Pool(data: Any) -> Pool:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Pool' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("cluster_id", None)
-    args["cluster_id"] = field
+    if field is not None:
+        args["cluster_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("node_type", None)
-    args["node_type"] = field
+    if field is not None:
+        args["node_type"] = field
 
     field = data.get("autoscaling", None)
-    args["autoscaling"] = field
+    if field is not None:
+        args["autoscaling"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("min_size", None)
-    args["min_size"] = field
+    if field is not None:
+        args["min_size"] = field
 
     field = data.get("max_size", None)
-    args["max_size"] = field
+    if field is not None:
+        args["max_size"] = field
 
     field = data.get("container_runtime", None)
-    args["container_runtime"] = field
+    if field is not None:
+        args["container_runtime"] = field
 
     field = data.get("autohealing", None)
-    args["autohealing"] = field
+    if field is not None:
+        args["autohealing"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("kubelet_args", None)
-    args["kubelet_args"] = field
+    if field is not None:
+        args["kubelet_args"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("root_volume_type", None)
-    args["root_volume_type"] = field
+    if field is not None:
+        args["root_volume_type"] = field
 
     field = data.get("public_ip_disabled", None)
-    args["public_ip_disabled"] = field
+    if field is not None:
+        args["public_ip_disabled"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("placement_group_id", None)
-    args["placement_group_id"] = field
+    if field is not None:
+        args["placement_group_id"] = field
 
     field = data.get("upgrade_policy", None)
-    args["upgrade_policy"] = unmarshal_PoolUpgradePolicy(field)
+    if field is not None:
+        args["upgrade_policy"] = unmarshal_PoolUpgradePolicy(field)
 
     field = data.get("root_volume_size", None)
-    args["root_volume_size"] = field
+    if field is not None:
+        args["root_volume_size"] = field
 
     return Pool(**args)
 
 
 def unmarshal_Version(data: Any) -> Version:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Version' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("label", None)
-    args["label"] = field
+    if field is not None:
+        args["label"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("available_cnis", None)
-    args["available_cnis"] = [CNI(v) for v in field] if field is not None else None
+    if field is not None:
+        args["available_cnis"] = [CNI(v) for v in field] if field is not None else None
 
     field = data.get("available_container_runtimes", None)
-    args["available_container_runtimes"] = (
-        [Runtime(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_container_runtimes"] = (
+            [Runtime(v) for v in field] if field is not None else None
+        )
 
     field = data.get("available_feature_gates", None)
-    args["available_feature_gates"] = field
+    if field is not None:
+        args["available_feature_gates"] = field
 
     field = data.get("available_admission_plugins", None)
-    args["available_admission_plugins"] = field
+    if field is not None:
+        args["available_admission_plugins"] = field
 
     field = data.get("available_kubelet_args", None)
-    args["available_kubelet_args"] = field
+    if field is not None:
+        args["available_kubelet_args"] = field
 
     field = data.get("available_ingresses", None)
-    args["available_ingresses"] = (
-        [Ingress(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_ingresses"] = (
+            [Ingress(v) for v in field] if field is not None else None
+        )
 
     return Version(**args)
 
 
 def unmarshal_MaintenanceWindow(data: Any) -> MaintenanceWindow:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'MaintenanceWindow' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("start_hour", None)
-    args["start_hour"] = field
+    if field is not None:
+        args["start_hour"] = field
 
     field = data.get("day", None)
-    args["day"] = field
+    if field is not None:
+        args["day"] = field
 
     return MaintenanceWindow(**args)
 
 
 def unmarshal_ClusterAutoUpgrade(data: Any) -> ClusterAutoUpgrade:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterAutoUpgrade' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("enabled", None)
-    args["enabled"] = field
+    if field is not None:
+        args["enabled"] = field
 
     field = data.get("maintenance_window", None)
-    args["maintenance_window"] = unmarshal_MaintenanceWindow(field)
+    if field is not None:
+        args["maintenance_window"] = unmarshal_MaintenanceWindow(field)
 
     return ClusterAutoUpgrade(**args)
 
 
 def unmarshal_ClusterAutoscalerConfig(data: Any) -> ClusterAutoscalerConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterAutoscalerConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("scale_down_disabled", None)
-    args["scale_down_disabled"] = field
+    if field is not None:
+        args["scale_down_disabled"] = field
 
     field = data.get("scale_down_delay_after_add", None)
-    args["scale_down_delay_after_add"] = field
+    if field is not None:
+        args["scale_down_delay_after_add"] = field
 
     field = data.get("estimator", None)
-    args["estimator"] = field
+    if field is not None:
+        args["estimator"] = field
 
     field = data.get("expander", None)
-    args["expander"] = field
+    if field is not None:
+        args["expander"] = field
 
     field = data.get("ignore_daemonsets_utilization", None)
-    args["ignore_daemonsets_utilization"] = field
+    if field is not None:
+        args["ignore_daemonsets_utilization"] = field
 
     field = data.get("balance_similar_node_groups", None)
-    args["balance_similar_node_groups"] = field
+    if field is not None:
+        args["balance_similar_node_groups"] = field
 
     field = data.get("expendable_pods_priority_cutoff", None)
-    args["expendable_pods_priority_cutoff"] = field
+    if field is not None:
+        args["expendable_pods_priority_cutoff"] = field
 
     field = data.get("scale_down_unneeded_time", None)
-    args["scale_down_unneeded_time"] = field
+    if field is not None:
+        args["scale_down_unneeded_time"] = field
 
     field = data.get("scale_down_utilization_threshold", None)
-    args["scale_down_utilization_threshold"] = field
+    if field is not None:
+        args["scale_down_utilization_threshold"] = field
 
     field = data.get("max_graceful_termination_sec", None)
-    args["max_graceful_termination_sec"] = field
+    if field is not None:
+        args["max_graceful_termination_sec"] = field
 
     return ClusterAutoscalerConfig(**args)
 
 
 def unmarshal_ClusterOpenIDConnectConfig(data: Any) -> ClusterOpenIDConnectConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterOpenIDConnectConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("issuer_url", None)
-    args["issuer_url"] = field
+    if field is not None:
+        args["issuer_url"] = field
 
     field = data.get("client_id", None)
-    args["client_id"] = field
+    if field is not None:
+        args["client_id"] = field
 
     field = data.get("username_claim", None)
-    args["username_claim"] = field
+    if field is not None:
+        args["username_claim"] = field
 
     field = data.get("username_prefix", None)
-    args["username_prefix"] = field
+    if field is not None:
+        args["username_prefix"] = field
 
     field = data.get("groups_claim", None)
-    args["groups_claim"] = field
+    if field is not None:
+        args["groups_claim"] = field
 
     field = data.get("groups_prefix", None)
-    args["groups_prefix"] = field
+    if field is not None:
+        args["groups_prefix"] = field
 
     field = data.get("required_claim", None)
-    args["required_claim"] = field
+    if field is not None:
+        args["required_claim"] = field
 
     return ClusterOpenIDConnectConfig(**args)
 
 
 def unmarshal_Cluster(data: Any) -> Cluster:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Cluster' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("cni", None)
-    args["cni"] = field
+    if field is not None:
+        args["cni"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("cluster_url", None)
-    args["cluster_url"] = field
+    if field is not None:
+        args["cluster_url"] = field
 
     field = data.get("dns_wildcard", None)
-    args["dns_wildcard"] = field
+    if field is not None:
+        args["dns_wildcard"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("autoscaler_config", None)
-    args["autoscaler_config"] = unmarshal_ClusterAutoscalerConfig(field)
+    if field is not None:
+        args["autoscaler_config"] = unmarshal_ClusterAutoscalerConfig(field)
 
     field = data.get("dashboard_enabled", None)
-    args["dashboard_enabled"] = field
+    if field is not None:
+        args["dashboard_enabled"] = field
 
     field = data.get("ingress", None)
-    args["ingress"] = field
+    if field is not None:
+        args["ingress"] = field
 
     field = data.get("auto_upgrade", None)
-    args["auto_upgrade"] = unmarshal_ClusterAutoUpgrade(field)
+    if field is not None:
+        args["auto_upgrade"] = unmarshal_ClusterAutoUpgrade(field)
 
     field = data.get("upgrade_available", None)
-    args["upgrade_available"] = field
+    if field is not None:
+        args["upgrade_available"] = field
 
     field = data.get("feature_gates", None)
-    args["feature_gates"] = field
+    if field is not None:
+        args["feature_gates"] = field
 
     field = data.get("admission_plugins", None)
-    args["admission_plugins"] = field
+    if field is not None:
+        args["admission_plugins"] = field
 
     field = data.get("apiserver_cert_sans", None)
-    args["apiserver_cert_sans"] = field
+    if field is not None:
+        args["apiserver_cert_sans"] = field
 
     field = data.get("open_id_connect_config", None)
-    args["open_id_connect_config"] = unmarshal_ClusterOpenIDConnectConfig(field)
+    if field is not None:
+        args["open_id_connect_config"] = unmarshal_ClusterOpenIDConnectConfig(field)
 
     field = data.get("private_network_id", None)
-    args["private_network_id"] = field
+    if field is not None:
+        args["private_network_id"] = field
 
     field = data.get("commitment_ends_at", None)
-    args["commitment_ends_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["commitment_ends_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return Cluster(**args)
 
 
 def unmarshal_Node(data: Any) -> Node:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Node' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("pool_id", None)
-    args["pool_id"] = field
+    if field is not None:
+        args["pool_id"] = field
 
     field = data.get("cluster_id", None)
-    args["cluster_id"] = field
+    if field is not None:
+        args["cluster_id"] = field
 
     field = data.get("provider_id", None)
-    args["provider_id"] = field
+    if field is not None:
+        args["provider_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("public_ip_v4", None)
-    args["public_ip_v4"] = field
+    if field is not None:
+        args["public_ip_v4"] = field
 
     field = data.get("public_ip_v6", None)
-    args["public_ip_v6"] = field
+    if field is not None:
+        args["public_ip_v6"] = field
 
     field = data.get("conditions", None)
-    args["conditions"] = field
+    if field is not None:
+        args["conditions"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("error_message", None)
-    args["error_message"] = field
+    if field is not None:
+        args["error_message"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Node(**args)
 
 
 def unmarshal_ExternalNode(data: Any) -> ExternalNode:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ExternalNode' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("cluster_url", None)
-    args["cluster_url"] = field
+    if field is not None:
+        args["cluster_url"] = field
 
     field = data.get("pool_version", None)
-    args["pool_version"] = field
+    if field is not None:
+        args["pool_version"] = field
 
     field = data.get("cluster_ca", None)
-    args["cluster_ca"] = field
+    if field is not None:
+        args["cluster_ca"] = field
 
     field = data.get("kube_token", None)
-    args["kube_token"] = field
+    if field is not None:
+        args["kube_token"] = field
 
     field = data.get("kubelet_config", None)
-    args["kubelet_config"] = field
+    if field is not None:
+        args["kubelet_config"] = field
 
     field = data.get("external_ip", None)
-    args["external_ip"] = field
+    if field is not None:
+        args["external_ip"] = field
 
     return ExternalNode(**args)
 
 
 def unmarshal_ClusterType(data: Any) -> ClusterType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("availability", None)
-    args["availability"] = field
+    if field is not None:
+        args["availability"] = field
 
     field = data.get("max_nodes", None)
-    args["max_nodes"] = field
+    if field is not None:
+        args["max_nodes"] = field
 
     field = data.get("sla", None)
-    args["sla"] = field
+    if field is not None:
+        args["sla"] = field
 
     field = data.get("resiliency", None)
-    args["resiliency"] = field
+    if field is not None:
+        args["resiliency"] = field
 
     field = data.get("memory", None)
-    args["memory"] = field
+    if field is not None:
+        args["memory"] = field
 
     field = data.get("dedicated", None)
-    args["dedicated"] = field
+    if field is not None:
+        args["dedicated"] = field
 
     field = data.get("commitment_delay", None)
-    args["commitment_delay"] = field
+    if field is not None:
+        args["commitment_delay"] = field
 
     return ClusterType(**args)
 
 
 def unmarshal_ListClusterAvailableTypesResponse(
     data: Any,
 ) -> ListClusterAvailableTypesResponse:
@@ -516,20 +626,22 @@
         raise TypeError(
             "Unmarshalling the type 'ListClusterAvailableTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("cluster_types", None)
-    args["cluster_types"] = (
-        [unmarshal_ClusterType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["cluster_types"] = (
+            [unmarshal_ClusterType(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListClusterAvailableTypesResponse(**args)
 
 
 def unmarshal_ListClusterAvailableVersionsResponse(
     data: Any,
 ) -> ListClusterAvailableVersionsResponse:
@@ -537,105 +649,119 @@
         raise TypeError(
             "Unmarshalling the type 'ListClusterAvailableVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_Version(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_Version(v) for v in field] if field is not None else None
+        )
 
     return ListClusterAvailableVersionsResponse(**args)
 
 
 def unmarshal_ListClusterTypesResponse(data: Any) -> ListClusterTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListClusterTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("cluster_types", None)
-    args["cluster_types"] = (
-        [unmarshal_ClusterType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["cluster_types"] = (
+            [unmarshal_ClusterType(v) for v in field] if field is not None else None
+        )
 
     return ListClusterTypesResponse(**args)
 
 
 def unmarshal_ListClustersResponse(data: Any) -> ListClustersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListClustersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("clusters", None)
-    args["clusters"] = (
-        [unmarshal_Cluster(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["clusters"] = (
+            [unmarshal_Cluster(v) for v in field] if field is not None else None
+        )
 
     return ListClustersResponse(**args)
 
 
 def unmarshal_ListNodesResponse(data: Any) -> ListNodesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNodesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("nodes", None)
-    args["nodes"] = [unmarshal_Node(v) for v in field] if field is not None else None
+    if field is not None:
+        args["nodes"] = (
+            [unmarshal_Node(v) for v in field] if field is not None else None
+        )
 
     return ListNodesResponse(**args)
 
 
 def unmarshal_ListPoolsResponse(data: Any) -> ListPoolsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPoolsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("pools", None)
-    args["pools"] = [unmarshal_Pool(v) for v in field] if field is not None else None
+    if field is not None:
+        args["pools"] = (
+            [unmarshal_Pool(v) for v in field] if field is not None else None
+        )
 
     return ListPoolsResponse(**args)
 
 
 def unmarshal_ListVersionsResponse(data: Any) -> ListVersionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_Version(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_Version(v) for v in field] if field is not None else None
+        )
 
     return ListVersionsResponse(**args)
 
 
 def marshal_MaintenanceWindow(
     request: MaintenanceWindow,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/k8s/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/k8s/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/k8s/v1/types_private.py` & `scaleway-2.0.0.dev6/scaleway/k8s/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/lb/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/lb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/lb/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/lb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/lb/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/lb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/lb/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/lb/v1/marshalling.py`

 * *Files 18% similar despite different names*

```diff
@@ -110,136 +110,159 @@
         raise TypeError(
             "Unmarshalling the type 'Ip' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("ip_address", None)
-    args["ip_address"] = field
+    if field is not None:
+        args["ip_address"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("reverse", None)
-    args["reverse"] = field
+    if field is not None:
+        args["reverse"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("lb_id", None)
-    args["lb_id"] = field
+    if field is not None:
+        args["lb_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return Ip(**args)
 
 
 def unmarshal_SubscriberEmailConfig(data: Any) -> SubscriberEmailConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SubscriberEmailConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("email", None)
-    args["email"] = field
+    if field is not None:
+        args["email"] = field
 
     return SubscriberEmailConfig(**args)
 
 
 def unmarshal_SubscriberWebhookConfig(data: Any) -> SubscriberWebhookConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SubscriberWebhookConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("uri", None)
-    args["uri"] = field
+    if field is not None:
+        args["uri"] = field
 
     return SubscriberWebhookConfig(**args)
 
 
 def unmarshal_Subscriber(data: Any) -> Subscriber:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Subscriber' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("email_config", None)
-    args["email_config"] = unmarshal_SubscriberEmailConfig(field)
+    if field is not None:
+        args["email_config"] = unmarshal_SubscriberEmailConfig(field)
 
     field = data.get("webhook_config", None)
-    args["webhook_config"] = unmarshal_SubscriberWebhookConfig(field)
+    if field is not None:
+        args["webhook_config"] = unmarshal_SubscriberWebhookConfig(field)
 
     return Subscriber(**args)
 
 
 def unmarshal_HealthCheckHttpConfig(data: Any) -> HealthCheckHttpConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'HealthCheckHttpConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("uri", None)
-    args["uri"] = field
+    if field is not None:
+        args["uri"] = field
 
     field = data.get("method", None)
-    args["method"] = field
+    if field is not None:
+        args["method"] = field
 
     field = data.get("host_header", None)
-    args["host_header"] = field
+    if field is not None:
+        args["host_header"] = field
 
     field = data.get("code", None)
-    args["code"] = field
+    if field is not None:
+        args["code"] = field
 
     return HealthCheckHttpConfig(**args)
 
 
 def unmarshal_HealthCheckHttpsConfig(data: Any) -> HealthCheckHttpsConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'HealthCheckHttpsConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("uri", None)
-    args["uri"] = field
+    if field is not None:
+        args["uri"] = field
 
     field = data.get("method", None)
-    args["method"] = field
+    if field is not None:
+        args["method"] = field
 
     field = data.get("host_header", None)
-    args["host_header"] = field
+    if field is not None:
+        args["host_header"] = field
 
     field = data.get("sni", None)
-    args["sni"] = field
+    if field is not None:
+        args["sni"] = field
 
     field = data.get("code", None)
-    args["code"] = field
+    if field is not None:
+        args["code"] = field
 
     return HealthCheckHttpsConfig(**args)
 
 
 def unmarshal_HealthCheckLdapConfig(data: Any) -> HealthCheckLdapConfig:
     if not isinstance(data, dict):
         raise TypeError(
@@ -256,29 +279,31 @@
         raise TypeError(
             "Unmarshalling the type 'HealthCheckMysqlConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("user", None)
-    args["user"] = field
+    if field is not None:
+        args["user"] = field
 
     return HealthCheckMysqlConfig(**args)
 
 
 def unmarshal_HealthCheckPgsqlConfig(data: Any) -> HealthCheckPgsqlConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'HealthCheckPgsqlConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("user", None)
-    args["user"] = field
+    if field is not None:
+        args["user"] = field
 
     return HealthCheckPgsqlConfig(**args)
 
 
 def unmarshal_HealthCheckRedisConfig(data: Any) -> HealthCheckRedisConfig:
     if not isinstance(data, dict):
         raise TypeError(
@@ -306,455 +331,564 @@
         raise TypeError(
             "Unmarshalling the type 'HealthCheck' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     field = data.get("check_max_retries", None)
-    args["check_max_retries"] = field
+    if field is not None:
+        args["check_max_retries"] = field
 
     field = data.get("check_delay", None)
-    args["check_delay"] = field
+    if field is not None:
+        args["check_delay"] = field
 
     field = data.get("check_timeout", None)
-    args["check_timeout"] = field
+    if field is not None:
+        args["check_timeout"] = field
 
     field = data.get("tcp_config", None)
-    args["tcp_config"] = unmarshal_HealthCheckTcpConfig(field)
+    if field is not None:
+        args["tcp_config"] = unmarshal_HealthCheckTcpConfig(field)
 
     field = data.get("mysql_config", None)
-    args["mysql_config"] = unmarshal_HealthCheckMysqlConfig(field)
+    if field is not None:
+        args["mysql_config"] = unmarshal_HealthCheckMysqlConfig(field)
 
     field = data.get("check_send_proxy", None)
-    args["check_send_proxy"] = field
+    if field is not None:
+        args["check_send_proxy"] = field
 
     field = data.get("pgsql_config", None)
-    args["pgsql_config"] = unmarshal_HealthCheckPgsqlConfig(field)
+    if field is not None:
+        args["pgsql_config"] = unmarshal_HealthCheckPgsqlConfig(field)
 
     field = data.get("ldap_config", None)
-    args["ldap_config"] = unmarshal_HealthCheckLdapConfig(field)
+    if field is not None:
+        args["ldap_config"] = unmarshal_HealthCheckLdapConfig(field)
 
     field = data.get("redis_config", None)
-    args["redis_config"] = unmarshal_HealthCheckRedisConfig(field)
+    if field is not None:
+        args["redis_config"] = unmarshal_HealthCheckRedisConfig(field)
 
     field = data.get("http_config", None)
-    args["http_config"] = unmarshal_HealthCheckHttpConfig(field)
+    if field is not None:
+        args["http_config"] = unmarshal_HealthCheckHttpConfig(field)
 
     field = data.get("https_config", None)
-    args["https_config"] = unmarshal_HealthCheckHttpsConfig(field)
+    if field is not None:
+        args["https_config"] = unmarshal_HealthCheckHttpsConfig(field)
 
     field = data.get("transient_check_delay", None)
-    args["transient_check_delay"] = field
+    if field is not None:
+        args["transient_check_delay"] = field
 
     return HealthCheck(**args)
 
 
 def unmarshal_Instance(data: Any) -> Instance:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Instance' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("ip_address", None)
-    args["ip_address"] = field
+    if field is not None:
+        args["ip_address"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return Instance(**args)
 
 
 def unmarshal_Lb(data: Any) -> Lb:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Lb' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("instances", None)
-    args["instances"] = (
-        [unmarshal_Instance(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["instances"] = (
+            [unmarshal_Instance(v) for v in field] if field is not None else None
+        )
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("ip", None)
-    args["ip"] = [unmarshal_Ip(v) for v in field] if field is not None else None
+    if field is not None:
+        args["ip"] = [unmarshal_Ip(v) for v in field] if field is not None else None
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("frontend_count", None)
-    args["frontend_count"] = field
+    if field is not None:
+        args["frontend_count"] = field
 
     field = data.get("backend_count", None)
-    args["backend_count"] = field
+    if field is not None:
+        args["backend_count"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("ssl_compatibility_level", None)
-    args["ssl_compatibility_level"] = field
+    if field is not None:
+        args["ssl_compatibility_level"] = field
 
     field = data.get("private_network_count", None)
-    args["private_network_count"] = field
+    if field is not None:
+        args["private_network_count"] = field
 
     field = data.get("route_count", None)
-    args["route_count"] = field
+    if field is not None:
+        args["route_count"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("subscriber", None)
-    args["subscriber"] = unmarshal_Subscriber(field)
+    if field is not None:
+        args["subscriber"] = unmarshal_Subscriber(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return Lb(**args)
 
 
 def unmarshal_Backend(data: Any) -> Backend:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Backend' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("forward_protocol", None)
-    args["forward_protocol"] = field
+    if field is not None:
+        args["forward_protocol"] = field
 
     field = data.get("forward_port", None)
-    args["forward_port"] = field
+    if field is not None:
+        args["forward_port"] = field
 
     field = data.get("forward_port_algorithm", None)
-    args["forward_port_algorithm"] = field
+    if field is not None:
+        args["forward_port_algorithm"] = field
 
     field = data.get("sticky_sessions", None)
-    args["sticky_sessions"] = field
+    if field is not None:
+        args["sticky_sessions"] = field
 
     field = data.get("sticky_sessions_cookie_name", None)
-    args["sticky_sessions_cookie_name"] = field
+    if field is not None:
+        args["sticky_sessions_cookie_name"] = field
 
     field = data.get("pool", None)
-    args["pool"] = field
+    if field is not None:
+        args["pool"] = field
 
     field = data.get("on_marked_down_action", None)
-    args["on_marked_down_action"] = field
+    if field is not None:
+        args["on_marked_down_action"] = field
 
     field = data.get("proxy_protocol", None)
-    args["proxy_protocol"] = field
+    if field is not None:
+        args["proxy_protocol"] = field
 
     field = data.get("health_check", None)
-    args["health_check"] = unmarshal_HealthCheck(field)
+    if field is not None:
+        args["health_check"] = unmarshal_HealthCheck(field)
 
     field = data.get("lb", None)
-    args["lb"] = unmarshal_Lb(field)
+    if field is not None:
+        args["lb"] = unmarshal_Lb(field)
 
     field = data.get("send_proxy_v2", None)
-    args["send_proxy_v2"] = field
+    if field is not None:
+        args["send_proxy_v2"] = field
 
     field = data.get("timeout_server", None)
-    args["timeout_server"] = field
+    if field is not None:
+        args["timeout_server"] = field
 
     field = data.get("timeout_connect", None)
-    args["timeout_connect"] = field
+    if field is not None:
+        args["timeout_connect"] = field
 
     field = data.get("timeout_tunnel", None)
-    args["timeout_tunnel"] = field
+    if field is not None:
+        args["timeout_tunnel"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("failover_host", None)
-    args["failover_host"] = field
+    if field is not None:
+        args["failover_host"] = field
 
     field = data.get("ssl_bridging", None)
-    args["ssl_bridging"] = field
+    if field is not None:
+        args["ssl_bridging"] = field
 
     field = data.get("ignore_ssl_server_verify", None)
-    args["ignore_ssl_server_verify"] = field
+    if field is not None:
+        args["ignore_ssl_server_verify"] = field
 
     field = data.get("redispatch_attempt_count", None)
-    args["redispatch_attempt_count"] = field
+    if field is not None:
+        args["redispatch_attempt_count"] = field
 
     field = data.get("max_retries", None)
-    args["max_retries"] = field
+    if field is not None:
+        args["max_retries"] = field
 
     field = data.get("max_connections", None)
-    args["max_connections"] = field
+    if field is not None:
+        args["max_connections"] = field
 
     field = data.get("timeout_queue", None)
-    args["timeout_queue"] = field
+    if field is not None:
+        args["timeout_queue"] = field
 
     return Backend(**args)
 
 
 def unmarshal_Certificate(data: Any) -> Certificate:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Certificate' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("common_name", None)
-    args["common_name"] = field
+    if field is not None:
+        args["common_name"] = field
 
     field = data.get("subject_alternative_name", None)
-    args["subject_alternative_name"] = field
+    if field is not None:
+        args["subject_alternative_name"] = field
 
     field = data.get("fingerprint", None)
-    args["fingerprint"] = field
+    if field is not None:
+        args["fingerprint"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("not_valid_before", None)
-    args["not_valid_before"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["not_valid_before"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("not_valid_after", None)
-    args["not_valid_after"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["not_valid_after"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("lb", None)
-    args["lb"] = unmarshal_Lb(field)
+    if field is not None:
+        args["lb"] = unmarshal_Lb(field)
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("status_details", None)
-    args["status_details"] = field
+    if field is not None:
+        args["status_details"] = field
 
     return Certificate(**args)
 
 
 def unmarshal_Frontend(data: Any) -> Frontend:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Frontend' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("inbound_port", None)
-    args["inbound_port"] = field
+    if field is not None:
+        args["inbound_port"] = field
 
     field = data.get("certificate_ids", None)
-    args["certificate_ids"] = field
+    if field is not None:
+        args["certificate_ids"] = field
 
     field = data.get("enable_http3", None)
-    args["enable_http3"] = field
+    if field is not None:
+        args["enable_http3"] = field
 
     field = data.get("backend", None)
-    args["backend"] = unmarshal_Backend(field)
+    if field is not None:
+        args["backend"] = unmarshal_Backend(field)
 
     field = data.get("lb", None)
-    args["lb"] = unmarshal_Lb(field)
+    if field is not None:
+        args["lb"] = unmarshal_Lb(field)
 
     field = data.get("timeout_client", None)
-    args["timeout_client"] = field
+    if field is not None:
+        args["timeout_client"] = field
 
     field = data.get("certificate", None)
-    args["certificate"] = unmarshal_Certificate(field)
+    if field is not None:
+        args["certificate"] = unmarshal_Certificate(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Frontend(**args)
 
 
 def unmarshal_AclActionRedirect(data: Any) -> AclActionRedirect:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AclActionRedirect' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("target", None)
-    args["target"] = field
+    if field is not None:
+        args["target"] = field
 
     field = data.get("code", None)
-    args["code"] = field
+    if field is not None:
+        args["code"] = field
 
     return AclActionRedirect(**args)
 
 
 def unmarshal_AclAction(data: Any) -> AclAction:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AclAction' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("redirect", None)
-    args["redirect"] = unmarshal_AclActionRedirect(field)
+    if field is not None:
+        args["redirect"] = unmarshal_AclActionRedirect(field)
 
     return AclAction(**args)
 
 
 def unmarshal_AclMatch(data: Any) -> AclMatch:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AclMatch' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip_subnet", None)
-    args["ip_subnet"] = field
+    if field is not None:
+        args["ip_subnet"] = field
 
     field = data.get("http_filter", None)
-    args["http_filter"] = field
+    if field is not None:
+        args["http_filter"] = field
 
     field = data.get("http_filter_value", None)
-    args["http_filter_value"] = field
+    if field is not None:
+        args["http_filter_value"] = field
 
     field = data.get("invert", None)
-    args["invert"] = field
+    if field is not None:
+        args["invert"] = field
 
     field = data.get("http_filter_option", None)
-    args["http_filter_option"] = field
+    if field is not None:
+        args["http_filter_option"] = field
 
     return AclMatch(**args)
 
 
 def unmarshal_Acl(data: Any) -> Acl:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Acl' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("index", None)
-    args["index"] = field
+    if field is not None:
+        args["index"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("match", None)
-    args["match"] = unmarshal_AclMatch(field)
+    if field is not None:
+        args["match"] = unmarshal_AclMatch(field)
 
     field = data.get("action", None)
-    args["action"] = unmarshal_AclAction(field)
+    if field is not None:
+        args["action"] = unmarshal_AclAction(field)
 
     field = data.get("frontend", None)
-    args["frontend"] = unmarshal_Frontend(field)
+    if field is not None:
+        args["frontend"] = unmarshal_Frontend(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Acl(**args)
 
 
 def unmarshal_PrivateNetworkDHCPConfig(data: Any) -> PrivateNetworkDHCPConfig:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PrivateNetworkDHCPConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip_id", None)
-    args["ip_id"] = field
+    if field is not None:
+        args["ip_id"] = field
 
     return PrivateNetworkDHCPConfig(**args)
 
 
 def unmarshal_PrivateNetworkIpamConfig(data: Any) -> PrivateNetworkIpamConfig:
     if not isinstance(data, dict):
         raise TypeError(
@@ -771,390 +905,450 @@
         raise TypeError(
             "Unmarshalling the type 'PrivateNetworkStaticConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip_address", None)
-    args["ip_address"] = field
+    if field is not None:
+        args["ip_address"] = field
 
     return PrivateNetworkStaticConfig(**args)
 
 
 def unmarshal_PrivateNetwork(data: Any) -> PrivateNetwork:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PrivateNetwork' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ipam_ids", None)
-    args["ipam_ids"] = field
+    if field is not None:
+        args["ipam_ids"] = field
 
     field = data.get("private_network_id", None)
-    args["private_network_id"] = field
+    if field is not None:
+        args["private_network_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("lb", None)
-    args["lb"] = unmarshal_Lb(field)
+    if field is not None:
+        args["lb"] = unmarshal_Lb(field)
 
     field = data.get("static_config", None)
-    args["static_config"] = unmarshal_PrivateNetworkStaticConfig(field)
+    if field is not None:
+        args["static_config"] = unmarshal_PrivateNetworkStaticConfig(field)
 
     field = data.get("dhcp_config", None)
-    args["dhcp_config"] = unmarshal_PrivateNetworkDHCPConfig(field)
+    if field is not None:
+        args["dhcp_config"] = unmarshal_PrivateNetworkDHCPConfig(field)
 
     field = data.get("ipam_config", None)
-    args["ipam_config"] = unmarshal_PrivateNetworkIpamConfig(field)
+    if field is not None:
+        args["ipam_config"] = unmarshal_PrivateNetworkIpamConfig(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return PrivateNetwork(**args)
 
 
 def unmarshal_RouteMatch(data: Any) -> RouteMatch:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'RouteMatch' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("sni", None)
-    args["sni"] = field
+    if field is not None:
+        args["sni"] = field
 
     field = data.get("host_header", None)
-    args["host_header"] = field
+    if field is not None:
+        args["host_header"] = field
 
     return RouteMatch(**args)
 
 
 def unmarshal_Route(data: Any) -> Route:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Route' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("frontend_id", None)
-    args["frontend_id"] = field
+    if field is not None:
+        args["frontend_id"] = field
 
     field = data.get("backend_id", None)
-    args["backend_id"] = field
+    if field is not None:
+        args["backend_id"] = field
 
     field = data.get("match", None)
-    args["match"] = unmarshal_RouteMatch(field)
+    if field is not None:
+        args["match"] = unmarshal_RouteMatch(field)
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Route(**args)
 
 
 def unmarshal_BackendServerStats(data: Any) -> BackendServerStats:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'BackendServerStats' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("instance_id", None)
-    args["instance_id"] = field
+    if field is not None:
+        args["instance_id"] = field
 
     field = data.get("backend_id", None)
-    args["backend_id"] = field
+    if field is not None:
+        args["backend_id"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("server_state", None)
-    args["server_state"] = field
+    if field is not None:
+        args["server_state"] = field
 
     field = data.get("last_health_check_status", None)
-    args["last_health_check_status"] = field
+    if field is not None:
+        args["last_health_check_status"] = field
 
     field = data.get("server_state_changed_at", None)
-    args["server_state_changed_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["server_state_changed_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return BackendServerStats(**args)
 
 
 def unmarshal_LbStats(data: Any) -> LbStats:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'LbStats' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("backend_servers_stats", None)
-    args["backend_servers_stats"] = (
-        [unmarshal_BackendServerStats(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["backend_servers_stats"] = (
+            [unmarshal_BackendServerStats(v) for v in field]
+            if field is not None
+            else None
+        )
 
     return LbStats(**args)
 
 
 def unmarshal_ListAclResponse(data: Any) -> ListAclResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListAclResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("acls", None)
-    args["acls"] = [unmarshal_Acl(v) for v in field] if field is not None else None
+    if field is not None:
+        args["acls"] = [unmarshal_Acl(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListAclResponse(**args)
 
 
 def unmarshal_ListBackendStatsResponse(data: Any) -> ListBackendStatsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListBackendStatsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("backend_servers_stats", None)
-    args["backend_servers_stats"] = (
-        [unmarshal_BackendServerStats(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["backend_servers_stats"] = (
+            [unmarshal_BackendServerStats(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListBackendStatsResponse(**args)
 
 
 def unmarshal_ListBackendsResponse(data: Any) -> ListBackendsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListBackendsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("backends", None)
-    args["backends"] = (
-        [unmarshal_Backend(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["backends"] = (
+            [unmarshal_Backend(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListBackendsResponse(**args)
 
 
 def unmarshal_ListCertificatesResponse(data: Any) -> ListCertificatesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListCertificatesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("certificates", None)
-    args["certificates"] = (
-        [unmarshal_Certificate(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["certificates"] = (
+            [unmarshal_Certificate(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListCertificatesResponse(**args)
 
 
 def unmarshal_ListFrontendsResponse(data: Any) -> ListFrontendsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListFrontendsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("frontends", None)
-    args["frontends"] = (
-        [unmarshal_Frontend(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["frontends"] = (
+            [unmarshal_Frontend(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListFrontendsResponse(**args)
 
 
 def unmarshal_ListIpsResponse(data: Any) -> ListIpsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListIpsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ips", None)
-    args["ips"] = [unmarshal_Ip(v) for v in field] if field is not None else None
+    if field is not None:
+        args["ips"] = [unmarshal_Ip(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListIpsResponse(**args)
 
 
 def unmarshal_ListLbPrivateNetworksResponse(data: Any) -> ListLbPrivateNetworksResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListLbPrivateNetworksResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_network", None)
-    args["private_network"] = (
-        [unmarshal_PrivateNetwork(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["private_network"] = (
+            [unmarshal_PrivateNetwork(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListLbPrivateNetworksResponse(**args)
 
 
 def unmarshal_LbType(data: Any) -> LbType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'LbType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("stock_status", None)
-    args["stock_status"] = field
+    if field is not None:
+        args["stock_status"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return LbType(**args)
 
 
 def unmarshal_ListLbTypesResponse(data: Any) -> ListLbTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListLbTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("lb_types", None)
-    args["lb_types"] = (
-        [unmarshal_LbType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["lb_types"] = (
+            [unmarshal_LbType(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListLbTypesResponse(**args)
 
 
 def unmarshal_ListLbsResponse(data: Any) -> ListLbsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListLbsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("lbs", None)
-    args["lbs"] = [unmarshal_Lb(v) for v in field] if field is not None else None
+    if field is not None:
+        args["lbs"] = [unmarshal_Lb(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListLbsResponse(**args)
 
 
 def unmarshal_ListRoutesResponse(data: Any) -> ListRoutesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListRoutesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("routes", None)
-    args["routes"] = [unmarshal_Route(v) for v in field] if field is not None else None
+    if field is not None:
+        args["routes"] = (
+            [unmarshal_Route(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListRoutesResponse(**args)
 
 
 def unmarshal_ListSubscriberResponse(data: Any) -> ListSubscriberResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSubscriberResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("subscribers", None)
-    args["subscribers"] = (
-        [unmarshal_Subscriber(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["subscribers"] = (
+            [unmarshal_Subscriber(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSubscriberResponse(**args)
 
 
 def unmarshal_SetAclsResponse(data: Any) -> SetAclsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetAclsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("acls", None)
-    args["acls"] = [unmarshal_Acl(v) for v in field] if field is not None else None
+    if field is not None:
+        args["acls"] = [unmarshal_Acl(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return SetAclsResponse(**args)
 
 
 def marshal_AddBackendServersRequest(
     request: AddBackendServersRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/lb/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/lb/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v1/marshalling.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,181 +21,218 @@
         raise TypeError(
             "Unmarshalling the type 'LocalImage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("compatible_commercial_types", None)
-    args["compatible_commercial_types"] = field
+    if field is not None:
+        args["compatible_commercial_types"] = field
 
     field = data.get("arch", None)
-    args["arch"] = field
+    if field is not None:
+        args["arch"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return LocalImage(**args)
 
 
 def unmarshal_Organization(data: Any) -> Organization:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Organization' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return Organization(**args)
 
 
 def unmarshal_Version(data: Any) -> Version:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Version' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("local_images", None)
-    args["local_images"] = (
-        [unmarshal_LocalImage(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["local_images"] = (
+            [unmarshal_LocalImage(v) for v in field] if field is not None else None
+        )
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return Version(**args)
 
 
 def unmarshal_Image(data: Any) -> Image:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Image' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("logo", None)
-    args["logo"] = field
+    if field is not None:
+        args["logo"] = field
 
     field = data.get("categories", None)
-    args["categories"] = field
+    if field is not None:
+        args["categories"] = field
 
     field = data.get("label", None)
-    args["label"] = field
+    if field is not None:
+        args["label"] = field
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_Version(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_Version(v) for v in field] if field is not None else None
+        )
 
     field = data.get("current_public_version", None)
-    args["current_public_version"] = field
+    if field is not None:
+        args["current_public_version"] = field
 
     field = data.get("creation_date", None)
-    args["creation_date"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["creation_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("modification_date", None)
-    args["modification_date"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["modification_date"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("valid_until", None)
-    args["valid_until"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["valid_until"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("organization", None)
-    args["organization"] = unmarshal_Organization(field)
+    if field is not None:
+        args["organization"] = unmarshal_Organization(field)
 
     return Image(**args)
 
 
 def unmarshal_GetImageResponse(data: Any) -> GetImageResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetImageResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("image", None)
-    args["image"] = unmarshal_Image(field)
+    if field is not None:
+        args["image"] = unmarshal_Image(field)
 
     return GetImageResponse(**args)
 
 
 def unmarshal_GetVersionResponse(data: Any) -> GetVersionResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetVersionResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("version", None)
-    args["version"] = unmarshal_Version(field)
+    if field is not None:
+        args["version"] = unmarshal_Version(field)
 
     return GetVersionResponse(**args)
 
 
 def unmarshal_ListImagesResponse(data: Any) -> ListImagesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListImagesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("images", None)
-    args["images"] = [unmarshal_Image(v) for v in field] if field is not None else None
+    if field is not None:
+        args["images"] = (
+            [unmarshal_Image(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListImagesResponse(**args)
 
 
 def unmarshal_ListVersionsResponse(data: Any) -> ListVersionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_Version(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_Version(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListVersionsResponse(**args)
```

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v2/__init__.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v2/api.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v2/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v2/marshalling.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,183 +21,220 @@
         raise TypeError(
             "Unmarshalling the type 'Category' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     return Category(**args)
 
 
 def unmarshal_Image(data: Any) -> Image:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Image' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("logo", None)
-    args["logo"] = field
+    if field is not None:
+        args["logo"] = field
 
     field = data.get("categories", None)
-    args["categories"] = field
+    if field is not None:
+        args["categories"] = field
 
     field = data.get("label", None)
-    args["label"] = field
+    if field is not None:
+        args["label"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("valid_until", None)
-    args["valid_until"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["valid_until"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return Image(**args)
 
 
 def unmarshal_LocalImage(data: Any) -> LocalImage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'LocalImage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("compatible_commercial_types", None)
-    args["compatible_commercial_types"] = field
+    if field is not None:
+        args["compatible_commercial_types"] = field
 
     field = data.get("arch", None)
-    args["arch"] = field
+    if field is not None:
+        args["arch"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("label", None)
-    args["label"] = field
+    if field is not None:
+        args["label"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     return LocalImage(**args)
 
 
 def unmarshal_Version(data: Any) -> Version:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Version' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("published_at", None)
-    args["published_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["published_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return Version(**args)
 
 
 def unmarshal_ListCategoriesResponse(data: Any) -> ListCategoriesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListCategoriesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("categories", None)
-    args["categories"] = (
-        [unmarshal_Category(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["categories"] = (
+            [unmarshal_Category(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListCategoriesResponse(**args)
 
 
 def unmarshal_ListImagesResponse(data: Any) -> ListImagesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListImagesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("images", None)
-    args["images"] = [unmarshal_Image(v) for v in field] if field is not None else None
+    if field is not None:
+        args["images"] = (
+            [unmarshal_Image(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListImagesResponse(**args)
 
 
 def unmarshal_ListLocalImagesResponse(data: Any) -> ListLocalImagesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListLocalImagesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("local_images", None)
-    args["local_images"] = (
-        [unmarshal_LocalImage(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["local_images"] = (
+            [unmarshal_LocalImage(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListLocalImagesResponse(**args)
 
 
 def unmarshal_ListVersionsResponse(data: Any) -> ListVersionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_Version(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_Version(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListVersionsResponse(**args)
```

### Comparing `scaleway-2.0.0.dev5/scaleway/marketplace/v2/types.py` & `scaleway-2.0.0.dev6/scaleway/marketplace/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/api.py` & `scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/marshalling.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,338 +38,400 @@
         raise TypeError(
             "Unmarshalling the type 'NatsAccount' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("endpoint", None)
-    args["endpoint"] = field
+    if field is not None:
+        args["endpoint"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return NatsAccount(**args)
 
 
 def unmarshal_File(data: Any) -> File:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'File' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("content", None)
-    args["content"] = field
+    if field is not None:
+        args["content"] = field
 
     return File(**args)
 
 
 def unmarshal_NatsCredentials(data: Any) -> NatsCredentials:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NatsCredentials' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("nats_account_id", None)
-    args["nats_account_id"] = field
+    if field is not None:
+        args["nats_account_id"] = field
 
     field = data.get("checksum", None)
-    args["checksum"] = field
+    if field is not None:
+        args["checksum"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("credentials", None)
-    args["credentials"] = unmarshal_File(field)
+    if field is not None:
+        args["credentials"] = unmarshal_File(field)
 
     return NatsCredentials(**args)
 
 
 def unmarshal_SnsPermissions(data: Any) -> SnsPermissions:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SnsPermissions' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("can_publish", None)
-    args["can_publish"] = field
+    if field is not None:
+        args["can_publish"] = field
 
     field = data.get("can_receive", None)
-    args["can_receive"] = field
+    if field is not None:
+        args["can_receive"] = field
 
     field = data.get("can_manage", None)
-    args["can_manage"] = field
+    if field is not None:
+        args["can_manage"] = field
 
     return SnsPermissions(**args)
 
 
 def unmarshal_SnsCredentials(data: Any) -> SnsCredentials:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SnsCredentials' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("access_key", None)
-    args["access_key"] = field
+    if field is not None:
+        args["access_key"] = field
 
     field = data.get("secret_key", None)
-    args["secret_key"] = field
+    if field is not None:
+        args["secret_key"] = field
 
     field = data.get("secret_checksum", None)
-    args["secret_checksum"] = field
+    if field is not None:
+        args["secret_checksum"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("permissions", None)
-    args["permissions"] = unmarshal_SnsPermissions(field)
+    if field is not None:
+        args["permissions"] = unmarshal_SnsPermissions(field)
 
     return SnsCredentials(**args)
 
 
 def unmarshal_SqsPermissions(data: Any) -> SqsPermissions:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SqsPermissions' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("can_publish", None)
-    args["can_publish"] = field
+    if field is not None:
+        args["can_publish"] = field
 
     field = data.get("can_receive", None)
-    args["can_receive"] = field
+    if field is not None:
+        args["can_receive"] = field
 
     field = data.get("can_manage", None)
-    args["can_manage"] = field
+    if field is not None:
+        args["can_manage"] = field
 
     return SqsPermissions(**args)
 
 
 def unmarshal_SqsCredentials(data: Any) -> SqsCredentials:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SqsCredentials' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("access_key", None)
-    args["access_key"] = field
+    if field is not None:
+        args["access_key"] = field
 
     field = data.get("secret_key", None)
-    args["secret_key"] = field
+    if field is not None:
+        args["secret_key"] = field
 
     field = data.get("secret_checksum", None)
-    args["secret_checksum"] = field
+    if field is not None:
+        args["secret_checksum"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("permissions", None)
-    args["permissions"] = unmarshal_SqsPermissions(field)
+    if field is not None:
+        args["permissions"] = unmarshal_SqsPermissions(field)
 
     return SqsCredentials(**args)
 
 
 def unmarshal_ListNatsAccountsResponse(data: Any) -> ListNatsAccountsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNatsAccountsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("nats_accounts", None)
-    args["nats_accounts"] = (
-        [unmarshal_NatsAccount(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["nats_accounts"] = (
+            [unmarshal_NatsAccount(v) for v in field] if field is not None else None
+        )
 
     return ListNatsAccountsResponse(**args)
 
 
 def unmarshal_ListNatsCredentialsResponse(data: Any) -> ListNatsCredentialsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNatsCredentialsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("nats_credentials", None)
-    args["nats_credentials"] = (
-        [unmarshal_NatsCredentials(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["nats_credentials"] = (
+            [unmarshal_NatsCredentials(v) for v in field] if field is not None else None
+        )
 
     return ListNatsCredentialsResponse(**args)
 
 
 def unmarshal_ListSnsCredentialsResponse(data: Any) -> ListSnsCredentialsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSnsCredentialsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("sns_credentials", None)
-    args["sns_credentials"] = (
-        [unmarshal_SnsCredentials(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["sns_credentials"] = (
+            [unmarshal_SnsCredentials(v) for v in field] if field is not None else None
+        )
 
     return ListSnsCredentialsResponse(**args)
 
 
 def unmarshal_ListSqsCredentialsResponse(data: Any) -> ListSqsCredentialsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSqsCredentialsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("sqs_credentials", None)
-    args["sqs_credentials"] = (
-        [unmarshal_SqsCredentials(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["sqs_credentials"] = (
+            [unmarshal_SqsCredentials(v) for v in field] if field is not None else None
+        )
 
     return ListSqsCredentialsResponse(**args)
 
 
 def unmarshal_SnsInfo(data: Any) -> SnsInfo:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SnsInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("sns_endpoint_url", None)
-    args["sns_endpoint_url"] = field
+    if field is not None:
+        args["sns_endpoint_url"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return SnsInfo(**args)
 
 
 def unmarshal_SqsInfo(data: Any) -> SqsInfo:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SqsInfo' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("sqs_endpoint_url", None)
-    args["sqs_endpoint_url"] = field
+    if field is not None:
+        args["sqs_endpoint_url"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return SqsInfo(**args)
 
 
 def marshal_NatsApiCreateNatsAccountRequest(
     request: NatsApiCreateNatsAccountRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/mnq/v1beta1/types.py` & `scaleway-2.0.0.dev6/scaleway/mnq/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/content.py` & `scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/qaas/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/qaas/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/rdb/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/rdb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/rdb/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/rdb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/rdb/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/rdb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/rdb/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/rdb/v1/marshalling.py`

 * *Files 16% similar despite different names*

```diff
@@ -124,549 +124,662 @@
         raise TypeError(
             "Unmarshalling the type 'EndpointPrivateNetworkDetails' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_network_id", None)
-    args["private_network_id"] = field
+    if field is not None:
+        args["private_network_id"] = field
 
     field = data.get("service_ip", None)
-    args["service_ip"] = field
+    if field is not None:
+        args["service_ip"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return EndpointPrivateNetworkDetails(**args)
 
 
 def unmarshal_Endpoint(data: Any) -> Endpoint:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Endpoint' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("private_network", None)
-    args["private_network"] = unmarshal_EndpointPrivateNetworkDetails(field)
+    if field is not None:
+        args["private_network"] = unmarshal_EndpointPrivateNetworkDetails(field)
 
     field = data.get("load_balancer", None)
-    args["load_balancer"] = unmarshal_EndpointLoadBalancerDetails(field)
+    if field is not None:
+        args["load_balancer"] = unmarshal_EndpointLoadBalancerDetails(field)
 
     field = data.get("direct_access", None)
-    args["direct_access"] = unmarshal_EndpointDirectAccessDetails(field)
+    if field is not None:
+        args["direct_access"] = unmarshal_EndpointDirectAccessDetails(field)
 
     field = data.get("hostname", None)
-    args["hostname"] = field
+    if field is not None:
+        args["hostname"] = field
 
     return Endpoint(**args)
 
 
 def unmarshal_ReadReplica(data: Any) -> ReadReplica:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ReadReplica' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("same_zone", None)
-    args["same_zone"] = field
+    if field is not None:
+        args["same_zone"] = field
 
     return ReadReplica(**args)
 
 
 def unmarshal_DatabaseBackup(data: Any) -> DatabaseBackup:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DatabaseBackup' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("instance_id", None)
-    args["instance_id"] = field
+    if field is not None:
+        args["instance_id"] = field
 
     field = data.get("database_name", None)
-    args["database_name"] = field
+    if field is not None:
+        args["database_name"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("instance_name", None)
-    args["instance_name"] = field
+    if field is not None:
+        args["instance_name"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("same_region", None)
-    args["same_region"] = field
+    if field is not None:
+        args["same_region"] = field
 
     field = data.get("download_url", None)
-    args["download_url"] = field
+    if field is not None:
+        args["download_url"] = field
 
     field = data.get("download_url_expires_at", None)
-    args["download_url_expires_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["download_url_expires_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return DatabaseBackup(**args)
 
 
 def unmarshal_Database(data: Any) -> Database:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Database' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("owner", None)
-    args["owner"] = field
+    if field is not None:
+        args["owner"] = field
 
     field = data.get("managed", None)
-    args["managed"] = field
+    if field is not None:
+        args["managed"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     return Database(**args)
 
 
 def unmarshal_InstanceLog(data: Any) -> InstanceLog:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceLog' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("node_name", None)
-    args["node_name"] = field
+    if field is not None:
+        args["node_name"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("download_url", None)
-    args["download_url"] = field
+    if field is not None:
+        args["download_url"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return InstanceLog(**args)
 
 
 def unmarshal_BackupSchedule(data: Any) -> BackupSchedule:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'BackupSchedule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("frequency", None)
-    args["frequency"] = field
+    if field is not None:
+        args["frequency"] = field
 
     field = data.get("retention", None)
-    args["retention"] = field
+    if field is not None:
+        args["retention"] = field
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("next_run_at", None)
-    args["next_run_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["next_run_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return BackupSchedule(**args)
 
 
 def unmarshal_InstanceSetting(data: Any) -> InstanceSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("value", None)
-    args["value"] = field
+    if field is not None:
+        args["value"] = field
 
     return InstanceSetting(**args)
 
 
 def unmarshal_LogsPolicy(data: Any) -> LogsPolicy:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'LogsPolicy' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("max_age_retention", None)
-    args["max_age_retention"] = field
+    if field is not None:
+        args["max_age_retention"] = field
 
     field = data.get("total_disk_retention", None)
-    args["total_disk_retention"] = field
+    if field is not None:
+        args["total_disk_retention"] = field
 
     return LogsPolicy(**args)
 
 
 def unmarshal_Maintenance(data: Any) -> Maintenance:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Maintenance' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("reason", None)
-    args["reason"] = field
+    if field is not None:
+        args["reason"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("starts_at", None)
-    args["starts_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["starts_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("stops_at", None)
-    args["stops_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["stops_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("closed_at", None)
-    args["closed_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["closed_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Maintenance(**args)
 
 
 def unmarshal_UpgradableVersion(data: Any) -> UpgradableVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'UpgradableVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("minor_version", None)
-    args["minor_version"] = field
+    if field is not None:
+        args["minor_version"] = field
 
     return UpgradableVersion(**args)
 
 
 def unmarshal_Volume(data: Any) -> Volume:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Volume' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("class_", None)
-    args["class_"] = field
+    if field is not None:
+        args["class_"] = field
 
     return Volume(**args)
 
 
 def unmarshal_Instance(data: Any) -> Instance:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Instance' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("volume", None)
-    args["volume"] = unmarshal_Volume(field)
+    if field is not None:
+        args["volume"] = unmarshal_Volume(field)
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("engine", None)
-    args["engine"] = field
+    if field is not None:
+        args["engine"] = field
 
     field = data.get("upgradable_version", None)
-    args["upgradable_version"] = (
-        [unmarshal_UpgradableVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["upgradable_version"] = (
+            [unmarshal_UpgradableVersion(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("is_ha_cluster", None)
-    args["is_ha_cluster"] = field
+    if field is not None:
+        args["is_ha_cluster"] = field
 
     field = data.get("endpoint", None)
-    args["endpoint"] = unmarshal_Endpoint(field)
+    if field is not None:
+        args["endpoint"] = unmarshal_Endpoint(field)
 
     field = data.get("backup_schedule", None)
-    args["backup_schedule"] = unmarshal_BackupSchedule(field)
+    if field is not None:
+        args["backup_schedule"] = unmarshal_BackupSchedule(field)
 
     field = data.get("read_replicas", None)
-    args["read_replicas"] = (
-        [unmarshal_ReadReplica(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["read_replicas"] = (
+            [unmarshal_ReadReplica(v) for v in field] if field is not None else None
+        )
 
     field = data.get("node_type", None)
-    args["node_type"] = field
+    if field is not None:
+        args["node_type"] = field
 
     field = data.get("init_settings", None)
-    args["init_settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["init_settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("backup_same_region", None)
-    args["backup_same_region"] = field
+    if field is not None:
+        args["backup_same_region"] = field
 
     field = data.get("maintenances", None)
-    args["maintenances"] = (
-        [unmarshal_Maintenance(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["maintenances"] = (
+            [unmarshal_Maintenance(v) for v in field] if field is not None else None
+        )
 
     field = data.get("logs_policy", None)
-    args["logs_policy"] = unmarshal_LogsPolicy(field)
+    if field is not None:
+        args["logs_policy"] = unmarshal_LogsPolicy(field)
 
     return Instance(**args)
 
 
 def unmarshal_Privilege(data: Any) -> Privilege:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Privilege' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("permission", None)
-    args["permission"] = field
+    if field is not None:
+        args["permission"] = field
 
     field = data.get("database_name", None)
-    args["database_name"] = field
+    if field is not None:
+        args["database_name"] = field
 
     field = data.get("user_name", None)
-    args["user_name"] = field
+    if field is not None:
+        args["user_name"] = field
 
     return Privilege(**args)
 
 
 def unmarshal_Snapshot(data: Any) -> Snapshot:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Snapshot' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("instance_id", None)
-    args["instance_id"] = field
+    if field is not None:
+        args["instance_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("instance_name", None)
-    args["instance_name"] = field
+    if field is not None:
+        args["instance_name"] = field
 
     field = data.get("node_type", None)
-    args["node_type"] = field
+    if field is not None:
+        args["node_type"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Snapshot(**args)
 
 
 def unmarshal_User(data: Any) -> User:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'User' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("is_admin", None)
-    args["is_admin"] = field
+    if field is not None:
+        args["is_admin"] = field
 
     return User(**args)
 
 
 def unmarshal_ACLRule(data: Any) -> ACLRule:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ACLRule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     field = data.get("protocol", None)
-    args["protocol"] = field
+    if field is not None:
+        args["protocol"] = field
 
     field = data.get("direction", None)
-    args["direction"] = field
+    if field is not None:
+        args["direction"] = field
 
     field = data.get("action", None)
-    args["action"] = field
+    if field is not None:
+        args["action"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     return ACLRule(**args)
 
 
 def unmarshal_AddInstanceACLRulesResponse(data: Any) -> AddInstanceACLRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return AddInstanceACLRulesResponse(**args)
 
 
 def unmarshal_AddInstanceSettingsResponse(data: Any) -> AddInstanceSettingsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddInstanceSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     return AddInstanceSettingsResponse(**args)
 
 
 def unmarshal_DeleteInstanceACLRulesResponse(
     data: Any,
 ) -> DeleteInstanceACLRulesResponse:
@@ -674,15 +787,18 @@
         raise TypeError(
             "Unmarshalling the type 'DeleteInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return DeleteInstanceACLRulesResponse(**args)
 
 
 def unmarshal_DeleteInstanceSettingsResponse(
     data: Any,
 ) -> DeleteInstanceSettingsResponse:
@@ -690,212 +806,248 @@
         raise TypeError(
             "Unmarshalling the type 'DeleteInstanceSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     return DeleteInstanceSettingsResponse(**args)
 
 
 def unmarshal_InstanceMetrics(data: Any) -> InstanceMetrics:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceMetrics' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("timeseries", None)
-    args["timeseries"] = (
-        [unmarshal_TimeSeries(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["timeseries"] = (
+            [unmarshal_TimeSeries(v) for v in field] if field is not None else None
+        )
 
     return InstanceMetrics(**args)
 
 
 def unmarshal_ListDatabaseBackupsResponse(data: Any) -> ListDatabaseBackupsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDatabaseBackupsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("database_backups", None)
-    args["database_backups"] = (
-        [unmarshal_DatabaseBackup(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["database_backups"] = (
+            [unmarshal_DatabaseBackup(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListDatabaseBackupsResponse(**args)
 
 
 def unmarshal_EngineSetting(data: Any) -> EngineSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'EngineSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("default_value", None)
-    args["default_value"] = field
+    if field is not None:
+        args["default_value"] = field
 
     field = data.get("hot_configurable", None)
-    args["hot_configurable"] = field
+    if field is not None:
+        args["hot_configurable"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("property_type", None)
-    args["property_type"] = field
+    if field is not None:
+        args["property_type"] = field
 
     field = data.get("unit", None)
-    args["unit"] = field
+    if field is not None:
+        args["unit"] = field
 
     field = data.get("string_constraint", None)
-    args["string_constraint"] = field
+    if field is not None:
+        args["string_constraint"] = field
 
     field = data.get("int_min", None)
-    args["int_min"] = field
+    if field is not None:
+        args["int_min"] = field
 
     field = data.get("int_max", None)
-    args["int_max"] = field
+    if field is not None:
+        args["int_max"] = field
 
     field = data.get("float_min", None)
-    args["float_min"] = field
+    if field is not None:
+        args["float_min"] = field
 
     field = data.get("float_max", None)
-    args["float_max"] = field
+    if field is not None:
+        args["float_max"] = field
 
     return EngineSetting(**args)
 
 
 def unmarshal_EngineVersion(data: Any) -> EngineVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'EngineVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("available_settings", None)
-    args["available_settings"] = (
-        [unmarshal_EngineSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_settings"] = (
+            [unmarshal_EngineSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("beta", None)
-    args["beta"] = field
+    if field is not None:
+        args["beta"] = field
 
     field = data.get("available_init_settings", None)
-    args["available_init_settings"] = (
-        [unmarshal_EngineSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_init_settings"] = (
+            [unmarshal_EngineSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("end_of_life", None)
-    args["end_of_life"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["end_of_life"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return EngineVersion(**args)
 
 
 def unmarshal_DatabaseEngine(data: Any) -> DatabaseEngine:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DatabaseEngine' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("logo_url", None)
-    args["logo_url"] = field
+    if field is not None:
+        args["logo_url"] = field
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_EngineVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_EngineVersion(v) for v in field] if field is not None else None
+        )
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return DatabaseEngine(**args)
 
 
 def unmarshal_ListDatabaseEnginesResponse(data: Any) -> ListDatabaseEnginesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDatabaseEnginesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("engines", None)
-    args["engines"] = (
-        [unmarshal_DatabaseEngine(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["engines"] = (
+            [unmarshal_DatabaseEngine(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListDatabaseEnginesResponse(**args)
 
 
 def unmarshal_ListDatabasesResponse(data: Any) -> ListDatabasesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDatabasesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("databases", None)
-    args["databases"] = (
-        [unmarshal_Database(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["databases"] = (
+            [unmarshal_Database(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListDatabasesResponse(**args)
 
 
 def unmarshal_ListInstanceACLRulesResponse(data: Any) -> ListInstanceACLRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListInstanceACLRulesResponse(**args)
 
 
 def unmarshal_ListInstanceLogsDetailsResponseInstanceLogDetail(
     data: Any,
 ) -> ListInstanceLogsDetailsResponseInstanceLogDetail:
@@ -903,18 +1055,20 @@
         raise TypeError(
             "Unmarshalling the type 'ListInstanceLogsDetailsResponseInstanceLogDetail' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("log_name", None)
-    args["log_name"] = field
+    if field is not None:
+        args["log_name"] = field
 
     field = data.get("size", None)
-    args["size"] = field
+    if field is not None:
+        args["size"] = field
 
     return ListInstanceLogsDetailsResponseInstanceLogDetail(**args)
 
 
 def unmarshal_ListInstanceLogsDetailsResponse(
     data: Any,
 ) -> ListInstanceLogsDetailsResponse:
@@ -922,275 +1076,321 @@
         raise TypeError(
             "Unmarshalling the type 'ListInstanceLogsDetailsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("details", None)
-    args["details"] = (
-        [unmarshal_ListInstanceLogsDetailsResponseInstanceLogDetail(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["details"] = (
+            [
+                unmarshal_ListInstanceLogsDetailsResponseInstanceLogDetail(v)
+                for v in field
+            ]
+            if field is not None
+            else None
+        )
 
     return ListInstanceLogsDetailsResponse(**args)
 
 
 def unmarshal_ListInstanceLogsResponse(data: Any) -> ListInstanceLogsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListInstanceLogsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("instance_logs", None)
-    args["instance_logs"] = (
-        [unmarshal_InstanceLog(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["instance_logs"] = (
+            [unmarshal_InstanceLog(v) for v in field] if field is not None else None
+        )
 
     return ListInstanceLogsResponse(**args)
 
 
 def unmarshal_ListInstancesResponse(data: Any) -> ListInstancesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListInstancesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("instances", None)
-    args["instances"] = (
-        [unmarshal_Instance(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["instances"] = (
+            [unmarshal_Instance(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListInstancesResponse(**args)
 
 
 def unmarshal_NodeTypeVolumeConstraintSizes(data: Any) -> NodeTypeVolumeConstraintSizes:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeTypeVolumeConstraintSizes' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("min_size", None)
-    args["min_size"] = field
+    if field is not None:
+        args["min_size"] = field
 
     field = data.get("max_size", None)
-    args["max_size"] = field
+    if field is not None:
+        args["max_size"] = field
 
     return NodeTypeVolumeConstraintSizes(**args)
 
 
 def unmarshal_NodeTypeVolumeType(data: Any) -> NodeTypeVolumeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeTypeVolumeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("min_size", None)
-    args["min_size"] = field
+    if field is not None:
+        args["min_size"] = field
 
     field = data.get("max_size", None)
-    args["max_size"] = field
+    if field is not None:
+        args["max_size"] = field
 
     field = data.get("chunk_size", None)
-    args["chunk_size"] = field
+    if field is not None:
+        args["chunk_size"] = field
 
     field = data.get("class_", None)
-    args["class_"] = field
+    if field is not None:
+        args["class_"] = field
 
     return NodeTypeVolumeType(**args)
 
 
 def unmarshal_NodeType(data: Any) -> NodeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("stock_status", None)
-    args["stock_status"] = field
+    if field is not None:
+        args["stock_status"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("vcpus", None)
-    args["vcpus"] = field
+    if field is not None:
+        args["vcpus"] = field
 
     field = data.get("memory", None)
-    args["memory"] = field
+    if field is not None:
+        args["memory"] = field
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("beta", None)
-    args["beta"] = field
+    if field is not None:
+        args["beta"] = field
 
     field = data.get("volume_constraint", None)
-    args["volume_constraint"] = unmarshal_NodeTypeVolumeConstraintSizes(field)
+    if field is not None:
+        args["volume_constraint"] = unmarshal_NodeTypeVolumeConstraintSizes(field)
 
     field = data.get("is_bssd_compatible", None)
-    args["is_bssd_compatible"] = field
+    if field is not None:
+        args["is_bssd_compatible"] = field
 
     field = data.get("available_volume_types", None)
-    args["available_volume_types"] = (
-        [unmarshal_NodeTypeVolumeType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["available_volume_types"] = (
+            [unmarshal_NodeTypeVolumeType(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("is_ha_required", None)
-    args["is_ha_required"] = field
+    if field is not None:
+        args["is_ha_required"] = field
 
     field = data.get("generation", None)
-    args["generation"] = field
+    if field is not None:
+        args["generation"] = field
 
     field = data.get("instance_range", None)
-    args["instance_range"] = field
+    if field is not None:
+        args["instance_range"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return NodeType(**args)
 
 
 def unmarshal_ListNodeTypesResponse(data: Any) -> ListNodeTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNodeTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("node_types", None)
-    args["node_types"] = (
-        [unmarshal_NodeType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["node_types"] = (
+            [unmarshal_NodeType(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListNodeTypesResponse(**args)
 
 
 def unmarshal_ListPrivilegesResponse(data: Any) -> ListPrivilegesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPrivilegesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("privileges", None)
-    args["privileges"] = (
-        [unmarshal_Privilege(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["privileges"] = (
+            [unmarshal_Privilege(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPrivilegesResponse(**args)
 
 
 def unmarshal_ListSnapshotsResponse(data: Any) -> ListSnapshotsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSnapshotsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("snapshots", None)
-    args["snapshots"] = (
-        [unmarshal_Snapshot(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["snapshots"] = (
+            [unmarshal_Snapshot(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSnapshotsResponse(**args)
 
 
 def unmarshal_ListUsersResponse(data: Any) -> ListUsersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListUsersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("users", None)
-    args["users"] = [unmarshal_User(v) for v in field] if field is not None else None
+    if field is not None:
+        args["users"] = (
+            [unmarshal_User(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListUsersResponse(**args)
 
 
 def unmarshal_PrepareInstanceLogsResponse(data: Any) -> PrepareInstanceLogsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PrepareInstanceLogsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("instance_logs", None)
-    args["instance_logs"] = (
-        [unmarshal_InstanceLog(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["instance_logs"] = (
+            [unmarshal_InstanceLog(v) for v in field] if field is not None else None
+        )
 
     return PrepareInstanceLogsResponse(**args)
 
 
 def unmarshal_SetInstanceACLRulesResponse(data: Any) -> SetInstanceACLRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetInstanceACLRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rules", None)
-    args["rules"] = [unmarshal_ACLRule(v) for v in field] if field is not None else None
+    if field is not None:
+        args["rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return SetInstanceACLRulesResponse(**args)
 
 
 def unmarshal_SetInstanceSettingsResponse(data: Any) -> SetInstanceSettingsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetInstanceSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_InstanceSetting(v) for v in field] if field is not None else None
+        )
 
     return SetInstanceSettingsResponse(**args)
 
 
 def marshal_ACLRuleRequest(
     request: ACLRuleRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/rdb/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/rdb/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/redis/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/redis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/redis/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/redis/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/redis/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/redis/v1/marshalling.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,44 +54,51 @@
         raise TypeError(
             "Unmarshalling the type 'ACLRule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("ip_cidr", None)
-    args["ip_cidr"] = field
+    if field is not None:
+        args["ip_cidr"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     return ACLRule(**args)
 
 
 def unmarshal_PrivateNetwork(data: Any) -> PrivateNetwork:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PrivateNetwork' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("service_ips", None)
-    args["service_ips"] = field
+    if field is not None:
+        args["service_ips"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("provisioning_mode", None)
-    args["provisioning_mode"] = field
+    if field is not None:
+        args["provisioning_mode"] = field
 
     return PrivateNetwork(**args)
 
 
 def unmarshal_PublicNetwork(data: Any) -> PublicNetwork:
     if not isinstance(data, dict):
         raise TypeError(
@@ -108,371 +115,432 @@
         raise TypeError(
             "Unmarshalling the type 'Endpoint' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("port", None)
-    args["port"] = field
+    if field is not None:
+        args["port"] = field
 
     field = data.get("ips", None)
-    args["ips"] = field
+    if field is not None:
+        args["ips"] = field
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("private_network", None)
-    args["private_network"] = unmarshal_PrivateNetwork(field)
+    if field is not None:
+        args["private_network"] = unmarshal_PrivateNetwork(field)
 
     field = data.get("public_network", None)
-    args["public_network"] = unmarshal_PublicNetwork(field)
+    if field is not None:
+        args["public_network"] = unmarshal_PublicNetwork(field)
 
     return Endpoint(**args)
 
 
 def unmarshal_ClusterSetting(data: Any) -> ClusterSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("value", None)
-    args["value"] = field
+    if field is not None:
+        args["value"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return ClusterSetting(**args)
 
 
 def unmarshal_Cluster(data: Any) -> Cluster:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Cluster' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("node_type", None)
-    args["node_type"] = field
+    if field is not None:
+        args["node_type"] = field
 
     field = data.get("tls_enabled", None)
-    args["tls_enabled"] = field
+    if field is not None:
+        args["tls_enabled"] = field
 
     field = data.get("cluster_settings", None)
-    args["cluster_settings"] = (
-        [unmarshal_ClusterSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["cluster_settings"] = (
+            [unmarshal_ClusterSetting(v) for v in field] if field is not None else None
+        )
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("acl_rules", None)
-    args["acl_rules"] = (
-        [unmarshal_ACLRule(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["acl_rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     field = data.get("cluster_size", None)
-    args["cluster_size"] = field
+    if field is not None:
+        args["cluster_size"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("user_name", None)
-    args["user_name"] = field
+    if field is not None:
+        args["user_name"] = field
 
     field = data.get("upgradable_versions", None)
-    args["upgradable_versions"] = field
+    if field is not None:
+        args["upgradable_versions"] = field
 
     return Cluster(**args)
 
 
 def unmarshal_AddAclRulesResponse(data: Any) -> AddAclRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddAclRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("acl_rules", None)
-    args["acl_rules"] = (
-        [unmarshal_ACLRule(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["acl_rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return AddAclRulesResponse(**args)
 
 
 def unmarshal_AddEndpointsResponse(data: Any) -> AddEndpointsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddEndpointsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return AddEndpointsResponse(**args)
 
 
 def unmarshal_ClusterMetricsResponse(data: Any) -> ClusterMetricsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterMetricsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("timeseries", None)
-    args["timeseries"] = (
-        [unmarshal_TimeSeries(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["timeseries"] = (
+            [unmarshal_TimeSeries(v) for v in field] if field is not None else None
+        )
 
     return ClusterMetricsResponse(**args)
 
 
 def unmarshal_ClusterSettingsResponse(data: Any) -> ClusterSettingsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterSettingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("settings", None)
-    args["settings"] = (
-        [unmarshal_ClusterSetting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["settings"] = (
+            [unmarshal_ClusterSetting(v) for v in field] if field is not None else None
+        )
 
     return ClusterSettingsResponse(**args)
 
 
 def unmarshal_AvailableClusterSetting(data: Any) -> AvailableClusterSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AvailableClusterSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("deprecated", None)
-    args["deprecated"] = field
+    if field is not None:
+        args["deprecated"] = field
 
     field = data.get("default_value", None)
-    args["default_value"] = field
+    if field is not None:
+        args["default_value"] = field
 
     field = data.get("max_value", None)
-    args["max_value"] = field
+    if field is not None:
+        args["max_value"] = field
 
     field = data.get("min_value", None)
-    args["min_value"] = field
+    if field is not None:
+        args["min_value"] = field
 
     field = data.get("regex", None)
-    args["regex"] = field
+    if field is not None:
+        args["regex"] = field
 
     return AvailableClusterSetting(**args)
 
 
 def unmarshal_ClusterVersion(data: Any) -> ClusterVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ClusterVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("version", None)
-    args["version"] = field
+    if field is not None:
+        args["version"] = field
 
     field = data.get("available_settings", None)
-    args["available_settings"] = (
-        [unmarshal_AvailableClusterSetting(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["available_settings"] = (
+            [unmarshal_AvailableClusterSetting(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("logo_url", None)
-    args["logo_url"] = field
+    if field is not None:
+        args["logo_url"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("end_of_life_at", None)
-    args["end_of_life_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["end_of_life_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return ClusterVersion(**args)
 
 
 def unmarshal_ListClusterVersionsResponse(data: Any) -> ListClusterVersionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListClusterVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_ClusterVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_ClusterVersion(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListClusterVersionsResponse(**args)
 
 
 def unmarshal_ListClustersResponse(data: Any) -> ListClustersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListClustersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("clusters", None)
-    args["clusters"] = (
-        [unmarshal_Cluster(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["clusters"] = (
+            [unmarshal_Cluster(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListClustersResponse(**args)
 
 
 def unmarshal_NodeType(data: Any) -> NodeType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'NodeType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("stock_status", None)
-    args["stock_status"] = field
+    if field is not None:
+        args["stock_status"] = field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("vcpus", None)
-    args["vcpus"] = field
+    if field is not None:
+        args["vcpus"] = field
 
     field = data.get("memory", None)
-    args["memory"] = field
+    if field is not None:
+        args["memory"] = field
 
     field = data.get("disabled", None)
-    args["disabled"] = field
+    if field is not None:
+        args["disabled"] = field
 
     field = data.get("beta", None)
-    args["beta"] = field
+    if field is not None:
+        args["beta"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return NodeType(**args)
 
 
 def unmarshal_ListNodeTypesResponse(data: Any) -> ListNodeTypesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListNodeTypesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("node_types", None)
-    args["node_types"] = (
-        [unmarshal_NodeType(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["node_types"] = (
+            [unmarshal_NodeType(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListNodeTypesResponse(**args)
 
 
 def unmarshal_SetAclRulesResponse(data: Any) -> SetAclRulesResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetAclRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("acl_rules", None)
-    args["acl_rules"] = (
-        [unmarshal_ACLRule(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["acl_rules"] = (
+            [unmarshal_ACLRule(v) for v in field] if field is not None else None
+        )
 
     return SetAclRulesResponse(**args)
 
 
 def unmarshal_SetEndpointsResponse(data: Any) -> SetEndpointsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetEndpointsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("endpoints", None)
-    args["endpoints"] = (
-        [unmarshal_Endpoint(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["endpoints"] = (
+            [unmarshal_Endpoint(v) for v in field] if field is not None else None
+        )
 
     return SetEndpointsResponse(**args)
 
 
 def marshal_ACLRuleSpec(
     request: ACLRuleSpec,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/redis/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/redis/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/registry/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/registry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/registry/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/registry/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/registry/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/registry/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/registry/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/jobs/v1alpha1/marshalling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,260 +1,244 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 
 from typing import Any, Dict
 from dateutil import parser
 
 from scaleway_core.profile import ProfileDefaults
-from scaleway_core.utils import (
-    OneOfPossibility,
-    resolve_one_of,
-)
 from .types import (
-    Image,
-    Namespace,
-    Tag,
-    ListImagesResponse,
-    ListNamespacesResponse,
-    ListTagsResponse,
-    CreateNamespaceRequest,
-    UpdateImageRequest,
-    UpdateNamespaceRequest,
+    JobDefinition,
+    JobRun,
+    ListJobDefinitionsResponse,
+    ListJobRunsResponse,
+    CreateJobDefinitionRequest,
+    UpdateJobDefinitionRequest,
 )
 
 
-def unmarshal_Image(data: Any) -> Image:
+def unmarshal_JobDefinition(data: Any) -> JobDefinition:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Image' failed as data isn't a dictionary."
+            "Unmarshalling the type 'JobDefinition' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("namespace_id", None)
-    args["namespace_id"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("visibility", None)
-    args["visibility"] = field
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("size", None)
-    args["size"] = field
+    field = data.get("cpu_limit", None)
+    if field is not None:
+        args["cpu_limit"] = field
+
+    field = data.get("memory_limit", None)
+    if field is not None:
+        args["memory_limit"] = field
+
+    field = data.get("image_uri", None)
+    if field is not None:
+        args["image_uri"] = field
+
+    field = data.get("command", None)
+    if field is not None:
+        args["command"] = field
 
-    field = data.get("tags", None)
-    args["tags"] = field
-
-    field = data.get("status_message", None)
-    args["status_message"] = field
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    return Image(**args)
-
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-def unmarshal_Namespace(data: Any) -> Namespace:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'Namespace' failed as data isn't a dictionary."
-        )
-
-    args: Dict[str, Any] = {}
-
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("environment_variables", None)
+    if field is not None:
+        args["environment_variables"] = field
 
     field = data.get("description", None)
-    args["description"] = field
-
-    field = data.get("organization_id", None)
-    args["organization_id"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("status_message", None)
-    args["status_message"] = field
-
-    field = data.get("endpoint", None)
-    args["endpoint"] = field
-
-    field = data.get("is_public", None)
-    args["is_public"] = field
-
-    field = data.get("size", None)
-    args["size"] = field
-
-    field = data.get("image_count", None)
-    args["image_count"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("job_timeout", None)
+    if field is not None:
+        args["job_timeout"] = field
 
-    return Namespace(**args)
+    return JobDefinition(**args)
 
 
-def unmarshal_Tag(data: Any) -> Tag:
+def unmarshal_JobRun(data: Any) -> JobRun:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Tag' failed as data isn't a dictionary."
+            "Unmarshalling the type 'JobRun' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("name", None)
-    args["name"] = field
-
-    field = data.get("image_id", None)
-    args["image_id"] = field
+    field = data.get("job_definition_id", None)
+    if field is not None:
+        args["job_definition_id"] = field
+
+    field = data.get("state", None)
+    if field is not None:
+        args["state"] = field
+
+    field = data.get("error_message", None)
+    if field is not None:
+        args["error_message"] = field
 
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("digest", None)
-    args["digest"] = field
+    field = data.get("region", None)
+    if field is not None:
+        args["region"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return Tag(**args)
-
-
-def unmarshal_ListImagesResponse(data: Any) -> ListImagesResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListImagesResponse' failed as data isn't a dictionary."
+    field = data.get("terminated_at", None)
+    if field is not None:
+        args["terminated_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
         )
 
-    args: Dict[str, Any] = {}
-
-    field = data.get("images", None)
-    args["images"] = [unmarshal_Image(v) for v in field] if field is not None else None
+    field = data.get("exit_code", None)
+    if field is not None:
+        args["exit_code"] = field
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    field = data.get("run_duration", None)
+    if field is not None:
+        args["run_duration"] = field
 
-    return ListImagesResponse(**args)
+    return JobRun(**args)
 
 
-def unmarshal_ListNamespacesResponse(data: Any) -> ListNamespacesResponse:
+def unmarshal_ListJobDefinitionsResponse(data: Any) -> ListJobDefinitionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListNamespacesResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListJobDefinitionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("namespaces", None)
-    args["namespaces"] = (
-        [unmarshal_Namespace(v) for v in field] if field is not None else None
-    )
+    field = data.get("job_definitions", None)
+    if field is not None:
+        args["job_definitions"] = (
+            [unmarshal_JobDefinition(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListNamespacesResponse(**args)
+    return ListJobDefinitionsResponse(**args)
 
 
-def unmarshal_ListTagsResponse(data: Any) -> ListTagsResponse:
+def unmarshal_ListJobRunsResponse(data: Any) -> ListJobRunsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListTagsResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListJobRunsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("tags", None)
-    args["tags"] = [unmarshal_Tag(v) for v in field] if field is not None else None
+    field = data.get("job_runs", None)
+    if field is not None:
+        args["job_runs"] = (
+            [unmarshal_JobRun(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListTagsResponse(**args)
+    return ListJobRunsResponse(**args)
 
 
-def marshal_CreateNamespaceRequest(
-    request: CreateNamespaceRequest,
+def marshal_CreateJobDefinitionRequest(
+    request: CreateJobDefinitionRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
-    output.update(
-        resolve_one_of(
-            [
-                OneOfPossibility(
-                    "project_id", request.project_id, defaults.default_project_id
-                ),
-                OneOfPossibility(
-                    "organization_id",
-                    request.organization_id,
-                    defaults.default_organization_id,
-                ),
-            ]
-        ),
-    )
+
+    if request.cpu_limit is not None:
+        output["cpu_limit"] = request.cpu_limit
+
+    if request.memory_limit is not None:
+        output["memory_limit"] = request.memory_limit
+
+    if request.image_uri is not None:
+        output["image_uri"] = request.image_uri
+
+    if request.command is not None:
+        output["command"] = request.command
 
     if request.description is not None:
         output["description"] = request.description
 
-    if request.is_public is not None:
-        output["is_public"] = request.is_public
-
     if request.name is not None:
         output["name"] = request.name
 
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
+
+    if request.environment_variables is not None:
+        output["environment_variables"] = {
+            key: value for key, value in request.environment_variables.items()
+        }
+
+    if request.job_timeout is not None:
+        output["job_timeout"] = request.job_timeout
+
     return output
 
 
-def marshal_UpdateImageRequest(
-    request: UpdateImageRequest,
+def marshal_UpdateJobDefinitionRequest(
+    request: UpdateJobDefinitionRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.visibility is not None:
-        output["visibility"] = str(request.visibility)
+    if request.name is not None:
+        output["name"] = request.name
+
+    if request.cpu_limit is not None:
+        output["cpu_limit"] = request.cpu_limit
 
-    return output
+    if request.memory_limit is not None:
+        output["memory_limit"] = request.memory_limit
 
+    if request.image_uri is not None:
+        output["image_uri"] = request.image_uri
 
-def marshal_UpdateNamespaceRequest(
-    request: UpdateNamespaceRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
+    if request.command is not None:
+        output["command"] = request.command
+
+    if request.environment_variables is not None:
+        output["environment_variables"] = request.environment_variables
 
     if request.description is not None:
         output["description"] = request.description
 
-    if request.is_public is not None:
-        output["is_public"] = request.is_public
+    if request.job_timeout is not None:
+        output["job_timeout"] = request.job_timeout
 
     return output
```

### Comparing `scaleway-2.0.0.dev5/scaleway/registry/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/registry/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/marshalling.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,218 +30,259 @@
         raise TypeError(
             "Unmarshalling the type 'Folder' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("path", None)
-    args["path"] = field
+    if field is not None:
+        args["path"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Folder(**args)
 
 
 def unmarshal_SecretVersion(data: Any) -> SecretVersion:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SecretVersion' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("revision", None)
-    args["revision"] = field
+    if field is not None:
+        args["revision"] = field
 
     field = data.get("secret_id", None)
-    args["secret_id"] = field
+    if field is not None:
+        args["secret_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("is_latest", None)
-    args["is_latest"] = field
+    if field is not None:
+        args["is_latest"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     return SecretVersion(**args)
 
 
 def unmarshal_Secret(data: Any) -> Secret:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Secret' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("version_count", None)
-    args["version_count"] = field
+    if field is not None:
+        args["version_count"] = field
 
     field = data.get("is_managed", None)
-    args["is_managed"] = field
+    if field is not None:
+        args["is_managed"] = field
 
     field = data.get("is_protected", None)
-    args["is_protected"] = field
+    if field is not None:
+        args["is_protected"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("path", None)
-    args["path"] = field
+    if field is not None:
+        args["path"] = field
 
     field = data.get("ephemeral_action", None)
-    args["ephemeral_action"] = field
+    if field is not None:
+        args["ephemeral_action"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("description", None)
-    args["description"] = field
+    if field is not None:
+        args["description"] = field
 
     field = data.get("expires_at", None)
-    args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Secret(**args)
 
 
 def unmarshal_AccessSecretVersionResponse(data: Any) -> AccessSecretVersionResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AccessSecretVersionResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("secret_id", None)
-    args["secret_id"] = field
+    if field is not None:
+        args["secret_id"] = field
 
     field = data.get("revision", None)
-    args["revision"] = field
+    if field is not None:
+        args["revision"] = field
 
     field = data.get("data", None)
-    args["data"] = field
+    if field is not None:
+        args["data"] = field
 
     field = data.get("data_crc32", None)
-    args["data_crc32"] = field
+    if field is not None:
+        args["data_crc32"] = field
 
     return AccessSecretVersionResponse(**args)
 
 
 def unmarshal_ListFoldersResponse(data: Any) -> ListFoldersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListFoldersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("folders", None)
-    args["folders"] = (
-        [unmarshal_Folder(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["folders"] = (
+            [unmarshal_Folder(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListFoldersResponse(**args)
 
 
 def unmarshal_ListSecretVersionsResponse(data: Any) -> ListSecretVersionsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSecretVersionsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("versions", None)
-    args["versions"] = (
-        [unmarshal_SecretVersion(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["versions"] = (
+            [unmarshal_SecretVersion(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSecretVersionsResponse(**args)
 
 
 def unmarshal_ListSecretsResponse(data: Any) -> ListSecretsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListSecretsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("secrets", None)
-    args["secrets"] = (
-        [unmarshal_Secret(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["secrets"] = (
+            [unmarshal_Secret(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListSecretsResponse(**args)
 
 
 def unmarshal_ListTagsResponse(data: Any) -> ListTagsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListTagsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListTagsResponse(**args)
 
 
 def marshal_AddSecretOwnerRequest(
     request: AddSecretOwnerRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/secret/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/secret/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/content.py` & `scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/marshalling.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,331 +31,407 @@
         raise TypeError(
             "Unmarshalling the type 'EmailTry' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("rank", None)
-    args["rank"] = field
+    if field is not None:
+        args["rank"] = field
 
     field = data.get("code", None)
-    args["code"] = field
+    if field is not None:
+        args["code"] = field
 
     field = data.get("message", None)
-    args["message"] = field
+    if field is not None:
+        args["message"] = field
 
     field = data.get("tried_at", None)
-    args["tried_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["tried_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return EmailTry(**args)
 
 
 def unmarshal_Email(data: Any) -> Email:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Email' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("message_id", None)
-    args["message_id"] = field
+    if field is not None:
+        args["message_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("mail_from", None)
-    args["mail_from"] = field
+    if field is not None:
+        args["mail_from"] = field
 
     field = data.get("mail_rcpt", None)
-    args["mail_rcpt"] = field
+    if field is not None:
+        args["mail_rcpt"] = field
 
     field = data.get("rcpt_to", None)
-    args["rcpt_to"] = field
+    if field is not None:
+        args["rcpt_to"] = field
 
     field = data.get("rcpt_type", None)
-    args["rcpt_type"] = field
+    if field is not None:
+        args["rcpt_type"] = field
 
     field = data.get("subject", None)
-    args["subject"] = field
+    if field is not None:
+        args["subject"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("try_count", None)
-    args["try_count"] = field
+    if field is not None:
+        args["try_count"] = field
 
     field = data.get("last_tries", None)
-    args["last_tries"] = (
-        [unmarshal_EmailTry(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["last_tries"] = (
+            [unmarshal_EmailTry(v) for v in field] if field is not None else None
+        )
 
     field = data.get("flags", None)
-    args["flags"] = [EmailFlag(v) for v in field] if field is not None else None
+    if field is not None:
+        args["flags"] = [EmailFlag(v) for v in field] if field is not None else None
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("status_details", None)
-    args["status_details"] = field
+    if field is not None:
+        args["status_details"] = field
 
     return Email(**args)
 
 
 def unmarshal_DomainReputation(data: Any) -> DomainReputation:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainReputation' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("score", None)
-    args["score"] = field
+    if field is not None:
+        args["score"] = field
 
     field = data.get("scored_at", None)
-    args["scored_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["scored_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("previous_score", None)
-    args["previous_score"] = field
+    if field is not None:
+        args["previous_score"] = field
 
     field = data.get("previous_scored_at", None)
-    args["previous_scored_at"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["previous_scored_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     return DomainReputation(**args)
 
 
 def unmarshal_DomainStatistics(data: Any) -> DomainStatistics:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainStatistics' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("sent_count", None)
-    args["sent_count"] = field
+    if field is not None:
+        args["sent_count"] = field
 
     field = data.get("failed_count", None)
-    args["failed_count"] = field
+    if field is not None:
+        args["failed_count"] = field
 
     field = data.get("canceled_count", None)
-    args["canceled_count"] = field
+    if field is not None:
+        args["canceled_count"] = field
 
     return DomainStatistics(**args)
 
 
 def unmarshal_Domain(data: Any) -> Domain:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Domain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("spf_config", None)
-    args["spf_config"] = field
+    if field is not None:
+        args["spf_config"] = field
 
     field = data.get("dkim_config", None)
-    args["dkim_config"] = field
+    if field is not None:
+        args["dkim_config"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("next_check_at", None)
-    args["next_check_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["next_check_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("last_valid_at", None)
-    args["last_valid_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["last_valid_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("revoked_at", None)
-    args["revoked_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["revoked_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("last_error", None)
-    args["last_error"] = field
+    if field is not None:
+        args["last_error"] = field
 
     field = data.get("statistics", None)
-    args["statistics"] = unmarshal_DomainStatistics(field)
+    if field is not None:
+        args["statistics"] = unmarshal_DomainStatistics(field)
 
     field = data.get("reputation", None)
-    args["reputation"] = unmarshal_DomainReputation(field)
+    if field is not None:
+        args["reputation"] = unmarshal_DomainReputation(field)
 
     return Domain(**args)
 
 
 def unmarshal_CreateEmailResponse(data: Any) -> CreateEmailResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'CreateEmailResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("emails", None)
-    args["emails"] = [unmarshal_Email(v) for v in field] if field is not None else None
+    if field is not None:
+        args["emails"] = (
+            [unmarshal_Email(v) for v in field] if field is not None else None
+        )
 
     return CreateEmailResponse(**args)
 
 
 def unmarshal_DomainLastStatusDkimRecord(data: Any) -> DomainLastStatusDkimRecord:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainLastStatusDkimRecord' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("last_valid_at", None)
-    args["last_valid_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["last_valid_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("error", None)
-    args["error"] = field
+    if field is not None:
+        args["error"] = field
 
     return DomainLastStatusDkimRecord(**args)
 
 
 def unmarshal_DomainLastStatusSpfRecord(data: Any) -> DomainLastStatusSpfRecord:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainLastStatusSpfRecord' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("last_valid_at", None)
-    args["last_valid_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["last_valid_at"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("error", None)
-    args["error"] = field
+    if field is not None:
+        args["error"] = field
 
     return DomainLastStatusSpfRecord(**args)
 
 
 def unmarshal_DomainLastStatus(data: Any) -> DomainLastStatus:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DomainLastStatus' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("domain_id", None)
-    args["domain_id"] = field
+    if field is not None:
+        args["domain_id"] = field
 
     field = data.get("domain_name", None)
-    args["domain_name"] = field
+    if field is not None:
+        args["domain_name"] = field
 
     field = data.get("spf_record", None)
-    args["spf_record"] = unmarshal_DomainLastStatusSpfRecord(field)
+    if field is not None:
+        args["spf_record"] = unmarshal_DomainLastStatusSpfRecord(field)
 
     field = data.get("dkim_record", None)
-    args["dkim_record"] = unmarshal_DomainLastStatusDkimRecord(field)
+    if field is not None:
+        args["dkim_record"] = unmarshal_DomainLastStatusDkimRecord(field)
 
     return DomainLastStatus(**args)
 
 
 def unmarshal_ListDomainsResponse(data: Any) -> ListDomainsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListDomainsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("domains", None)
-    args["domains"] = (
-        [unmarshal_Domain(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["domains"] = (
+            [unmarshal_Domain(v) for v in field] if field is not None else None
+        )
 
     return ListDomainsResponse(**args)
 
 
 def unmarshal_ListEmailsResponse(data: Any) -> ListEmailsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListEmailsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("emails", None)
-    args["emails"] = [unmarshal_Email(v) for v in field] if field is not None else None
+    if field is not None:
+        args["emails"] = (
+            [unmarshal_Email(v) for v in field] if field is not None else None
+        )
 
     return ListEmailsResponse(**args)
 
 
 def unmarshal_Statistics(data: Any) -> Statistics:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Statistics' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("new_count", None)
-    args["new_count"] = field
+    if field is not None:
+        args["new_count"] = field
 
     field = data.get("sending_count", None)
-    args["sending_count"] = field
+    if field is not None:
+        args["sending_count"] = field
 
     field = data.get("sent_count", None)
-    args["sent_count"] = field
+    if field is not None:
+        args["sent_count"] = field
 
     field = data.get("failed_count", None)
-    args["failed_count"] = field
+    if field is not None:
+        args["failed_count"] = field
 
     field = data.get("canceled_count", None)
-    args["canceled_count"] = field
+    if field is not None:
+        args["canceled_count"] = field
 
     return Statistics(**args)
 
 
 def marshal_CreateDomainRequest(
     request: CreateDomainRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/tem/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/tem/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/test/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/test/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/test/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/test/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/test/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/test/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/testinternal/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/testinternal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/testinternal/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/testinternal/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/testinternal/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/testinternal/v1/marshalling.py`

 * *Files 16% similar despite different names*

```diff
@@ -81,558 +81,705 @@
         raise TypeError(
             "Unmarshalling the type 'PostAllTypesMessageNestedMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("bb", None)
-    args["bb"] = field
+    if field is not None:
+        args["bb"] = field
 
     return PostAllTypesMessageNestedMessage(**args)
 
 
 def unmarshal_PostAllTypesMessage(data: Any) -> PostAllTypesMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostAllTypesMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("singular_int32", None)
-    args["singular_int32"] = field
+    if field is not None:
+        args["singular_int32"] = field
 
     field = data.get("singular_int64", None)
-    args["singular_int64"] = field
+    if field is not None:
+        args["singular_int64"] = field
 
     field = data.get("singular_uint32", None)
-    args["singular_uint32"] = field
+    if field is not None:
+        args["singular_uint32"] = field
 
     field = data.get("singular_uint64", None)
-    args["singular_uint64"] = field
+    if field is not None:
+        args["singular_uint64"] = field
 
     field = data.get("singular_sint32", None)
-    args["singular_sint32"] = field
+    if field is not None:
+        args["singular_sint32"] = field
 
     field = data.get("singular_sint64", None)
-    args["singular_sint64"] = field
+    if field is not None:
+        args["singular_sint64"] = field
 
     field = data.get("singular_fixed32", None)
-    args["singular_fixed32"] = field
+    if field is not None:
+        args["singular_fixed32"] = field
 
     field = data.get("singular_fixed64", None)
-    args["singular_fixed64"] = field
+    if field is not None:
+        args["singular_fixed64"] = field
 
     field = data.get("singular_sfixed32", None)
-    args["singular_sfixed32"] = field
+    if field is not None:
+        args["singular_sfixed32"] = field
 
     field = data.get("singular_sfixed64", None)
-    args["singular_sfixed64"] = field
+    if field is not None:
+        args["singular_sfixed64"] = field
 
     field = data.get("singular_float", None)
-    args["singular_float"] = field
+    if field is not None:
+        args["singular_float"] = field
 
     field = data.get("singular_double", None)
-    args["singular_double"] = field
+    if field is not None:
+        args["singular_double"] = field
 
     field = data.get("singular_bool", None)
-    args["singular_bool"] = field
+    if field is not None:
+        args["singular_bool"] = field
 
     field = data.get("singular_string", None)
-    args["singular_string"] = field
+    if field is not None:
+        args["singular_string"] = field
 
     field = data.get("singular_bytes", None)
-    args["singular_bytes"] = field
+    if field is not None:
+        args["singular_bytes"] = field
 
     field = data.get("singular_nested_message", None)
-    args["singular_nested_message"] = unmarshal_PostAllTypesMessageNestedMessage(field)
+    if field is not None:
+        args["singular_nested_message"] = unmarshal_PostAllTypesMessageNestedMessage(
+            field
+        )
 
     field = data.get("singular_nested_enum", None)
-    args["singular_nested_enum"] = field
+    if field is not None:
+        args["singular_nested_enum"] = field
 
     field = data.get("repeated_int32", None)
-    args["repeated_int32"] = field
+    if field is not None:
+        args["repeated_int32"] = field
 
     field = data.get("repeated_int64", None)
-    args["repeated_int64"] = field
+    if field is not None:
+        args["repeated_int64"] = field
 
     field = data.get("repeated_uint32", None)
-    args["repeated_uint32"] = field
+    if field is not None:
+        args["repeated_uint32"] = field
 
     field = data.get("repeated_uint64", None)
-    args["repeated_uint64"] = field
+    if field is not None:
+        args["repeated_uint64"] = field
 
     field = data.get("repeated_sint32", None)
-    args["repeated_sint32"] = field
+    if field is not None:
+        args["repeated_sint32"] = field
 
     field = data.get("repeated_sint64", None)
-    args["repeated_sint64"] = field
+    if field is not None:
+        args["repeated_sint64"] = field
 
     field = data.get("repeated_fixed32", None)
-    args["repeated_fixed32"] = field
+    if field is not None:
+        args["repeated_fixed32"] = field
 
     field = data.get("repeated_fixed64", None)
-    args["repeated_fixed64"] = field
+    if field is not None:
+        args["repeated_fixed64"] = field
 
     field = data.get("repeated_sfixed32", None)
-    args["repeated_sfixed32"] = field
+    if field is not None:
+        args["repeated_sfixed32"] = field
 
     field = data.get("repeated_sfixed64", None)
-    args["repeated_sfixed64"] = field
+    if field is not None:
+        args["repeated_sfixed64"] = field
 
     field = data.get("repeated_float", None)
-    args["repeated_float"] = field
+    if field is not None:
+        args["repeated_float"] = field
 
     field = data.get("repeated_double", None)
-    args["repeated_double"] = field
+    if field is not None:
+        args["repeated_double"] = field
 
     field = data.get("repeated_bool", None)
-    args["repeated_bool"] = field
+    if field is not None:
+        args["repeated_bool"] = field
 
     field = data.get("repeated_string", None)
-    args["repeated_string"] = field
+    if field is not None:
+        args["repeated_string"] = field
 
     field = data.get("repeated_bytes", None)
-    args["repeated_bytes"] = field
+    if field is not None:
+        args["repeated_bytes"] = field
 
     field = data.get("repeated_nested_message", None)
-    args["repeated_nested_message"] = (
-        [unmarshal_PostAllTypesMessageNestedMessage(v) for v in field]
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["repeated_nested_message"] = (
+            [unmarshal_PostAllTypesMessageNestedMessage(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("repeated_nested_enum", None)
-    args["repeated_nested_enum"] = (
-        [PostAllTypesMessageNestedEnum(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["repeated_nested_enum"] = (
+            [PostAllTypesMessageNestedEnum(v) for v in field]
+            if field is not None
+            else None
+        )
 
     field = data.get("oneof_uint32", None)
-    args["oneof_uint32"] = field
+    if field is not None:
+        args["oneof_uint32"] = field
 
     field = data.get("oneof_nested_message", None)
-    args["oneof_nested_message"] = unmarshal_PostAllTypesMessageNestedMessage(field)
+    if field is not None:
+        args["oneof_nested_message"] = unmarshal_PostAllTypesMessageNestedMessage(field)
 
     field = data.get("oneof_string", None)
-    args["oneof_string"] = field
+    if field is not None:
+        args["oneof_string"] = field
 
     field = data.get("oneof_bytes", None)
-    args["oneof_bytes"] = field
+    if field is not None:
+        args["oneof_bytes"] = field
 
     field = data.get("singular_double_value", None)
-    args["singular_double_value"] = field
+    if field is not None:
+        args["singular_double_value"] = field
 
     field = data.get("singular_float_value", None)
-    args["singular_float_value"] = field
+    if field is not None:
+        args["singular_float_value"] = field
 
     field = data.get("singular_int64_value", None)
-    args["singular_int64_value"] = field
+    if field is not None:
+        args["singular_int64_value"] = field
 
     field = data.get("singular_uint64_value", None)
-    args["singular_uint64_value"] = field
+    if field is not None:
+        args["singular_uint64_value"] = field
 
     field = data.get("singular_int32_value", None)
-    args["singular_int32_value"] = field
+    if field is not None:
+        args["singular_int32_value"] = field
 
     field = data.get("singular_uint32_value", None)
-    args["singular_uint32_value"] = field
+    if field is not None:
+        args["singular_uint32_value"] = field
 
     field = data.get("singular_bool_value", None)
-    args["singular_bool_value"] = field
+    if field is not None:
+        args["singular_bool_value"] = field
 
     field = data.get("singular_string_value", None)
-    args["singular_string_value"] = field
+    if field is not None:
+        args["singular_string_value"] = field
 
     field = data.get("singular_bytes_value", None)
-    args["singular_bytes_value"] = field
+    if field is not None:
+        args["singular_bytes_value"] = field
 
     field = data.get("singular_timestamp", None)
-    args["singular_timestamp"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["singular_timestamp"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("singular_any", None)
-    args["singular_any"] = field
+    if field is not None:
+        args["singular_any"] = field
 
     field = data.get("singular_struct", None)
-    args["singular_struct"] = field
+    if field is not None:
+        args["singular_struct"] = field
 
     field = data.get("singular_money", None)
-    args["singular_money"] = unmarshal_Money(field)
+    if field is not None:
+        args["singular_money"] = unmarshal_Money(field)
 
     field = data.get("singular_strings_value", None)
-    args["singular_strings_value"] = field
+    if field is not None:
+        args["singular_strings_value"] = field
 
     field = data.get("singular_duration", None)
-    args["singular_duration"] = field
+    if field is not None:
+        args["singular_duration"] = field
 
     field = data.get("singular_ip", None)
-    args["singular_ip"] = field
+    if field is not None:
+        args["singular_ip"] = field
 
     field = data.get("singular_string_ip", None)
-    args["singular_string_ip"] = field
+    if field is not None:
+        args["singular_string_ip"] = field
 
     field = data.get("singular_string_ipv4", None)
-    args["singular_string_ipv4"] = field
+    if field is not None:
+        args["singular_string_ipv4"] = field
 
     field = data.get("singular_string_ipv6", None)
-    args["singular_string_ipv6"] = field
+    if field is not None:
+        args["singular_string_ipv6"] = field
 
     field = data.get("singular_string_value_ip", None)
-    args["singular_string_value_ip"] = field
+    if field is not None:
+        args["singular_string_value_ip"] = field
 
     field = data.get("singular_ipv4", None)
-    args["singular_ipv4"] = field
+    if field is not None:
+        args["singular_ipv4"] = field
 
     field = data.get("singular_string_value_ipv4", None)
-    args["singular_string_value_ipv4"] = field
+    if field is not None:
+        args["singular_string_value_ipv4"] = field
 
     field = data.get("singular_ipv6", None)
-    args["singular_ipv6"] = field
+    if field is not None:
+        args["singular_ipv6"] = field
 
     field = data.get("singular_string_value_ipv6", None)
-    args["singular_string_value_ipv6"] = field
+    if field is not None:
+        args["singular_string_value_ipv6"] = field
 
     field = data.get("singular_std_duration", None)
-    args["singular_std_duration"] = field
+    if field is not None:
+        args["singular_std_duration"] = field
 
     field = data.get("singular_std_long_duration", None)
-    args["singular_std_long_duration"] = field
+    if field is not None:
+        args["singular_std_long_duration"] = field
 
     field = data.get("singular_size", None)
-    args["singular_size"] = field
+    if field is not None:
+        args["singular_size"] = field
 
     field = data.get("singular_uint64_size", None)
-    args["singular_uint64_size"] = field
+    if field is not None:
+        args["singular_uint64_size"] = field
 
     field = data.get("singular_string_ipnet", None)
-    args["singular_string_ipnet"] = field
+    if field is not None:
+        args["singular_string_ipnet"] = field
 
     field = data.get("repeated_double_value", None)
-    args["repeated_double_value"] = field
+    if field is not None:
+        args["repeated_double_value"] = field
 
     field = data.get("repeated_float_value", None)
-    args["repeated_float_value"] = field
+    if field is not None:
+        args["repeated_float_value"] = field
 
     field = data.get("repeated_int64_value", None)
-    args["repeated_int64_value"] = field
+    if field is not None:
+        args["repeated_int64_value"] = field
 
     field = data.get("repeated_uint64_value", None)
-    args["repeated_uint64_value"] = field
+    if field is not None:
+        args["repeated_uint64_value"] = field
 
     field = data.get("repeated_int32_value", None)
-    args["repeated_int32_value"] = field
+    if field is not None:
+        args["repeated_int32_value"] = field
 
     field = data.get("repeated_uint32_value", None)
-    args["repeated_uint32_value"] = field
+    if field is not None:
+        args["repeated_uint32_value"] = field
 
     field = data.get("singular_uint64value_size", None)
-    args["singular_uint64value_size"] = field
+    if field is not None:
+        args["singular_uint64value_size"] = field
 
     field = data.get("singular_string_value_ipnet", None)
-    args["singular_string_value_ipnet"] = field
+    if field is not None:
+        args["singular_string_value_ipnet"] = field
 
     field = data.get("repeated_bool_value", None)
-    args["repeated_bool_value"] = field
+    if field is not None:
+        args["repeated_bool_value"] = field
 
     field = data.get("repeated_string_value", None)
-    args["repeated_string_value"] = field
+    if field is not None:
+        args["repeated_string_value"] = field
 
     field = data.get("repeated_bytes_value", None)
-    args["repeated_bytes_value"] = field
+    if field is not None:
+        args["repeated_bytes_value"] = field
 
     field = data.get("repeated_timestamp", None)
-    args["repeated_timestamp"] = field
+    if field is not None:
+        args["repeated_timestamp"] = field
 
     field = data.get("repeated_any", None)
-    args["repeated_any"] = field
+    if field is not None:
+        args["repeated_any"] = field
 
     field = data.get("repeated_struct", None)
-    args["repeated_struct"] = field
+    if field is not None:
+        args["repeated_struct"] = field
 
     field = data.get("repeated_money", None)
-    args["repeated_money"] = (
-        [unmarshal_Money(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["repeated_money"] = (
+            [unmarshal_Money(v) for v in field] if field is not None else None
+        )
 
     field = data.get("repeated_strings_value", None)
-    args["repeated_strings_value"] = field
+    if field is not None:
+        args["repeated_strings_value"] = field
 
     field = data.get("repeated_duration", None)
-    args["repeated_duration"] = field
+    if field is not None:
+        args["repeated_duration"] = field
 
     field = data.get("repeated_ip", None)
-    args["repeated_ip"] = field
+    if field is not None:
+        args["repeated_ip"] = field
 
     field = data.get("repeated_string_ip", None)
-    args["repeated_string_ip"] = field
+    if field is not None:
+        args["repeated_string_ip"] = field
 
     field = data.get("repeated_string_value_ip", None)
-    args["repeated_string_value_ip"] = field
+    if field is not None:
+        args["repeated_string_value_ip"] = field
 
     field = data.get("repeated_ipv4", None)
-    args["repeated_ipv4"] = field
+    if field is not None:
+        args["repeated_ipv4"] = field
 
     field = data.get("repeated_string_ipv4", None)
-    args["repeated_string_ipv4"] = field
+    if field is not None:
+        args["repeated_string_ipv4"] = field
 
     field = data.get("repeated_string_value_ipv4", None)
-    args["repeated_string_value_ipv4"] = field
+    if field is not None:
+        args["repeated_string_value_ipv4"] = field
 
     field = data.get("repeated_ipv6", None)
-    args["repeated_ipv6"] = field
+    if field is not None:
+        args["repeated_ipv6"] = field
 
     field = data.get("repeated_string_ipv6", None)
-    args["repeated_string_ipv6"] = field
+    if field is not None:
+        args["repeated_string_ipv6"] = field
 
     field = data.get("repeated_string_value_ipv6", None)
-    args["repeated_string_value_ipv6"] = field
+    if field is not None:
+        args["repeated_string_value_ipv6"] = field
 
     field = data.get("repeated_std_duration", None)
-    args["repeated_std_duration"] = field
+    if field is not None:
+        args["repeated_std_duration"] = field
 
     field = data.get("repeated_std_long_duration", None)
-    args["repeated_std_long_duration"] = field
+    if field is not None:
+        args["repeated_std_long_duration"] = field
 
     field = data.get("repeated_size", None)
-    args["repeated_size"] = field
+    if field is not None:
+        args["repeated_size"] = field
 
     field = data.get("repeated_uint64_size", None)
-    args["repeated_uint64_size"] = field
+    if field is not None:
+        args["repeated_uint64_size"] = field
 
     field = data.get("repeated_uint64value_size", None)
-    args["repeated_uint64value_size"] = field
+    if field is not None:
+        args["repeated_uint64value_size"] = field
 
     field = data.get("repeated_string_ipnet", None)
-    args["repeated_string_ipnet"] = field
+    if field is not None:
+        args["repeated_string_ipnet"] = field
 
     field = data.get("repeated_string_value_ipnet", None)
-    args["repeated_string_value_ipnet"] = field
+    if field is not None:
+        args["repeated_string_value_ipnet"] = field
 
     return PostAllTypesMessage(**args)
 
 
 def unmarshal_PostBodyAndPathSimpleMessage(data: Any) -> PostBodyAndPathSimpleMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostBodyAndPathSimpleMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("path", None)
-    args["path"] = field
+    if field is not None:
+        args["path"] = field
 
     field = data.get("body", None)
-    args["body"] = field
+    if field is not None:
+        args["body"] = field
 
     return PostBodyAndPathSimpleMessage(**args)
 
 
 def unmarshal_EchoMessage(data: Any) -> EchoMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'EchoMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("str_", None)
-    args["str_"] = field
+    if field is not None:
+        args["str_"] = field
 
     field = data.get("strs", None)
-    args["strs"] = field
+    if field is not None:
+        args["strs"] = field
 
     return EchoMessage(**args)
 
 
 def unmarshal_GetEnumMessage(data: Any) -> GetEnumMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetEnumMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     return GetEnumMessage(**args)
 
 
 def unmarshal_GetZoneResponse(data: Any) -> GetZoneResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetZoneResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     return GetZoneResponse(**args)
 
 
 def unmarshal_ListCharactersResponse(data: Any) -> ListCharactersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListCharactersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("characters", None)
-    args["characters"] = field
+    if field is not None:
+        args["characters"] = field
 
     return ListCharactersResponse(**args)
 
 
 def unmarshal_MetadataResponse(data: Any) -> MetadataResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'MetadataResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("metadata", None)
-    args["metadata"] = field
+    if field is not None:
+        args["metadata"] = field
 
     return MetadataResponse(**args)
 
 
 def unmarshal_PatchEnumMessage(data: Any) -> PatchEnumMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PatchEnumMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     return PatchEnumMessage(**args)
 
 
 def unmarshal_PostAllMapTypesMessage(data: Any) -> PostAllMapTypesMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostAllMapTypesMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("map_int32_int32", None)
-    args["map_int32_int32"] = field
+    if field is not None:
+        args["map_int32_int32"] = field
 
     field = data.get("map_int64_int64", None)
-    args["map_int64_int64"] = field
+    if field is not None:
+        args["map_int64_int64"] = field
 
     field = data.get("map_uint32_uint32", None)
-    args["map_uint32_uint32"] = field
+    if field is not None:
+        args["map_uint32_uint32"] = field
 
     field = data.get("map_uint64_uint64", None)
-    args["map_uint64_uint64"] = field
+    if field is not None:
+        args["map_uint64_uint64"] = field
 
     field = data.get("map_sint32_sint32", None)
-    args["map_sint32_sint32"] = field
+    if field is not None:
+        args["map_sint32_sint32"] = field
 
     field = data.get("map_sint64_sint64", None)
-    args["map_sint64_sint64"] = field
+    if field is not None:
+        args["map_sint64_sint64"] = field
 
     field = data.get("map_fixed32_fixed32", None)
-    args["map_fixed32_fixed32"] = field
+    if field is not None:
+        args["map_fixed32_fixed32"] = field
 
     field = data.get("map_fixed64_fixed64", None)
-    args["map_fixed64_fixed64"] = field
+    if field is not None:
+        args["map_fixed64_fixed64"] = field
 
     field = data.get("map_sfixed32_sfixed32", None)
-    args["map_sfixed32_sfixed32"] = field
+    if field is not None:
+        args["map_sfixed32_sfixed32"] = field
 
     field = data.get("map_sfixed64_sfixed64", None)
-    args["map_sfixed64_sfixed64"] = field
+    if field is not None:
+        args["map_sfixed64_sfixed64"] = field
 
     field = data.get("map_int32_float", None)
-    args["map_int32_float"] = field
+    if field is not None:
+        args["map_int32_float"] = field
 
     field = data.get("map_int32_double", None)
-    args["map_int32_double"] = field
+    if field is not None:
+        args["map_int32_double"] = field
 
     field = data.get("map_string_string", None)
-    args["map_string_string"] = field
+    if field is not None:
+        args["map_string_string"] = field
 
     field = data.get("map_int32_bytes", None)
-    args["map_int32_bytes"] = field
+    if field is not None:
+        args["map_int32_bytes"] = field
 
     field = data.get("map_int32_enum", None)
-    args["map_int32_enum"] = (
-        {key: MapEnum(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["map_int32_enum"] = (
+            {key: MapEnum(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     field = data.get("map_int32_all_types", None)
-    args["map_int32_all_types"] = (
-        {key: unmarshal_PostAllTypesMessage(value) for key, value in field.items()}
-        if field is not None
-        else None
-    )
+    if field is not None:
+        args["map_int32_all_types"] = (
+            {key: unmarshal_PostAllTypesMessage(value) for key, value in field.items()}
+            if field is not None
+            else None
+        )
 
     field = data.get("map_int32_ip", None)
-    args["map_int32_ip"] = field
+    if field is not None:
+        args["map_int32_ip"] = field
 
     field = data.get("map_int32_std_duration", None)
-    args["map_int32_std_duration"] = field
+    if field is not None:
+        args["map_int32_std_duration"] = field
 
     field = data.get("map_int32_std_long_duration", None)
-    args["map_int32_std_long_duration"] = field
+    if field is not None:
+        args["map_int32_std_long_duration"] = field
 
     field = data.get("map_int32_size", None)
-    args["map_int32_size"] = field
+    if field is not None:
+        args["map_int32_size"] = field
 
     field = data.get("map_int32_uint64_size", None)
-    args["map_int32_uint64_size"] = field
+    if field is not None:
+        args["map_int32_uint64_size"] = field
 
     field = data.get("map_int32_uint64value_size", None)
-    args["map_int32_uint64value_size"] = field
+    if field is not None:
+        args["map_int32_uint64value_size"] = field
 
     field = data.get("map_int32_string_ip", None)
-    args["map_int32_string_ip"] = field
+    if field is not None:
+        args["map_int32_string_ip"] = field
 
     field = data.get("map_int32_string_value_ip", None)
-    args["map_int32_string_value_ip"] = field
+    if field is not None:
+        args["map_int32_string_value_ip"] = field
 
     field = data.get("map_int32_ipv4", None)
-    args["map_int32_ipv4"] = field
+    if field is not None:
+        args["map_int32_ipv4"] = field
 
     field = data.get("map_int32_string_ipv4", None)
-    args["map_int32_string_ipv4"] = field
+    if field is not None:
+        args["map_int32_string_ipv4"] = field
 
     field = data.get("map_int32_string_value_ipv4", None)
-    args["map_int32_string_value_ipv4"] = field
+    if field is not None:
+        args["map_int32_string_value_ipv4"] = field
 
     field = data.get("map_int32_ipv6", None)
-    args["map_int32_ipv6"] = field
+    if field is not None:
+        args["map_int32_ipv6"] = field
 
     field = data.get("map_int32_string_ipv6", None)
-    args["map_int32_string_ipv6"] = field
+    if field is not None:
+        args["map_int32_string_ipv6"] = field
 
     field = data.get("map_int32_string_value_ipv6", None)
-    args["map_int32_string_value_ipv6"] = field
+    if field is not None:
+        args["map_int32_string_value_ipv6"] = field
 
     field = data.get("map_int32_strings_value", None)
-    args["map_int32_strings_value"] = field
+    if field is not None:
+        args["map_int32_strings_value"] = field
 
     field = data.get("map_int32_duration", None)
-    args["map_int32_duration"] = field
+    if field is not None:
+        args["map_int32_duration"] = field
 
     return PostAllMapTypesMessage(**args)
 
 
 def unmarshal_PostAllOptionalMessageNestedMessage(
     data: Any,
 ) -> PostAllOptionalMessageNestedMessage:
@@ -640,15 +787,16 @@
         raise TypeError(
             "Unmarshalling the type 'PostAllOptionalMessageNestedMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("s", None)
-    args["s"] = field
+    if field is not None:
+        args["s"] = field
 
     return PostAllOptionalMessageNestedMessage(**args)
 
 
 def unmarshal_PostAllOptionalMessageNestedMessageWithOptional(
     data: Any,
 ) -> PostAllOptionalMessageNestedMessageWithOptional:
@@ -656,154 +804,195 @@
         raise TypeError(
             "Unmarshalling the type 'PostAllOptionalMessageNestedMessageWithOptional' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("bb", None)
-    args["bb"] = field
+    if field is not None:
+        args["bb"] = field
 
     return PostAllOptionalMessageNestedMessageWithOptional(**args)
 
 
 def unmarshal_PostAllOptionalMessage(data: Any) -> PostAllOptionalMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostAllOptionalMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("optional_int32", None)
-    args["optional_int32"] = field
+    if field is not None:
+        args["optional_int32"] = field
 
     field = data.get("optional_int64", None)
-    args["optional_int64"] = field
+    if field is not None:
+        args["optional_int64"] = field
 
     field = data.get("optional_uint32", None)
-    args["optional_uint32"] = field
+    if field is not None:
+        args["optional_uint32"] = field
 
     field = data.get("optional_uint64", None)
-    args["optional_uint64"] = field
+    if field is not None:
+        args["optional_uint64"] = field
 
     field = data.get("optional_sint32", None)
-    args["optional_sint32"] = field
+    if field is not None:
+        args["optional_sint32"] = field
 
     field = data.get("optional_sint64", None)
-    args["optional_sint64"] = field
+    if field is not None:
+        args["optional_sint64"] = field
 
     field = data.get("optional_fixed32", None)
-    args["optional_fixed32"] = field
+    if field is not None:
+        args["optional_fixed32"] = field
 
     field = data.get("optional_fixed64", None)
-    args["optional_fixed64"] = field
+    if field is not None:
+        args["optional_fixed64"] = field
 
     field = data.get("optional_sfixed32", None)
-    args["optional_sfixed32"] = field
+    if field is not None:
+        args["optional_sfixed32"] = field
 
     field = data.get("optional_sfixed64", None)
-    args["optional_sfixed64"] = field
+    if field is not None:
+        args["optional_sfixed64"] = field
 
     field = data.get("optional_float", None)
-    args["optional_float"] = field
+    if field is not None:
+        args["optional_float"] = field
 
     field = data.get("optional_double", None)
-    args["optional_double"] = field
+    if field is not None:
+        args["optional_double"] = field
 
     field = data.get("optional_bool", None)
-    args["optional_bool"] = field
+    if field is not None:
+        args["optional_bool"] = field
 
     field = data.get("optional_string", None)
-    args["optional_string"] = field
+    if field is not None:
+        args["optional_string"] = field
 
     field = data.get("optional_bytes", None)
-    args["optional_bytes"] = field
+    if field is not None:
+        args["optional_bytes"] = field
 
     field = data.get("optional_cord", None)
-    args["optional_cord"] = field
+    if field is not None:
+        args["optional_cord"] = field
 
     field = data.get("optional_nested_message_with_optional", None)
-    args[
-        "optional_nested_message_with_optional"
-    ] = unmarshal_PostAllOptionalMessageNestedMessageWithOptional(field)
+    if field is not None:
+        args[
+            "optional_nested_message_with_optional"
+        ] = unmarshal_PostAllOptionalMessageNestedMessageWithOptional(field)
 
     field = data.get("lazy_nested_message_with_optional", None)
-    args[
-        "lazy_nested_message_with_optional"
-    ] = unmarshal_PostAllOptionalMessageNestedMessageWithOptional(field)
+    if field is not None:
+        args[
+            "lazy_nested_message_with_optional"
+        ] = unmarshal_PostAllOptionalMessageNestedMessageWithOptional(field)
 
     field = data.get("optional_nested_enum", None)
-    args["optional_nested_enum"] = field
+    if field is not None:
+        args["optional_nested_enum"] = field
 
     field = data.get("optional_nested_message", None)
-    args["optional_nested_message"] = unmarshal_PostAllOptionalMessageNestedMessage(
-        field
-    )
+    if field is not None:
+        args["optional_nested_message"] = unmarshal_PostAllOptionalMessageNestedMessage(
+            field
+        )
 
     field = data.get("singular_int32", None)
-    args["singular_int32"] = field
+    if field is not None:
+        args["singular_int32"] = field
 
     field = data.get("singular_int64", None)
-    args["singular_int64"] = field
+    if field is not None:
+        args["singular_int64"] = field
 
     field = data.get("nested_message", None)
-    args["nested_message"] = unmarshal_PostAllOptionalMessageNestedMessage(field)
+    if field is not None:
+        args["nested_message"] = unmarshal_PostAllOptionalMessageNestedMessage(field)
 
     field = data.get("singular_double_value", None)
-    args["singular_double_value"] = field
+    if field is not None:
+        args["singular_double_value"] = field
 
     field = data.get("singular_float_value", None)
-    args["singular_float_value"] = field
+    if field is not None:
+        args["singular_float_value"] = field
 
     field = data.get("singular_int64_value", None)
-    args["singular_int64_value"] = field
+    if field is not None:
+        args["singular_int64_value"] = field
 
     field = data.get("singular_uint64_value", None)
-    args["singular_uint64_value"] = field
+    if field is not None:
+        args["singular_uint64_value"] = field
 
     field = data.get("singular_int32_value", None)
-    args["singular_int32_value"] = field
+    if field is not None:
+        args["singular_int32_value"] = field
 
     field = data.get("singular_uint32_value", None)
-    args["singular_uint32_value"] = field
+    if field is not None:
+        args["singular_uint32_value"] = field
 
     field = data.get("singular_bool_value", None)
-    args["singular_bool_value"] = field
+    if field is not None:
+        args["singular_bool_value"] = field
 
     field = data.get("singular_string_value", None)
-    args["singular_string_value"] = field
+    if field is not None:
+        args["singular_string_value"] = field
 
     field = data.get("singular_bytes_value", None)
-    args["singular_bytes_value"] = field
+    if field is not None:
+        args["singular_bytes_value"] = field
 
     field = data.get("singular_timestamp", None)
-    args["singular_timestamp"] = (
-        parser.isoparse(field) if isinstance(field, str) else field
-    )
+    if field is not None:
+        args["singular_timestamp"] = (
+            parser.isoparse(field) if isinstance(field, str) else field
+        )
 
     field = data.get("singular_any", None)
-    args["singular_any"] = field
+    if field is not None:
+        args["singular_any"] = field
 
     field = data.get("singular_struct", None)
-    args["singular_struct"] = field
+    if field is not None:
+        args["singular_struct"] = field
 
     field = data.get("singular_money", None)
-    args["singular_money"] = unmarshal_Money(field)
+    if field is not None:
+        args["singular_money"] = unmarshal_Money(field)
 
     field = data.get("singular_strings_value", None)
-    args["singular_strings_value"] = field
+    if field is not None:
+        args["singular_strings_value"] = field
 
     field = data.get("singular_duration", None)
-    args["singular_duration"] = field
+    if field is not None:
+        args["singular_duration"] = field
 
     field = data.get("map_string_string", None)
-    args["map_string_string"] = field
+    if field is not None:
+        args["map_string_string"] = field
 
     field = data.get("timeseries", None)
-    args["timeseries"] = unmarshal_TimeSeries(field)
+    if field is not None:
+        args["timeseries"] = unmarshal_TimeSeries(field)
 
     return PostAllOptionalMessage(**args)
 
 
 def unmarshal_PostBodyAndPathAndQueryMessage(
     data: Any,
 ) -> PostBodyAndPathAndQueryMessage:
@@ -811,131 +1000,156 @@
         raise TypeError(
             "Unmarshalling the type 'PostBodyAndPathAndQueryMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("path", None)
-    args["path"] = field
+    if field is not None:
+        args["path"] = field
 
     field = data.get("query", None)
-    args["query"] = field
+    if field is not None:
+        args["query"] = field
 
     field = data.get("body", None)
-    args["body"] = unmarshal_PostBodyAndPathSimpleMessage(field)
+    if field is not None:
+        args["body"] = unmarshal_PostBodyAndPathSimpleMessage(field)
 
     return PostBodyAndPathAndQueryMessage(**args)
 
 
 def unmarshal_PostBodyAndPathComplexMessage(data: Any) -> PostBodyAndPathComplexMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostBodyAndPathComplexMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("path", None)
-    args["path"] = field
+    if field is not None:
+        args["path"] = field
 
     field = data.get("body", None)
-    args["body"] = unmarshal_PostBodyAndPathSimpleMessage(field)
+    if field is not None:
+        args["body"] = unmarshal_PostBodyAndPathSimpleMessage(field)
 
     return PostBodyAndPathComplexMessage(**args)
 
 
 def unmarshal_PostBodyAndPathSimple2Message(data: Any) -> PostBodyAndPathSimple2Message:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostBodyAndPathSimple2Message' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("path", None)
-    args["path"] = field
+    if field is not None:
+        args["path"] = field
 
     field = data.get("body", None)
-    args["body"] = field
+    if field is not None:
+        args["body"] = field
 
     return PostBodyAndPathSimple2Message(**args)
 
 
 def unmarshal_ComplexValidateMsg(data: Any) -> ComplexValidateMsg:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ComplexValidateMsg' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("const", None)
-    args["const"] = field
+    if field is not None:
+        args["const"] = field
 
     field = data.get("int_const", None)
-    args["int_const"] = field
+    if field is not None:
+        args["int_const"] = field
 
     field = data.get("bool_const", None)
-    args["bool_const"] = field
+    if field is not None:
+        args["bool_const"] = field
 
     field = data.get("float_const", None)
-    args["float_const"] = field
+    if field is not None:
+        args["float_const"] = field
 
     field = data.get("double_in", None)
-    args["double_in"] = field
+    if field is not None:
+        args["double_in"] = field
 
     field = data.get("enum_const", None)
-    args["enum_const"] = field
+    if field is not None:
+        args["enum_const"] = field
 
     field = data.get("nested", None)
-    args["nested"] = unmarshal_ComplexValidateMsg(field)
+    if field is not None:
+        args["nested"] = unmarshal_ComplexValidateMsg(field)
 
     field = data.get("float_val", None)
-    args["float_val"] = field
+    if field is not None:
+        args["float_val"] = field
 
     field = data.get("dur_val", None)
-    args["dur_val"] = field
+    if field is not None:
+        args["dur_val"] = field
 
     field = data.get("ts_val", None)
-    args["ts_val"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["ts_val"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("another", None)
-    args["another"] = unmarshal_ComplexValidateMsg(field)
+    if field is not None:
+        args["another"] = unmarshal_ComplexValidateMsg(field)
 
     field = data.get("any_val", None)
-    args["any_val"] = field
+    if field is not None:
+        args["any_val"] = field
 
     field = data.get("rep_ts_val", None)
-    args["rep_ts_val"] = field
+    if field is not None:
+        args["rep_ts_val"] = field
 
     field = data.get("map_val", None)
-    args["map_val"] = field
+    if field is not None:
+        args["map_val"] = field
 
     field = data.get("bytes_val", None)
-    args["bytes_val"] = field
+    if field is not None:
+        args["bytes_val"] = field
 
     field = data.get("x", None)
-    args["x"] = field
+    if field is not None:
+        args["x"] = field
 
     field = data.get("y", None)
-    args["y"] = field
+    if field is not None:
+        args["y"] = field
 
     return ComplexValidateMsg(**args)
 
 
 def unmarshal_PostComplexValidateMessage(data: Any) -> PostComplexValidateMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostComplexValidateMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("val", None)
-    args["val"] = unmarshal_ComplexValidateMsg(field)
+    if field is not None:
+        args["val"] = unmarshal_ComplexValidateMsg(field)
 
     return PostComplexValidateMessage(**args)
 
 
 def unmarshal_PostDeprecatedOrganizationMessage(
     data: Any,
 ) -> PostDeprecatedOrganizationMessage:
@@ -943,211 +1157,237 @@
         raise TypeError(
             "Unmarshalling the type 'PostDeprecatedOrganizationMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("organization", None)
-    args["organization"] = field
+    if field is not None:
+        args["organization"] = field
 
     return PostDeprecatedOrganizationMessage(**args)
 
 
 def unmarshal_PostDeprecatedProjectMessage(data: Any) -> PostDeprecatedProjectMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostDeprecatedProjectMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("project", None)
-    args["project"] = field
+    if field is not None:
+        args["project"] = field
 
     return PostDeprecatedProjectMessage(**args)
 
 
 def unmarshal_PostEchoTimeSeriesMessage(data: Any) -> PostEchoTimeSeriesMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostEchoTimeSeriesMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("metrics", None)
-    args["metrics"] = unmarshal_TimeSeries(field)
+    if field is not None:
+        args["metrics"] = unmarshal_TimeSeries(field)
 
     return PostEchoTimeSeriesMessage(**args)
 
 
 def unmarshal_PostEnumMessage(data: Any) -> PostEnumMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostEnumMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("type2", None)
-    args["type2"] = field
+    if field is not None:
+        args["type2"] = field
 
     field = data.get("type3", None)
-    args["type3"] = field
+    if field is not None:
+        args["type3"] = field
 
     return PostEnumMessage(**args)
 
 
 def unmarshal_PostIPMessage(data: Any) -> PostIPMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostIPMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("ip_v4", None)
-    args["ip_v4"] = field
+    if field is not None:
+        args["ip_v4"] = field
 
     field = data.get("ip_v6", None)
-    args["ip_v6"] = field
+    if field is not None:
+        args["ip_v6"] = field
 
     field = data.get("ip", None)
-    args["ip"] = field
+    if field is not None:
+        args["ip"] = field
 
     return PostIPMessage(**args)
 
 
 def unmarshal_PostOneOfMessage(data: Any) -> PostOneOfMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostOneOfMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("test", None)
-    args["test"] = field
+    if field is not None:
+        args["test"] = field
 
     field = data.get("test2", None)
-    args["test2"] = field
+    if field is not None:
+        args["test2"] = field
 
     field = data.get("test_nested", None)
-    args["test_nested"] = unmarshal_EchoMessage(field)
+    if field is not None:
+        args["test_nested"] = unmarshal_EchoMessage(field)
 
     field = data.get("test3", None)
-    args["test3"] = field
+    if field is not None:
+        args["test3"] = field
 
     return PostOneOfMessage(**args)
 
 
 def unmarshal_PostOrganizationIdMessage(data: Any) -> PostOrganizationIdMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostOrganizationIdMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     return PostOrganizationIdMessage(**args)
 
 
 def unmarshal_PostProjectIdMessage(data: Any) -> PostProjectIdMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostProjectIdMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     return PostProjectIdMessage(**args)
 
 
 def unmarshal_PostScalarTypesMessage(data: Any) -> PostScalarTypesMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostScalarTypesMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("double_field", None)
-    args["double_field"] = field
+    if field is not None:
+        args["double_field"] = field
 
     field = data.get("float_field", None)
-    args["float_field"] = field
+    if field is not None:
+        args["float_field"] = field
 
     field = data.get("int32_field", None)
-    args["int32_field"] = field
+    if field is not None:
+        args["int32_field"] = field
 
     field = data.get("int64_field", None)
-    args["int64_field"] = field
+    if field is not None:
+        args["int64_field"] = field
 
     field = data.get("uint32_field", None)
-    args["uint32_field"] = field
+    if field is not None:
+        args["uint32_field"] = field
 
     field = data.get("uint64_field", None)
-    args["uint64_field"] = field
+    if field is not None:
+        args["uint64_field"] = field
 
     field = data.get("bool_field", None)
-    args["bool_field"] = field
+    if field is not None:
+        args["bool_field"] = field
 
     field = data.get("string_field", None)
-    args["string_field"] = field
+    if field is not None:
+        args["string_field"] = field
 
     return PostScalarTypesMessage(**args)
 
 
 def unmarshal_PostTagsMessage(data: Any) -> PostTagsMessage:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PostTagsMessage' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     return PostTagsMessage(**args)
 
 
 def unmarshal_Transient(data: Any) -> Transient:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Transient' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     return Transient(**args)
 
 
 def unmarshal__GetRegionResponse(data: Any) -> _GetRegionResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type '_GetRegionResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     return _GetRegionResponse(**args)
 
 
 def marshal_PatchEnumRequest(
     request: PatchEnumRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/testinternal/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/testinternal/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v1/marshalling.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,58 +18,69 @@
         raise TypeError(
             "Unmarshalling the type 'PrivateNetwork' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["zone"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("subnets", None)
-    args["subnets"] = field
+    if field is not None:
+        args["subnets"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return PrivateNetwork(**args)
 
 
 def unmarshal_ListPrivateNetworksResponse(data: Any) -> ListPrivateNetworksResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPrivateNetworksResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_networks", None)
-    args["private_networks"] = (
-        [unmarshal_PrivateNetwork(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["private_networks"] = (
+            [unmarshal_PrivateNetwork(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPrivateNetworksResponse(**args)
 
 
 def marshal_CreatePrivateNetworkRequest(
     request: CreatePrivateNetworkRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v2/__init__.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v2/api.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v2/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v2/marshalling.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,189 +34,221 @@
         raise TypeError(
             "Unmarshalling the type 'Subnet' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("subnet", None)
-    args["subnet"] = field
+    if field is not None:
+        args["subnet"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return Subnet(**args)
 
 
 def unmarshal_PrivateNetwork(data: Any) -> PrivateNetwork:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'PrivateNetwork' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("subnets", None)
-    args["subnets"] = (
-        [unmarshal_Subnet(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["subnets"] = (
+            [unmarshal_Subnet(v) for v in field] if field is not None else None
+        )
 
     field = data.get("vpc_id", None)
-    args["vpc_id"] = field
+    if field is not None:
+        args["vpc_id"] = field
 
     field = data.get("dhcp_enabled", None)
-    args["dhcp_enabled"] = field
+    if field is not None:
+        args["dhcp_enabled"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return PrivateNetwork(**args)
 
 
 def unmarshal_VPC(data: Any) -> VPC:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'VPC' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("is_default", None)
-    args["is_default"] = field
+    if field is not None:
+        args["is_default"] = field
 
     field = data.get("private_network_count", None)
-    args["private_network_count"] = field
+    if field is not None:
+        args["private_network_count"] = field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     return VPC(**args)
 
 
 def unmarshal_AddSubnetsResponse(data: Any) -> AddSubnetsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'AddSubnetsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("subnets", None)
-    args["subnets"] = field
+    if field is not None:
+        args["subnets"] = field
 
     return AddSubnetsResponse(**args)
 
 
 def unmarshal_DeleteSubnetsResponse(data: Any) -> DeleteSubnetsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DeleteSubnetsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("subnets", None)
-    args["subnets"] = field
+    if field is not None:
+        args["subnets"] = field
 
     return DeleteSubnetsResponse(**args)
 
 
 def unmarshal_ListPrivateNetworksResponse(data: Any) -> ListPrivateNetworksResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListPrivateNetworksResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("private_networks", None)
-    args["private_networks"] = (
-        [unmarshal_PrivateNetwork(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["private_networks"] = (
+            [unmarshal_PrivateNetwork(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListPrivateNetworksResponse(**args)
 
 
 def unmarshal_ListVPCsResponse(data: Any) -> ListVPCsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVPCsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("vpcs", None)
-    args["vpcs"] = [unmarshal_VPC(v) for v in field] if field is not None else None
+    if field is not None:
+        args["vpcs"] = [unmarshal_VPC(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     return ListVPCsResponse(**args)
 
 
 def unmarshal_SetSubnetsResponse(data: Any) -> SetSubnetsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'SetSubnetsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("subnets", None)
-    args["subnets"] = field
+    if field is not None:
+        args["subnets"] = field
 
     return SetSubnetsResponse(**args)
 
 
 def marshal_AddSubnetsRequest(
     request: AddSubnetsRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/vpc/v2/types.py` & `scaleway-2.0.0.dev6/scaleway/vpc/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpcgw/v1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/vpcgw/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpcgw/v1/api.py` & `scaleway-2.0.0.dev6/scaleway/vpcgw/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpcgw/v1/content.py` & `scaleway-2.0.0.dev6/scaleway/vpcgw/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/vpcgw/v1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/container/v1beta1/marshalling.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,969 +6,1049 @@
 
 from scaleway_core.profile import ProfileDefaults
 from scaleway_core.utils import (
     OneOfPossibility,
     resolve_one_of,
 )
 from .types import (
-    DHCP,
-    IpamConfig,
-    GatewayNetwork,
-    IP,
-    DHCPEntry,
-    GatewayType,
-    Gateway,
-    PATRule,
-    ListDHCPEntriesResponse,
-    ListDHCPsResponse,
-    ListGatewayNetworksResponse,
-    ListGatewayTypesResponse,
-    ListGatewaysResponse,
-    ListIPsResponse,
-    ListPATRulesResponse,
-    SetDHCPEntriesResponse,
-    SetPATRulesResponse,
-    CreateDHCPRequest,
-    CreateDHCPEntryRequest,
-    CreateGatewayNetworkRequestIpamConfig,
-    CreateGatewayNetworkRequest,
-    CreateGatewayRequest,
-    CreateIPRequest,
-    CreatePATRuleRequest,
-    SetDHCPEntriesRequestEntry,
-    SetDHCPEntriesRequest,
-    SetPATRulesRequestRule,
-    SetPATRulesRequest,
-    UpdateDHCPEntryRequest,
-    UpdateDHCPRequest,
-    UpdateGatewayNetworkRequestIpamConfig,
-    UpdateGatewayNetworkRequest,
-    UpdateGatewayRequest,
-    UpdateIPRequest,
-    UpdatePATRuleRequest,
+    SecretHashedValue,
+    Container,
+    Cron,
+    Domain,
+    Namespace,
+    Token,
+    TriggerMnqNatsClientConfig,
+    TriggerMnqSqsClientConfig,
+    TriggerSqsClientConfig,
+    Trigger,
+    ListContainersResponse,
+    ListCronsResponse,
+    ListDomainsResponse,
+    Log,
+    ListLogsResponse,
+    ListNamespacesResponse,
+    ListTokensResponse,
+    ListTriggersResponse,
+    Secret,
+    CreateContainerRequest,
+    CreateCronRequest,
+    CreateDomainRequest,
+    CreateNamespaceRequest,
+    CreateTokenRequest,
+    CreateTriggerRequestMnqNatsClientConfig,
+    CreateTriggerRequestMnqSqsClientConfig,
+    CreateTriggerRequestSqsClientConfig,
+    CreateTriggerRequest,
+    UpdateContainerRequest,
+    UpdateCronRequest,
+    UpdateNamespaceRequest,
+    UpdateTriggerRequestSqsClientConfig,
+    UpdateTriggerRequest,
 )
 
 
-def unmarshal_DHCP(data: Any) -> DHCP:
+def unmarshal_SecretHashedValue(data: Any) -> SecretHashedValue:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'DHCP' failed as data isn't a dictionary."
+            "Unmarshalling the type 'SecretHashedValue' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("organization_id", None)
-    args["organization_id"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
-
-    field = data.get("subnet", None)
-    args["subnet"] = field
-
-    field = data.get("address", None)
-    args["address"] = field
+    field = data.get("key", None)
+    if field is not None:
+        args["key"] = field
 
-    field = data.get("pool_low", None)
-    args["pool_low"] = field
+    field = data.get("hashed_value", None)
+    if field is not None:
+        args["hashed_value"] = field
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    return SecretHashedValue(**args)
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    field = data.get("pool_high", None)
-    args["pool_high"] = field
+def unmarshal_Container(data: Any) -> Container:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'Container' failed as data isn't a dictionary."
+        )
 
-    field = data.get("enable_dynamic", None)
-    args["enable_dynamic"] = field
+    args: Dict[str, Any] = {}
 
-    field = data.get("push_default_route", None)
-    args["push_default_route"] = field
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("push_dns_server", None)
-    args["push_dns_server"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("dns_servers_override", None)
-    args["dns_servers_override"] = field
+    field = data.get("namespace_id", None)
+    if field is not None:
+        args["namespace_id"] = field
 
-    field = data.get("dns_search", None)
-    args["dns_search"] = field
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("dns_local_name", None)
-    args["dns_local_name"] = field
+    field = data.get("environment_variables", None)
+    if field is not None:
+        args["environment_variables"] = field
+
+    field = data.get("min_scale", None)
+    if field is not None:
+        args["min_scale"] = field
+
+    field = data.get("max_scale", None)
+    if field is not None:
+        args["max_scale"] = field
+
+    field = data.get("memory_limit", None)
+    if field is not None:
+        args["memory_limit"] = field
+
+    field = data.get("cpu_limit", None)
+    if field is not None:
+        args["cpu_limit"] = field
+
+    field = data.get("privacy", None)
+    if field is not None:
+        args["privacy"] = field
+
+    field = data.get("registry_image", None)
+    if field is not None:
+        args["registry_image"] = field
+
+    field = data.get("max_concurrency", None)
+    if field is not None:
+        args["max_concurrency"] = field
+
+    field = data.get("timeout", None)
+    if field is not None:
+        args["timeout"] = field
+
+    field = data.get("error_message", None)
+    if field is not None:
+        args["error_message"] = field
+
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
+
+    field = data.get("domain_name", None)
+    if field is not None:
+        args["domain_name"] = field
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("protocol", None)
+    if field is not None:
+        args["protocol"] = field
 
-    field = data.get("valid_lifetime", None)
-    args["valid_lifetime"] = field
+    field = data.get("port", None)
+    if field is not None:
+        args["port"] = field
+
+    field = data.get("secret_environment_variables", None)
+    if field is not None:
+        args["secret_environment_variables"] = (
+            [unmarshal_SecretHashedValue(v) for v in field]
+            if field is not None
+            else None
+        )
 
-    field = data.get("renew_timer", None)
-    args["renew_timer"] = field
+    field = data.get("http_option", None)
+    if field is not None:
+        args["http_option"] = field
 
-    field = data.get("rebind_timer", None)
-    args["rebind_timer"] = field
+    field = data.get("region", None)
+    if field is not None:
+        args["region"] = field
 
-    return DHCP(**args)
+    return Container(**args)
 
 
-def unmarshal_IpamConfig(data: Any) -> IpamConfig:
+def unmarshal_Cron(data: Any) -> Cron:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'IpamConfig' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Cron' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("push_default_route", None)
-    args["push_default_route"] = field
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
+
+    field = data.get("container_id", None)
+    if field is not None:
+        args["container_id"] = field
+
+    field = data.get("schedule", None)
+    if field is not None:
+        args["schedule"] = field
+
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
+
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("ipam_ip_id", None)
-    args["ipam_ip_id"] = field
+    field = data.get("args", None)
+    if field is not None:
+        args["args"] = field
 
-    return IpamConfig(**args)
+    return Cron(**args)
 
 
-def unmarshal_GatewayNetwork(data: Any) -> GatewayNetwork:
+def unmarshal_Domain(data: Any) -> Domain:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'GatewayNetwork' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Domain' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("gateway_id", None)
-    args["gateway_id"] = field
-
-    field = data.get("private_network_id", None)
-    args["private_network_id"] = field
-
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
-
-    field = data.get("mac_address", None)
-    args["mac_address"] = field
+    field = data.get("hostname", None)
+    if field is not None:
+        args["hostname"] = field
 
-    field = data.get("enable_masquerade", None)
-    args["enable_masquerade"] = field
+    field = data.get("container_id", None)
+    if field is not None:
+        args["container_id"] = field
+
+    field = data.get("url", None)
+    if field is not None:
+        args["url"] = field
 
     field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("enable_dhcp", None)
-    args["enable_dhcp"] = field
-
-    field = data.get("zone", None)
-    args["zone"] = field
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("dhcp", None)
-    args["dhcp"] = unmarshal_DHCP(field)
+    field = data.get("error_message", None)
+    if field is not None:
+        args["error_message"] = field
 
-    field = data.get("address", None)
-    args["address"] = field
+    return Domain(**args)
 
-    field = data.get("ipam_config", None)
-    args["ipam_config"] = unmarshal_IpamConfig(field)
 
-    return GatewayNetwork(**args)
-
-
-def unmarshal_IP(data: Any) -> IP:
+def unmarshal_Namespace(data: Any) -> Namespace:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'IP' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Namespace' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("organization_id", None)
-    args["organization_id"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("project_id", None)
-    args["project_id"] = field
+    field = data.get("environment_variables", None)
+    if field is not None:
+        args["environment_variables"] = field
 
-    field = data.get("tags", None)
-    args["tags"] = field
+    field = data.get("organization_id", None)
+    if field is not None:
+        args["organization_id"] = field
 
-    field = data.get("address", None)
-    args["address"] = field
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("registry_namespace_id", None)
+    if field is not None:
+        args["registry_namespace_id"] = field
+
+    field = data.get("registry_endpoint", None)
+    if field is not None:
+        args["registry_endpoint"] = field
+
+    field = data.get("secret_environment_variables", None)
+    if field is not None:
+        args["secret_environment_variables"] = (
+            [unmarshal_SecretHashedValue(v) for v in field]
+            if field is not None
+            else None
+        )
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("region", None)
+    if field is not None:
+        args["region"] = field
 
-    field = data.get("reverse", None)
-    args["reverse"] = field
+    field = data.get("error_message", None)
+    if field is not None:
+        args["error_message"] = field
 
-    field = data.get("gateway_id", None)
-    args["gateway_id"] = field
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
 
-    return IP(**args)
+    return Namespace(**args)
 
 
-def unmarshal_DHCPEntry(data: Any) -> DHCPEntry:
+def unmarshal_Token(data: Any) -> Token:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'DHCPEntry' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Token' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("gateway_network_id", None)
-    args["gateway_network_id"] = field
+    field = data.get("token", None)
+    if field is not None:
+        args["token"] = field
 
-    field = data.get("mac_address", None)
-    args["mac_address"] = field
-
-    field = data.get("ip_address", None)
-    args["ip_address"] = field
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("hostname", None)
-    args["hostname"] = field
+    field = data.get("container_id", None)
+    if field is not None:
+        args["container_id"] = field
 
-    field = data.get("type_", None)
-    args["type_"] = field
+    field = data.get("namespace_id", None)
+    if field is not None:
+        args["namespace_id"] = field
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("public_key", None)
+    if field is not None:
+        args["public_key"] = field
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("expires_at", None)
+    if field is not None:
+        args["expires_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return DHCPEntry(**args)
+    return Token(**args)
 
 
-def unmarshal_GatewayType(data: Any) -> GatewayType:
+def unmarshal_TriggerMnqNatsClientConfig(data: Any) -> TriggerMnqNatsClientConfig:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'GatewayType' failed as data isn't a dictionary."
+            "Unmarshalling the type 'TriggerMnqNatsClientConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("subject", None)
+    if field is not None:
+        args["subject"] = field
+
+    field = data.get("mnq_nats_account_id", None)
+    if field is not None:
+        args["mnq_nats_account_id"] = field
+
+    field = data.get("mnq_project_id", None)
+    if field is not None:
+        args["mnq_project_id"] = field
 
-    field = data.get("bandwidth", None)
-    args["bandwidth"] = field
+    field = data.get("mnq_region", None)
+    if field is not None:
+        args["mnq_region"] = field
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("mnq_namespace_id", None)
+    if field is not None:
+        args["mnq_namespace_id"] = field
 
-    return GatewayType(**args)
+    field = data.get("mnq_credential_id", None)
+    if field is not None:
+        args["mnq_credential_id"] = field
 
+    return TriggerMnqNatsClientConfig(**args)
 
-def unmarshal_Gateway(data: Any) -> Gateway:
+
+def unmarshal_TriggerMnqSqsClientConfig(data: Any) -> TriggerMnqSqsClientConfig:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'Gateway' failed as data isn't a dictionary."
+            "Unmarshalling the type 'TriggerMnqSqsClientConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("organization_id", None)
-    args["organization_id"] = field
-
-    field = data.get("project_id", None)
-    args["project_id"] = field
-
-    field = data.get("status", None)
-    args["status"] = field
-
-    field = data.get("name", None)
-    args["name"] = field
+    field = data.get("queue", None)
+    if field is not None:
+        args["queue"] = field
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("mnq_project_id", None)
+    if field is not None:
+        args["mnq_project_id"] = field
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("mnq_region", None)
+    if field is not None:
+        args["mnq_region"] = field
 
-    field = data.get("type_", None)
-    args["type_"] = unmarshal_GatewayType(field)
-
-    field = data.get("tags", None)
-    args["tags"] = field
-
-    field = data.get("gateway_networks", None)
-    args["gateway_networks"] = (
-        [unmarshal_GatewayNetwork(v) for v in field] if field is not None else None
-    )
+    field = data.get("mnq_namespace_id", None)
+    if field is not None:
+        args["mnq_namespace_id"] = field
 
-    field = data.get("upstream_dns_servers", None)
-    args["upstream_dns_servers"] = field
+    field = data.get("mnq_credential_id", None)
+    if field is not None:
+        args["mnq_credential_id"] = field
 
-    field = data.get("bastion_enabled", None)
-    args["bastion_enabled"] = field
+    return TriggerMnqSqsClientConfig(**args)
 
-    field = data.get("bastion_port", None)
-    args["bastion_port"] = field
 
-    field = data.get("smtp_enabled", None)
-    args["smtp_enabled"] = field
+def unmarshal_TriggerSqsClientConfig(data: Any) -> TriggerSqsClientConfig:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'TriggerSqsClientConfig' failed as data isn't a dictionary."
+        )
 
-    field = data.get("is_legacy", None)
-    args["is_legacy"] = field
+    args: Dict[str, Any] = {}
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("endpoint", None)
+    if field is not None:
+        args["endpoint"] = field
 
-    field = data.get("ip", None)
-    args["ip"] = unmarshal_IP(field)
+    field = data.get("queue_url", None)
+    if field is not None:
+        args["queue_url"] = field
 
-    field = data.get("version", None)
-    args["version"] = field
+    field = data.get("access_key", None)
+    if field is not None:
+        args["access_key"] = field
 
-    field = data.get("can_upgrade_to", None)
-    args["can_upgrade_to"] = field
+    field = data.get("secret_key", None)
+    if field is not None:
+        args["secret_key"] = field
 
-    return Gateway(**args)
+    return TriggerSqsClientConfig(**args)
 
 
-def unmarshal_PATRule(data: Any) -> PATRule:
+def unmarshal_Trigger(data: Any) -> Trigger:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'PATRule' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Trigger' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
-
-    field = data.get("gateway_id", None)
-    args["gateway_id"] = field
+    if field is not None:
+        args["id"] = field
 
-    field = data.get("public_port", None)
-    args["public_port"] = field
+    field = data.get("name", None)
+    if field is not None:
+        args["name"] = field
 
-    field = data.get("private_ip", None)
-    args["private_ip"] = field
+    field = data.get("description", None)
+    if field is not None:
+        args["description"] = field
+
+    field = data.get("container_id", None)
+    if field is not None:
+        args["container_id"] = field
+
+    field = data.get("input_type", None)
+    if field is not None:
+        args["input_type"] = field
 
-    field = data.get("private_port", None)
-    args["private_port"] = field
+    field = data.get("status", None)
+    if field is not None:
+        args["status"] = field
 
-    field = data.get("protocol", None)
-    args["protocol"] = field
+    field = data.get("error_message", None)
+    if field is not None:
+        args["error_message"] = field
 
-    field = data.get("zone", None)
-    args["zone"] = field
+    field = data.get("scw_sqs_config", None)
+    if field is not None:
+        args["scw_sqs_config"] = unmarshal_TriggerMnqSqsClientConfig(field)
 
-    field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("scw_nats_config", None)
+    if field is not None:
+        args["scw_nats_config"] = unmarshal_TriggerMnqNatsClientConfig(field)
 
-    field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    field = data.get("sqs_config", None)
+    if field is not None:
+        args["sqs_config"] = unmarshal_TriggerSqsClientConfig(field)
 
-    return PATRule(**args)
+    return Trigger(**args)
 
 
-def unmarshal_ListDHCPEntriesResponse(data: Any) -> ListDHCPEntriesResponse:
+def unmarshal_ListContainersResponse(data: Any) -> ListContainersResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListDHCPEntriesResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListContainersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("dhcp_entries", None)
-    args["dhcp_entries"] = (
-        [unmarshal_DHCPEntry(v) for v in field] if field is not None else None
-    )
+    field = data.get("containers", None)
+    if field is not None:
+        args["containers"] = (
+            [unmarshal_Container(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListDHCPEntriesResponse(**args)
+    return ListContainersResponse(**args)
 
 
-def unmarshal_ListDHCPsResponse(data: Any) -> ListDHCPsResponse:
+def unmarshal_ListCronsResponse(data: Any) -> ListCronsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListDHCPsResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListCronsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("dhcps", None)
-    args["dhcps"] = [unmarshal_DHCP(v) for v in field] if field is not None else None
+    field = data.get("crons", None)
+    if field is not None:
+        args["crons"] = (
+            [unmarshal_Cron(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListDHCPsResponse(**args)
+    return ListCronsResponse(**args)
 
 
-def unmarshal_ListGatewayNetworksResponse(data: Any) -> ListGatewayNetworksResponse:
+def unmarshal_ListDomainsResponse(data: Any) -> ListDomainsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListGatewayNetworksResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListDomainsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("gateway_networks", None)
-    args["gateway_networks"] = (
-        [unmarshal_GatewayNetwork(v) for v in field] if field is not None else None
-    )
+    field = data.get("domains", None)
+    if field is not None:
+        args["domains"] = (
+            [unmarshal_Domain(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListGatewayNetworksResponse(**args)
+    return ListDomainsResponse(**args)
 
 
-def unmarshal_ListGatewayTypesResponse(data: Any) -> ListGatewayTypesResponse:
+def unmarshal_Log(data: Any) -> Log:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListGatewayTypesResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'Log' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("types", None)
-    args["types"] = (
-        [unmarshal_GatewayType(v) for v in field] if field is not None else None
-    )
-
-    return ListGatewayTypesResponse(**args)
+    field = data.get("message", None)
+    if field is not None:
+        args["message"] = field
 
+    field = data.get("id", None)
+    if field is not None:
+        args["id"] = field
 
-def unmarshal_ListGatewaysResponse(data: Any) -> ListGatewaysResponse:
-    if not isinstance(data, dict):
-        raise TypeError(
-            "Unmarshalling the type 'ListGatewaysResponse' failed as data isn't a dictionary."
-        )
+    field = data.get("level", None)
+    if field is not None:
+        args["level"] = field
 
-    args: Dict[str, Any] = {}
+    field = data.get("source", None)
+    if field is not None:
+        args["source"] = field
 
-    field = data.get("gateways", None)
-    args["gateways"] = (
-        [unmarshal_Gateway(v) for v in field] if field is not None else None
-    )
+    field = data.get("stream", None)
+    if field is not None:
+        args["stream"] = field
 
-    field = data.get("total_count", None)
-    args["total_count"] = field
+    field = data.get("timestamp", None)
+    if field is not None:
+        args["timestamp"] = parser.isoparse(field) if isinstance(field, str) else field
 
-    return ListGatewaysResponse(**args)
+    return Log(**args)
 
 
-def unmarshal_ListIPsResponse(data: Any) -> ListIPsResponse:
+def unmarshal_ListLogsResponse(data: Any) -> ListLogsResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListIPsResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListLogsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("ips", None)
-    args["ips"] = [unmarshal_IP(v) for v in field] if field is not None else None
+    field = data.get("logs", None)
+    if field is not None:
+        args["logs"] = [unmarshal_Log(v) for v in field] if field is not None else None
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListIPsResponse(**args)
+    return ListLogsResponse(**args)
 
 
-def unmarshal_ListPATRulesResponse(data: Any) -> ListPATRulesResponse:
+def unmarshal_ListNamespacesResponse(data: Any) -> ListNamespacesResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'ListPATRulesResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListNamespacesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("pat_rules", None)
-    args["pat_rules"] = (
-        [unmarshal_PATRule(v) for v in field] if field is not None else None
-    )
+    field = data.get("namespaces", None)
+    if field is not None:
+        args["namespaces"] = (
+            [unmarshal_Namespace(v) for v in field] if field is not None else None
+        )
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
-    return ListPATRulesResponse(**args)
+    return ListNamespacesResponse(**args)
 
 
-def unmarshal_SetDHCPEntriesResponse(data: Any) -> SetDHCPEntriesResponse:
+def unmarshal_ListTokensResponse(data: Any) -> ListTokensResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'SetDHCPEntriesResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListTokensResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("dhcp_entries", None)
-    args["dhcp_entries"] = (
-        [unmarshal_DHCPEntry(v) for v in field] if field is not None else None
-    )
+    field = data.get("tokens", None)
+    if field is not None:
+        args["tokens"] = (
+            [unmarshal_Token(v) for v in field] if field is not None else None
+        )
+
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return SetDHCPEntriesResponse(**args)
+    return ListTokensResponse(**args)
 
 
-def unmarshal_SetPATRulesResponse(data: Any) -> SetPATRulesResponse:
+def unmarshal_ListTriggersResponse(data: Any) -> ListTriggersResponse:
     if not isinstance(data, dict):
         raise TypeError(
-            "Unmarshalling the type 'SetPATRulesResponse' failed as data isn't a dictionary."
+            "Unmarshalling the type 'ListTriggersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("pat_rules", None)
-    args["pat_rules"] = (
-        [unmarshal_PATRule(v) for v in field] if field is not None else None
-    )
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
 
-    return SetPATRulesResponse(**args)
+    field = data.get("triggers", None)
+    if field is not None:
+        args["triggers"] = (
+            [unmarshal_Trigger(v) for v in field] if field is not None else None
+        )
 
+    return ListTriggersResponse(**args)
 
-def marshal_CreateDHCPRequest(
-    request: CreateDHCPRequest,
+
+def marshal_Secret(
+    request: Secret,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.subnet is not None:
-        output["subnet"] = request.subnet
+    if request.key is not None:
+        output["key"] = request.key
 
-    if request.project_id is not None:
-        output["project_id"] = request.project_id or defaults.default_project_id
+    if request.value is not None:
+        output["value"] = request.value
 
-    if request.address is not None:
-        output["address"] = request.address
+    return output
 
-    if request.pool_low is not None:
-        output["pool_low"] = request.pool_low
 
-    if request.pool_high is not None:
-        output["pool_high"] = request.pool_high
+def marshal_CreateContainerRequest(
+    request: CreateContainerRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
 
-    if request.enable_dynamic is not None:
-        output["enable_dynamic"] = request.enable_dynamic
+    if request.namespace_id is not None:
+        output["namespace_id"] = request.namespace_id
 
-    if request.valid_lifetime is not None:
-        output["valid_lifetime"] = request.valid_lifetime
+    if request.name is not None:
+        output["name"] = request.name
 
-    if request.renew_timer is not None:
-        output["renew_timer"] = request.renew_timer
+    if request.environment_variables is not None:
+        output["environment_variables"] = request.environment_variables
 
-    if request.rebind_timer is not None:
-        output["rebind_timer"] = request.rebind_timer
+    if request.min_scale is not None:
+        output["min_scale"] = request.min_scale
 
-    if request.push_default_route is not None:
-        output["push_default_route"] = request.push_default_route
+    if request.max_scale is not None:
+        output["max_scale"] = request.max_scale
 
-    if request.push_dns_server is not None:
-        output["push_dns_server"] = request.push_dns_server
+    if request.memory_limit is not None:
+        output["memory_limit"] = request.memory_limit
 
-    if request.dns_servers_override is not None:
-        output["dns_servers_override"] = request.dns_servers_override
+    if request.cpu_limit is not None:
+        output["cpu_limit"] = request.cpu_limit
 
-    if request.dns_search is not None:
-        output["dns_search"] = request.dns_search
+    if request.timeout is not None:
+        output["timeout"] = request.timeout
 
-    if request.dns_local_name is not None:
-        output["dns_local_name"] = request.dns_local_name
+    if request.privacy is not None:
+        output["privacy"] = str(request.privacy)
 
-    return output
+    if request.description is not None:
+        output["description"] = request.description
 
+    if request.registry_image is not None:
+        output["registry_image"] = request.registry_image
 
-def marshal_CreateDHCPEntryRequest(
-    request: CreateDHCPEntryRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
+    if request.max_concurrency is not None:
+        output["max_concurrency"] = request.max_concurrency
 
-    if request.gateway_network_id is not None:
-        output["gateway_network_id"] = request.gateway_network_id
+    if request.protocol is not None:
+        output["protocol"] = str(request.protocol)
 
-    if request.mac_address is not None:
-        output["mac_address"] = request.mac_address
+    if request.port is not None:
+        output["port"] = request.port
 
-    if request.ip_address is not None:
-        output["ip_address"] = request.ip_address
+    if request.secret_environment_variables is not None:
+        output["secret_environment_variables"] = [
+            marshal_Secret(item, defaults)
+            for item in request.secret_environment_variables
+        ]
+
+    if request.http_option is not None:
+        output["http_option"] = str(request.http_option)
 
     return output
 
 
-def marshal_CreateGatewayNetworkRequestIpamConfig(
-    request: CreateGatewayNetworkRequestIpamConfig,
+def marshal_CreateCronRequest(
+    request: CreateCronRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.push_default_route is not None:
-        output["push_default_route"] = request.push_default_route
+    if request.container_id is not None:
+        output["container_id"] = request.container_id
+
+    if request.schedule is not None:
+        output["schedule"] = request.schedule
 
-    if request.ipam_ip_id is not None:
-        output["ipam_ip_id"] = request.ipam_ip_id
+    if request.args is not None:
+        output["args"] = request.args
+
+    if request.name is not None:
+        output["name"] = request.name
 
     return output
 
 
-def marshal_CreateGatewayNetworkRequest(
-    request: CreateGatewayNetworkRequest,
+def marshal_CreateDomainRequest(
+    request: CreateDomainRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
-    output.update(
-        resolve_one_of(
-            [
-                OneOfPossibility("dhcp_id", request.dhcp_id),
-                OneOfPossibility("dhcp", request.dhcp),
-                OneOfPossibility("address", request.address),
-                OneOfPossibility("ipam_config", request.ipam_config),
-            ]
-        ),
-    )
-
-    if request.gateway_id is not None:
-        output["gateway_id"] = request.gateway_id
 
-    if request.private_network_id is not None:
-        output["private_network_id"] = request.private_network_id
+    if request.hostname is not None:
+        output["hostname"] = request.hostname
 
-    if request.enable_masquerade is not None:
-        output["enable_masquerade"] = request.enable_masquerade
-
-    if request.enable_dhcp is not None:
-        output["enable_dhcp"] = request.enable_dhcp
+    if request.container_id is not None:
+        output["container_id"] = request.container_id
 
     return output
 
 
-def marshal_CreateGatewayRequest(
-    request: CreateGatewayRequest,
+def marshal_CreateNamespaceRequest(
+    request: CreateNamespaceRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.type_ is not None:
-        output["type"] = request.type_
-
-    if request.enable_smtp is not None:
-        output["enable_smtp"] = request.enable_smtp
-
-    if request.enable_bastion is not None:
-        output["enable_bastion"] = request.enable_bastion
-
-    if request.project_id is not None:
-        output["project_id"] = request.project_id or defaults.default_project_id
-
     if request.name is not None:
         output["name"] = request.name
 
-    if request.tags is not None:
-        output["tags"] = request.tags
+    if request.environment_variables is not None:
+        output["environment_variables"] = request.environment_variables
 
-    if request.upstream_dns_servers is not None:
-        output["upstream_dns_servers"] = request.upstream_dns_servers
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
 
-    if request.ip_id is not None:
-        output["ip_id"] = request.ip_id
+    if request.description is not None:
+        output["description"] = request.description
 
-    if request.bastion_port is not None:
-        output["bastion_port"] = request.bastion_port
+    if request.secret_environment_variables is not None:
+        output["secret_environment_variables"] = [
+            marshal_Secret(item, defaults)
+            for item in request.secret_environment_variables
+        ]
 
     return output
 
 
-def marshal_CreateIPRequest(
-    request: CreateIPRequest,
+def marshal_CreateTokenRequest(
+    request: CreateTokenRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
+    output.update(
+        resolve_one_of(
+            [
+                OneOfPossibility("container_id", request.container_id),
+                OneOfPossibility("namespace_id", request.namespace_id),
+            ]
+        ),
+    )
 
-    if request.project_id is not None:
-        output["project_id"] = request.project_id or defaults.default_project_id
+    if request.description is not None:
+        output["description"] = request.description
 
-    if request.tags is not None:
-        output["tags"] = request.tags
+    if request.expires_at is not None:
+        output["expires_at"] = request.expires_at
 
     return output
 
 
-def marshal_CreatePATRuleRequest(
-    request: CreatePATRuleRequest,
+def marshal_CreateTriggerRequestMnqNatsClientConfig(
+    request: CreateTriggerRequestMnqNatsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.gateway_id is not None:
-        output["gateway_id"] = request.gateway_id
+    if request.subject is not None:
+        output["subject"] = request.subject
 
-    if request.public_port is not None:
-        output["public_port"] = request.public_port
+    if request.mnq_nats_account_id is not None:
+        output["mnq_nats_account_id"] = request.mnq_nats_account_id
 
-    if request.private_ip is not None:
-        output["private_ip"] = request.private_ip
+    if request.mnq_project_id is not None:
+        output["mnq_project_id"] = request.mnq_project_id
 
-    if request.private_port is not None:
-        output["private_port"] = request.private_port
+    if request.mnq_region is not None:
+        output["mnq_region"] = request.mnq_region
 
-    if request.protocol is not None:
-        output["protocol"] = str(request.protocol)
+    if request.mnq_namespace_id is not None:
+        output["mnq_namespace_id"] = request.mnq_namespace_id
 
     return output
 
 
-def marshal_SetDHCPEntriesRequestEntry(
-    request: SetDHCPEntriesRequestEntry,
+def marshal_CreateTriggerRequestMnqSqsClientConfig(
+    request: CreateTriggerRequestMnqSqsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.mac_address is not None:
-        output["mac_address"] = request.mac_address
+    if request.queue is not None:
+        output["queue"] = request.queue
 
-    if request.ip_address is not None:
-        output["ip_address"] = request.ip_address
+    if request.mnq_project_id is not None:
+        output["mnq_project_id"] = request.mnq_project_id
 
-    return output
+    if request.mnq_region is not None:
+        output["mnq_region"] = request.mnq_region
 
-
-def marshal_SetDHCPEntriesRequest(
-    request: SetDHCPEntriesRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
-
-    if request.gateway_network_id is not None:
-        output["gateway_network_id"] = request.gateway_network_id
-
-    if request.dhcp_entries is not None:
-        output["dhcp_entries"] = [
-            marshal_SetDHCPEntriesRequestEntry(item, defaults)
-            for item in request.dhcp_entries
-        ]
+    if request.mnq_namespace_id is not None:
+        output["mnq_namespace_id"] = request.mnq_namespace_id
 
     return output
 
 
-def marshal_SetPATRulesRequestRule(
-    request: SetPATRulesRequestRule,
+def marshal_CreateTriggerRequestSqsClientConfig(
+    request: CreateTriggerRequestSqsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.public_port is not None:
-        output["public_port"] = request.public_port
+    if request.endpoint is not None:
+        output["endpoint"] = request.endpoint
 
-    if request.private_ip is not None:
-        output["private_ip"] = request.private_ip
+    if request.queue_url is not None:
+        output["queue_url"] = request.queue_url
 
-    if request.private_port is not None:
-        output["private_port"] = request.private_port
+    if request.access_key is not None:
+        output["access_key"] = request.access_key
 
-    if request.protocol is not None:
-        output["protocol"] = str(request.protocol)
+    if request.secret_key is not None:
+        output["secret_key"] = request.secret_key
 
     return output
 
 
-def marshal_SetPATRulesRequest(
-    request: SetPATRulesRequest,
+def marshal_CreateTriggerRequest(
+    request: CreateTriggerRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
+    output.update(
+        resolve_one_of(
+            [
+                OneOfPossibility("scw_sqs_config", request.scw_sqs_config),
+                OneOfPossibility("scw_nats_config", request.scw_nats_config),
+                OneOfPossibility("sqs_config", request.sqs_config),
+            ]
+        ),
+    )
 
-    if request.gateway_id is not None:
-        output["gateway_id"] = request.gateway_id
+    if request.name is not None:
+        output["name"] = request.name
 
-    if request.pat_rules is not None:
-        output["pat_rules"] = [
-            marshal_SetPATRulesRequestRule(item, defaults) for item in request.pat_rules
-        ]
+    if request.container_id is not None:
+        output["container_id"] = request.container_id
+
+    if request.description is not None:
+        output["description"] = request.description
 
     return output
 
 
-def marshal_UpdateDHCPEntryRequest(
-    request: UpdateDHCPEntryRequest,
+def marshal_UpdateContainerRequest(
+    request: UpdateContainerRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.ip_address is not None:
-        output["ip_address"] = request.ip_address
+    if request.environment_variables is not None:
+        output["environment_variables"] = request.environment_variables
 
-    return output
+    if request.min_scale is not None:
+        output["min_scale"] = request.min_scale
 
+    if request.max_scale is not None:
+        output["max_scale"] = request.max_scale
 
-def marshal_UpdateDHCPRequest(
-    request: UpdateDHCPRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
+    if request.memory_limit is not None:
+        output["memory_limit"] = request.memory_limit
 
-    if request.subnet is not None:
-        output["subnet"] = request.subnet
+    if request.cpu_limit is not None:
+        output["cpu_limit"] = request.cpu_limit
 
-    if request.address is not None:
-        output["address"] = request.address
+    if request.timeout is not None:
+        output["timeout"] = request.timeout
 
-    if request.pool_low is not None:
-        output["pool_low"] = request.pool_low
+    if request.redeploy is not None:
+        output["redeploy"] = request.redeploy
 
-    if request.pool_high is not None:
-        output["pool_high"] = request.pool_high
+    if request.privacy is not None:
+        output["privacy"] = str(request.privacy)
 
-    if request.enable_dynamic is not None:
-        output["enable_dynamic"] = request.enable_dynamic
+    if request.description is not None:
+        output["description"] = request.description
 
-    if request.valid_lifetime is not None:
-        output["valid_lifetime"] = request.valid_lifetime
+    if request.registry_image is not None:
+        output["registry_image"] = request.registry_image
 
-    if request.renew_timer is not None:
-        output["renew_timer"] = request.renew_timer
+    if request.max_concurrency is not None:
+        output["max_concurrency"] = request.max_concurrency
 
-    if request.rebind_timer is not None:
-        output["rebind_timer"] = request.rebind_timer
-
-    if request.push_default_route is not None:
-        output["push_default_route"] = request.push_default_route
-
-    if request.push_dns_server is not None:
-        output["push_dns_server"] = request.push_dns_server
+    if request.protocol is not None:
+        output["protocol"] = str(request.protocol)
 
-    if request.dns_servers_override is not None:
-        output["dns_servers_override"] = request.dns_servers_override
+    if request.port is not None:
+        output["port"] = request.port
 
-    if request.dns_search is not None:
-        output["dns_search"] = request.dns_search
+    if request.secret_environment_variables is not None:
+        output["secret_environment_variables"] = [
+            marshal_Secret(item, defaults)
+            for item in request.secret_environment_variables
+        ]
 
-    if request.dns_local_name is not None:
-        output["dns_local_name"] = request.dns_local_name
+    if request.http_option is not None:
+        output["http_option"] = str(request.http_option)
 
     return output
 
 
-def marshal_UpdateGatewayNetworkRequestIpamConfig(
-    request: UpdateGatewayNetworkRequestIpamConfig,
+def marshal_UpdateCronRequest(
+    request: UpdateCronRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.push_default_route is not None:
-        output["push_default_route"] = request.push_default_route
-
-    if request.ipam_ip_id is not None:
-        output["ipam_ip_id"] = request.ipam_ip_id
+    if request.container_id is not None:
+        output["container_id"] = request.container_id
 
-    return output
+    if request.schedule is not None:
+        output["schedule"] = request.schedule
 
+    if request.args is not None:
+        output["args"] = request.args
 
-def marshal_UpdateGatewayNetworkRequest(
-    request: UpdateGatewayNetworkRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    output: Dict[str, Any] = {}
-    output.update(
-        resolve_one_of(
-            [
-                OneOfPossibility("dhcp_id", request.dhcp_id),
-                OneOfPossibility("address", request.address),
-                OneOfPossibility("ipam_config", request.ipam_config),
-            ]
-        ),
-    )
-
-    if request.enable_masquerade is not None:
-        output["enable_masquerade"] = request.enable_masquerade
-
-    if request.enable_dhcp is not None:
-        output["enable_dhcp"] = request.enable_dhcp
+    if request.name is not None:
+        output["name"] = request.name
 
     return output
 
 
-def marshal_UpdateGatewayRequest(
-    request: UpdateGatewayRequest,
+def marshal_UpdateNamespaceRequest(
+    request: UpdateNamespaceRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.name is not None:
-        output["name"] = request.name
-
-    if request.tags is not None:
-        output["tags"] = request.tags
-
-    if request.upstream_dns_servers is not None:
-        output["upstream_dns_servers"] = request.upstream_dns_servers
+    if request.environment_variables is not None:
+        output["environment_variables"] = request.environment_variables
 
-    if request.enable_bastion is not None:
-        output["enable_bastion"] = request.enable_bastion
+    if request.description is not None:
+        output["description"] = request.description
 
-    if request.bastion_port is not None:
-        output["bastion_port"] = request.bastion_port
-
-    if request.enable_smtp is not None:
-        output["enable_smtp"] = request.enable_smtp
+    if request.secret_environment_variables is not None:
+        output["secret_environment_variables"] = [
+            marshal_Secret(item, defaults)
+            for item in request.secret_environment_variables
+        ]
 
     return output
 
 
-def marshal_UpdateIPRequest(
-    request: UpdateIPRequest,
+def marshal_UpdateTriggerRequestSqsClientConfig(
+    request: UpdateTriggerRequestSqsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
-    if request.tags is not None:
-        output["tags"] = request.tags
-
-    if request.reverse is not None:
-        output["reverse"] = request.reverse
+    if request.access_key is not None:
+        output["access_key"] = request.access_key
 
-    if request.gateway_id is not None:
-        output["gateway_id"] = request.gateway_id
+    if request.secret_key is not None:
+        output["secret_key"] = request.secret_key
 
     return output
 
 
-def marshal_UpdatePATRuleRequest(
-    request: UpdatePATRuleRequest,
+def marshal_UpdateTriggerRequest(
+    request: UpdateTriggerRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
+    output.update(
+        resolve_one_of(
+            [
+                OneOfPossibility("sqs_config", request.sqs_config),
+            ]
+        ),
+    )
 
-    if request.public_port is not None:
-        output["public_port"] = request.public_port
-
-    if request.private_ip is not None:
-        output["private_ip"] = request.private_ip
-
-    if request.private_port is not None:
-        output["private_port"] = request.private_port
+    if request.name is not None:
+        output["name"] = request.name
 
-    if request.protocol is not None:
-        output["protocol"] = str(request.protocol)
+    if request.description is not None:
+        output["description"] = request.description
 
     return output
```

### Comparing `scaleway-2.0.0.dev5/scaleway/vpcgw/v1/types.py` & `scaleway-2.0.0.dev6/scaleway/vpcgw/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/__init__.py` & `scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/api.py` & `scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/marshalling.py` & `scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/marshalling.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,328 +32,391 @@
         raise TypeError(
             "Unmarshalling the type 'HostingCpanelUrls' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("dashboard", None)
-    args["dashboard"] = field
+    if field is not None:
+        args["dashboard"] = field
 
     field = data.get("webmail", None)
-    args["webmail"] = field
+    if field is not None:
+        args["webmail"] = field
 
     return HostingCpanelUrls(**args)
 
 
 def unmarshal_HostingOption(data: Any) -> HostingOption:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'HostingOption' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     return HostingOption(**args)
 
 
 def unmarshal_Hosting(data: Any) -> Hosting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Hosting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("organization_id", None)
-    args["organization_id"] = field
+    if field is not None:
+        args["organization_id"] = field
 
     field = data.get("project_id", None)
-    args["project_id"] = field
+    if field is not None:
+        args["project_id"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("platform_hostname", None)
-    args["platform_hostname"] = field
+    if field is not None:
+        args["platform_hostname"] = field
 
     field = data.get("offer_id", None)
-    args["offer_id"] = field
+    if field is not None:
+        args["offer_id"] = field
 
     field = data.get("offer_name", None)
-    args["offer_name"] = field
+    if field is not None:
+        args["offer_name"] = field
 
     field = data.get("domain", None)
-    args["domain"] = field
+    if field is not None:
+        args["domain"] = field
 
     field = data.get("tags", None)
-    args["tags"] = field
+    if field is not None:
+        args["tags"] = field
 
     field = data.get("updated_at", None)
-    args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("created_at", None)
-    args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    if field is not None:
+        args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
 
     field = data.get("platform_number", None)
-    args["platform_number"] = field
+    if field is not None:
+        args["platform_number"] = field
 
     field = data.get("options", None)
-    args["options"] = (
-        [unmarshal_HostingOption(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["options"] = (
+            [unmarshal_HostingOption(v) for v in field] if field is not None else None
+        )
 
     field = data.get("dns_status", None)
-    args["dns_status"] = field
+    if field is not None:
+        args["dns_status"] = field
 
     field = data.get("username", None)
-    args["username"] = field
+    if field is not None:
+        args["username"] = field
 
     field = data.get("offer_end_of_life", None)
-    args["offer_end_of_life"] = field
+    if field is not None:
+        args["offer_end_of_life"] = field
 
     field = data.get("control_panel_name", None)
-    args["control_panel_name"] = field
+    if field is not None:
+        args["control_panel_name"] = field
 
     field = data.get("region", None)
-    args["region"] = field
+    if field is not None:
+        args["region"] = field
 
     field = data.get("cpanel_urls", None)
-    args["cpanel_urls"] = unmarshal_HostingCpanelUrls(field)
+    if field is not None:
+        args["cpanel_urls"] = unmarshal_HostingCpanelUrls(field)
 
     return Hosting(**args)
 
 
 def unmarshal_DnsRecord(data: Any) -> DnsRecord:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DnsRecord' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("type_", None)
-    args["type_"] = field
+    if field is not None:
+        args["type_"] = field
 
     field = data.get("ttl", None)
-    args["ttl"] = field
+    if field is not None:
+        args["ttl"] = field
 
     field = data.get("value", None)
-    args["value"] = field
+    if field is not None:
+        args["value"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("priority", None)
-    args["priority"] = field
+    if field is not None:
+        args["priority"] = field
 
     return DnsRecord(**args)
 
 
 def unmarshal_Nameserver(data: Any) -> Nameserver:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Nameserver' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("hostname", None)
-    args["hostname"] = field
+    if field is not None:
+        args["hostname"] = field
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     field = data.get("is_default", None)
-    args["is_default"] = field
+    if field is not None:
+        args["is_default"] = field
 
     return Nameserver(**args)
 
 
 def unmarshal_DnsRecords(data: Any) -> DnsRecords:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'DnsRecords' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("records", None)
-    args["records"] = (
-        [unmarshal_DnsRecord(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["records"] = (
+            [unmarshal_DnsRecord(v) for v in field] if field is not None else None
+        )
 
     field = data.get("name_servers", None)
-    args["name_servers"] = (
-        [unmarshal_Nameserver(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["name_servers"] = (
+            [unmarshal_Nameserver(v) for v in field] if field is not None else None
+        )
 
     field = data.get("status", None)
-    args["status"] = field
+    if field is not None:
+        args["status"] = field
 
     return DnsRecords(**args)
 
 
 def unmarshal_ControlPanel(data: Any) -> ControlPanel:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ControlPanel' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("available", None)
-    args["available"] = field
+    if field is not None:
+        args["available"] = field
 
     field = data.get("logo_url", None)
-    args["logo_url"] = field
+    if field is not None:
+        args["logo_url"] = field
 
     return ControlPanel(**args)
 
 
 def unmarshal_ListControlPanelsResponse(data: Any) -> ListControlPanelsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListControlPanelsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("control_panels", None)
-    args["control_panels"] = (
-        [unmarshal_ControlPanel(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["control_panels"] = (
+            [unmarshal_ControlPanel(v) for v in field] if field is not None else None
+        )
 
     return ListControlPanelsResponse(**args)
 
 
 def unmarshal_ListHostingsResponse(data: Any) -> ListHostingsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListHostingsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("total_count", None)
-    args["total_count"] = field
+    if field is not None:
+        args["total_count"] = field
 
     field = data.get("hostings", None)
-    args["hostings"] = (
-        [unmarshal_Hosting(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["hostings"] = (
+            [unmarshal_Hosting(v) for v in field] if field is not None else None
+        )
 
     return ListHostingsResponse(**args)
 
 
 def unmarshal_OfferProduct(data: Any) -> OfferProduct:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'OfferProduct' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("name", None)
-    args["name"] = field
+    if field is not None:
+        args["name"] = field
 
     field = data.get("option", None)
-    args["option"] = field
+    if field is not None:
+        args["option"] = field
 
     field = data.get("email_accounts_quota", None)
-    args["email_accounts_quota"] = field
+    if field is not None:
+        args["email_accounts_quota"] = field
 
     field = data.get("email_storage_quota", None)
-    args["email_storage_quota"] = field
+    if field is not None:
+        args["email_storage_quota"] = field
 
     field = data.get("databases_quota", None)
-    args["databases_quota"] = field
+    if field is not None:
+        args["databases_quota"] = field
 
     field = data.get("hosting_storage_quota", None)
-    args["hosting_storage_quota"] = field
+    if field is not None:
+        args["hosting_storage_quota"] = field
 
     field = data.get("support_included", None)
-    args["support_included"] = field
+    if field is not None:
+        args["support_included"] = field
 
     field = data.get("v_cpu", None)
-    args["v_cpu"] = field
+    if field is not None:
+        args["v_cpu"] = field
 
     field = data.get("ram", None)
-    args["ram"] = field
+    if field is not None:
+        args["ram"] = field
 
     field = data.get("max_addon_domains", None)
-    args["max_addon_domains"] = field
+    if field is not None:
+        args["max_addon_domains"] = field
 
     return OfferProduct(**args)
 
 
 def unmarshal_Offer(data: Any) -> Offer:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Offer' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("id", None)
-    args["id"] = field
+    if field is not None:
+        args["id"] = field
 
     field = data.get("billing_operation_path", None)
-    args["billing_operation_path"] = field
+    if field is not None:
+        args["billing_operation_path"] = field
 
     field = data.get("available", None)
-    args["available"] = field
+    if field is not None:
+        args["available"] = field
 
     field = data.get("quota_warnings", None)
-    args["quota_warnings"] = (
-        [OfferQuotaWarning(v) for v in field] if field is not None else None
-    )
+    if field is not None:
+        args["quota_warnings"] = (
+            [OfferQuotaWarning(v) for v in field] if field is not None else None
+        )
 
     field = data.get("end_of_life", None)
-    args["end_of_life"] = field
+    if field is not None:
+        args["end_of_life"] = field
 
     field = data.get("control_panel_name", None)
-    args["control_panel_name"] = field
+    if field is not None:
+        args["control_panel_name"] = field
 
     field = data.get("product", None)
-    args["product"] = unmarshal_OfferProduct(field)
+    if field is not None:
+        args["product"] = unmarshal_OfferProduct(field)
 
     field = data.get("price", None)
-    args["price"] = unmarshal_Money(field)
+    if field is not None:
+        args["price"] = unmarshal_Money(field)
 
     return Offer(**args)
 
 
 def unmarshal_ListOffersResponse(data: Any) -> ListOffersResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListOffersResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("offers", None)
-    args["offers"] = [unmarshal_Offer(v) for v in field] if field is not None else None
+    if field is not None:
+        args["offers"] = (
+            [unmarshal_Offer(v) for v in field] if field is not None else None
+        )
 
     return ListOffersResponse(**args)
 
 
 def marshal_CreateHostingRequest(
     request: CreateHostingRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.0.0.dev5/scaleway/webhosting/v1alpha1/types.py` & `scaleway-2.0.0.dev6/scaleway/webhosting/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.0.0.dev5/PKG-INFO` & `scaleway-2.0.0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway
-Version: 2.0.0.dev5
+Version: 2.0.0.dev6
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -19,14 +19,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
-Requires-Dist: scaleway-core (==2.0.0.dev5)
+Requires-Dist: scaleway-core (==2.0.0.dev6)
 Description-Content-Type: text/markdown
 
 # Scaleway Python SDK
 
 This SDK enables you to interact with Scaleway APIs.
```

