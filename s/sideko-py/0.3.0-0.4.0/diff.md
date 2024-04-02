# Comparing `tmp/sideko_py-0.3.0.tar.gz` & `tmp/sideko_py-0.4.0.tar.gz`

## Comparing `sideko_py-0.3.0.tar` & `sideko_py-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0      501       20      484 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/Cargo.toml
--rw-r--r--   0      501       20     2195 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/README.md
--rw-r--r--   0      501       20     3169 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/auth.rs
--rw-r--r--   0      501       20     6610 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/blocking.rs
--rw-r--r--   0      501       20      433 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/error_enums.rs
--rw-r--r--   0      501       20     7223 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/lib.rs
--rw-r--r--   0      501       20      445 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/request_types.rs
--rw-r--r--   0      501       20     1522 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/result.rs
--rw-r--r--   0      501       20     2154 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-api/src/schemas.rs
--rw-r--r--   0      501       20      835 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/Cargo.toml
--rw-r--r--   0      501       20     5685 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/cli.rs
--rw-r--r--   0      501       20     4544 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/cmds/generate.rs
--rw-r--r--   0      501       20     3493 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/cmds/login.rs
--rw-r--r--   0      501       20       33 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/cmds/mod.rs
--rw-r--r--   0      501       20     2011 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/config.rs
--rw-r--r--   0      501       20     1264 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/html/failure.html
--rw-r--r--   0      501       20     1216 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/html/success.html
--rw-r--r--   0      501       20       90 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/lib.rs
--rw-r--r--   0      501       20      203 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/main.rs
--rw-r--r--   0      501       20     1850 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/result.rs
--rw-r--r--   0      501       20     1060 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/styles.rs
--rw-r--r--   0      501       20     3176 2024-03-07 23:27:17.000000 sideko_py-0.3.0/core/src/utils.rs
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 sideko_py-0.3.0/sideko-py/Cargo.toml
--rw-r--r--   0      501       20     3860 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-py/LICENSE
--rw-r--r--   0      501       20     1691 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-py/README.md
--rw-r--r--   0      501       20     2334 2024-03-07 23:27:17.000000 sideko_py-0.3.0/sideko-py/src/lib.rs
--rw-r--r--   0      501       20    62967 2024-03-07 23:27:17.000000 sideko_py-0.3.0/Cargo.lock
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 sideko_py-0.3.0/Cargo.toml
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 sideko_py-0.3.0/pyproject.toml
--rw-r--r--   0      501       20     3860 2024-03-07 23:27:17.000000 sideko_py-0.3.0/LICENSE
--rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 sideko_py-0.3.0/PKG-INFO
+-rw-r--r--   0      501       20      484 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/Cargo.toml
+-rw-r--r--   0      501       20     2195 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/README.md
+-rw-r--r--   0      501       20     3169 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/auth.rs
+-rw-r--r--   0      501       20     6513 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/blocking.rs
+-rw-r--r--   0      501       20      433 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/error_enums.rs
+-rw-r--r--   0      501       20     7141 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/lib.rs
+-rw-r--r--   0      501       20      445 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/request_types.rs
+-rw-r--r--   0      501       20     1522 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/result.rs
+-rw-r--r--   0      501       20     2154 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-api/src/schemas.rs
+-rw-r--r--   0      501       20      835 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/Cargo.toml
+-rw-r--r--   0      501       20     5685 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/cli.rs
+-rw-r--r--   0      501       20     4544 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/cmds/generate.rs
+-rw-r--r--   0      501       20     3492 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/cmds/login.rs
+-rw-r--r--   0      501       20       33 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/cmds/mod.rs
+-rw-r--r--   0      501       20     2011 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/config.rs
+-rw-r--r--   0      501       20     1264 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/html/failure.html
+-rw-r--r--   0      501       20     1216 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/html/success.html
+-rw-r--r--   0      501       20       90 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/lib.rs
+-rw-r--r--   0      501       20      203 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/main.rs
+-rw-r--r--   0      501       20     1850 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/result.rs
+-rw-r--r--   0      501       20     1060 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/styles.rs
+-rw-r--r--   0      501       20     3176 2024-04-02 12:44:42.000000 sideko_py-0.4.0/core/src/utils.rs
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 sideko_py-0.4.0/sideko-py/Cargo.toml
+-rw-r--r--   0      501       20     3860 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-py/LICENSE
+-rw-r--r--   0      501       20     1691 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-py/README.md
+-rw-r--r--   0      501       20     2334 2024-04-02 12:44:42.000000 sideko_py-0.4.0/sideko-py/src/lib.rs
+-rw-r--r--   0      501       20    62967 2024-04-02 12:44:42.000000 sideko_py-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 sideko_py-0.4.0/Cargo.toml
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 sideko_py-0.4.0/pyproject.toml
+-rw-r--r--   0      501       20     3860 2024-04-02 12:44:42.000000 sideko_py-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 sideko_py-0.4.0/PKG-INFO
```

### Comparing `sideko_py-0.3.0/sideko-api/README.md` & `sideko_py-0.4.0/sideko-api/README.md`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/sideko-api/src/auth.rs` & `sideko_py-0.4.0/sideko-api/src/auth.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/sideko-api/src/blocking.rs` & `sideko_py-0.4.0/sideko-api/src/blocking.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 /// Generatedby Sideko (sideko.dev)
 use crate::auth;
+use crate::error_enums;
 use crate::request_types::*;
 use crate::result;
-use crate::error_enums;
 use crate::schemas::*;
-use reqwest::blocking::Client as ReqwestClient;
-use reqwest::blocking::RequestBuilder as ReqwestRequestBuilder;
 #[allow(unused)]
 use reqwest::blocking::multipart as reqwest_multipart;
+use reqwest::blocking::Client as ReqwestClient;
+use reqwest::blocking::RequestBuilder as ReqwestRequestBuilder;
 use std::collections::BTreeMap;
 #[derive(Clone, Debug)]
 pub struct Client {
     pub base_url: String,
     auth: BTreeMap<String, auth::AuthProvider>,
 }
 impl Default for Client {
     fn default() -> Self {
         Self {
-            base_url: "http://server-not-specified".to_string(),
+            base_url: "https://api.sideko.dev".to_string(),
             auth: BTreeMap::new(),
         }
     }
 }
 impl Client {
     /// Override the default base url
     pub fn with_base_url(mut self, base_url: &str) -> Self {
         self.base_url = base_url.into();
         self
     }
     /// Authentication  builder function to store api-key credentials in the client
     pub fn with_api_key_auth(mut self, val: &str) -> Self {
-        self.auth
-            .insert(
-                "ApiKeyAuth".to_string(),
-                auth::AuthProvider::KeyHeader(
-                    "x-sideko-key".to_string(),
-                    val.to_string(),
-                ),
-            );
+        self.auth.insert(
+            "ApiKeyAuth".to_string(),
+            auth::AuthProvider::KeyHeader("x-sideko-key".to_string(), val.to_string()),
+        );
         self
     }
     fn builder_with_auth(
         &self,
         mut req_builder: ReqwestRequestBuilder,
         auth_names: &[&str],
     ) -> ReqwestRequestBuilder {
@@ -52,111 +48,111 @@
         }
         req_builder
     }
     pub fn exchange_code_for_key(
         &self,
         request: ExchangeCodeForKeyRequest,
     ) -> result::Result<ApiKey, error_enums::ExchangeCodeForKeyErrors> {
-        let endpoint = "/api/auth/exchange_key";
+        let endpoint = "/v1/auth/exchange_key";
         let url = format!("{}{}", self.base_url, endpoint);
         let mut query_params: Vec<(&str, String)> = vec![];
-        query_params.push(("code", format!("{}", & request.code)));
+        query_params.push(("code", format!("{}", &request.code)));
         let unauthed_builder = ReqwestClient::default().get(&url).query(&query_params);
         let authed_builder = self.builder_with_auth(unauthed_builder, &["ApiKeyAuth"]);
         let response = authed_builder.send().map_err(result::Error::Dispatch)?;
         let status_code = response.status().as_u16();
         match status_code {
             200 => {
                 let response_text = response.text().unwrap_or_default();
-                let data = serde_json::from_str::<ApiKey>(&response_text)
-                    .map_err(|serde_err| result::Error::UnexpectedResponseBody {
+                let data = serde_json::from_str::<ApiKey>(&response_text).map_err(|serde_err| {
+                    result::Error::UnexpectedResponseBody {
                         status_code,
                         method: "GET".to_string(),
                         url: url.to_string(),
                         response_text,
                         expected_signature: "ApiKey".to_string(),
                         serde_err,
-                    })?;
+                    }
+                })?;
                 Ok(data)
             }
             _ => {
-                let expected_status_codes: Vec<String> = vec!["200".to_string(),];
+                let expected_status_codes: Vec<String> = vec!["200".to_string()];
                 Err(result::Error::BlockingUnexpectedStatus {
                     status_code,
                     method: "".to_string(),
                     url: url.to_string(),
                     response,
                     expected_status_codes,
                 })
             }
         }
     }
     pub fn cli_check_updates(
         &self,
         request: CliCheckUpdatesRequest,
     ) -> result::Result<Vec<CliUpdate>, error_enums::CliCheckUpdatesErrors> {
-        let endpoint = format!("/api/cli/updates/{}", request.cli_version);
+        let endpoint = format!("/v1/cli/updates/{}", request.cli_version);
         let url = format!("{}{}", self.base_url, endpoint);
         let query_params: Vec<(&str, String)> = vec![];
         let unauthed_builder = ReqwestClient::default().get(&url).query(&query_params);
         let authed_builder = self.builder_with_auth(unauthed_builder, &["ApiKeyAuth"]);
         let response = authed_builder.send().map_err(result::Error::Dispatch)?;
         let status_code = response.status().as_u16();
         match status_code {
             200 => {
                 let response_text = response.text().unwrap_or_default();
-                let data = serde_json::from_str::<Vec<CliUpdate>>(&response_text)
-                    .map_err(|serde_err| result::Error::UnexpectedResponseBody {
+                let data = serde_json::from_str::<Vec<CliUpdate>>(&response_text).map_err(
+                    |serde_err| result::Error::UnexpectedResponseBody {
                         status_code,
                         method: "GET".to_string(),
                         url: url.to_string(),
                         response_text,
                         expected_signature: "Vec<CliUpdate>".to_string(),
                         serde_err,
-                    })?;
+                    },
+                )?;
                 Ok(data)
             }
             _ => {
-                let expected_status_codes: Vec<String> = vec!["200".to_string(),];
+                let expected_status_codes: Vec<String> = vec!["200".to_string()];
                 Err(result::Error::BlockingUnexpectedStatus {
                     status_code,
                     method: "".to_string(),
                     url: url.to_string(),
                     response,
                     expected_status_codes,
                 })
             }
         }
     }
     pub fn stateless_generate_sdk(
         &self,
         request: StatelessGenerateSdkRequest,
     ) -> result::Result<BinaryResponse, error_enums::StatelessGenerateSdkErrors> {
-        let endpoint = "/api/stateless/generate_sdk";
+        let endpoint = "/v1/stateless/generate_sdk";
         let url = format!("{}{}", self.base_url, endpoint);
         let query_params: Vec<(&str, String)> = vec![];
         let unauthed_builder = ReqwestClient::default().post(&url).query(&query_params);
         let authed_builder = self.builder_with_auth(unauthed_builder, &["ApiKeyAuth"]);
-        let request_body: serde_json::Value = serde_json::to_value(request.data)
-            .map_err(result::Error::Serialize)?;
+        let request_body: serde_json::Value =
+            serde_json::to_value(request.data).map_err(result::Error::Serialize)?;
         let response = authed_builder
             .json(&request_body)
             .send()
             .map_err(result::Error::Dispatch)?;
         let status_code = response.status().as_u16();
         match status_code {
             201 => {
                 let res_bytes = response.bytes().map_err(result::Error::ResponseBytes)?;
-                let data = BinaryResponse {
-                    content: res_bytes,
-                };
+                let data = BinaryResponse { content: res_bytes };
                 Ok(data)
             }
             _ => {
-                let expected_status_codes: Vec<String> = vec!["201".to_string(),];
+                let expected_status_codes: Vec<String> = vec!["201".to_string()];
                 Err(result::Error::BlockingUnexpectedStatus {
                     status_code,
                     method: "".to_string(),
                     url: url.to_string(),
                     response,
                     expected_status_codes,
                 })
```

