# Comparing `tmp/lbrlabs_pulumi_eks-0.9.0.tar.gz` & `tmp/lbrlabs_pulumi_eks-0.9.1a1707243566.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_eks-0.9.0.tar", last modified: Thu Feb  1 01:39:02 2024, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_eks-0.9.1a1707243566.tar", last modified: Tue Feb  6 18:26:59 2024, max compression
```

## Comparing `lbrlabs_pulumi_eks-0.9.0.tar` & `lbrlabs_pulumi_eks-0.9.1a1707243566.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/attached_fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/attached_node_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/autoscaled_node_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    26815 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/iam_role_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/iam_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 01:39:02.000000 lbrlabs_pulumi_eks-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-01 01:39:01.000000 lbrlabs_pulumi_eks-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/attached_fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/attached_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/autoscaled_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/iam_role_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/iam_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 18:26:59.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-06 18:26:58.000000 lbrlabs_pulumi_eks-0.9.1a1707243566/setup.py
```

### Comparing `lbrlabs_pulumi_eks-0.9.0/PKG-INFO` & `lbrlabs_pulumi_eks-0.9.1a1707243566/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs_pulumi_eks
-Version: 0.9.0
+Version: 0.9.1a1707243566
 Summary: A batteries included EKS cluster following best practices.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-lbrlabs-eks
 Description: # Pulumi LBr Labs EKS 
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a "batteries included" cluster ready for you to attach your EKS nodes to.
```

### Comparing `lbrlabs_pulumi_eks-0.9.0/README.md` & `lbrlabs_pulumi_eks-0.9.1a1707243566/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/__init__.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/_inputs.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/_inputs.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/_utilities.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/attached_fargate_profile.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/attached_fargate_profile.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/attached_node_group.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/attached_node_group.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/autoscaled_node_group.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/autoscaled_node_group.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/cluster.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/cluster.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,16 @@
                  cert_manager_version: Optional[pulumi.Input[str]] = None,
                  certificate_arn: Optional[pulumi.Input[str]] = None,
                  cluster_version: Optional[pulumi.Input[str]] = None,
                  eks_iam_auth_controller_version: Optional[pulumi.Input[str]] = None,
                  enable_cert_manager: Optional[bool] = None,
                  enable_cloud_watch_agent: Optional[bool] = None,
                  enable_external_dns: Optional[bool] = None,
+                 enable_external_ingress: Optional[bool] = None,
+                 enable_internal_ingress: Optional[bool] = None,
                  enable_karpenter: Optional[bool] = None,
                  enable_otel: Optional[bool] = None,
                  enabled_cluster_log_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  external_dns_version: Optional[pulumi.Input[str]] = None,
                  lb_type: Optional[pulumi.Input[str]] = None,
                  lets_encrypt_email: Optional[str] = None,
                  nginx_ingress_version: Optional[pulumi.Input[str]] = None,
@@ -41,14 +43,16 @@
         :param pulumi.Input[str] cert_manager_version: The version of the cert-manager helm chart to deploy.
         :param pulumi.Input[str] certificate_arn: The ARN of the certificate to use for the ingress controller.
         :param pulumi.Input[str] cluster_version: The version of the EKS cluster to create.
         :param pulumi.Input[str] eks_iam_auth_controller_version: The version of the eks-iam-auth-controller helm chart to deploy.
         :param bool enable_cert_manager: Whether to enable cert-manager with route 53 integration.
         :param bool enable_cloud_watch_agent: Whether to enable cloudwatch container insights for EKS.
         :param bool enable_external_dns: Whether to enable external dns with route 53 integration.
+        :param bool enable_external_ingress: Whether to create an ingress controller for external traffic.
+        :param bool enable_internal_ingress: Whether to create an ingress controller for internal traffic.
         :param bool enable_karpenter: Whether to enable karpenter.
         :param bool enable_otel: Whether to enable the OTEL Distro for EKS.
         :param pulumi.Input[str] external_dns_version: The version of the external-dns helm chart to deploy.
         :param pulumi.Input[str] lb_type: The type of loadbalancer to provision.
         :param str lets_encrypt_email: The email address to use to issue certificates from Lets Encrypt.
         :param pulumi.Input[str] nginx_ingress_version: The version of the nginx ingress controller helm chart to deploy.
         :param pulumi.Input[float] system_node_desired_count: The initial number of nodes in the system autoscaling group.
