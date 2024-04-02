# Comparing `tmp/pulumi_kafka-3.8.0a1711778096.tar.gz` & `tmp/pulumi_kafka-3.8.0a1712078841.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.8.0a1711778096.tar", last modified: Sat Mar 30 06:00:36 2024, max compression
+gzip compressed data, was "pulumi_kafka-3.8.0a1712078841.tar", last modified: Tue Apr  2 17:31:31 2024, max compression
```

## Comparing `pulumi_kafka-3.8.0a1711778096.tar` & `pulumi_kafka-3.8.0a1712078841.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:00:36.814000 pulumi_kafka-3.8.0a1711778096/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-30 06:00:36.810000 pulumi_kafka-3.8.0a1711778096/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:00:36.810000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23273 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:00:36.810000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    29712 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka/user_scram_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:00:36.810000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-30 06:00:36.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-30 06:00:36.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 06:00:36.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-30 06:00:36.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-30 06:00:36.000000 pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-30 06:00:29.000000 pulumi_kafka-3.8.0a1711778096/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 06:00:36.814000 pulumi_kafka-3.8.0a1711778096/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:31:31.594383 pulumi_kafka-3.8.0a1712078841/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-02 17:31:31.594383 pulumi_kafka-3.8.0a1712078841/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:31:31.590383 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23273 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:31:31.594383 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka/user_scram_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:31:31.594383 pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-02 17:31:31.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-02 17:31:31.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:31:31.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 17:31:31.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 17:31:31.000000 pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-02 17:31:25.000000 pulumi_kafka-3.8.0a1712078841/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:31:31.594383 pulumi_kafka-3.8.0a1712078841/setup.cfg
```

### Comparing `pulumi_kafka-3.8.0a1711778096/PKG-INFO` & `pulumi_kafka-3.8.0a1712078841/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1711778096
+Version: 3.8.0a1712078841
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1711778096/README.md` & `pulumi_kafka-3.8.0a1712078841/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/__init__.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/acl.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/config/__init__.pyi` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/config/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 """
 
 clientKeyPassphrase: Optional[str]
 """
 The passphrase for the private key that the certificate was issued for.
 """
 
+kafkaVersion: Optional[str]
+"""
+The version of Kafka protocol to use in `$MAJOR.$MINOR.$PATCH` format. Some features may not be available on older
+versions. Default is 2.7.0.
+"""
+
 saslAwsCredsDebug: Optional[bool]
 """
 Set this to true to turn AWS credentials debug.
 """
 
 saslAwsProfile: Optional[str]
 """
```

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/config/vars.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,22 @@
     def client_key_passphrase(self) -> Optional[str]:
         """
         The passphrase for the private key that the certificate was issued for.
         """
         return __config__.get('clientKeyPassphrase')
 
     @property
+    def kafka_version(self) -> Optional[str]:
+        """
+        The version of Kafka protocol to use in `$MAJOR.$MINOR.$PATCH` format. Some features may not be available on older
+        versions. Default is 2.7.0.
+        """
+        return __config__.get('kafkaVersion')
+
+    @property
     def sasl_aws_creds_debug(self) -> Optional[bool]:
         """
         Set this to true to turn AWS credentials debug.
         """
         return __config__.get_bool('saslAwsCredsDebug')
 
     @property