### Comparing `sideko_py-0.3.0/sideko-api/src/lib.rs` & `sideko_py-0.4.0/sideko-api/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,48 +3,44 @@
 mod auth;
 pub mod blocking;
 pub mod error_enums;
 pub mod request_types;
 pub mod result;
 pub mod schemas;
 use request_types::*;
-use schemas::*;
+use reqwest::multipart as reqwest_multipart;
 use reqwest::Client as ReqwestClient;
 use reqwest::RequestBuilder as ReqwestRequestBuilder;
-use reqwest::multipart as reqwest_multipart;
+use schemas::*;
 use std::collections::BTreeMap;
 #[derive(Clone, Debug)]
 pub struct Client {
     pub base_url: String,
     auth: BTreeMap<String, auth::AuthProvider>,
 }
 impl Default for Client {
     fn default() -> Self {
         Self {
-            base_url: "http://server-not-specified".to_string(),
+            base_url: "https://api.sideko.dev".to_string(),
             auth: BTreeMap::new(),
         }
     }
 }
 impl Client {
     /// Override the default base url
     pub fn with_base_url(mut self, base_url: &str) -> Self {
         self.base_url = base_url.into();
         self
     }
     /// Authentication  builder function to store api-key credentials in the client
     pub fn with_api_key_auth(mut self, val: &str) -> Self {
-        self.auth
-            .insert(
-                "ApiKeyAuth".to_string(),
-                auth::AuthProvider::KeyHeader(
-                    "x-sideko-key".to_string(),
-                    val.to_string(),
-                ),
-            );
+        self.auth.insert(
+            "ApiKeyAuth".to_string(),
+            auth::AuthProvider::KeyHeader("x-sideko-key".to_string(), val.to_string()),
+        );
         self
     }
     fn builder_with_auth(
         &self,
         mut req_builder: ReqwestRequestBuilder,
         auth_names: &[&str],
     ) -> ReqwestRequestBuilder {
@@ -52,133 +48,133 @@
             if let Some(provider) = self.auth.get(&auth_name.to_string()) {
                 req_builder = provider.add_auth(req_builder);
             }
         }
         req_builder
     }
     #[allow(unused)]