@@ -74,14 +78,22 @@
             enable_cloud_watch_agent = False
         if enable_cloud_watch_agent is not None:
             pulumi.set(__self__, "enable_cloud_watch_agent", enable_cloud_watch_agent)
         if enable_external_dns is None:
             enable_external_dns = True
         if enable_external_dns is not None:
             pulumi.set(__self__, "enable_external_dns", enable_external_dns)
+        if enable_external_ingress is None:
+            enable_external_ingress = True
+        if enable_external_ingress is not None:
+            pulumi.set(__self__, "enable_external_ingress", enable_external_ingress)
+        if enable_internal_ingress is None:
+            enable_internal_ingress = True
+        if enable_internal_ingress is not None:
+            pulumi.set(__self__, "enable_internal_ingress", enable_internal_ingress)
         if enable_karpenter is None:
             enable_karpenter = True
         if enable_karpenter is not None:
             pulumi.set(__self__, "enable_karpenter", enable_karpenter)
         if enable_otel is None:
             enable_otel = False
         if enable_otel is not None:
@@ -208,14 +220,38 @@
         return pulumi.get(self, "enable_external_dns")
 
     @enable_external_dns.setter
     def enable_external_dns(self, value: Optional[bool]):
         pulumi.set(self, "enable_external_dns", value)
 
     @property
+    @pulumi.getter(name="enableExternalIngress")
+    def enable_external_ingress(self) -> Optional[bool]:
+        """
+        Whether to create an ingress controller for external traffic.
+        """
+        return pulumi.get(self, "enable_external_ingress")
+
+    @enable_external_ingress.setter
+    def enable_external_ingress(self, value: Optional[bool]):
+        pulumi.set(self, "enable_external_ingress", value)
+
+    @property
+    @pulumi.getter(name="enableInternalIngress")
+    def enable_internal_ingress(self) -> Optional[bool]:
+        """
+        Whether to create an ingress controller for internal traffic.
+        """
+        return pulumi.get(self, "enable_internal_ingress")
+
+    @enable_internal_ingress.setter
+    def enable_internal_ingress(self, value: Optional[bool]):
+        pulumi.set(self, "enable_internal_ingress", value)
+
+    @property
     @pulumi.getter(name="enableKarpenter")
     def enable_karpenter(self) -> Optional[bool]:
         """
         Whether to enable karpenter.
         """
         return pulumi.get(self, "enable_karpenter")
 
@@ -359,14 +395,16 @@
                  certificate_arn: Optional[pulumi.Input[str]] = None,
                  cluster_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_version: Optional[pulumi.Input[str]] = None,
                  eks_iam_auth_controller_version: Optional[pulumi.Input[str]] = None,
                  enable_cert_manager: Optional[bool] = None,
                  enable_cloud_watch_agent: Optional[bool] = None,
                  enable_external_dns: Optional[bool] = None,
+                 enable_external_ingress: Optional[bool] = None,
+                 enable_internal_ingress: Optional[bool] = None,
                  enable_karpenter: Optional[bool] = None,
                  enable_otel: Optional[bool] = None,
                  enabled_cluster_log_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  external_dns_version: Optional[pulumi.Input[str]] = None,
                  lb_type: Optional[pulumi.Input[str]] = None,
                  lets_encrypt_email: Optional[str] = None,
                  nginx_ingress_version: Optional[pulumi.Input[str]] = None,
@@ -384,14 +422,16 @@
         :param pulumi.Input[str] cert_manager_version: The version of the cert-manager helm chart to deploy.
         :param pulumi.Input[str] certificate_arn: The ARN of the certificate to use for the ingress controller.
         :param pulumi.Input[str] cluster_version: The version of the EKS cluster to create.
         :param pulumi.Input[str] eks_iam_auth_controller_version: The version of the eks-iam-auth-controller helm chart to deploy.
         :param bool enable_cert_manager: Whether to enable cert-manager with route 53 integration.
         :param bool enable_cloud_watch_agent: Whether to enable cloudwatch container insights for EKS.
         :param bool enable_external_dns: Whether to enable external dns with route 53 integration.
