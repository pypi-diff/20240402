# Comparing `tmp/antigranular_enterprise-0.0.8.tar.gz` & `tmp/antigranular_enterprise-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular_enterprise-0.0.8.tar", max compression
+gzip compressed data, was "antigranular_enterprise-0.0.9.tar", max compression
```

## Comparing `antigranular_enterprise-0.0.8.tar` & `antigranular_enterprise-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-11 13:42:13.506293 antigranular_enterprise-0.0.8/LICENSE
--rw-r--r--   0        0        0     4047 2024-03-27 13:18:03.560056 antigranular_enterprise-0.0.8/README.md
--rw-r--r--   0        0        0      801 2024-03-31 00:20:20.322114 antigranular_enterprise-0.0.8/antigranular_enterprise/__init__.py
--rw-r--r--   0        0        0     3675 2024-03-31 00:15:03.692157 antigranular_enterprise-0.0.8/antigranular_enterprise/agent_client/agent_client.py
--rw-r--r--   0        0        0    20361 2024-03-31 00:16:33.202145 antigranular_enterprise-0.0.8/antigranular_enterprise/client.py
--rw-r--r--   0        0        0     5396 2024-03-29 12:09:29.602788 antigranular_enterprise-0.0.8/antigranular_enterprise/config/config.py
--rw-r--r--   0        0        0      945 2024-03-26 18:39:10.451789 antigranular_enterprise-0.0.8/antigranular_enterprise/magics/errors.py
--rw-r--r--   0        0        0     6656 2024-03-26 18:39:10.451789 antigranular_enterprise-0.0.8/antigranular_enterprise/magics/magics.py
--rw-r--r--   0        0        0        0 2024-03-26 18:39:10.451789 antigranular_enterprise-0.0.8/antigranular_enterprise/models/__init__.py
--rw-r--r--   0        0        0      622 2024-03-31 00:15:03.692157 antigranular_enterprise-0.0.8/antigranular_enterprise/models/models.py
--rw-r--r--   0        0        0     2800 2024-03-27 06:14:29.873404 antigranular_enterprise-0.0.8/antigranular_enterprise/nb.ipynb
--rw-r--r--   0        0        0      211 2024-03-28 17:28:11.331853 antigranular_enterprise-0.0.8/antigranular_enterprise/utils/error_print.py
--rw-r--r--   0        0        0      192 2024-03-26 18:39:10.451789 antigranular_enterprise-0.0.8/antigranular_enterprise/utils/print_request_id.py
--rw-r--r--   0        0        0     1369 2024-03-31 00:19:29.962122 antigranular_enterprise-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 antigranular_enterprise-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      834 2024-03-31 11:51:09.553243 antigranular_enterprise-0.0.9/antigranular_enterprise/__init__.py
+-rw-r--r--   0        0        0     3775 2024-03-31 11:49:53.569980 antigranular_enterprise-0.0.9/antigranular_enterprise/agent_client/agent_client.py
+-rw-r--r--   0        0        0    20871 2024-03-31 11:49:32.238859 antigranular_enterprise-0.0.9/antigranular_enterprise/client.py
+-rw-r--r--   0        0        0     5543 2024-03-31 11:00:59.432585 antigranular_enterprise-0.0.9/antigranular_enterprise/config/config.py
+-rw-r--r--   0        0        0      975 2024-03-31 11:00:59.444890 antigranular_enterprise-0.0.9/antigranular_enterprise/magics/errors.py
+-rw-r--r--   0        0        0     6840 2024-03-31 11:00:59.450425 antigranular_enterprise-0.0.9/antigranular_enterprise/magics/magics.py
+-rw-r--r--   0        0        0        0 2024-03-31 11:00:59.452425 antigranular_enterprise-0.0.9/antigranular_enterprise/models/__init__.py
+-rw-r--r--   0        0        0      657 2024-03-31 11:00:59.461696 antigranular_enterprise-0.0.9/antigranular_enterprise/models/models.py
+-rw-r--r--   0        0        0      222 2024-03-31 11:00:59.501570 antigranular_enterprise-0.0.9/antigranular_enterprise/utils/error_print.py
+-rw-r--r--   0        0        0      196 2024-03-31 11:00:59.511135 antigranular_enterprise-0.0.9/antigranular_enterprise/utils/print_request_id.py
+-rw-r--r--   0        0        0    11558 2024-03-31 11:00:32.751829 antigranular_enterprise-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1402 2024-03-31 11:50:41.517308 antigranular_enterprise-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4128 2024-03-31 11:00:59.400545 antigranular_enterprise-0.0.9/README.md
+-rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 antigranular_enterprise-0.0.9/PKG-INFO
```

### Comparing `antigranular_enterprise-0.0.8/LICENSE` & `antigranular_enterprise-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `antigranular_enterprise-0.0.8/README.md` & `antigranular_enterprise-0.0.9/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# Antigranular Enterprise: Secure, Privacy-Preserving Data Science in Jupyter Environments
-
-The `antigranular_enterprise` package is a specialized Jupyter client designed for secure and private interaction with the Antigranular Enterprise platform. It facilitates secure data analysis and model training within a Jupyter notebook environment, emphasizing privacy and data protection. This documentation guides you through installing, configuring, and utilizing the client package to integrate Antigranular Enterprise capabilities directly into your Jupyter notebooks.
-
-## Installation
-
-To integrate Antigranular Enterprise with your Jupyter environment, install the package using pip:
-
-```bash
-pip install antigranular_enterprise
-```
-
-This command installs the `antigranular_enterprise` package and its necessary dependencies, preparing your Jupyter environment for secure, privacy-preserving data analysis.
-
-## Configuration
-
-### Initial Configuration
-
-The initial setup requires configuring the package to communicate with your Antigranular Enterprise instance. Required configuration parameters include:
-
-- **AGENT Jupyter Server URL**: URL for the Proxy server that routes requests to the Antigranular platform.
-- **AGENT Jupyter Server Port**: Port on which Proxy listens.
-- **AGENT Console URL**: URL for the Antigranular management console.
-- **AGENT Console API Key Parameter**: Name of the parameter used for the API key in requests.
-
-### Creating a Configuration File
-
-Configure your environment by creating a configuration file with the required parameters:
-
-1. Import the package in a Jupyter notebook:
-
-    ```python
-    import antigranular_enterprise as ag
-    ```
-
-2. Define and write the configuration file using the `write_config` method. Replace placeholder values with those specific to your Antigranular Enterprise setup:
-
-    ```python
-    ag.write_config(profile='default', yaml_config="""
-    agent_jupyter_url: <Jupyter URL>
-    agent_jupyter_port: <Jupyter Port>
-    agent_AGENT_CONSOLE_URL: <Console URL>
-    agent_console_api_key_param: <Console API Key Parameter>
-    """)
-    ```
-
-This configuration allows the `antigranular_enterprise` client to correctly route and authenticate requests to your Antigranular instance.
-
-## Client Login
-
-Access the Antigranular Enterprise services by logging in through the Jupyter notebook:
-
-1. Login using your API key:
-
-    ```python
-    client = ag.login("<api_key>")
-    ```
-
-2. A UI notification or link will prompt you for approval. Upon approval, the session starts, allowing secure interaction with the Antigranular platform.
-
-###  Switching to a Different Profile
-Once you have multiple profiles configured, you can switch between them by reading the desired profile's configuration before initiating any operations or sessions. Use the read_config method to load the configuration for a specific profile:
-
-```python
-ag.read_config(profile='profile_name')
-```
-
-## Features and Usage
-
-The `antigranular_enterprise` Jupyter client package offers a suite of features for data analysis and model training, prioritizing data privacy and security:
-
-- **Session Management**: Easily manage your connection sessions to the Antigranular server.
-- **Secure Data Analysis**: Perform data analysis operations within the secure confines of the Antigranular environment.
-- **Privacy-Enhanced Machine Learning**: Train machine learning models while adhering to privacy regulations and standards.
-- **Jupyter Notebook Integration**: Leverage the `%ag` cell magic for executing secure Python code directly in Jupyter notebooks, facilitating a seamless workflow with Antigranular services.
-
-Refer to the in-package documentation or the Antigranular Enterprise platform for detailed examples and advanced usage instructions.
-
-## Support
-
-For assistance, troubleshooting, or to report issues with the `antigranular_enterprise` Jupyter client package, please reach out to the Antigranular support team or consult the comprehensive documentation provided on the Antigranular Enterprise platform.
+# Antigranular Enterprise: Secure, Privacy-Preserving Data Science in Jupyter Environments
+
+The `antigranular_enterprise` package is a specialized Jupyter client designed for secure and private interaction with the Antigranular Enterprise platform. It facilitates secure data analysis and model training within a Jupyter notebook environment, emphasizing privacy and data protection. This documentation guides you through installing, configuring, and utilizing the client package to integrate Antigranular Enterprise capabilities directly into your Jupyter notebooks.
+
+## Installation
+
+To integrate Antigranular Enterprise with your Jupyter environment, install the package using pip:
+
+```bash
+pip install antigranular_enterprise
+```
+
+This command installs the `antigranular_enterprise` package and its necessary dependencies, preparing your Jupyter environment for secure, privacy-preserving data analysis.
+
+## Configuration
+
+### Initial Configuration
+
+The initial setup requires configuring the package to communicate with your Antigranular Enterprise instance. Required configuration parameters include:
+
+- **AGENT Jupyter Server URL**: URL for the Proxy server that routes requests to the Antigranular platform.
+- **AGENT Jupyter Server Port**: Port on which Proxy listens.
+- **AGENT Console URL**: URL for the Antigranular management console.
+- **AGENT Console API Key Parameter**: Name of the parameter used for the API key in requests.
+
+### Creating a Configuration File
+
+Configure your environment by creating a configuration file with the required parameters:
+
+1. Import the package in a Jupyter notebook:
+
+    ```python
+    import antigranular_enterprise as ag
+    ```
+
+2. Define and write the configuration file using the `write_config` method. Replace placeholder values with those specific to your Antigranular Enterprise setup:
+
+    ```python
+    ag.write_config(profile='default', yaml_config="""
+    agent_jupyter_url: <Jupyter URL>
+    agent_jupyter_port: <Jupyter Port>
+    agent_AGENT_CONSOLE_URL: <Console URL>
+    agent_console_api_key_param: <Console API Key Parameter>
+    """)
+    ```
+
+This configuration allows the `antigranular_enterprise` client to correctly route and authenticate requests to your Antigranular instance.
+
+## Client Login
+
+Access the Antigranular Enterprise services by logging in through the Jupyter notebook:
+
+1. Login using your API key:
+
+    ```python
+    client = ag.login("<api_key>")
+    ```
+
+2. A UI notification or link will prompt you for approval. Upon approval, the session starts, allowing secure interaction with the Antigranular platform.
+
+###  Switching to a Different Profile
+Once you have multiple profiles configured, you can switch between them by reading the desired profile's configuration before initiating any operations or sessions. Use the read_config method to load the configuration for a specific profile:
+
+```python
+ag.read_config(profile='profile_name')
+```
+
+## Features and Usage
+
+The `antigranular_enterprise` Jupyter client package offers a suite of features for data analysis and model training, prioritizing data privacy and security:
+
+- **Session Management**: Easily manage your connection sessions to the Antigranular server.
+- **Secure Data Analysis**: Perform data analysis operations within the secure confines of the Antigranular environment.
+- **Privacy-Enhanced Machine Learning**: Train machine learning models while adhering to privacy regulations and standards.
+- **Jupyter Notebook Integration**: Leverage the `%ag` cell magic for executing secure Python code directly in Jupyter notebooks, facilitating a seamless workflow with Antigranular services.
+
+Refer to the in-package documentation or the Antigranular Enterprise platform for detailed examples and advanced usage instructions.
+
+## Support
+
+For assistance, troubleshooting, or to report issues with the `antigranular_enterprise` Jupyter client package, please reach out to the Antigranular support team or consult the comprehensive documentation provided on the Antigranular Enterprise platform.
```