-    fn async_multipart_file(
-        &self,
-        path: &str,
-    ) -> std::io::Result<reqwest_multipart::Part> {
+    fn async_multipart_file(&self, path: &str) -> std::io::Result<reqwest_multipart::Part> {
         let path: &std::path::Path = path.as_ref();
         let file_name = path
             .file_name()
             .map(|filename| filename.to_string_lossy().into_owned());
         let file_bytes = std::fs::read(path)?;
-        Ok(
-            reqwest_multipart::Part::bytes(file_bytes)
-                .file_name(file_name.unwrap_or_default()),
-        )
+        Ok(reqwest_multipart::Part::bytes(file_bytes).file_name(file_name.unwrap_or_default()))
     }
     pub async fn exchange_code_for_key(
         &self,
         request: ExchangeCodeForKeyRequest,
     ) -> result::Result<ApiKey, error_enums::ExchangeCodeForKeyErrors> {
-        let endpoint = "/api/auth/exchange_key";
+        let endpoint = "/v1/auth/exchange_key";
         let url = format!("{}{}", self.base_url, endpoint);
         let mut query_params: Vec<(&str, String)> = vec![];
-        query_params.push(("code", format!("{}", & request.code)));
+        query_params.push(("code", format!("{}", &request.code)));
         let unauthed_builder = ReqwestClient::default().get(&url).query(&query_params);
         let authed_builder = self.builder_with_auth(unauthed_builder, &["ApiKeyAuth"]);
-        let response = authed_builder.send().await.map_err(result::Error::Dispatch)?;
+        let response = authed_builder
+            .send()
+            .await
+            .map_err(result::Error::Dispatch)?;
         let status_code = response.status().as_u16();
         match status_code {
             200 => {
                 let response_text = response.text().await.unwrap_or_default();
-                let data = serde_json::from_str::<ApiKey>(&response_text)
-                    .map_err(|serde_err| result::Error::UnexpectedResponseBody {
+                let data = serde_json::from_str::<ApiKey>(&response_text).map_err(|serde_err| {
+                    result::Error::UnexpectedResponseBody {
                         status_code,
                         method: "GET".to_string(),
                         url: url.to_string(),
                         response_text,
                         expected_signature: "ApiKey".to_string(),
                         serde_err,
-                    })?;
+                    }
+                })?;
                 Ok(data)
             }
             _ => {
-                let expected_status_codes: Vec<String> = vec!["200".to_string(),];
+                let expected_status_codes: Vec<String> = vec!["200".to_string()];
                 Err(result::Error::UnexpectedStatus {
                     status_code,
                     method: "".to_string(),
                     url: url.to_string(),
                     response,
                     expected_status_codes,
                 })
             }
         }
     }
     pub async fn cli_check_updates(
         &self,
         request: CliCheckUpdatesRequest,
     ) -> result::Result<Vec<CliUpdate>, error_enums::CliCheckUpdatesErrors> {
-        let endpoint = format!("/api/cli/updates/{}", request.cli_version);
+        let endpoint = format!("/v1/cli/updates/{}", request.cli_version);
         let url = format!("{}{}", self.base_url, endpoint);
         let query_params: Vec<(&str, String)> = vec![];
         let unauthed_builder = ReqwestClient::default().get(&url).query(&query_params);
         let authed_builder = self.builder_with_auth(unauthed_builder, &["ApiKeyAuth"]);
-        let response = authed_builder.send().await.map_err(result::Error::Dispatch)?;
+        let response = authed_builder
+            .send()
+            .await
+            .map_err(result::Error::Dispatch)?;
         let status_code = response.status().as_u16();
         match status_code {
             200 => {
                 let response_text = response.text().await.unwrap_or_default();
-                let data = serde_json::from_str::<Vec<CliUpdate>>(&response_text)
-                    .map_err(|serde_err| result::Error::UnexpectedResponseBody {
+                let data = serde_json::from_str::<Vec<CliUpdate>>(&response_text).map_err(
+                    |serde_err| result::Error::UnexpectedResponseBody {
                         status_code,
                         method: "GET".to_string(),
                         url: url.to_string(),
                         response_text,
                         expected_signature: "Vec<CliUpdate>".to_string(),
                         serde_err,
-                    })?;
+                    },
+                )?;
                 Ok(data)
             }
             _ => {
-                let expected_status_codes: Vec<String> = vec!["200".to_string(),];
+                let expected_status_codes: Vec<String> = vec!["200".to_string()];
                 Err(result::Error::UnexpectedStatus {
                     status_code,
                     method: "".to_string(),
                     url: url.to_string(),
                     response,
                     expected_status_codes,
                 })
             }
         }
     }
     pub async fn stateless_generate_sdk(
         &self,
         request: StatelessGenerateSdkRequest,
     ) -> result::Result<BinaryResponse, error_enums::StatelessGenerateSdkErrors> {
-        let endpoint = "/api/stateless/generate_sdk";
+        let endpoint = "/v1/stateless/generate_sdk";
         let url = format!("{}{}", self.base_url, endpoint);
         let query_params: Vec<(&str, String)> = vec![];
         let unauthed_builder = ReqwestClient::default().post(&url).query(&query_params);
         let authed_builder = self.builder_with_auth(unauthed_builder, &["ApiKeyAuth"]);
-        let request_body: serde_json::Value = serde_json::to_value(request.data)
-            .map_err(result::Error::Serialize)?;
+        let request_body: serde_json::Value =
+            serde_json::to_value(request.data).map_err(result::Error::Serialize)?;
         let response = authed_builder
             .json(&request_body)
             .send()
             .await
             .map_err(result::Error::Dispatch)?;
         let status_code = response.status().as_u16();
         match status_code {
             201 => {
                 let res_bytes = response
                     .bytes()
                     .await
                     .map_err(result::Error::ResponseBytes)?;
-                let data = BinaryResponse {
-                    content: res_bytes,
-                };
+                let data = BinaryResponse { content: res_bytes };
                 Ok(data)
             }
             _ => {
-                let expected_status_codes: Vec<String> = vec!["201".to_string(),];
+                let expected_status_codes: Vec<String> = vec!["201".to_string()];
                 Err(result::Error::UnexpectedStatus {
                     status_code,
                     method: "".to_string(),
                     url: url.to_string(),
                     response,
                     expected_status_codes,
                 })
```

### Comparing `sideko_py-0.3.0/sideko-api/src/result.rs` & `sideko_py-0.4.0/sideko-api/src/result.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/sideko-api/src/schemas.rs` & `sideko_py-0.4.0/sideko-api/src/schemas.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/Cargo.toml` & `sideko_py-0.4.0/core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "sideko"
-version = "0.3.0"
+version = "0.4.0"
 edition = "2021"
 authors = [
     "Elias Posen <elias@sideko.dev>",
     "Patrick Kelly <patrick@sideko.dev>",
 ]
 
 [target.x86_64-unknown-linux-musl.dependencies]
```

### Comparing `sideko_py-0.3.0/core/src/cli.rs` & `sideko_py-0.4.0/core/src/cli.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/cmds/generate.rs` & `sideko_py-0.4.0/core/src/cmds/generate.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/cmds/login.rs` & `sideko_py-0.4.0/core/src/cmds/login.rs`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     utils::validate_path(output.clone(), &utils::PathKind::File, true)?;
 
     // check for updates after all other validation passed
     check_for_updates().await?;
 
     // open browser for login
     let login_url = url::Url::parse_with_params(
-        &format!("{}/api/auth/login_url", config::get_base_url()),
+        &format!("{}/v1/auth/login_url", config::get_base_url()),
         &[
             ("cli_output", output.to_str().unwrap_or(".")),
             ("cli_port", &port.to_string()),
         ],
     )
     .unwrap()
     .to_string();
```

### Comparing `sideko_py-0.3.0/core/src/config.rs` & `sideko_py-0.4.0/core/src/config.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/html/failure.html` & `sideko_py-0.4.0/core/src/html/failure.html`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/html/success.html` & `sideko_py-0.4.0/core/src/html/success.html`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/result.rs` & `sideko_py-0.4.0/core/src/result.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/styles.rs` & `sideko_py-0.4.0/core/src/styles.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/core/src/utils.rs` & `sideko_py-0.4.0/core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/sideko-py/LICENSE` & `sideko_py-0.4.0/sideko-py/LICENSE`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/sideko-py/README.md` & `sideko_py-0.4.0/sideko-py/README.md`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/sideko-py/src/lib.rs` & `sideko_py-0.4.0/sideko-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/Cargo.lock` & `sideko_py-0.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1659,15 +1659,15 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "sideko"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "anstyle",
  "bytes",
  "camino",
  "clap",
  "dotenv",
  "env_logger",
@@ -1685,15 +1685,15 @@
  "tar",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "sideko-py"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "log",
  "pyo3",
  "sideko",
  "sideko_api",
  "tokio",
 ]
```

### Comparing `sideko_py-0.3.0/pyproject.toml` & `sideko_py-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/LICENSE` & `sideko_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sideko_py-0.3.0/PKG-INFO` & `sideko_py-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sideko-py
-Version: 0.3.0
+Version: 0.4.0
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
 License-File: LICENSE
```