+        :param bool enable_external_ingress: Whether to create an ingress controller for external traffic.
+        :param bool enable_internal_ingress: Whether to create an ingress controller for internal traffic.
         :param bool enable_karpenter: Whether to enable karpenter.
         :param bool enable_otel: Whether to enable the OTEL Distro for EKS.
         :param pulumi.Input[str] external_dns_version: The version of the external-dns helm chart to deploy.
         :param pulumi.Input[str] lb_type: The type of loadbalancer to provision.
         :param str lets_encrypt_email: The email address to use to issue certificates from Lets Encrypt.
         :param pulumi.Input[str] nginx_ingress_version: The version of the nginx ingress controller helm chart to deploy.
         :param pulumi.Input[float] system_node_desired_count: The initial number of nodes in the system autoscaling group.
@@ -426,14 +466,16 @@
                  certificate_arn: Optional[pulumi.Input[str]] = None,
                  cluster_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cluster_version: Optional[pulumi.Input[str]] = None,
                  eks_iam_auth_controller_version: Optional[pulumi.Input[str]] = None,
                  enable_cert_manager: Optional[bool] = None,
                  enable_cloud_watch_agent: Optional[bool] = None,
                  enable_external_dns: Optional[bool] = None,
+                 enable_external_ingress: Optional[bool] = None,
+                 enable_internal_ingress: Optional[bool] = None,
                  enable_karpenter: Optional[bool] = None,
                  enable_otel: Optional[bool] = None,
                  enabled_cluster_log_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  external_dns_version: Optional[pulumi.Input[str]] = None,
                  lb_type: Optional[pulumi.Input[str]] = None,
                  lets_encrypt_email: Optional[str] = None,
                  nginx_ingress_version: Optional[pulumi.Input[str]] = None,
@@ -466,14 +508,20 @@
             __props__.__dict__["enable_cert_manager"] = enable_cert_manager
             if enable_cloud_watch_agent is None:
                 enable_cloud_watch_agent = False
             __props__.__dict__["enable_cloud_watch_agent"] = enable_cloud_watch_agent
             if enable_external_dns is None:
                 enable_external_dns = True
             __props__.__dict__["enable_external_dns"] = enable_external_dns
+            if enable_external_ingress is None:
+                enable_external_ingress = True
+            __props__.__dict__["enable_external_ingress"] = enable_external_ingress
+            if enable_internal_ingress is None:
+                enable_internal_ingress = True
+            __props__.__dict__["enable_internal_ingress"] = enable_internal_ingress
             if enable_karpenter is None:
                 enable_karpenter = True
             __props__.__dict__["enable_karpenter"] = enable_karpenter
             if enable_otel is None:
                 enable_otel = False
             __props__.__dict__["enable_otel"] = enable_otel
             __props__.__dict__["enabled_cluster_log_types"] = enabled_cluster_log_types
```

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/iam_role_mapping.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/iam_role_mapping.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/iam_service_account_role.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/iam_service_account_role.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks/provider.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/PKG-INFO` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs-pulumi-eks
-Version: 0.9.0
+Version: 0.9.1a1707243566
 Summary: A batteries included EKS cluster following best practices.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-lbrlabs-eks
 Description: # Pulumi LBr Labs EKS 
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a "batteries included" cluster ready for you to attach your EKS nodes to.
```

### Comparing `lbrlabs_pulumi_eks-0.9.0/lbrlabs_pulumi_eks.egg-info/SOURCES.txt` & `lbrlabs_pulumi_eks-0.9.1a1707243566/lbrlabs_pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_eks-0.9.0/setup.py` & `lbrlabs_pulumi_eks-0.9.1a1707243566/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.0"
+VERSION = "0.9.1a1707243566"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "lbrlabs-eks Pulumi Package - Development Version"
```