### Comparing `antigranular_enterprise-0.0.8/antigranular_enterprise/__init__.py` & `antigranular_enterprise-0.0.9/antigranular_enterprise/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""
-Antigranular client package
-"""
-
-
-from .client import login
-from .client import read_config
-from .client import write_config
-from .client import load_config
-# Package version dunder
-__version__ = "0.0.8"
-
-# Package author dunder
-__author__ = "Oblivious Software Pvt. Ltd."
-
-# Package * imports dunder
-__all__ = ["login", "read_config", "write_config", "load_config", "__version__", "__author__"]
-
-"""
-Raise an error if client in loaded in a non-Jupyter environment.
-"""
-from IPython.core.getipython import get_ipython
-
-ipython = get_ipython()
-if ipython is None:
-    raise ValueError(
-        "Please ensure antigranuler is loaded in a valid Jupyter environment."
-    )
-
-# Read default config on import
-# try:
-#     read_config()
-# except Exception:
+"""
+Antigranular client package
+"""
+
+
+from .client import login
+from .client import read_config
+from .client import write_config
+from .client import load_config
+# Package version dunder
+__version__ = "0.0.9"
+
+# Package author dunder
+__author__ = "Oblivious Software Pvt. Ltd."
+
+# Package * imports dunder
+__all__ = ["login", "read_config", "write_config", "load_config", "__version__", "__author__"]
+
+"""
+Raise an error if client in loaded in a non-Jupyter environment.
+"""
+from IPython.core.getipython import get_ipython
+
+ipython = get_ipython()
+if ipython is None:
+    raise ValueError(
+        "Please ensure antigranuler is loaded in a valid Jupyter environment."
+    )
+
+# Read default config on import
+# try:
+#     read_config()
+# except Exception:
 #     pass # Ignore if config file is not found
```

### Comparing `antigranular_enterprise-0.0.8/antigranular_enterprise/agent_client/agent_client.py` & `antigranular_enterprise-0.0.9/antigranular_enterprise/agent_client/agent_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import json
-import jwt
-import time
-import requests
-from ..config.config import config
-
-class AGClient:
-    """
-    Class to test AGClient when the AG Server with Oblv server is not available. 
-    Instead using AG private python server directly(passing custom x_oblv_name headers).
-    """
-    def __init__(
-        self,
-        URL,
-        PORT,
-        headers={},
-    ):
-        self.url = URL
-        self.port = PORT
-        self.base_url = URL + ":" + PORT
-        self.session = requests.Session()
-        if headers:
-            self.session.headers.update(headers)
-
-    def update_headers(self, headers):
-        self.session.headers.update(headers)
-
-    def get(self, endpoint, data=None, json=None, params=None, headers=None):
-        return self._make_request(
-            "GET", endpoint, data=data, json=json, params=params, headers=headers
-        )
-
-    def post(self, endpoint, data=None, json=None, params=None, headers=None, files=None):
-        return self._make_request(
-            "POST", endpoint, data=data, json=json, params=params, headers=headers, files=files
-        )
-
-    def put(self, endpoint, data=None, json=None, params=None, headers=None):
-        return self._make_request(
-            "PUT", endpoint, data=data, json=json, params=params, headers=headers
-        )
-
-    def delete(self, endpoint, data=None, json=None, params=None, headers=None):
-        return self._make_request(
-            "DELETE", endpoint, data=data, json=json, params=params, headers=headers
-        )
-    
-    def __is_token_expired(self) -> bool:
-        try:
-            payload = jwt.decode(self.session.headers['Authorization'], options={"verify_signature": False})
-            current_time = time.time() - 10  # 10 seconds for network latency
-
-            return payload.get('exp', 0) < current_time
-        except Exception as e:
-            raise ConnectionError(f"Error while checking token expiry: {str(e)}")
-
-    def __get_refresh_token(self) -> None:
-        try:
-            if not self.__is_token_expired():
-                return
-            res = requests.get(
-                config.AGENT_CONSOLE_URL + "/user/token/refresh",
-                params={"token": self.session.headers.get('refresh_token')},
-            )
-            res.raise_for_status()
-            data = json.loads(res.text)
-            if data.get("status") == "success":
-                self.session.headers['refresh_token'] = data.get("refresh_token")
-                self.session.headers['Authorization'] = data.get("token")
-            else:
-                raise ConnectionError(f"Error while refreshing token: {data}")
-        except Exception as e:
-            raise ConnectionError(f"Error while refreshing token: {str(e)}")
-
-    def _make_request(
-        self, method, endpoint, data=None, json=None, params=None, headers=None, files=None
-    ):
-        if self.session.headers.get('Authorization'):
-            self.__get_refresh_token()
-        url = endpoint
-        if headers:
-            with self.session as s:
-                s.headers.update(headers)
-                response = s.request(method, url, data=data, json=json, params=params, files=files, verify=getattr(config, 'tls_enabled', True))
-                s.headers.update(self.session.headers)
-        else:
-            response = self.session.request(
-                method, url, data=data, json=json, params=params
-            )
-        return response
-
-
-def get_ag_client():
-    """
-    Connect to AG server Server and initialize the Oblv client, AG server Server URL and port from config.
-    """
-    return AGClient(
-        config.AGENT_JUPYTER_URL,
-        config.AGENT_JUPYTER_PORT,
-    )
+import json
+import jwt
+import time
+import requests
+from ..config.config import config
+
+class AGClient:
+    """
+    Class to test AGClient when the AG Server with Oblv server is not available. 
+    Instead using AG private python server directly(passing custom x_oblv_name headers).
+    """
+    def __init__(
+        self,
+        URL,
+        PORT,
+        headers={},
+    ):
+        self.url = URL
+        self.port = PORT
+        self.base_url = URL + ":" + PORT
+        self.session = requests.Session()
+        if headers:
+            self.session.headers.update(headers)
+
+    def update_headers(self, headers):
+        self.session.headers.update(headers)
+
+    def get(self, endpoint, data=None, json=None, params=None, headers=None):
+        return self._make_request(
+            "GET", endpoint, data=data, json=json, params=params, headers=headers
+        )
+
+    def post(self, endpoint, data=None, json=None, params=None, headers=None, files=None):
+        return self._make_request(
+            "POST", endpoint, data=data, json=json, params=params, headers=headers, files=files
+        )
+
+    def put(self, endpoint, data=None, json=None, params=None, headers=None):
+        return self._make_request(
+            "PUT", endpoint, data=data, json=json, params=params, headers=headers
+        )
+
+    def delete(self, endpoint, data=None, json=None, params=None, headers=None):
+        return self._make_request(
+            "DELETE", endpoint, data=data, json=json, params=params, headers=headers
+        )
+    
+    def __is_token_expired(self) -> bool:
+        try:
+            payload = jwt.decode(self.session.headers['Authorization'], options={"verify_signature": False})
+            current_time = time.time() + 10  # 10 seconds for network latency
+
+            return payload.get('exp', 0) < current_time
+        except Exception as e:
+            raise ConnectionError(f"Error while checking token expiry: {str(e)}")
+
+    def __get_refresh_token(self) -> None:
+        try:
+            if not self.__is_token_expired():
+                return
+            res = requests.get(
+                config.AGENT_CONSOLE_URL + "/user/token/refresh",
+                params={"token": self.session.headers.get('refresh_token')},
+            )
+            res.raise_for_status()
+            data = json.loads(res.text)
+            if data.get("status") == "success":
+                self.session.headers['refresh_token'] = data.get("refresh_token")
+                self.session.headers['Authorization'] = data.get("token")
+            else:
+                raise ConnectionError(f"Error while refreshing token: {data}")
+        except Exception as e:
+            raise ConnectionError(f"Error while refreshing token: {str(e)}")
+
+    def _make_request(
+        self, method, endpoint, data=None, json=None, params=None, headers=None, files=None
+    ):
+        if self.session.headers.get('Authorization'):
+            self.__get_refresh_token()
+        url = endpoint
+        if headers:
+            with self.session as s:
+                s.headers.update(headers)
+                response = s.request(method, url, data=data, json=json, params=params, files=files, verify=getattr(config, 'tls_enabled', True))
+                s.headers.update(self.session.headers)
+        else:
+            response = self.session.request(
+                method, url, data=data, json=json, params=params
+            )
+        return response
+
+
+def get_ag_client():
+    """
+    Connect to AG server Server and initialize the Oblv client, AG server Server URL and port from config.
+    """
+    return AGClient(
+        config.AGENT_JUPYTER_URL,
+        config.AGENT_JUPYTER_PORT,
+    )
```

### Comparing `antigranular_enterprise-0.0.8/antigranular_enterprise/client.py` & `antigranular_enterprise-0.0.9/antigranular_enterprise/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,510 +1,510 @@
-"""
-Module for AGClient class.
-
-AGClient class contians all the methods to interact with the AG server like creating a session, uploading results, etc.
-It also contains methods to get the budget, privacy odometer, etc.
-
-"""
-
-import requests
-import json
-from typing import Any, Dict, Union
-import base64
-
-from antigranular_enterprise.utils.error_print import eprint
-try:
-    import onnx
-    onnx_installed = True
-except ImportError:
-    onnx_installed = False
-from .magics.magics import AGMagic
-from .agent_client.agent_client import get_ag_client, AGClient
-from .config.config import config
-from .models.models import AGServerInfo
-import onnx
-import pandas as pd
-from io import BytesIO
-from .utils.print_request_id import print_request_id
-import time
-from collections import OrderedDict
-import jwt
-import time
-
-def login(
-        api_key: str,
-        profile: str = "default"
-):
-    """
-    Login to the AG server and get the client objects.
-    Returns:
-        AGClient: The AGClient object.
-
-    Raises:
-        ConnectionError: If there is an error while creating the client.
-    """
-    try:
-        return AGClient(
-            api_key,
-            profile
-        )
-    except Exception as err:
-        raise ConnectionError(f"Error while creating client: {str(err)}")
-
-def read_config(profile="default") -> None:
-    """
-    Reads the configuration from a given profile.
-
-    Args:
-        profile (str): The profile to read the configuration from.
-    """
-    config.read_config(profile=profile)
-
-def write_config(yaml_config, profile) -> None:
-    """
-    Writes the configuration to a given profile.
-
-    Args:
-        yaml_config (dict): The configuration to write.
-        profile (str): The profile to write the configuration to.
-    """
-    config.write_config(yaml_config, profile)
-
-def load_config(config_url=None, profile="default") -> None:
-    """
-    Load the configuration from the given URL.
-
-    Args:
-        config_url (str): The URL to load the configuration from.
-        profile (str): The profile to load the configuration to.
-    """
-    config.load_config(config_url, profile)
-
-class AGClient:
-    """
-    AGClient class to interact with the AG server for competitions as well as accessing datasets for functionalities like creating a session, uploading competition submissions, downloading metadata, etc.
-    """
-
-    oblv_ag: AGClient
-    session_id: str
-    user_name: str = ""
-
-    def __init__(
-        self,
-        api_key: str,
-        profile: str
-    ):
-        """
-        Initialize AGClient class and check for headers if Client.
-
-        Raises:
-            ConnectionError: If there is an error while connecting to the server.
-        """
-        config.load_config(profile=profile)
-        # Make client if headers are provided
-        self.oblv_ag = get_ag_client(
-        )
-        self.headers = {
-            "Content-type": "application/json",
-            "accept": "application/json",
-            "Authorization": "",
-            "refresh_token": ""
-        }
-
-        # Create an AG session
-        self.connect(api_key)
-        if hasattr(self, 'session_id'):
-            try:
-                res = AGMagic.load_ag_magic()
-            except Exception as ex:
-                print(
-                    "Error loading %%ag magic functions, you might not be able to use cell magics as intended: ",
-                    str(ex),
-                )
-            AGMagic.load_oblv_client(self.oblv_ag, self.session_id)
-
-    @classmethod
-    def _from_agent_client(cls, ag_client_secret):
-        """
-        Initialize AGClient class from Client.
-        """
-        return cls(ag_client_secret)
-
-    def __is_token_expired(self) -> bool:
-        try:
-            payload = jwt.decode(self.headers['Authorization'], options={"verify_signature": False})
-            current_time = time.time() - 10 # 10 seconds for network latency
-            return payload.get('exp', 0) < current_time
-        except Exception as e:
-            raise ConnectionError(f"Error while checking token expiry: {str(e)}")
-
-    def __get_refresh_token(self) -> None:
-        try:
-            if not self.__is_token_expired():
-                return
-            res = requests.get(
-                config.AGENT_CONSOLE_URL + "/user/token/refresh",
-                params={"token": self.headers.get('refresh_token')},
-            )
-            res.raise_for_status()
-            data = json.loads(res.text)
-            if data.get("status") == "success":
-                self.headers['Authorization'] = data.get("token")
-                self.headers['refresh_token'] = data.get("refresh_token")
-            else:
-                raise ConnectionError(f"Error while refreshing token: {data}")
-        except Exception as e:
-            raise ConnectionError(f"Error while refreshing token: {str(e)}")
-
-    def connect(self, api_key: str = None) -> None:
-        try:
-            params = {"apikey": api_key}
-            try: 
-                response = requests.get(config.AGENT_CONSOLE_URL + "/user/token/request", params=params, stream=True)
-
-                response.raise_for_status()
-
-            except requests.exceptions.HTTPError as err:
-                print(f"Error while requesting token: {str(err)}")
-                
-            for line in response.iter_lines():
-                if line:
-                    json_obj = line.decode().strip()
-                    if json_obj.startswith('data: '):
-                        try:
-                            data = json.loads(json_obj[6:])  # Parse JSON directly from the sliced string
-                            self.__process_message(data)
-                        except json.JSONDecodeError as e:
-                            print(f"Error parsing JSON: {e}")
-            if self.headers.get('Authorization') != "":
-                try:
-                    res = self._exec(
-                        "POST",
-                        "/start-session",
-                        headers=self.headers,
-                    )
-                    if res.status_code != 200:
-                        raise requests.exceptions.HTTPError(
-                            f"Error while starting a new session in server status code: {res.status_code} message: {res.text}"
-                        )
-                    self.session_id = json.loads(res.text)["session_id"]
-                except Exception as err:
-                    raise ConnectionError(f"Error calling /start-session: {str(err)}")
-            else:
-                eprint("Error during API key authentication. Please ensure login approval on AGENT Console.")
-
-        except Exception as err:
-            raise ConnectionError(f"Error while creating client: {str(err)}")
-    
-    def __process_message(self, data: Dict[str, Any]) -> None:
-        approval_status = data.get('approval_status')
-        if approval_status == 'approved':
-            token = data.get('token')
-            if token:
-                self.headers['Authorization'] = data.get('token')
-                self.headers['refresh_token'] = data.get('refresh_token')
-                print("\033[92m" + "Request approved." + "\033[0m")
-            else:
-                print("Token not found in the approved message.")
-        elif approval_status == 'pending':
-            # print(json.dumps(data, indent=2))  # Pretty print the JSON message
-            print(f"Your request is pending approval. Please visit the following URL to approve the request: {data.get('approval_url', '')}")
-        elif approval_status == 'expired':
-            print("\033[91m Request Expired \033[0m")
-        elif approval_status == 'failed':
-            print(f"\033[91m {json.dumps(data, indent=2)} \033[0m")
-
-
-    def __get_output(self, message_id) -> None:
-        """
-        Retrieves the code execution output from the Antigranular server.
-        """
-        count = 1
-        return_value = None
-        while True:
-            if count > int(config.AG_EXEC_TIMEOUT):
-                print("Error : AG execution timeout.")
-                return_value = True
-                break
-            try:
-                res = self._exec(
-                    "GET",
-                    "/sessions/output",
-                    params={"session_id": self.session_id}
-                )
-            except Exception as err:
-                raise ConnectionError(
-                    f"Error during code execution on AG Server: {str(err)}"
-                )
-            if res.status_code != 200:
-                raise HTTPError(
-                    f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            kernel_messages = json.loads(res.text)["output_list"]
-            for message in kernel_messages:
-                if message.get("parent_header", {}).get("msg_id") == message_id:
-                    if message["msg_type"] == "status":
-                        if message["content"]["execution_state"] == "idle":
-                            return return_value
-                    elif message["msg_type"] == "stream":
-                        if message["content"]["name"] == "stdout":
-                            print(message["content"]["text"])
-                            return_value = True
-                        elif message["content"]["name"] == "stderr":
-                            print(message["content"]["text"])
-                            return_value = True
-
-                    elif message["msg_type"] == "error":
-                        tb_str = ""
-                        for tb in message["content"]["traceback"]:
-                            tb_str += tb
-
-                        print(tb_str)
-                        return_value = True
-                        return return_value
-            time.sleep(1)
-            count += 1
-
-        return return_value
-    
-    def __session_execute(self, code) -> None:
-        if not code:
-            raise ValueError("Code must be provided.")
-        try:
-            res = self._exec(
-                "POST",
-                "/sessions/execute",
-                headers=self.headers,
-                json={"session_id": self.session_id, "code": code},
-            )
-        except Exception as err:
-            raise ConnectionError(f"Error calling /sessions/execute: {str(err)}")
-        else:
-            if res.status_code != 200:
-                raise requests.exceptions.HTTPError(
-                    f"Error while executing the provided compute operation in the server status code: {res.status_code} message: {res.text}"
-                )
-            res_body_dict = json.loads(res.text)
-            return self.__get_output(res_body_dict.get('message_id'))
-
-    def interrupt_kernel(self) -> dict:
-        try:
-            res = self._exec(
-                "POST",
-                "/sessions/interrupt-kernel",
-                headers=self.headers,
-                json={"session_id": self.session_id},
-            )
-        except Exception as e:
-            raise ConnectionError(f"Error calling /terminate-session: {str(e)}")
-        else:
-            if res.status_code != 200:
-                raise requests.exceptions.HTTPError(
-                    f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            return json.loads(res.text)
-
-    def terminate_session(self) -> dict:
-        try:
-            res = self._exec(
-                "POST",
-                "/sessions/terminate-session",
-                headers=self.headers,
-                json={"session_id": self.session_id},
-            )
-        except Exception as e:
-            raise ConnectionError(f"Error calling /terminate-session: {str(e)}")
-        else:
-            if res.status_code != 200:
-                raise requests.exceptions.HTTPError(
-                    f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            return json.loads(res.text)
-
-    def active_count(self) -> dict:
-        """
-        Get the active count.
-        """
-        try:
-            res = self._exec("GET", "/sessions/active-count", headers=self.headers)
-        except Exception as e:
-            raise ConnectionError(f"Error calling /sessions/active-count: {str(e)}")
-        else:
-            if res.status_code != 200:
-                raise requests.exceptions.HTTPError(
-                    f"Error while fetching the active_count, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            return json.loads(res.text)
-
-    def privacy_odometer(self, lifetime=False) -> dict:
-        """
-        Get the privacy odometer.
-
-        Returns:
-            dict: The privacy odometer.
-
-        Raises:
-            ConnectionError: If there is an error while calling /privacy_odometer.
-            requests.exceptions.HTTPError: If there is an error while fetching the privacy odometer.
-        """
-        try:
-            res = self._exec(
-                "GET",
-                "/sessions/privacy_odometer",
-                params={"session_id": self.session_id, "show_only_session_budgets": not lifetime},
-                headers=self.headers,
-            )
-        except Exception as e:
-            raise ConnectionError(f"Error calling /privacy_odometer: {str(e)}")
-        else:
-            if res.status_code != 200:
-                raise requests.exceptions.HTTPError(
-                    f"Error while fetching the privacy odometer, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            return json.loads(res.text)
-
-    def __load(self, name, data_type: str, metadata: dict, categorical_metadata: dict, is_private: bool) -> None:
-        if data_type == "model":
-            code = f"{name} = load_model('{name}')"
-        if data_type == "dataframe" or data_type == "series":
-            code = f"{name} = load_dataframe('{name}', metadata={metadata}, categorical_metadata={categorical_metadata}, is_private={is_private}, data_type='{data_type}')"
-        if data_type == "dict" or data_type == "OrderedDict":
-            code = f"{name} = load_dict('{name}', data_type='{data_type}')"
-        try:
-            self.__session_execute(code)
-        except Exception as e:
-            raise ConnectionError(f"Error calling /sessions/execute: {str(e)}")
-    
-
-    def private_import(self, data=None, name: str = None, path=None, is_private=False, metadata={}, categorical_metadata={}) -> None:
-        """
-        Load a user provided model or dataset into the AG server.
-
-        Parameters:
-            name (str): The name to use for the model or dataset.
-            data (onnx.ModelProto, pd.DataFrame, dict, OrderedDict, pd.Series): The data to load. Defaults to None.
-            path (str, optional): The path to the model, the external data should be under the same directory of the model. Defaults to None.
-            is_private (bool, optional): Whether the data is private. Defaults to False.
-            metadata (dict, optional): The metadata for the dataset. Defaults to {}.
-            categorical_metadata (dict, optional): The categorical metadata for the dataset. Defaults to {}.
-        Returns:
-            None
-        """
-        if (name is None) or (not isinstance(name, str) and not name.isidentifier()):
-            raise ValueError("name must be a valid identifier")
-        if not (data is None or path is None):
-            raise ValueError("Both data and path cannot be provided, please provide only one of them")
-        if isinstance(data, pd.DataFrame):
-            res = self._exec(
-                "POST",
-                "/sessions/cache_data",
-                headers=self.headers,
-                json={"session_id": self.session_id, "data": base64.b64encode(data.to_csv(index=True).encode()).decode(), "name": name},
-            )
-            data_type = "dataframe"
-        elif isinstance(data, pd.Series):
-            res = self._exec(
-                "POST",
-                "/sessions/cache_data",
-                headers=self.headers,
-                json={"session_id": self.session_id, "data": base64.b64encode(data.to_csv(header=False).encode()).decode(), "name": name},
-            )
-            data_type = "series"
-        elif onnx_installed and isinstance(data, onnx.ModelProto):
-            try:
-                onnx.checker.check_model(data)
-                onnx_bytes_io = BytesIO()
-                onnx_bytes_io.seek(0)
-                onnx.save_model(data, onnx_bytes_io)
-            except Exception as e:
-                raise ValueError(f"Invalid ONNX model: {str(e)}")
-            res = self._exec(
-                "POST",
-                "/sessions/cache_model",
-                headers=self.headers,
-                json={"session_id": self.session_id, "name": name, "model": base64.b64encode(onnx_bytes_io.getvalue()).decode()},
-            )
-            data_type = "model"
-        elif isinstance(data, (dict, OrderedDict)):
-            res = self._exec(
-                "POST",
-                "/sessions/cache_data",
-                headers=self.headers,
-                json={"session_id": self.session_id, "data": base64.b64encode(json.dumps(data).encode()).decode(), "name": name},
-            )
-            data_type = "dict" if isinstance(data, dict) else "OrderedDict"
-        elif path:
-            if not onnx_installed:
-                raise ValueError("ONNX is not installed, please install ONNX to use this feature")
-            if not path.endswith(".onnx"):
-                raise ValueError("Invalid model file format, only .onnx files are supported")
-            try:
-                onnx_model = onnx.load(path)
-                onnx.checker.check_model(onnx_model)
-            except Exception as e:
-                raise ValueError(f"Invalid ONNX model: {str(e)}")
-            res = self._exec(
-                "POST",
-                "/sessions/cache_model",
-                headers=self.headers,
-                json={"session_id": self.session_id, "name": name, "model": base64.b64encode(open(path, "rb").read()).decode()},
-            )
-            data_type = "model"
-        else:
-            raise ValueError("Either a DataFrame, ONNX model, or path must be provided")
-        
-
-        if res.status_code != 200:
-            raise requests.exceptions.HTTPError(
-                print_request_id(f"Error: {res.text}", res)
-            )
-        else:
-            print(f"{data_type} cached to server, loading to kernel...")
-            self.__load(name, data_type, metadata, categorical_metadata, is_private)
-
-
-    # Use Oblv Client server to make HTTP requests
-    def _exec(self, method, endpoint, data="", json={}, params={}, headers={}, files=None):
-        """
-        Execute an HTTP request using the Oblv Client server.
-
-        Parameters:
-            method (str): The HTTP method.
-            endpoint (str): The endpoint URL.
-            data (Any, optional): The request data. Defaults to None.
-            json (Any, optional): The request JSON. Defaults to None.
-            params (dict, optional): The request parameters. Defaults to None.
-            headers (dict, optional): The request headers. Defaults to None.
-
-        Returns:
-            Response: The HTTP response.
-
-        Raises:
-            ValueError: If the method is not supported by the client.
-        """
-        if hasattr(self, 'session_id'):
-            self.__get_refresh_token()
-        url_endpoint = f"{self.oblv_ag.url}:{self.oblv_ag.port}{endpoint}"
-        # print(url_endpoint)
-        if method == "GET":
-            r = self.oblv_ag.get(
-                url_endpoint,
-                json=json,
-                params=params,
-                headers=headers,
-            )
-        elif method == "POST":
-            r = self.oblv_ag.post(
-                url_endpoint, json=json, params=params, headers=headers, files=files
-            )
-        elif method == "PUT":
-            r = self.oblv_ag.put(
-                url_endpoint, json=json, params=params, headers=headers
-            )
-        elif method == "DELETE":
-            r = self.oblv_ag.delete(
-                url_endpoint, json=json, params=params, headers=headers
-            )
-        else:
-            raise ValueError(f"{method} not supported by client")
-        return r
-    
+"""
+Module for AGClient class.
+
+AGClient class contians all the methods to interact with the AG server like creating a session, uploading results, etc.
+It also contains methods to get the budget, privacy odometer, etc.
+
+"""
+
+import requests
+import json
+from typing import Any, Dict, Union
+import base64
+
+from antigranular_enterprise.utils.error_print import eprint
+try:
+    import onnx
+    onnx_installed = True
+except ImportError:
+    onnx_installed = False
+from .magics.magics import AGMagic
+from .agent_client.agent_client import get_ag_client, AGClient
+from .config.config import config
+from .models.models import AGServerInfo
+import onnx
+import pandas as pd
+from io import BytesIO
+from .utils.print_request_id import print_request_id
+import time
+from collections import OrderedDict
+import jwt
+import time
+
+def login(
+        api_key: str,
+        profile: str = "default"
+):
+    """
+    Login to the AG server and get the client objects.
+    Returns:
+        AGClient: The AGClient object.
+
+    Raises:
+        ConnectionError: If there is an error while creating the client.
+    """
+    try:
+        return AGClient(
+            api_key,
+            profile
+        )
+    except Exception as err:
+        raise ConnectionError(f"Error while creating client: {str(err)}")
+
+def read_config(profile="default") -> None:
+    """
+    Reads the configuration from a given profile.
+
+    Args:
+        profile (str): The profile to read the configuration from.
+    """
+    config.read_config(profile=profile)
+
+def write_config(yaml_config, profile) -> None:
+    """
+    Writes the configuration to a given profile.
+
+    Args:
+        yaml_config (dict): The configuration to write.
+        profile (str): The profile to write the configuration to.
+    """
+    config.write_config(yaml_config, profile)
+
+def load_config(config_url=None, profile="default") -> None:
+    """
+    Load the configuration from the given URL.
+
+    Args:
+        config_url (str): The URL to load the configuration from.
+        profile (str): The profile to load the configuration to.
+    """
+    config.load_config(config_url, profile)
+
+class AGClient:
+    """
+    AGClient class to interact with the AG server for competitions as well as accessing datasets for functionalities like creating a session, uploading competition submissions, downloading metadata, etc.
+    """
+
+    oblv_ag: AGClient
+    session_id: str
+    user_name: str = ""
+
+    def __init__(
+        self,
+        api_key: str,
+        profile: str
+    ):
+        """
+        Initialize AGClient class and check for headers if Client.
+
+        Raises:
+            ConnectionError: If there is an error while connecting to the server.
+        """
+        config.load_config(profile=profile)
+        # Make client if headers are provided
+        self.oblv_ag = get_ag_client(
+        )
+        self.headers = {
+            "Content-type": "application/json",
+            "accept": "application/json",
+            "Authorization": "",
+            "refresh_token": ""
+        }
+
+        # Create an AG session
+        self.connect(api_key)
+        if hasattr(self, 'session_id'):
+            try:
+                res = AGMagic.load_ag_magic()
+            except Exception as ex:
+                print(
+                    "Error loading %%ag magic functions, you might not be able to use cell magics as intended: ",
+                    str(ex),
+                )
+            AGMagic.load_oblv_client(self.oblv_ag, self.session_id)
+
+    @classmethod
+    def _from_agent_client(cls, ag_client_secret):
+        """
+        Initialize AGClient class from Client.
+        """
+        return cls(ag_client_secret)
+
+    def __is_token_expired(self) -> bool:
+        try:
+            payload = jwt.decode(self.headers['Authorization'], options={"verify_signature": False})
+            current_time = time.time() + 10 # 10 seconds for network latency
+            return payload.get('exp', 0) < current_time
+        except Exception as e:
+            raise ConnectionError(f"Error while checking token expiry: {str(e)}")
+
+    def __get_refresh_token(self) -> None:
+        try:
+            if not self.__is_token_expired():
+                return
+            res = requests.get(
+                config.AGENT_CONSOLE_URL + "/user/token/refresh",
+                params={"token": self.headers.get('refresh_token')},
+            )
+            res.raise_for_status()
+            data = json.loads(res.text)
+            if data.get("status") == "success":
+                self.headers['Authorization'] = data.get("token")
+                self.headers['refresh_token'] = data.get("refresh_token")
+            else:
+                raise ConnectionError(f"Error while refreshing token: {data}")
+        except Exception as e:
+            raise ConnectionError(f"Error while refreshing token: {str(e)}")
+
+    def connect(self, api_key: str = None) -> None:
+        try:
+            params = {"apikey": api_key}
+            try: 
+                response = requests.get(config.AGENT_CONSOLE_URL + "/user/token/request", params=params, stream=True)
+
+                response.raise_for_status()
+
+            except requests.exceptions.HTTPError as err:
+                print(f"Error while requesting token: {str(err)}")
+                
+            for line in response.iter_lines():
+                if line:
+                    json_obj = line.decode().strip()
+                    if json_obj.startswith('data: '):
+                        try:
+                            data = json.loads(json_obj[6:])  # Parse JSON directly from the sliced string
+                            self.__process_message(data)
+                        except json.JSONDecodeError as e:
+                            print(f"Error parsing JSON: {e}")
+            if self.headers.get('Authorization') != "":
+                try:
+                    res = self._exec(
+                        "POST",
+                        "/start-session",
+                        headers=self.headers,
+                    )
+                    if res.status_code != 200:
+                        raise requests.exceptions.HTTPError(
+                            f"Error while starting a new session in server status code: {res.status_code} message: {res.text}"
+                        )
+                    self.session_id = json.loads(res.text)["session_id"]
+                except Exception as err:
+                    raise ConnectionError(f"Error calling /start-session: {str(err)}")
+            else:
+                eprint("Error during API key authentication. Please ensure login approval on AGENT Console.")
+
+        except Exception as err:
+            raise ConnectionError(f"Error while creating client: {str(err)}")
+    
+    def __process_message(self, data: Dict[str, Any]) -> None:
+        approval_status = data.get('approval_status')
+        if approval_status == 'approved':
+            token = data.get('token')
+            if token:
+                self.headers['Authorization'] = data.get('token')
+                self.headers['refresh_token'] = data.get('refresh_token')
+                print("\033[92m" + "Request approved." + "\033[0m")
+            else:
+                print("Token not found in the approved message.")
+        elif approval_status == 'pending':
+            # print(json.dumps(data, indent=2))  # Pretty print the JSON message
+            print(f"Your request is pending approval. Please visit the following URL to approve the request: {data.get('approval_url', '')}")
+        elif approval_status == 'expired':
+            print("\033[91m Request Expired \033[0m")
+        elif approval_status == 'failed':
+            print(f"\033[91m {json.dumps(data, indent=2)} \033[0m")
+
+
+    def __get_output(self, message_id) -> None:
+        """
+        Retrieves the code execution output from the Antigranular server.
+        """
+        count = 1
+        return_value = None
+        while True:
+            if count > int(config.AG_EXEC_TIMEOUT):
+                print("Error : AG execution timeout.")
+                return_value = True
+                break
+            try:
+                res = self._exec(
+                    "GET",
+                    "/sessions/output",
+                    params={"session_id": self.session_id}
+                )
+            except Exception as err:
+                raise ConnectionError(
+                    f"Error during code execution on AG Server: {str(err)}"
+                )
+            if res.status_code != 200:
+                raise HTTPError(
+                    f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            kernel_messages = json.loads(res.text)["output_list"]
+            for message in kernel_messages:
+                if message.get("parent_header", {}).get("msg_id") == message_id:
+                    if message["msg_type"] == "status":
+                        if message["content"]["execution_state"] == "idle":
+                            return return_value
+                    elif message["msg_type"] == "stream":
+                        if message["content"]["name"] == "stdout":
+                            print(message["content"]["text"])
+                            return_value = True
+                        elif message["content"]["name"] == "stderr":
+                            print(message["content"]["text"])
+                            return_value = True
+
+                    elif message["msg_type"] == "error":
+                        tb_str = ""
+                        for tb in message["content"]["traceback"]:
+                            tb_str += tb
+
+                        print(tb_str)
+                        return_value = True
+                        return return_value
+            time.sleep(1)
+            count += 1
+
+        return return_value
+    
+    def __session_execute(self, code) -> None:
+        if not code:
+            raise ValueError("Code must be provided.")
+        try:
+            res = self._exec(
+                "POST",
+                "/sessions/execute",
+                headers=self.headers,
+                json={"session_id": self.session_id, "code": code},
+            )
+        except Exception as err:
+            raise ConnectionError(f"Error calling /sessions/execute: {str(err)}")
+        else:
+            if res.status_code != 200:
+                raise requests.exceptions.HTTPError(
+                    f"Error while executing the provided compute operation in the server status code: {res.status_code} message: {res.text}"
+                )
+            res_body_dict = json.loads(res.text)
+            return self.__get_output(res_body_dict.get('message_id'))
+
+    def interrupt_kernel(self) -> dict:
+        try:
+            res = self._exec(
+                "POST",
+                "/sessions/interrupt-kernel",
+                headers=self.headers,
+                json={"session_id": self.session_id},
+            )
+        except Exception as e:
+            raise ConnectionError(f"Error calling /terminate-session: {str(e)}")
+        else:
+            if res.status_code != 200:
+                raise requests.exceptions.HTTPError(
+                    f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            return json.loads(res.text)
+
+    def terminate_session(self) -> dict:
+        try:
+            res = self._exec(
+                "POST",
+                "/sessions/terminate-session",
+                headers=self.headers,
+                json={"session_id": self.session_id},
+            )
+        except Exception as e:
+            raise ConnectionError(f"Error calling /terminate-session: {str(e)}")
+        else:
+            if res.status_code != 200:
+                raise requests.exceptions.HTTPError(
+                    f"Error while fetching the terminate-session, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            return json.loads(res.text)
+
+    def active_count(self) -> dict:
+        """
+        Get the active count.
+        """
+        try:
+            res = self._exec("GET", "/sessions/active-count", headers=self.headers)
+        except Exception as e:
+            raise ConnectionError(f"Error calling /sessions/active-count: {str(e)}")
+        else:
+            if res.status_code != 200:
+                raise requests.exceptions.HTTPError(
+                    f"Error while fetching the active_count, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            return json.loads(res.text)
+
+    def privacy_odometer(self, lifetime=False) -> dict:
+        """
+        Get the privacy odometer.
+
+        Returns:
+            dict: The privacy odometer.
+
+        Raises:
+            ConnectionError: If there is an error while calling /privacy_odometer.
+            requests.exceptions.HTTPError: If there is an error while fetching the privacy odometer.
+        """
+        try:
+            res = self._exec(
+                "GET",
+                "/sessions/privacy_odometer",
+                params={"session_id": self.session_id, "show_only_session_budgets": not lifetime},
+                headers=self.headers,
+            )
+        except Exception as e:
+            raise ConnectionError(f"Error calling /privacy_odometer: {str(e)}")
+        else:
+            if res.status_code != 200:
+                raise requests.exceptions.HTTPError(
+                    f"Error while fetching the privacy odometer, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            return json.loads(res.text)
+
+    def __load(self, name, data_type: str, metadata: dict, categorical_metadata: dict, is_private: bool) -> None:
+        if data_type == "model":
+            code = f"{name} = load_model('{name}')"
+        if data_type == "dataframe" or data_type == "series":
+            code = f"{name} = load_dataframe('{name}', metadata={metadata}, categorical_metadata={categorical_metadata}, is_private={is_private}, data_type='{data_type}')"
+        if data_type == "dict" or data_type == "OrderedDict":
+            code = f"{name} = load_dict('{name}', data_type='{data_type}')"
+        try:
+            self.__session_execute(code)
+        except Exception as e:
+            raise ConnectionError(f"Error calling /sessions/execute: {str(e)}")
+    
+
+    def private_import(self, data=None, name: str = None, path=None, is_private=False, metadata={}, categorical_metadata={}) -> None:
+        """
+        Load a user provided model or dataset into the AG server.
+
+        Parameters:
+            name (str): The name to use for the model or dataset.
+            data (onnx.ModelProto, pd.DataFrame, dict, OrderedDict, pd.Series): The data to load. Defaults to None.
+            path (str, optional): The path to the model, the external data should be under the same directory of the model. Defaults to None.
+            is_private (bool, optional): Whether the data is private. Defaults to False.
+            metadata (dict, optional): The metadata for the dataset. Defaults to {}.
+            categorical_metadata (dict, optional): The categorical metadata for the dataset. Defaults to {}.
+        Returns:
+            None
+        """
+        if (name is None) or (not isinstance(name, str) and not name.isidentifier()):
+            raise ValueError("name must be a valid identifier")
+        if not (data is None or path is None):
+            raise ValueError("Both data and path cannot be provided, please provide only one of them")
+        if isinstance(data, pd.DataFrame):
+            res = self._exec(
+                "POST",
+                "/sessions/cache_data",
+                headers=self.headers,
+                json={"session_id": self.session_id, "data": base64.b64encode(data.to_csv(index=True).encode()).decode(), "name": name},
+            )
+            data_type = "dataframe"
+        elif isinstance(data, pd.Series):
+            res = self._exec(
+                "POST",
+                "/sessions/cache_data",
+                headers=self.headers,
+                json={"session_id": self.session_id, "data": base64.b64encode(data.to_csv(header=False).encode()).decode(), "name": name},
+            )
+            data_type = "series"
+        elif onnx_installed and isinstance(data, onnx.ModelProto):
+            try:
+                onnx.checker.check_model(data)
+                onnx_bytes_io = BytesIO()
+                onnx_bytes_io.seek(0)
+                onnx.save_model(data, onnx_bytes_io)
+            except Exception as e:
+                raise ValueError(f"Invalid ONNX model: {str(e)}")
+            res = self._exec(
+                "POST",
+                "/sessions/cache_model",
+                headers=self.headers,
+                json={"session_id": self.session_id, "name": name, "model": base64.b64encode(onnx_bytes_io.getvalue()).decode()},
+            )
+            data_type = "model"
+        elif isinstance(data, (dict, OrderedDict)):
+            res = self._exec(
+                "POST",
+                "/sessions/cache_data",
+                headers=self.headers,
+                json={"session_id": self.session_id, "data": base64.b64encode(json.dumps(data).encode()).decode(), "name": name},
+            )
+            data_type = "dict" if isinstance(data, dict) else "OrderedDict"
+        elif path:
+            if not onnx_installed:
+                raise ValueError("ONNX is not installed, please install ONNX to use this feature")
+            if not path.endswith(".onnx"):
+                raise ValueError("Invalid model file format, only .onnx files are supported")
+            try:
+                onnx_model = onnx.load(path)
+                onnx.checker.check_model(onnx_model)
+            except Exception as e:
+                raise ValueError(f"Invalid ONNX model: {str(e)}")
+            res = self._exec(
+                "POST",
+                "/sessions/cache_model",
+                headers=self.headers,
+                json={"session_id": self.session_id, "name": name, "model": base64.b64encode(open(path, "rb").read()).decode()},
+            )
+            data_type = "model"
+        else:
+            raise ValueError("Either a DataFrame, ONNX model, or path must be provided")
+        
+
+        if res.status_code != 200:
+            raise requests.exceptions.HTTPError(
+                print_request_id(f"Error: {res.text}", res)
+            )
+        else:
+            print(f"{data_type} cached to server, loading to kernel...")
+            self.__load(name, data_type, metadata, categorical_metadata, is_private)
+
+
+    # Use Oblv Client server to make HTTP requests
+    def _exec(self, method, endpoint, data="", json={}, params={}, headers={}, files=None):
+        """
+        Execute an HTTP request using the Oblv Client server.
+
+        Parameters:
+            method (str): The HTTP method.
+            endpoint (str): The endpoint URL.
+            data (Any, optional): The request data. Defaults to None.
+            json (Any, optional): The request JSON. Defaults to None.
+            params (dict, optional): The request parameters. Defaults to None.
+            headers (dict, optional): The request headers. Defaults to None.
+
+        Returns:
+            Response: The HTTP response.
+
+        Raises:
+            ValueError: If the method is not supported by the client.
+        """
+        if hasattr(self, 'session_id'):
+            self.__get_refresh_token()
+        url_endpoint = f"{self.oblv_ag.url}:{self.oblv_ag.port}{endpoint}"
+        # print(url_endpoint)
+        if method == "GET":
+            r = self.oblv_ag.get(
+                url_endpoint,
+                json=json,
+                params=params,
+                headers=headers,
+            )
+        elif method == "POST":
+            r = self.oblv_ag.post(
+                url_endpoint, json=json, params=params, headers=headers, files=files
+            )
+        elif method == "PUT":
+            r = self.oblv_ag.put(
+                url_endpoint, json=json, params=params, headers=headers
+            )
+        elif method == "DELETE":
+            r = self.oblv_ag.delete(
+                url_endpoint, json=json, params=params, headers=headers
+            )
+        else:
+            raise ValueError(f"{method} not supported by client")
+        return r
+
```

### Comparing `antigranular_enterprise-0.0.8/antigranular_enterprise/magics/errors.py` & `antigranular_enterprise-0.0.9/antigranular_enterprise/magics/errors.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from IPython import get_ipython
-class AGRuntimeError(Exception):
-    def __init__(self, etype="Error", evalue="AG Runtime Error", msg=None):
-        self.error_data = f"{etype}:\n{evalue}"
-        self.tb = evalue
-
-    def __str__(self):
-        error_msg = f"{self.error_data}"
-        if self.tb:
-            error_msg += f"\nServer Traceback:\n{self.tb}"
-        return error_msg
-
-
-class AGTimeOutError(Exception):
-    def __init__(self, etype="Error", evalue="AG TimeOut Error", msg=None):
-        self.error_data = f"{etype}:\n{evalue}"
-        self.tb = "Client TimeOut while waiting for server output"
-
-    def __str__(self):
-        error_msg = f"{self.error_data}"
-        if self.tb:
-            error_msg += f"\nServer Traceback:\n{self.tb}"
-        return error_msg
-
-
-def custom_exc(shell, etype, evalue, tb, tb_offset=None):
-    return
-
-# Use our custom exception handler
-get_ipython().set_custom_exc((AGRuntimeError,), custom_exc)
+from IPython import get_ipython
+class AGRuntimeError(Exception):
+    def __init__(self, etype="Error", evalue="AG Runtime Error", msg=None):
+        self.error_data = f"{etype}:\n{evalue}"
+        self.tb = evalue
+
+    def __str__(self):
+        error_msg = f"{self.error_data}"
+        if self.tb:
+            error_msg += f"\nServer Traceback:\n{self.tb}"
+        return error_msg
+
+
+class AGTimeOutError(Exception):
+    def __init__(self, etype="Error", evalue="AG TimeOut Error", msg=None):
+        self.error_data = f"{etype}:\n{evalue}"
+        self.tb = "Client TimeOut while waiting for server output"
+
+    def __str__(self):
+        error_msg = f"{self.error_data}"
+        if self.tb:
+            error_msg += f"\nServer Traceback:\n{self.tb}"
+        return error_msg
+
+
+def custom_exc(shell, etype, evalue, tb, tb_offset=None):
+    return
+
+# Use our custom exception handler
+get_ipython().set_custom_exc((AGRuntimeError,), custom_exc)
```

### Comparing `antigranular_enterprise-0.0.8/antigranular_enterprise/magics/magics.py` & `antigranular_enterprise-0.0.9/antigranular_enterprise/magics/magics.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-from IPython.display import display, HTML
-from IPython.core.magic import (
-    Magics,
-    magics_class,
-    line_cell_magic,
-)
-from IPython import get_ipython
-
-import json
-import base64
-import pickle
-import time
-from requests import HTTPError
-
-from ..agent_client.agent_client import AGClient
-from ..utils.error_print import eprint
-from .errors import AGRuntimeError
-from ..config.config import config
-
-@magics_class
-class AGMagic(Magics):
-    """
-    Provides %%ag cell magic and private python code execution on Antigranular server
-    """
-
-    session_id: str
-    # user_name: str
-    ag_server: AGClient
-
-    @classmethod
-    def load_oblv_client(cls, ag_server, session_id):
-        cls.ag_server = ag_server
-        cls.session_id = session_id
-        # cls.user_name = user_name
-
-    @line_cell_magic
-    def ag(self, line, cell=None):
-        """
-        Executes the provided code on the Antigranular server.
-
-        Parameters:
-            line (str): The code in a single line.
-            cell (str): The code in a cell format.
-
-        Returns:
-            None
-        """
-        if cell is None:
-            print("Please call ag as a cell magic using '%%ag'")
-            return
-        else:
-            try:
-                self.execute(cell)
-            # except any exception
-            except KeyboardInterrupt:
-                res = self.interrupt_kernel()
-                if res["status"] == "ok":
-                    # return interrupt message
-                    eprint("Kernel interrupted successfully")
-                else:
-                    eprint("Error while interrupting kernel")
-                    eprint(res)
-
-    def execute(self, code: str):
-        """
-        Executes the code on the Antigranular server.
-
-        Parameters:
-            code (str): The code to be executed.
-
-        Returns:
-            None
-        """
-        try:
-            res = self.ag_server.post(
-                f"{self.ag_server.url}:{self.ag_server.port}/sessions/execute",
-                json={"session_id": self.session_id, "code": code},
-            )
-        except Exception as err:
-            raise ConnectionError(f"Error calling /execute: {str(err)}")
-        else:
-            if res.status_code != 200:
-                raise HTTPError(
-                    f"Error while requesting AG server to execute the code, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            res_body_dict = json.loads(res.text)
-            self.get_output(res_body_dict.get('message_id'))
-
-    def interrupt_kernel(self) -> dict:
-        try:
-            res = self.ag_server.post(
-                f"{self.ag_server.url}:{self.ag_server.port}/sessions/interrupt-kernel",
-                json={"session_id": self.session_id},
-            )
-        except Exception as err:
-            raise ConnectionError(
-                f"Error calling /sessions/interrupt-kernel: {str(err)}"
-            )
-        else:
-            if res.status_code != 200:
-                raise HTTPError(
-                    f"Error while requesting AG server to interrupt the kernel, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            return json.loads(res.text)
-
-    def get_output(self, message_id):
-        """
-        Retrieves the code execution output from the Antigranular server.
-        """
-        count = 1
-
-        while True:
-            if count > int(config.AG_EXEC_TIMEOUT):
-                eprint("Error : AG execution timeout.")
-                break
-            try:
-                res = self.ag_server.get(
-                    f"{self.ag_server.url}:{self.ag_server.port}/sessions/output",
-                    params={"session_id": self.session_id},
-                )
-            except Exception as err:
-                raise ConnectionError(
-                    f"Error during code execution on AG Server: {str(err)}"
-                )
-            if res.status_code != 200:
-                raise HTTPError(
-                    f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}"
-                )
-            kernel_messages = json.loads(res.text)["output_list"]
-            for message in kernel_messages:
-                if message.get("parent_header", {}).get("msg_id") == message_id:
-                    if message["msg_type"] == "status":
-                        if message["content"]["execution_state"] == "idle":
-                            return
-                    elif message["msg_type"] == "stream":
-                        if message["content"]["name"] == "stdout":
-                            print("Output:", message["content"]["text"])
-                        elif message["content"]["name"] == "stderr":
-                            eprint(message["content"]["text"])
-
-                    elif message["msg_type"] == "error":
-                        tb_str = ""
-                        for tb in message["content"]["traceback"]:
-                            tb_str += tb
-
-                        print(tb_str)
-                        raise AGRuntimeError(
-                            etype=str(message["content"]["evalue"]),
-                            evalue="RuntimeError",
-                            msg=tb_str,
-                        )
-
-                    elif message["msg_type"] == "ag_export_value":
-                        try:
-                            user_ns = get_ipython().user_ns
-                            data = message["content"]
-                            for name, value in data.items():
-                                user_ns[name] = pickle.loads(base64.b64decode(value))
-                                print(
-                                    "Setting up exported variable in local environment:",
-                                    name,
-                                )
-
-                        except Exception as err:
-                            raise ValueError(
-                                f"Error while parsing export values message: {str(err)}"
-                            )
-            time.sleep(1)
-            count += 1
-
-    @staticmethod
-    def load_ag_magic():
-        """
-        Loads the AGMagic class as a magic in the IPython session.
-        """
-        ipython = get_ipython()
-        if ipython is None:
-            raise RuntimeError(
-                "This function can only be called from an IPython session"
-            )
-        ipython.register_magics(AGMagic)
-        print(
-            "Cell magic '%%ag' registered successfully, use `%%ag` in a notebook cell to execute your python code on Antigranular private python server"
-        )
+from IPython.display import display, HTML
+from IPython.core.magic import (
+    Magics,
+    magics_class,
+    line_cell_magic,
+)
+from IPython import get_ipython
+
+import json
+import base64
+import pickle
+import time
+from requests import HTTPError
+
+from ..agent_client.agent_client import AGClient
+from ..utils.error_print import eprint
+from .errors import AGRuntimeError
+from ..config.config import config
+
+@magics_class
+class AGMagic(Magics):
+    """
+    Provides %%ag cell magic and private python code execution on Antigranular server
+    """
+
+    session_id: str
+    # user_name: str
+    ag_server: AGClient
+
+    @classmethod
+    def load_oblv_client(cls, ag_server, session_id):
+        cls.ag_server = ag_server
+        cls.session_id = session_id
+        # cls.user_name = user_name
+
+    @line_cell_magic
+    def ag(self, line, cell=None):
+        """
+        Executes the provided code on the Antigranular server.
+
+        Parameters:
+            line (str): The code in a single line.
+            cell (str): The code in a cell format.
+
+        Returns:
+            None
+        """
+        if cell is None:
+            print("Please call ag as a cell magic using '%%ag'")
+            return
+        else:
+            try:
+                self.execute(cell)
+            # except any exception
+            except KeyboardInterrupt:
+                res = self.interrupt_kernel()
+                if res["status"] == "ok":
+                    # return interrupt message
+                    eprint("Kernel interrupted successfully")
+                else:
+                    eprint("Error while interrupting kernel")
+                    eprint(res)
+
+    def execute(self, code: str):
+        """
+        Executes the code on the Antigranular server.
+
+        Parameters:
+            code (str): The code to be executed.
+
+        Returns:
+            None
+        """
+        try:
+            res = self.ag_server.post(
+                f"{self.ag_server.url}:{self.ag_server.port}/sessions/execute",
+                json={"session_id": self.session_id, "code": code},
+            )
+        except Exception as err:
+            raise ConnectionError(f"Error calling /execute: {str(err)}")
+        else:
+            if res.status_code != 200:
+                raise HTTPError(
+                    f"Error while requesting AG server to execute the code, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            res_body_dict = json.loads(res.text)
+            self.get_output(res_body_dict.get('message_id'))
+
+    def interrupt_kernel(self) -> dict:
+        try:
+            res = self.ag_server.post(
+                f"{self.ag_server.url}:{self.ag_server.port}/sessions/interrupt-kernel",
+                json={"session_id": self.session_id},
+            )
+        except Exception as err:
+            raise ConnectionError(
+                f"Error calling /sessions/interrupt-kernel: {str(err)}"
+            )
+        else:
+            if res.status_code != 200:
+                raise HTTPError(
+                    f"Error while requesting AG server to interrupt the kernel, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            return json.loads(res.text)
+
+    def get_output(self, message_id):
+        """
+        Retrieves the code execution output from the Antigranular server.
+        """
+        count = 1
+
+        while True:
+            if count > int(config.AG_EXEC_TIMEOUT):
+                eprint("Error : AG execution timeout.")
+                break
+            try:
+                res = self.ag_server.get(
+                    f"{self.ag_server.url}:{self.ag_server.port}/sessions/output",
+                    params={"session_id": self.session_id},
+                )
+            except Exception as err:
+                raise ConnectionError(
+                    f"Error during code execution on AG Server: {str(err)}"
+                )
+            if res.status_code != 200:
+                raise HTTPError(
+                    f"Error while requesting AG server for output, HTTP status code: {res.status_code}, message: {res.text}"
+                )
+            kernel_messages = json.loads(res.text)["output_list"]
+            for message in kernel_messages:
+                if message.get("parent_header", {}).get("msg_id") == message_id:
+                    if message["msg_type"] == "status":
+                        if message["content"]["execution_state"] == "idle":
+                            return
+                    elif message["msg_type"] == "stream":
+                        if message["content"]["name"] == "stdout":
+                            print("Output:", message["content"]["text"])
+                        elif message["content"]["name"] == "stderr":
+                            eprint(message["content"]["text"])
+
+                    elif message["msg_type"] == "error":
+                        tb_str = ""
+                        for tb in message["content"]["traceback"]:
+                            tb_str += tb
+
+                        print(tb_str)
+                        raise AGRuntimeError(
+                            etype=str(message["content"]["evalue"]),
+                            evalue="RuntimeError",
+                            msg=tb_str,
+                        )
+
+                    elif message["msg_type"] == "ag_export_value":
+                        try:
+                            user_ns = get_ipython().user_ns
+                            data = message["content"]
+                            for name, value in data.items():
+                                user_ns[name] = pickle.loads(base64.b64decode(value))
+                                print(
+                                    "Setting up exported variable in local environment:",
+                                    name,
+                                )
+
+                        except Exception as err:
+                            raise ValueError(
+                                f"Error while parsing export values message: {str(err)}"
+                            )
+            time.sleep(1)
+            count += 1
+
+    @staticmethod
+    def load_ag_magic():
+        """
+        Loads the AGMagic class as a magic in the IPython session.
+        """
+        ipython = get_ipython()
+        if ipython is None:
+            raise RuntimeError(
+                "This function can only be called from an IPython session"
+            )
+        ipython.register_magics(AGMagic)
+        print(
+            "Cell magic '%%ag' registered successfully, use `%%ag` in a notebook cell to execute your python code on Antigranular private python server"
+        )
```

### Comparing `antigranular_enterprise-0.0.8/pyproject.toml` & `antigranular_enterprise-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-[tool.poetry]
-name = "antigranular_enterprise"
-version = "0.0.8"
-description = "Antigranular Enterprise is a robust, scalable version of the Antigranular platform. It combines the power of differential privacy, providing a secure environment for handling and unlocking the full potential of unseen data. With enhanced features and dedicated support, Antigranular Enterprise is the ideal solution for businesses seeking to leverage the power of data privacy and security."
-authors = ["Oblivious Software Pvt. Ltd. <support@oblivious.com>"]
-readme = "README.md"
-packages = [{include = "antigranular_enterprise"}]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-ipython = "^7.34.0"
-requests = "^2.31.0"
-pydantic = "^1.10.7"
-numpy = [
-    { version = "^1.26.0", markers = "python_version >= '3.12' and python_version < '4.0'" },
-    { version = "^1.19.0", markers = "python_version >= '3.8' and python_version < '3.12'" }
-]
-pandas = [
-    { version = "^2.1.4", markers = "python_version >= '3.12' and python_version <= '4.0'" },
-    { version = "^1.5.3", markers = "python_version >= '3.8' and python_version < '3.12'" }
-]
-onnx = "^1.16.0"
-pyJWT = "^2.8.0"
-PyYAML = "^6.0.1"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-nbclient = "^0.8.0"
-nbformat = "^5.9.1"
-
-[build-system]
-requires = ["poetry-core"]
+[tool.poetry]
+name = "antigranular_enterprise"
+version = "0.0.9"
+description = "Antigranular Enterprise is a robust, scalable version of the Antigranular platform. It combines the power of differential privacy, providing a secure environment for handling and unlocking the full potential of unseen data. With enhanced features and dedicated support, Antigranular Enterprise is the ideal solution for businesses seeking to leverage the power of data privacy and security."
+authors = ["Oblivious Software Pvt. Ltd. <support@oblivious.com>"]
+readme = "README.md"
+packages = [{include = "antigranular_enterprise"}]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+ipython = "^7.34.0"
+requests = "^2.31.0"
+pydantic = "^1.10.7"
+numpy = [
+    { version = "^1.26.0", markers = "python_version >= '3.12' and python_version < '4.0'" },
+    { version = "^1.19.0", markers = "python_version >= '3.8' and python_version < '3.12'" }
+]
+pandas = [
+    { version = "^2.1.4", markers = "python_version >= '3.12' and python_version <= '4.0'" },
+    { version = "^1.5.3", markers = "python_version >= '3.8' and python_version < '3.12'" }
+]
+onnx = "^1.16.0"
+pyJWT = "^2.8.0"
+PyYAML = "^6.0.1"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+nbclient = "^0.8.0"
+nbformat = "^5.9.1"
+
+[build-system]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `antigranular_enterprise-0.0.8/PKG-INFO` & `antigranular_enterprise-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: antigranular-enterprise
-Version: 0.0.8
+Name: antigranular_enterprise
+Version: 0.0.9
 Summary: Antigranular Enterprise is a robust, scalable version of the Antigranular platform. It combines the power of differential privacy, providing a secure environment for handling and unlocking the full potential of unseen data. With enhanced features and dedicated support, Antigranular Enterprise is the ideal solution for businesses seeking to leverage the power of data privacy and security.
 Author: Oblivious Software Pvt. Ltd.
 Author-email: support@oblivious.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: ipython (>=7.34.0,<8.0.0)
 Requires-Dist: numpy (>=1.19.0,<2.0.0) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: numpy (>=1.26.0,<2.0.0) ; python_version >= "3.12" and python_version < "4.0"
 Requires-Dist: onnx (>=1.16.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: pandas (>=2.1.4,<3.0.0) ; python_version >= "3.12" and python_version <= "4.0"
```