```

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/provider.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
                  ca_cert: Optional[pulumi.Input[str]] = None,
                  ca_cert_file: Optional[pulumi.Input[str]] = None,
                  client_cert: Optional[pulumi.Input[str]] = None,
                  client_cert_file: Optional[pulumi.Input[str]] = None,
                  client_key: Optional[pulumi.Input[str]] = None,
                  client_key_file: Optional[pulumi.Input[str]] = None,
                  client_key_passphrase: Optional[pulumi.Input[str]] = None,
+                 kafka_version: Optional[pulumi.Input[str]] = None,
                  sasl_aws_creds_debug: Optional[pulumi.Input[bool]] = None,
                  sasl_aws_profile: Optional[pulumi.Input[str]] = None,
                  sasl_aws_region: Optional[pulumi.Input[str]] = None,
                  sasl_aws_role_arn: Optional[pulumi.Input[str]] = None,
                  sasl_mechanism: Optional[pulumi.Input[str]] = None,
                  sasl_password: Optional[pulumi.Input[str]] = None,
                  sasl_token_url: Optional[pulumi.Input[str]] = None,
@@ -39,14 +40,16 @@
         :param pulumi.Input[str] ca_cert: CA certificate file to validate the server's certificate.
         :param pulumi.Input[str] ca_cert_file: Path to a CA certificate file to validate the server's certificate.
         :param pulumi.Input[str] client_cert: The client certificate.
         :param pulumi.Input[str] client_cert_file: Path to a file containing the client certificate.
         :param pulumi.Input[str] client_key: The private key that the certificate was issued for.
         :param pulumi.Input[str] client_key_file: Path to a file containing the private key that the certificate was issued for.
         :param pulumi.Input[str] client_key_passphrase: The passphrase for the private key that the certificate was issued for.
+        :param pulumi.Input[str] kafka_version: The version of Kafka protocol to use in `$MAJOR.$MINOR.$PATCH` format. Some features may not be available on older
+               versions. Default is 2.7.0.
         :param pulumi.Input[bool] sasl_aws_creds_debug: Set this to true to turn AWS credentials debug.
         :param pulumi.Input[str] sasl_aws_profile: AWS profile name to use
         :param pulumi.Input[str] sasl_aws_region: AWS region where MSK is deployed.
         :param pulumi.Input[str] sasl_aws_role_arn: Arn of an AWS IAM role to assume
         :param pulumi.Input[str] sasl_mechanism: SASL mechanism, can be plain, scram-sha512, scram-sha256, aws-iam
         :param pulumi.Input[str] sasl_password: Password for SASL authentication.
         :param pulumi.Input[str] sasl_token_url: The url to retrieve oauth2 tokens from, when using sasl mechanism oauthbearer
@@ -75,14 +78,16 @@
         if client_key_file is not None:
             warnings.warn("""This parameter is now deprecated and will be removed in a later release, please use `client_key` instead.""", DeprecationWarning)
             pulumi.log.warn("""client_key_file is deprecated: This parameter is now deprecated and will be removed in a later release, please use `client_key` instead.""")
         if client_key_file is not None:
             pulumi.set(__self__, "client_key_file", client_key_file)
         if client_key_passphrase is not None:
             pulumi.set(__self__, "client_key_passphrase", client_key_passphrase)
+        if kafka_version is not None:
+            pulumi.set(__self__, "kafka_version", kafka_version)
         if sasl_aws_creds_debug is not None:
             pulumi.set(__self__, "sasl_aws_creds_debug", sasl_aws_creds_debug)
         if sasl_aws_profile is not None:
             pulumi.set(__self__, "sasl_aws_profile", sasl_aws_profile)
         if sasl_aws_region is not None:
             pulumi.set(__self__, "sasl_aws_region", sasl_aws_region)
         if sasl_aws_role_arn is not None:
@@ -210,14 +215,27 @@
         return pulumi.get(self, "client_key_passphrase")
 
     @client_key_passphrase.setter
     def client_key_passphrase(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_key_passphrase", value)
 
     @property
+    @pulumi.getter(name="kafkaVersion")
+    def kafka_version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The version of Kafka protocol to use in `$MAJOR.$MINOR.$PATCH` format. Some features may not be available on older
+        versions. Default is 2.7.0.
+        """
+        return pulumi.get(self, "kafka_version")
+
+    @kafka_version.setter
+    def kafka_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "kafka_version", value)
+
+    @property
     @pulumi.getter(name="saslAwsCredsDebug")
     def sasl_aws_creds_debug(self) -> Optional[pulumi.Input[bool]]:
         """
         Set this to true to turn AWS credentials debug.
         """
         return pulumi.get(self, "sasl_aws_creds_debug")
 
@@ -355,14 +373,15 @@
                  ca_cert: Optional[pulumi.Input[str]] = None,
                  ca_cert_file: Optional[pulumi.Input[str]] = None,
                  client_cert: Optional[pulumi.Input[str]] = None,
                  client_cert_file: Optional[pulumi.Input[str]] = None,
                  client_key: Optional[pulumi.Input[str]] = None,
                  client_key_file: Optional[pulumi.Input[str]] = None,
                  client_key_passphrase: Optional[pulumi.Input[str]] = None,
+                 kafka_version: Optional[pulumi.Input[str]] = None,
                  sasl_aws_creds_debug: Optional[pulumi.Input[bool]] = None,
                  sasl_aws_profile: Optional[pulumi.Input[str]] = None,
                  sasl_aws_region: Optional[pulumi.Input[str]] = None,
                  sasl_aws_role_arn: Optional[pulumi.Input[str]] = None,
                  sasl_mechanism: Optional[pulumi.Input[str]] = None,
                  sasl_password: Optional[pulumi.Input[str]] = None,
                  sasl_token_url: Optional[pulumi.Input[str]] = None,
@@ -383,14 +402,16 @@
         :param pulumi.Input[str] ca_cert: CA certificate file to validate the server's certificate.
         :param pulumi.Input[str] ca_cert_file: Path to a CA certificate file to validate the server's certificate.
         :param pulumi.Input[str] client_cert: The client certificate.
         :param pulumi.Input[str] client_cert_file: Path to a file containing the client certificate.
         :param pulumi.Input[str] client_key: The private key that the certificate was issued for.
         :param pulumi.Input[str] client_key_file: Path to a file containing the private key that the certificate was issued for.
         :param pulumi.Input[str] client_key_passphrase: The passphrase for the private key that the certificate was issued for.
+        :param pulumi.Input[str] kafka_version: The version of Kafka protocol to use in `$MAJOR.$MINOR.$PATCH` format. Some features may not be available on older
+               versions. Default is 2.7.0.
         :param pulumi.Input[bool] sasl_aws_creds_debug: Set this to true to turn AWS credentials debug.
         :param pulumi.Input[str] sasl_aws_profile: AWS profile name to use
         :param pulumi.Input[str] sasl_aws_region: AWS region where MSK is deployed.
         :param pulumi.Input[str] sasl_aws_role_arn: Arn of an AWS IAM role to assume
         :param pulumi.Input[str] sasl_mechanism: SASL mechanism, can be plain, scram-sha512, scram-sha256, aws-iam
         :param pulumi.Input[str] sasl_password: Password for SASL authentication.
         :param pulumi.Input[str] sasl_token_url: The url to retrieve oauth2 tokens from, when using sasl mechanism oauthbearer
@@ -430,14 +451,15 @@
                  ca_cert: Optional[pulumi.Input[str]] = None,
                  ca_cert_file: Optional[pulumi.Input[str]] = None,
                  client_cert: Optional[pulumi.Input[str]] = None,
                  client_cert_file: Optional[pulumi.Input[str]] = None,
                  client_key: Optional[pulumi.Input[str]] = None,
                  client_key_file: Optional[pulumi.Input[str]] = None,
                  client_key_passphrase: Optional[pulumi.Input[str]] = None,
+                 kafka_version: Optional[pulumi.Input[str]] = None,
                  sasl_aws_creds_debug: Optional[pulumi.Input[bool]] = None,
                  sasl_aws_profile: Optional[pulumi.Input[str]] = None,
                  sasl_aws_region: Optional[pulumi.Input[str]] = None,
                  sasl_aws_role_arn: Optional[pulumi.Input[str]] = None,
                  sasl_mechanism: Optional[pulumi.Input[str]] = None,
                  sasl_password: Optional[pulumi.Input[str]] = None,
                  sasl_token_url: Optional[pulumi.Input[str]] = None,
@@ -460,14 +482,15 @@
             __props__.__dict__["ca_cert"] = ca_cert
             __props__.__dict__["ca_cert_file"] = ca_cert_file
             __props__.__dict__["client_cert"] = client_cert
             __props__.__dict__["client_cert_file"] = client_cert_file
             __props__.__dict__["client_key"] = client_key
             __props__.__dict__["client_key_file"] = client_key_file
             __props__.__dict__["client_key_passphrase"] = client_key_passphrase
+            __props__.__dict__["kafka_version"] = kafka_version
             __props__.__dict__["sasl_aws_creds_debug"] = pulumi.Output.from_input(sasl_aws_creds_debug).apply(pulumi.runtime.to_json) if sasl_aws_creds_debug is not None else None
             __props__.__dict__["sasl_aws_profile"] = sasl_aws_profile
             __props__.__dict__["sasl_aws_region"] = sasl_aws_region
             __props__.__dict__["sasl_aws_role_arn"] = sasl_aws_role_arn
             if sasl_mechanism is None:
                 sasl_mechanism = (_utilities.get_env('KAFKA_SASL_MECHANISM') or 'plain')
             __props__.__dict__["sasl_mechanism"] = sasl_mechanism
@@ -549,14 +572,23 @@
     def client_key_passphrase(self) -> pulumi.Output[Optional[str]]:
         """
         The passphrase for the private key that the certificate was issued for.
         """
         return pulumi.get(self, "client_key_passphrase")
 
     @property
+    @pulumi.getter(name="kafkaVersion")
+    def kafka_version(self) -> pulumi.Output[Optional[str]]:
+        """
+        The version of Kafka protocol to use in `$MAJOR.$MINOR.$PATCH` format. Some features may not be available on older
+        versions. Default is 2.7.0.
+        """
+        return pulumi.get(self, "kafka_version")
+
+    @property
     @pulumi.getter(name="saslAwsProfile")
     def sasl_aws_profile(self) -> pulumi.Output[Optional[str]]:
         """
         AWS profile name to use
         """
         return pulumi.get(self, "sasl_aws_profile")
```

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/quota.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/topic.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka/user_scram_credential.py` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka/user_scram_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1711778096
+Version: 3.8.0a1712078841
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1711778096/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.8.0a1712078841/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1711778096/pyproject.toml` & `pulumi_kafka-3.8.0a1712078841/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kafka"
   description = "A Pulumi package for creating and managing Kafka."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kafka"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.8.0a1711778096"
+  version = "3.8.0a1712078841"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kafka"
 
 [build-system]
```

