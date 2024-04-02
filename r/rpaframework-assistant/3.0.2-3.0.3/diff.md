# Comparing `tmp/rpaframework_assistant-3.0.2.tar.gz` & `tmp/rpaframework_assistant-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_assistant-3.0.2.tar", max compression
+gzip compressed data, was "rpaframework_assistant-3.0.3.tar", max compression
```

## Comparing `rpaframework_assistant-3.0.2.tar` & `rpaframework_assistant-3.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-02-08 22:30:10.093540 rpaframework_assistant-3.0.2/LICENSE
--rw-r--r--   0        0        0      288 2023-02-08 22:30:10.093718 rpaframework_assistant-3.0.2/README.rst
--rw-r--r--   0        0        0     2335 2023-11-01 16:11:41.076800 rpaframework_assistant-3.0.2/pyproject.toml
--rw-r--r--   0        0        0       94 2023-03-14 14:16:25.880080 rpaframework_assistant-3.0.2/src/RPA/Assistant/__init__.py
--rw-r--r--   0        0        0     3387 2023-05-31 09:03:32.486581 rpaframework_assistant-3.0.2/src/RPA/Assistant/background_flet.py
--rw-r--r--   0        0        0     5168 2023-08-23 15:36:47.458053 rpaframework_assistant-3.0.2/src/RPA/Assistant/callback_runner.py
--rw-r--r--   0        0        0    11972 2023-10-31 12:15:36.257684 rpaframework_assistant-3.0.2/src/RPA/Assistant/flet_client.py
--rw-r--r--   0        0        0    72899 2023-11-01 16:11:41.077375 rpaframework_assistant-3.0.2/src/RPA/Assistant/library.py
--rw-r--r--   0        0        0     1530 2023-03-14 14:16:25.880895 rpaframework_assistant-3.0.2/src/RPA/Assistant/types.py
--rw-r--r--   0        0        0     3646 2023-03-14 14:16:25.881009 rpaframework_assistant-3.0.2/src/RPA/Assistant/utils.py
--rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 rpaframework_assistant-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.211231 rpaframework_assistant-3.0.3/LICENSE
+-rw-r--r--   0        0        0     2412 2024-04-02 12:28:54.963905 rpaframework_assistant-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-12-05 08:21:31.212234 rpaframework_assistant-3.0.3/README.rst
+-rw-r--r--   0        0        0    86080 2024-04-02 12:30:04.841860 rpaframework_assistant-3.0.3/RPA_Assistant.libspec
+-rw-r--r--   0        0        0       96 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/__init__.py
+-rw-r--r--   0        0        0     3498 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/background_flet.py
+-rw-r--r--   0        0        0     5304 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/callback_runner.py
+-rw-r--r--   0        0        0    12305 2023-12-05 08:21:31.214237 rpaframework_assistant-3.0.3/src/RPA/Assistant/flet_client.py
+-rw-r--r--   0        0        0    74890 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.3/src/RPA/Assistant/library.py
+-rw-r--r--   0        0        0     1597 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.3/src/RPA/Assistant/types.py
+-rw-r--r--   0        0        0     3765 2023-12-05 08:21:31.215236 rpaframework_assistant-3.0.3/src/RPA/Assistant/utils.py
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 rpaframework_assistant-3.0.3/PKG-INFO
```

### Comparing `rpaframework_assistant-3.0.2/LICENSE` & `rpaframework_assistant-3.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
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
-   Copyright 2020 Robocorp Technologies, Inc.
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
+
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
+   Copyright 2020 Robocorp Technologies, Inc.
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

### Comparing `rpaframework_assistant-3.0.2/pyproject.toml` & `rpaframework_assistant-3.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-[tool.poetry]
-name = "rpaframework-assistant"
-version = "3.0.2"
-description = "Interactive UI library for RPA Framework"
-authors = ["RPA Framework <rpafw@robocorp.com>"]
-license = "Apache-2.0"
-readme = "README.rst"
-
-homepage = "https://rpaframework.org/"
-documentation = "https://rpaframework.org/"
-repository = "https://github.com/robocorp/rpaframework"
-
-keywords = ["robotframework", "rpa", "automation", "dialogs", "assistant"]
-classifiers = [
-	"License :: OSI Approved :: Apache Software License",
-	"Development Status :: 5 - Production/Stable",
-	"Operating System :: OS Independent",
-	"Intended Audience :: Developers",
-	"Topic :: Software Development :: Libraries :: Python Modules",
-	"Topic :: Software Development :: Libraries",
-	"Framework :: Robot Framework :: Library",
-	"Framework :: Robot Framework",
-	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.9",
-	"Programming Language :: Python :: 3.10",
-]
-
-include = ["*.libspec"]
-
-packages = [{ include = "RPA", from = "src" }]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
-# Flet needs `packaging>=23`. Earlier rpaframework-core versions don't allow
-# installing it. This make resolution errors simpler and faster.
-rpaframework-core = "^11.0.0"
-flet="0.4.2"
-# We only need the Literal type on python 3.7 from the module, but it has to be
-# installed on all pythons so the imports work
-typing-extensions = { version = "^4.4.0" }
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-flake8 = "^3.7.9"
-pylint = "^2.4.4, <2.13"
-pytest = "^7.2.0"
-mock = "^5.0.0"
-pytest-cov = "^4.0.0"
-invoke = "^2.2.0"
-toml = "^0.10.2"
-robotframework-tidy = "^3.3.3"
-robotframework-docgen = "^0.16.0"
-colorama = "^0.4.5"
-keyring = "^24.2.0"
-PyYAML = ">=5.4.1,<7.0.0"
-importlib-metadata = "^4.13.0"
-flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.7"
-
-[tool.black]
-target-version = ["py38", "py39", "py310"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-addopts = "-v --cov=src --cov-report term-missing --cov-branch"
-testpaths = ["tests"]
-
-filterwarnings = [
-  # Ignore `pkg_resources.declare_namespace` that gets raised by dependencies
-  # when running pytest
-  "ignore:.*pkg_resources\\.declare_namespace.*:DeprecationWarning",
-]
+[tool.poetry]
+name = "rpaframework-assistant"
+version = "3.0.3"
+description = "Interactive UI library for RPA Framework"
+authors = ["RPA Framework <rpafw@robocorp.com>"]
+license = "Apache-2.0"
+readme = "README.rst"
+
+homepage = "https://rpaframework.org/"
+documentation = "https://rpaframework.org/"
+repository = "https://github.com/robocorp/rpaframework"
+
+keywords = ["robotframework", "rpa", "automation", "dialogs", "assistant"]
+classifiers = [
+	"License :: OSI Approved :: Apache Software License",
+	"Development Status :: 5 - Production/Stable",
+	"Operating System :: OS Independent",
+	"Intended Audience :: Developers",
+	"Topic :: Software Development :: Libraries :: Python Modules",
+	"Topic :: Software Development :: Libraries",
+	"Framework :: Robot Framework :: Library",
+	"Framework :: Robot Framework",
+	"Programming Language :: Python :: 3.8",
+	"Programming Language :: Python :: 3.9",
+	"Programming Language :: Python :: 3.10",
+]
+
+include = ["*.libspec"]
+
+packages = [{ include = "RPA", from = "src" }]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
+# Flet needs `packaging>=23`. Earlier rpaframework-core versions don't allow
+# installing it. This make resolution errors simpler and faster.
+rpaframework-core = "^11.3.1"
+flet="0.4.2"
+# We only need the Literal type on python 3.7 from the module, but it has to be
+# installed on all pythons so the imports work
+typing-extensions = { version = "^4.4.0" }
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.3.0"
+flake8 = "^3.7.9"
+pylint = "^2.4.4, <2.13"
+pytest = "^7.2.0"
+mock = "^5.0.0"
+pytest-cov = "^4.0.0"
+invoke = "^2.2.0"
+toml = "^0.10.2"
+robotframework-tidy = "^3.3.3"
+robotframework-docgen = "^0.16.0"
+colorama = "^0.4.5"
+keyring = "^24.2.0"
+PyYAML = ">=5.4.1,<7.0.0"
+importlib-metadata = "^4.13.0"
+flake8-docstrings = "^1.6.0"
+flake8-rst-docstrings = "^0.2.7"
+
+[tool.black]
+target-version = ["py38", "py39", "py310"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+addopts = "-v --cov=src --cov-report term-missing --cov-branch"
+testpaths = ["tests"]
+
+filterwarnings = [
+  # Ignore `pkg_resources.declare_namespace` that gets raised by dependencies
+  # when running pytest
+  "ignore:.*pkg_resources\\.declare_namespace.*:DeprecationWarning",
+]
```

### Comparing `rpaframework_assistant-3.0.2/src/RPA/Assistant/background_flet.py` & `rpaframework_assistant-3.0.3/src/RPA/Assistant/background_flet.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import atexit
-from logging import getLogger
-from subprocess import Popen
-from typing import Optional, Tuple
-from typing_extensions import Literal
-
-from flet import flet as ft
-from flet_core.page import Connection
-
-
-def _connect_internal_sync(
-    page_name,
-    view: Literal["flet_app"],
-    host,
-    port,
-    server,
-    auth_token,
-    session_handler,
-    assets_dir,
-    upload_dir,
-    web_renderer,
-    route_url_strategy,
-) -> ft.SyncLocalSocketConnection:
-    # For some reason this is necessary to disable getting `flet.flet` linting errors
-    # pylint: disable=all
-    return ft.__connect_internal_sync(  # pylint: disable=protected-access
-        page_name,
-        view,
-        host,
-        port,
-        server,
-        auth_token,
-        session_handler,
-        assets_dir,
-        upload_dir,
-        web_renderer,
-        route_url_strategy,
-    )
-
-
-class BackgroundFlet:
-    """Class that manages the graphical flet subrocess and related operations"""
-
-    def __init__(self):
-        atexit.register(self.close_flet_view)
-        self.logger = getLogger(__name__)
-        self._conn: Optional[Connection] = None
-        self._fvp: Optional[Popen] = None
-        self._pid_file: Optional[str] = None
-
-    def _app_sync(
-        self,
-        target,
-        name="",
-        host=None,
-        port=0,
-        view: ft.AppViewer = ft.FLET_APP,
-        assets_dir=None,
-        upload_dir=None,
-        web_renderer="canvaskit",
-        route_url_strategy="path",
-        auth_token=None,
-    ) -> Tuple[Connection, Popen, str]:
-        # Based on https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet/src/flet/flet.py#L96 # noqa: E501
-        # We access Flet internals because it is simplest way to control the specifics
-        # In the future we should migrate / ask for a stable API that fits our needs
-        # pylint: disable=protected-access
-        conn = _connect_internal_sync(
-            page_name=name,
-            view=ft.FLET_APP,
-            host=host,
-            port=port,
-            server=None,
-            auth_token=auth_token,
-            session_handler=target,
-            assets_dir=assets_dir,
-            upload_dir=upload_dir,
-            web_renderer=web_renderer,
-            route_url_strategy=route_url_strategy,
-        )
-
-        self.logger.info("Connected to Flet app and handling user sessions...")
-
-        fvp, pid_file = ft.open_flet_view(
-            conn.page_url, assets_dir, view == ft.FLET_APP_HIDDEN
-        )
-        return conn, fvp, pid_file
-
-    def start_flet_view(self, target) -> None:
-        """Starts the flet process and places the connection, view process Popen and
-        flet python server PID file into self
-        """
-        self._conn, self._fvp, self._pid_file = self._app_sync(target)
-
-    def close_flet_view(self) -> None:
-        """Close the currently open flet view"""
-        if not all([self._conn, self._fvp, self._pid_file]):
-            # Library was not open
-            return
-        assert self._conn is not None
-        assert self._fvp is not None
-        assert self._pid_file is not None
-        self._conn.close()
-        ft.close_flet_view(self._pid_file)
-        self._fvp.terminate()
-        self._conn = None
-        self._fvp = None
-        self._pid_file = None
-
-    def poll(self):
-        return self._fvp.poll()
+import atexit
+from logging import getLogger
+from subprocess import Popen
+from typing import Optional, Tuple
+from typing_extensions import Literal
+
+from flet import flet as ft
+from flet_core.page import Connection
+
+
+def _connect_internal_sync(
+    page_name,
+    view: Literal["flet_app"],
+    host,
+    port,
+    server,
+    auth_token,
+    session_handler,
+    assets_dir,
+    upload_dir,
+    web_renderer,
+    route_url_strategy,
+) -> ft.SyncLocalSocketConnection:
+    # For some reason this is necessary to disable getting `flet.flet` linting errors
+    # pylint: disable=all
+    return ft.__connect_internal_sync(  # pylint: disable=protected-access
+        page_name,
+        view,
+        host,
+        port,
+        server,
+        auth_token,
+        session_handler,
+        assets_dir,
+        upload_dir,
+        web_renderer,
+        route_url_strategy,
+    )
+
+
+class BackgroundFlet:
+    """Class that manages the graphical flet subrocess and related operations"""
+
+    def __init__(self):
+        atexit.register(self.close_flet_view)
+        self.logger = getLogger(__name__)
+        self._conn: Optional[Connection] = None
+        self._fvp: Optional[Popen] = None
+        self._pid_file: Optional[str] = None
+
+    def _app_sync(
+        self,
+        target,
+        name="",
+        host=None,
+        port=0,
+        view: ft.AppViewer = ft.FLET_APP,
+        assets_dir=None,
+        upload_dir=None,
+        web_renderer="canvaskit",
+        route_url_strategy="path",
+        auth_token=None,
+    ) -> Tuple[Connection, Popen, str]:
+        # Based on https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet/src/flet/flet.py#L96 # noqa: E501
+        # We access Flet internals because it is simplest way to control the specifics
+        # In the future we should migrate / ask for a stable API that fits our needs
+        # pylint: disable=protected-access
+        conn = _connect_internal_sync(
+            page_name=name,
+            view=ft.FLET_APP,
+            host=host,
+            port=port,
+            server=None,
+            auth_token=auth_token,
+            session_handler=target,
+            assets_dir=assets_dir,
+            upload_dir=upload_dir,
+            web_renderer=web_renderer,
+            route_url_strategy=route_url_strategy,
+        )
+
+        self.logger.info("Connected to Flet app and handling user sessions...")
+
+        fvp, pid_file = ft.open_flet_view(
+            conn.page_url, assets_dir, view == ft.FLET_APP_HIDDEN
+        )
+        return conn, fvp, pid_file
+
+    def start_flet_view(self, target) -> None:
+        """Starts the flet process and places the connection, view process Popen and
+        flet python server PID file into self
+        """
+        self._conn, self._fvp, self._pid_file = self._app_sync(target)
+
+    def close_flet_view(self) -> None:
+        """Close the currently open flet view"""
+        if not all([self._conn, self._fvp, self._pid_file]):
+            # Library was not open
+            return
+        assert self._conn is not None
+        assert self._fvp is not None
+        assert self._pid_file is not None
+        self._conn.close()
+        ft.close_flet_view(self._pid_file)
+        self._fvp.terminate()
+        self._conn = None
+        self._fvp = None
+        self._pid_file = None
+
+    def poll(self):
+        return self._fvp.poll()
```

### Comparing `rpaframework_assistant-3.0.2/src/RPA/Assistant/callback_runner.py` & `rpaframework_assistant-3.0.3/src/RPA/Assistant/callback_runner.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import logging
-import types
-from typing import Any, Callable, Dict, Optional, Union
-
-from flet_core import ControlEvent
-from robot.errors import RobotError
-from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
-from robot.output.logger import LOGGER
-
-
-class CallbackRunner:
-    """provides helper functionality for running Robot and Python callbacks in
-    RPA.Assistant."""
-
-    def __init__(self, client) -> None:
-        self.logger = logging.getLogger(__name__)
-        self.validation_errors: Dict[str, Optional[str]] = {}
-        self._client = client
-
-    def _python_callback(
-        self, function: Callable[[Any], None], *args, **kwargs
-    ) -> Callable[[], None]:
-        """wrapper code that is used to add wrapping for user functions when binding
-        them to be run by buttons
-        """
-
-        def func_wrapper() -> None:
-            return self._run_python_callback(function, *args, **kwargs)
-
-        return func_wrapper
-
-    def python_validation(
-        self, element_name: str, function: Callable[[Any], Optional[str]]
-    ) -> Callable[[ControlEvent], None]:
-        """wrapper code that is used to add wrapping for user functions when binding
-        them to be run on validations buttons
-        """
-
-        def validate(e: ControlEvent) -> None:
-            error = self._run_python_callback(function, e.data)
-            casted_error = str(error) if error else None
-            e.control.error_text = casted_error
-            self._client.flet_update()
-            self.validation_errors[element_name] = casted_error
-
-        return validate
-
-    def _run_python_callback(self, function: Callable, *args, **kwargs):
-        try:
-            return function(*args, **kwargs)
-
-        # This can be anything since it comes from the user function, we don't
-        # want to let the user function crash the UI
-        except Exception as err:  # pylint: disable=broad-except
-            self.logger.error(f"Error calling Python function {function.__name__}")
-            self.logger.error(err)
-        finally:
-            self._client.unlock_elements()
-            self._client.flet_update()
-        return None
-
-    def _robot_callback(self, kw_name: str, *args, **kwargs) -> Callable[[], None]:
-        """wrapper code that is used to add wrapping for user functions when binding
-        them to be run by buttons
-        """
-
-        def func_wrapper() -> None:
-            return self._run_robot_callback(kw_name, *args, **kwargs)
-
-        return func_wrapper
-
-    def robot_validation(
-        self, element_name: str, kw_name: str
-    ) -> Callable[[ControlEvent], None]:
-        """wrapper code that is used to add wrapping for user functions when binding
-        them to be run on validation
-        """
-
-        def validate(e: ControlEvent) -> None:
-            def _nothing(*args, **kwargs):  # pylint: disable=unused-argument
-                pass
-
-            logging_methods = (LOGGER.start_keyword, LOGGER.end_keyword)
-            try:
-                # Disable logging by monkey patching the robot logger
-                LOGGER.start_keyword = types.MethodType(_nothing, LOGGER)
-                LOGGER.end_keyword = types.MethodType(_nothing, LOGGER)
-
-                error = self._run_robot_callback(kw_name, e.control.value)
-                e.control.error_text = error
-                self._client.flet_update()
-                self.validation_errors[element_name] = error
-            finally:
-                LOGGER.start_keyword, LOGGER.end_keyword = logging_methods
-
-        return validate
-
-    def _run_robot_callback(self, kw_name: str, *args, **kwargs):
-
-        try:
-            return BuiltIn().run_keyword(kw_name, *args, **kwargs)
-        except RobotNotRunningError:
-            self.logger.error(
-                f"Robot Framework not running so cannot call keyword {kw_name}"
-            )
-        except RobotError as e:
-            self.logger.error(f"Error calling robot keyword {kw_name}")
-            self.logger.error(e)
-        # This can be anything since it comes from the user function, we don't
-        # want to let the user function crash the UI
-        except Exception as err:  # pylint: disable=broad-except
-            self.logger.error(f"Unexpected error running robot keyword {kw_name}")
-            self.logger.error(err)
-        finally:
-            self._client.unlock_elements()
-            self._client.flet_update()
-        return None
-
-    def queue_fn_or_kw(self, function: Union[Callable, str], *args, **kwargs):
-        """Check if function is a Python function or a Robot Keyword, and schedule it
-        for execution appropriately.
-        """
-        if self._client.pending_operation:
-            self.logger.error("Can't have more than one pending operation.")
-            return
-        self._client.lock_elements()
-        self._client.flet_update()
-
-        if isinstance(function, Callable):
-            self._client.pending_operation = self._python_callback(
-                function, *args, **kwargs
-            )
-        else:
-            self._client.pending_operation = self._robot_callback(
-                function, *args, **kwargs
-            )
+import logging
+import types
+from typing import Any, Callable, Dict, Optional, Union
+
+from flet_core import ControlEvent
+from robot.errors import RobotError
+from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
+from robot.output.logger import LOGGER
+
+
+class CallbackRunner:
+    """provides helper functionality for running Robot and Python callbacks in
+    RPA.Assistant."""
+
+    def __init__(self, client) -> None:
+        self.logger = logging.getLogger(__name__)
+        self.validation_errors: Dict[str, Optional[str]] = {}
+        self._client = client
+
+    def _python_callback(
+        self, function: Callable[[Any], None], *args, **kwargs
+    ) -> Callable[[], None]:
+        """wrapper code that is used to add wrapping for user functions when binding
+        them to be run by buttons
+        """
+
+        def func_wrapper() -> None:
+            return self._run_python_callback(function, *args, **kwargs)
+
+        return func_wrapper
+
+    def python_validation(
+        self, element_name: str, function: Callable[[Any], Optional[str]]
+    ) -> Callable[[ControlEvent], None]:
+        """wrapper code that is used to add wrapping for user functions when binding
+        them to be run on validations buttons
+        """
+
+        def validate(e: ControlEvent) -> None:
+            error = self._run_python_callback(function, e.data)
+            casted_error = str(error) if error else None
+            e.control.error_text = casted_error
+            self._client.flet_update()
+            self.validation_errors[element_name] = casted_error
+
+        return validate
+
+    def _run_python_callback(self, function: Callable, *args, **kwargs):
+        try:
+            return function(*args, **kwargs)
+
+        # This can be anything since it comes from the user function, we don't
+        # want to let the user function crash the UI
+        except Exception as err:  # pylint: disable=broad-except
+            self.logger.error(f"Error calling Python function {function.__name__}")
+            self.logger.error(err)
+        finally:
+            self._client.unlock_elements()
+            self._client.flet_update()
+        return None
+
+    def _robot_callback(self, kw_name: str, *args, **kwargs) -> Callable[[], None]:
+        """wrapper code that is used to add wrapping for user functions when binding
+        them to be run by buttons
+        """
+
+        def func_wrapper() -> None:
+            return self._run_robot_callback(kw_name, *args, **kwargs)
+
+        return func_wrapper
+
+    def robot_validation(
+        self, element_name: str, kw_name: str
+    ) -> Callable[[ControlEvent], None]:
+        """wrapper code that is used to add wrapping for user functions when binding
+        them to be run on validation
+        """
+
+        def validate(e: ControlEvent) -> None:
+            def _nothing(*args, **kwargs):  # pylint: disable=unused-argument
+                pass
+
+            logging_methods = (LOGGER.start_keyword, LOGGER.end_keyword)
+            try:
+                # Disable logging by monkey patching the robot logger
+                LOGGER.start_keyword = types.MethodType(_nothing, LOGGER)
+                LOGGER.end_keyword = types.MethodType(_nothing, LOGGER)
+
+                error = self._run_robot_callback(kw_name, e.control.value)
+                e.control.error_text = error
+                self._client.flet_update()
+                self.validation_errors[element_name] = error
+            finally:
+                LOGGER.start_keyword, LOGGER.end_keyword = logging_methods
+
+        return validate
+
+    def _run_robot_callback(self, kw_name: str, *args, **kwargs):
+
+        try:
+            return BuiltIn().run_keyword(kw_name, *args, **kwargs)
+        except RobotNotRunningError:
+            self.logger.error(
+                f"Robot Framework not running so cannot call keyword {kw_name}"
+            )
+        except RobotError as e:
+            self.logger.error(f"Error calling robot keyword {kw_name}")
+            self.logger.error(e)
+        # This can be anything since it comes from the user function, we don't
+        # want to let the user function crash the UI
+        except Exception as err:  # pylint: disable=broad-except
+            self.logger.error(f"Unexpected error running robot keyword {kw_name}")
+            self.logger.error(err)
+        finally:
+            self._client.unlock_elements()
+            self._client.flet_update()
+        return None
+
+    def queue_fn_or_kw(self, function: Union[Callable, str], *args, **kwargs):
+        """Check if function is a Python function or a Robot Keyword, and schedule it
+        for execution appropriately.
+        """
+        if self._client.pending_operation:
+            self.logger.error("Can't have more than one pending operation.")
+            return
+        self._client.lock_elements()
+        self._client.flet_update()
+
+        if isinstance(function, Callable):
+            self._client.pending_operation = self._python_callback(
+                function, *args, **kwargs
+            )
+        else:
+            self._client.pending_operation = self._robot_callback(
+                function, *args, **kwargs
+            )
```

### Comparing `rpaframework_assistant-3.0.2/src/RPA/Assistant/library.py` & `rpaframework_assistant-3.0.3/src/RPA/Assistant/library.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1991 +1,1991 @@
-import glob
-import logging
-import os
-import platform
-import subprocess
-from datetime import date
-from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-
-import flet
-from flet import (
-    AppBar,
-    Checkbox,
-    Column,
-    Container,
-    Control,
-    Dropdown,
-    ElevatedButton,
-    FilePicker,
-    FilePickerResultEvent,
-    Image,
-    MainAxisAlignment,
-    Markdown,
-    Radio,
-    RadioGroup,
-    Row,
-    Slider,
-    Text,
-    TextField,
-    alignment,
-    colors,
-    icons,
-)
-from flet_core import Stack
-from flet_core.control_event import ControlEvent
-from flet_core.dropdown import Option
-from robot.api.deco import keyword, library
-from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
-from robot.utils.dotdict import DotDict
-from typing_extensions import Literal
-from RPA.Assistant.callback_runner import CallbackRunner
-
-from RPA.Assistant.flet_client import FletClient
-from RPA.Assistant.types import (
-    Icon,
-    LayoutError,
-    Location,
-    Options,
-    Result,
-    Size,
-    VerticalLocation,
-    WindowLocation,
-)
-from RPA.Assistant.utils import location_to_absolute, optional_str, to_options
-
-
-@library(scope="GLOBAL", doc_format="REST", auto_keywords=False)
-class Assistant:
-    """The `Assistant` library provides a way to display information to a user
-    and request input while a robot is running. It allows building processes
-    that require human interaction. Also it offers capabilities of running
-    other robots inside the current one and determine what to display to the
-    user based on his previous responses.
-
-    It is not included in the `rpaframework` package, so in order to use it
-    you have to add `rpaframework-assistant` with the desired version in your
-    *conda.yaml* file
-
-    Some examples of use-cases could be the following:
-
-    - Displaying generated files after an execution is finished
-    - Displaying dynamic and user-friendly error messages
-    - Requesting passwords or other personal information
-    - Running Keywords based on user's actions
-    - Displaying dynamic content based on user's actions
-    - Automating based on files created by the user
-
-    **Workflow**
-
-    The library is used to create dialogs, i.e. windows, that can be composed
-    on-the-fly based on the current state of the execution.
-
-    The content of the dialog is defined by calling relevant keywords
-    such as ``Add text`` or ``Add file input``. When the dialog is opened
-    the content is generated based on the previous keywords.
-
-    Depending on the way the dialog is started, the execution will either
-    block or continue while the dialog is open. During this time the user
-    can freely edit any possible input fields or handle other tasks.
-
-    After the user has successfully submitted the dialog, any possible
-    entered input will be returned as a result. The user also has the option
-    to abort by closing the dialog window forcefully.
-
-    **Results**
-
-    Each input field has a required ``name`` argument that controls what
-    the value will be called in the result object. Each input name should be
-    unique, and must not be called ``submit`` as that is reserved for the submit
-    button value.
-
-    A result object is a Robot Framework DotDict, where each key
-    is the name of the input field and the value is what the user entered.
-    The data type of each field depends on the input. For instance,
-    a text input will have a string, a checkbox will have a boolean, and
-    a file input will have a list of paths.
-
-    If the user closed the window before submitting or there was an internal
-    error, the results object returned by Run Dialog or Ask User won't have a "submit"
-    key.
-
-    **Layouting**
-
-    By default elements are added to the assistant dialog from top to bottom, with a bit
-    of margin around each element to add spaciousness. This margin is added as a
-    ``Container`` you can manually use ``Open Container`` to override the default
-    container. You can use it to set smaller margins.
-
-    You can combine layouting elements with each other. Layouting elements need to be
-    closed with the corresponding ``Close`` keyword. (So ``Open Row`` and then
-    ``Close Row``.)
-
-    ``Open Row`` can be used to layout elements in the same row.
-
-    ``Open Column`` can be used to layout elements in columns.
-
-    ``Open Stack`` and multiple ``Open Container``'s inside it can be used to set
-    positions like Center, Topleft, BottomRight, or coordinate tuples likes (0, 0),
-    (100, 100) and such.
-
-    ``Open Container`` can bse used for absolute positioning inside a Stack, or anywhere
-    for setting background color or margins and paddings.
-
-    ``Open Navbar`` can be used to make a navigation bar that will stay at the top of
-    the dialog. Its contents won't be cleared when.
-
-
-    **Examples**
-
-    .. code-block:: robotframework
-
-        *** Keywords ***
-        Success dialog
-            Add icon      Success
-            Add heading   Your orders have been processed
-            Add files     *.txt
-            Run dialog    title=Success
-
-        Failure dialog
-            Add icon      Failure
-            Add heading   There was an error
-            Add text      The assistant failed to login to the Enterprise portal
-            Add link      https://robocorp.com/docs    label=Troubleshooting guide
-            Run dialog    title=Failure
-
-        Large dialog
-            Add heading    A real chonker   size=large
-            Add image      fat-cat.jpeg
-            Run dialog     title=Large    height=1024    width=1024
-
-        Confirmation dialog
-            Add icon      Warning
-            Add heading   Delete user ${username}?
-            Add submit buttons    buttons=No,Yes    default=Yes
-            ${result}=    Run dialog
-            IF   $result.submit == "Yes"
-                Delete user    ${username}
-            END
-
-        Input form dialog
-            Add heading       Send feedback
-            Add text input    email    label=E-mail address
-            Add text input    message
-            ...    label=Feedback
-            ...    placeholder=Enter feedback here
-            ...    maximum_rows=5
-            ${result}=    Run dialog
-            Send feedback message    ${result.email}  ${result.message}
-
-
-    .. code-block:: python
-
-        def success_dialog():
-            assistant = Assistant()
-            assistant.add_icon("success")
-            assistant.add_heading("Your orders have been processed")
-            assistant.add_files("*.txt")
-            assistant.run_dialog(title="Success")
-
-        def failure_dialog():
-            assistant = Assistant()
-            assistant.add_icon("failure")
-            assistant.add_heading("There was an error")
-            assistant.add_text("The assistant failed to login to the Enterprise portal")
-            assistant.add_link("https://robocorp.com/docs", label="Troubleshooting guide")
-            assistant.add_files("*.txt")
-            assistant.run_dialog(title="Failure")
-
-        def large_dialog():
-            assistant = Assistant()
-            assistant.add_heading("A real chonker", size="large")
-            assistant.add_image("fat-cat.jpeg")
-            assistant.run_dialog(title="Large", height=1024, width=1024)
-
-        def confirmation_dialog():
-            assistant = Assistant()
-            assistant.add_icon("warning")
-            assistant.add_heading("Delete user ${username}?")
-            assistant.add_submit_buttons(buttons="No, Yes", default="Yes")
-            result = assistant.run_dialog()
-            if result.submit == "Yes":
-                delete_user(username)
-
-        def input_from_dialog():
-            assistant = Assistant()
-            assistant.add_heading("Send feedback")
-            assistant.add_text_input("email", label="E-mail address")
-            assistant.add_text_input("message", label="Feedback", placeholder="Enter feedback here", maximum_rows=5)
-            assistant.add_submit_buttons("Submit", default="Submit")
-            result = assistant.run_dialog()
-            send_feedback_message(result.email, result.message)
-    """  # noqa: E501
-
-    def __init__(self) -> None:
-        self.logger = logging.getLogger(__name__)
-        os.environ["FLET_LOG_LEVEL"] = "warning"
-        self._client = FletClient()
-        self._callbacks = CallbackRunner(self._client)
-        self._required_fields: Set[str] = set()
-        self._open_layouting: List[str] = []
-
-        try:
-            # Prevent logging from keywords that return results
-            keywords = [
-                "Run dialog",
-                "Ask user",
-            ]
-            BuiltIn().import_library(
-                "RPA.core.logger.RobotLogListener", "WITH NAME", "RPA.RobotLogListener"
-            )
-            listener = BuiltIn().get_library_instance("RPA.RobotLogListener")
-            # useful to comment out when debugging
-            listener.register_protected_keywords(keywords)
-        except RobotNotRunningError:
-            pass
-
-    def _create_closing_button(self, label="Submit") -> Control:
-        def validate_and_close(*_):
-            # remove None's from the result dictionary
-            for field_name in list(self._client.results.keys()):
-                if self._client.results[field_name] is None:
-                    self._client.results.pop(field_name)
-
-            should_close = True
-
-            for field_name in self._required_fields:
-                value = self._client.results.get(field_name)
-                error_message = (
-                    None if value else f"Mandatory field {field_name} was not completed"
-                )
-                if error_message:
-                    should_close = False
-                    self._client.set_error(field_name, error_message)
-                    self._client.flet_update()
-
-            for field_name, error in self._callbacks.validation_errors.items():
-                if error is not None:
-                    should_close = False
-                    self._client.set_error(field_name, error)
-            self._client.flet_update()
-
-            if should_close:
-                self._client.results["submit"] = label
-                self._client.page.window_destroy()
-
-        return ElevatedButton(label, on_click=validate_and_close)
-
-    @keyword(tags=["dialog", "running"])
-    def clear_dialog(self) -> None:
-        """Clear dialog and results while it is running."""
-        self._client.results = {}
-        self._client.clear_elements()
-
-    @keyword
-    def add_heading(
-        self,
-        heading: str,
-        size: Size = Size.Medium,
-    ) -> None:
-        """Add a centered heading text element
-
-        :param heading: The text content for the heading
-        :param size:    The size of the heading
-
-        Supported ``size`` values are Small, Medium, and Large. By default uses
-        the value Medium.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Add dialog heading
-                Add heading     User information  size=Large
-                Add heading     Location          size=Small
-                Add text input  address           label=User address
-                Run dialog
-
-
-        .. code-block:: python
-
-            def add_dialog_heading():
-                assistant = Assistant()
-                assistant.add_heading("User information", size="large")
-                assistant.add_heading("Location", size="small")
-                assistant.add_text_input("address", label="User address")
-                assistant.run_dialog()
-        """
-        if not isinstance(size, Size):
-            size = Size(size)
-
-        size_dict = {
-            Size.Small: "headlineSmall",
-            Size.Medium: "headlineMedium",
-            Size.Large: "headlineLarge",
-        }
-
-        self._client.add_element(element=Text(heading, style=size_dict[size]))
-
-    @keyword
-    def add_text(
-        self,
-        text: str,
-        size: Size = Size.Medium,
-    ) -> None:
-        """Add a text paragraph element, for larger bodies of text
-
-        :param text: The text content for the paragraph
-        :param size: The size of the text
-
-        Supported ``size`` values are Small, Medium, and Large. By default uses
-        the value Medium.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Show error dialog
-                Add heading   An error occurred
-                Add text      There was an error while requesting user information
-                Add text      ${error}   size=Small
-                Run dialog
-
-        .. code-block:: python
-
-            def show_error_dialog():
-                error = "Your error message"
-                assistant = Assistant()
-                assistant.add_heading("An error occurred")
-                assistant.add_text("There was an error while requesting user information")
-                assistant.add_text(f"{error}", size="small")
-                assistant.run_dialog()
-        """  # noqa: E501
-        if not isinstance(size, Size):
-            size = Size(size)
-
-        if size == Size.Small:
-            self._client.add_element(element=Text(text, style="bodySmall"))
-        elif size == Size.Medium:
-            self._client.add_element(element=Text(text, style="bodyMedium"))
-        elif size == Size.Large:
-            self._client.add_element(element=Text(text, style="bodyLarge"))
-
-    @keyword
-    def add_link(
-        self,
-        url: str,
-        label: Optional[str] = None,
-    ) -> None:
-        """Add an external URL link element
-
-        :param url:   The URL for the link
-        :param label: A custom label text for the link
-
-        Adds a clickable link element, which opens the user's default
-        browser to the given ``url``. Optionally a ``label`` can be given
-        which is shown as the link text, instead of the raw URL.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Display troubleshoot link
-                Add heading    An error occurred
-                Add text       See link for documentation
-                Add link       https://robocorp.com/docs    label=Troubleshooting
-                Run dialog
-
-        .. code-block:: python
-
-            def add_troubleshoot_link():
-                assistant = Assistant()
-                assistant.add_heading("An error occurred")
-                assistant.add_text("See link for documentation")
-                assistant.add_link("https://robocorp.com/docs", label="Troubleshooting")
-                assistant.run_dialog()
-        """
-        if not label:
-            label = url
-        self._client.add_element(
-            Markdown(
-                f"[{label}]({url})",
-                on_tap_link=lambda e: self._client.page.launch_url(e.data),
-            )
-        )
-
-    @keyword
-    def add_image(
-        self,
-        url_or_path: str,
-        width: Optional[int] = None,
-        height: Optional[int] = None,
-    ) -> None:
-        """Add an image element, from a local file or remote URL
-
-        :param url_or_path: The location of the image
-        :param width:       The static width of the image, in pixels
-        :param height:      The static height of the image, in pixels
-
-        Adds an inline image to the dialog, which can either
-        point to a local file path on the executing machine or to
-        a remote URL. If it's a local file path it has to be absolute path.
-
-        By default the image is resized to fit the width of the dialog
-        window, but the width and/or height can be explicitly defined
-        to a custom value. If only one of the dimensions is given,
-        the other is automatically changed to maintain the correct aspect ratio.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Display image
-                Add image      C:\\Users\\me\\company-logo.png
-                Add heading    To start, please press the Continue button   size=Small
-                Add submit buttons    Continue
-                Run dialog
-
-        .. code-block:: python
-            def display_image():
-                assistant = Assistant()
-                assistant.add_image("C:\\Users\\me\\company-logo.png")
-                assistant.add_heading("To start, please press the Continue button", size="small")
-                assistant.add_submit_buttons("Continue")
-                assistant.run_dialog()
-        """  # noqa: E501
-
-        is_url = url_or_path.startswith(("http://", "https://"))
-        is_absolute_path = os.path.isabs(url_or_path)
-        is_absolute_and_file_exists = is_absolute_path and os.path.isfile(url_or_path)
-
-        if is_url or is_absolute_and_file_exists:
-            self._client.add_element(
-                Container(content=Image(src=url_or_path, width=width, height=height))
-            )
-        else:
-            self.logger.warning(
-                "The image path you specified should be a valid URL or absolute path "
-                + f" to an existing file. The value provided: {url_or_path}"
-            )
-
-    @keyword
-    def add_file(
-        self,
-        path: str,
-        label: Optional[str] = None,
-    ) -> None:
-        """Add a file element, which links to a local file
-
-        :param path:  The path to the file
-        :param label: A custom label text for the file
-
-        Adds a button which opens a local file with the corresponding
-        default application. Can be used for instance to display generated
-        files from the robot to the end-user.
-
-        Optionally a custom ``label`` can be given for the button text.
-        By default uses the filename of the linked file.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Open file button
-                ${path}=   Generate order files
-                Add heading    Current orders
-                Add file    ${path}    label=Current
-                Run dialog
-
-        .. code-block:: python
-
-            def open_file_button():
-                path = generate_order_files()
-                assistant = Assistant()
-                assistant.add_heading("Current orders")
-                assistant.add_file(path, label="Current")
-                assistant.run_dialog()
-        """
-        resolved = Path(path).resolve()
-        self.logger.info("Adding file: %s", resolved)
-
-        if not resolved.exists():
-            self.logger.warning("File does not exist: %s", resolved)
-
-        def open_file(*_):
-            if platform.system() == "Windows":
-                os.startfile(resolved)  # type: ignore # pylint: disable=no-member
-            elif platform.system() == "Darwin":
-                subprocess.call(["open", resolved])
-            else:
-                subprocess.call(["xdg-open", resolved])
-
-        self._client.add_element(
-            element=ElevatedButton(
-                text=(label or str(resolved)), icon=icons.FILE_OPEN, on_click=open_file
-            )
-        )
-
-    @keyword
-    def add_files(
-        self,
-        pattern: str,
-    ) -> None:
-        """Add multiple file elements according to the given file pattern
-
-        :param pattern: File matching pattern
-
-        See the keyword ``Add file`` for information about the inserted
-        element itself.
-
-        The keyword uses Unix-style glob patterns for finding matching files,
-        and the supported pattern expressions are as follow:
-
-        ========== ================================================
-        Pattern    Meaning
-        ========== ================================================
-        ``*``      Match everything
-        ``?``      Match any single character
-        ``[seq]``  Match any character in seq
-        ``[!seq]`` Match any character not in seq
-        ``**``     Match all files, directories, and subdirectories
-        ========== ================================================
-
-        If a filename has any of these special characters, they
-        can be escaped by wrapping them with square brackets.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Open multiple files buttons
-                # Add all excel files
-                Add files    *.xlsx
-
-                # Add all log files in any subdirectory
-                Add files    **/*.log
-
-                # Add all PDFs between order0 and order9
-                Add files    order[0-9].pdf
-
-        .. code-block:: python
-
-            def open_multiple_files_buttons():
-                assistant = Assistant()
-                # Add all excel files
-                assistant.add_file("*.xlsx")
-                # Add all log files in any subdirectory
-                assistant.add_file("**/*.log")
-                # Add all PDFs between order0 and order9
-                assistant.add_file("order[0-9].pdf")
-                assistant.run_dialog()
-        """
-        matches = glob.glob(pattern, recursive=True)
-        for match in sorted(matches):
-            self.add_file(match)
-
-    @keyword
-    def add_icon(self, variant: Icon, size: int = 48) -> None:
-        """Add an icon element from RPA.Assistant's short icon list.
-
-        :param variant: The icon type
-        :param size:    The size of the icon
-
-        Adds an icon which can be used to indicate status
-        or the type of dialog being presented.
-
-        The currently supported icon types are:
-
-        ======= ==========================
-        Name    Description
-        ======= ==========================
-        Success A green check mark
-        Warning An orange warning triangle
-        Failure A red cross or X mark
-        ======= ==========================
-
-        The ``size`` of the icon can also be changed,
-        to a given height/width of pixels.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Confirmation dialog
-                Add icon              Warning    size=64
-                Add heading           Do you want to delete this order?
-                Add submit buttons    buttons=No,Yes
-                ${result}=    Run dialog
-
-        .. code-block:: python
-
-            def confirmation_dialog():
-                assistant = Assistant()
-                assistant.add_icon("warning", size="64")
-                assistant.add_heading("Do you want to delete this order?")
-                assistant.add_submit_buttons(buttons="No, Yes")
-                result = assistant.run_dialog()
-        """
-        if not isinstance(variant, Icon):
-            variant = Icon(variant)
-
-        flet_icon_conversions: Dict[Icon, Tuple[str, str]] = {
-            Icon.Success: (icons.CHECK, colors.GREEN_500),
-            Icon.Warning: (icons.WARNING, colors.YELLOW_500),
-            Icon.Failure: (icons.CLOSE, colors.RED_500),
-        }
-        flet_icon, color = flet_icon_conversions[variant]
-
-        self._client.add_element(flet.Icon(name=flet_icon, color=color, size=size))
-
-    @keyword
-    def add_flet_icon(
-        self,
-        icon: str,
-        color: Optional[str] = None,
-        size: Optional[int] = 24,
-    ):
-        """Add an icon from a large gallery of icons.
-
-        :param icon:      Corresponding flet icon name. Check
-                          https://gallery.flet.dev/icons-browser/ for a list of icons.
-                          Write the name in ``lower_case``
-        :param color:     Color for the icon. Default depends on icon. Allowed values
-                          are colors from
-                          https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37
-                          or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).
-        :param size:      Integer size for the icon.
-
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Add custom icon
-                Add Heading    Check icon
-                Add Flet Icon  icon_name=check_circle_rounded  color=FF00FF  size=48
-                Run Dialog
-
-        .. code-block:: python
-
-            def add_custom_icon()
-                assistant = Assistant()
-                assistant.add_heading("Check icon")
-                assistant.add_flet_icon(icon="check_circle_rounded", color="FF00FF", size="48")
-                assistant.run_dialog()
-        """  # noqa: E501
-
-        self._client.add_element(flet.Icon(name=icon, color=color, size=size))
-
-    @keyword(tags=["input"])
-    def add_text_input(
-        self,
-        name: str,
-        label: Optional[str] = None,
-        placeholder: Optional[str] = None,
-        validation: Optional[Union[Callable, str]] = None,
-        default: Optional[str] = None,
-        required: bool = False,
-        minimum_rows: Optional[int] = None,
-        maximum_rows: Optional[int] = None,
-    ) -> None:
-        """Add a text input element
-
-        :param name:        Name of result field
-        :param label:       Label for field
-        :param placeholder: Placeholder text in input field
-        :param validation:   Validation function for the input field
-        :param default:     Default value if the field wasn't completed
-        :param required:    If true, will display an error if not completed
-        :param minimum_rows: Minimum number of rows to display for the input field
-        :param maximum_rows: Maximum number of rows to display for the input field, the
-                             input content can be longer but a scrollbar will appear
-
-        Adds a text field that can be filled by the user. The entered
-        content will be available in the ``name`` field of the result.
-
-        For customizing the look of the input, the ``label`` text can be given
-        to add a descriptive label and the ``placholder`` text can be given
-        to act as an example of the input value.
-
-        The `default` value will be assigned to the input field if the user
-        doesn't complete it. If provided, the placeholder won't be shown.
-        This is `None` by default. Also, if a default value is provided
-        and the user deletes it, `None` will be the corresponding value in
-        the results dictionary.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Send feedback
-                Add heading    Send feedback
-                Add text input    email    label=E-mail address
-                Add text input    message
-                ...    label=Feedback
-                ...    placeholder=Enter feedback here
-                ${result}=    Run dialog
-                Send feedback message    ${result.email}  ${result.message}
-
-        Validation example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Validate Email
-                [Arguments]    ${email}
-                # E-mail specification is complicated, this matches that the e-mail has
-                # at least one character before and after the @ sign, and at least one
-                # character after the dot.
-                ${regex}=    Set Variable    ^.+@.+\\..+
-                ${valid}=    Run Keyword And Return Status    Should Match Regexp  ${email}  ${regex}
-                IF  not $valid
-                    RETURN  Invalid email address
-                END
-
-            Open Dialog
-                Add heading    Send feedback
-                Add text input    email
-                ...    label=Email
-                ...    validation=Validate Email
-                ${result}=    Run dialog
-                Log  ${result.email}
-
-        .. code-block:: python
-
-            import re
-            def validate_email(email):
-                # E-mail specification is complicated, this matches that the e-mail has
-                # at least one character before and after the @ sign, and at least one
-                # character after the dot.
-                regex = r"^.+@.+\\..+"
-                valid = re.match(regex, email)
-                if not valid:
-                    return "Invalid email address"
-
-            def open_dialog():
-                assistant.add_heading("Send feedback")
-                assistant.add_text_input("email", label="Email", validation=validate_email)
-                result = run_dialog()
-                print(result.email)
-
-
-
-        """  # noqa: E501
-        validation_function = None
-        if validation:
-            if isinstance(validation, str):
-                validation_function = self._callbacks.robot_validation(name, validation)
-            elif isinstance(validation, Callable):
-                validation_function = self._callbacks.python_validation(
-                    name, validation
-                )
-            else:
-                raise ValueError("Invalid validation function.")
-
-        if required:
-            self._required_fields.add(name)
-
-        self._client.results[name] = default
-
-        def empty_string_to_none(e):
-            if e.control.value == "":
-                e.data = None
-
-        if minimum_rows or maximum_rows:
-            multiline = True
-        else:
-            multiline = None
-
-        self._client.add_element(
-            name=name,
-            element=TextField(
-                label=label,
-                hint_text=placeholder,
-                value=default,
-                min_lines=minimum_rows,
-                max_lines=maximum_rows,
-                multiline=multiline,
-            ),
-            extra_handler=empty_string_to_none,
-            validation_func=validation_function,
-        )
-
-    @keyword(tags=["input"])
-    def add_password_input(
-        self,
-        name: str,
-        label: Optional[str] = None,
-        placeholder: Optional[str] = None,
-    ) -> None:
-        """Add a password input element
-
-        :param name:        Name of result field
-        :param label:       Label for field
-        :param placeholder: Placeholder text in input field
-
-        Adds a text field that hides the user's input. The entered
-        content will be available in the ``name`` field of the result.
-
-        For customizing the look of the input, the ``label`` text can be given
-        to add a descriptive label and the ``placholder`` text can be given
-        to act as an example of the input value.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Change password
-                Add heading    Change password
-                Add text input        username    label=Current username
-                Add password input    password    label=New password
-                Add submit buttons    buttons=Submit
-                ${result}=    Run dialog
-                Change user password    ${result.username}  ${result.password}
-
-        .. code-block:: python
-
-            def change_password():
-                assistant = Assistant()
-                assistant.add_heading("Change password")
-                assistant.add_text_input("username", label="Current username")
-                assistant.add_password_input("password", label="New password")
-                assistant.add_submit_buttons(buttons="Submit")
-                result = assistant.run_dialog()
-                change_user_password(result.username, result.password)
-        """
-        self._client.add_element(
-            name=name, element=TextField(label=label, value=placeholder, password=True)
-        )
-
-    @keyword(tags=["input"])
-    def add_hidden_input(
-        self,
-        name: str,
-        value: str,
-    ) -> None:
-        """Add a hidden input element
-
-        :param name:  Name of result feild
-        :param value: Value for input
-
-        Adds a special hidden result field that is not visible
-        to the user and always contains the given static value.
-
-        Can be used to keep user input together with already known
-        values such as user IDs, or to ensure that dialogs with differing
-        elements all have the same fields in results.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Get user information
-                Add hidden input   user_id   ${USER_ID}
-                Add text input     username
-                ${result}=         Run dialog
-                Enter user information    ${result.user_id}    ${result.username}
-
-        .. code-block:: python
-
-            def get_user_information():
-                assistant = Assistant()
-                user_id = "Your user value"
-                assistant.add_hidden_input("user_id", user_id)
-                assistant.add_text_input("username")
-                result = assistant.run_dialog()
-                enter_user_information(result.user_id, result.username)
-        """
-        self._client.results[name] = value
-
-    @keyword(tags=["input"])
-    def add_file_input(
-        self,
-        name: str,
-        label: Optional[str] = None,
-        source: Optional[str] = None,
-        file_type: Optional[str] = None,
-        multiple: bool = False,
-    ) -> None:
-        """Add a file input element
-
-        :param name:        Name of result field
-        :param label:       Label for input field
-        :param source:      Default source directory
-        :param file_type:   Accepted file types
-        :param multiple:    Allow selecting multiple files
-
-        Adds a native file selection dialog for inputting one or more files.
-        The list of selected files will be available in the ``name`` field
-        of the result.
-
-        By default opens up in the user's home directory, but it can be
-        set to a custom path with the ``source`` argument.
-
-        The argument ``file_type`` restricts the possible file extensions
-        that the user can select. The format of the argument is as follows:
-        ``pdf,png,svg``. For instance, an argument
-        to limit options to Excel files could be: ``xls,xlsx``.
-
-        To allow selecting more than one file, the ``multiple`` argument
-        can be enabled.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Multiple file selections
-                # This can be any one file
-                Add file input    name=anything
-
-                # This can be multiple files
-                Add file input    name=multiple  multiple=True
-
-                # This opens the select dialog to a custom folder
-                Add file input    name=src       source=C:\\Temp\\Output\\
-
-                # This restricts files to certain types
-                Add file input    name=types     file_type=pdf
-
-                # Every file input result is a list of paths
-                ${result}=    Run dialog
-                FOR    ${path}    IN    @{result.multiple}
-                    Log    Selected file: ${path}
-                END
-
-        .. code-block:: python
-
-            def multiple_file_selections():
-                assistant = Assistant()
-                # This can be any one file
-                assistant.add_file_input(name="anything")
-
-                # This can be multiple files
-                assistant.add_file_input(name="multiple", multiple=True)
-
-                # This opens the select dialog to a custom folder
-                assistant.add_file_input(name="src", source="C:\\Temp\\Output")
-
-                # This restricts files to certain types
-                assistant.add_file_input(name="types", file_type="pdf")
-
-                # Every file input result is a list of paths
-                result = assistant.run_dialog()
-                for path in result.multiple:
-                    print("Selected file: ", path)
-        """
-
-        def on_pick_result(event: FilePickerResultEvent):
-            if event.files:
-                self._client.results[str(name)] = [f.path for f in event.files]
-                selected_files.value = (
-                    ", ".join(map(lambda f: f.name, event.files))
-                    if event.files
-                    else "Cancelled!"
-                )
-                selected_files.update()
-
-        file_picker = FilePicker(on_result=on_pick_result)
-        self._client.add_invisible_element(file_picker)
-        selected_files = Text()
-
-        options = {
-            "source": optional_str(source),
-            "file_type": optional_str(file_type),
-        }
-
-        if not options["source"]:
-            options["source"] = os.path.expanduser("~")
-
-        if options["file_type"]:
-            options["file_type"] = options["file_type"].split(",")
-
-        self._client.add_element(
-            Row(
-                [
-                    ElevatedButton(
-                        label or "Choose files...",
-                        on_click=lambda _: file_picker.pick_files(
-                            allow_multiple=bool(multiple),
-                            initial_directory=options["source"],
-                            allowed_extensions=options["file_type"],
-                        ),
-                    ),
-                    selected_files,
-                ]
-            )
-        )
-
-    @keyword("Add Drop-Down", tags=["input"])
-    def add_drop_down(
-        self,
-        name: str,
-        options: Options,
-        default: Optional[str] = None,
-        label: Optional[str] = None,
-    ) -> None:
-        """Add a drop-down element
-
-        :param name:    Name of result field
-        :param options: List of drop-down options
-        :param default: The default selection
-        :param label:   Label for input field
-
-        Creates a drop-down menu with the given ``options``. The selection
-        the user makes will be available in the ``name`` field of the result.
-
-        The ``default`` argument can be one of the defined options,
-        and the dialog automatically selects that option for the input.
-
-        A custom ``label`` text can also be added.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Select user type from drop down
-                Add heading     Select user type
-                Add drop-down
-                ...    name=user_type
-                ...    options=Admin,Maintainer,Operator
-                ...    default=Operator
-                ...    label=User type
-                ${result}=      Run dialog
-                Log    User type should be: ${result.user_type}
-
-        .. code-block:: python
-
-            def select_user_type_from_drop_down():
-                assistant = Assistant()
-                assistant.add_heading("Select user type")
-                assistant.add_drop_down(
-                    name="user_type",
-                    options="Admin,Maintainer,Operator",
-                    default="Operator",
-                    label="User type"
-                )
-                result = assistant.run_dialog()
-                print("User type should be: ", result.user_type)
-        """
-        options, default = to_options(options, default)
-        options: List[Control] = list(map(Option, options))
-        dropdown = Dropdown(options=options, value=default)
-
-        self._client.results[name] = default
-        self._client.add_element(Text(value=label))
-        self._client.add_element(dropdown, name=str(name))
-
-    @keyword(tags=["input"])
-    def add_date_input(
-        self,
-        name: str,
-        default: Optional[Union[date, str]] = None,
-        label: Optional[str] = None,
-    ) -> None:
-        """Add a date input element.
-
-        :param name:    Name of the result field
-        :param default: The default set date
-        :param label:   Label for the date input field
-
-        Displays a date input. The selection the user makes will be available
-        as a ``date`` object in the ``name`` field of the result.
-        The ``default`` argument can be a pre-set date as object or string in
-        "YYYY-MM-DD" format, otherwise the current date is used.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Select birthdate
-                Add heading       Enter your birthdate
-                Add Date Input    birthdate    default=1993-04-26
-                ${result} =       Run dialog
-                Log To Console    User birthdate year should be: ${result.birthdate.year}
-
-        .. code-block:: python
-
-            def select_birthdate():
-                assistant = Assistant()
-                assistant.add_heading("Enter your birthdate")
-                assistant.add_date_input("birthdate", default="1993-04-26")
-                result = assistant.run_dialog()
-                print("User birthdate year should be: ", result.birthdate.year)
-        """  # noqa: E501
-
-        def validate(date_text: str):
-            if not date_text:
-                return None
-            try:
-                date.fromisoformat(date_text)
-                return None
-            except ValueError:
-                return "Date should be in format YYYY-MM-DD"
-
-        if default:
-            if isinstance(default, str):
-                try:
-                    default = date.fromisoformat(default)
-                except ValueError as e:
-                    self.logger.error(
-                        f"Default date value {default} is not in a valid ISO format."
-                    )
-                    raise e
-            self._client.results[name] = default
-
-        self._client.date_inputs.append(name)
-        self._client.add_element(
-            name=name,
-            element=TextField(label=label, hint_text="YYYY-MM-DD", value=default),
-            validation_func=self._callbacks.python_validation(name, validate),
-        )
-
-    @keyword(tags=["input"])
-    def add_radio_buttons(
-        self,
-        name: str,
-        options: Options,
-        default: Optional[str] = None,
-        label: Optional[str] = None,
-    ) -> None:
-        """Add radio button elements
-
-        :param name:    Name of result field
-        :param options: List of drop-down options
-        :param default: The default selection
-        :param label:   Label for input field
-
-        Creates a set of radio buttons with the given ``options``. The selection
-        the user makes will be available in the ``name`` field of the result.
-
-        The ``default`` argument can be one of the defined options,
-        and the dialog automatically selects that option for the input.
-
-        A custom ``label`` text can also be added.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Select user type from radio buttons
-                Add heading     Select user type
-                Add radio buttons
-                ...    name=user_type
-                ...    options=Admin,Maintainer,Operator
-                ...    default=Operator
-                ...    label=User type
-                ${result}=      Run dialog
-                Log    User type should be: ${result.user_type}
-
-        .. code-block:: python
-
-            def select_user_type_from_radio_buttons():
-                assistant = Assistant()
-                assistant.add_heading("Select user type")
-                assistant.add_radio_buttons(
-                    name="user_type",
-                    options="Admin,Maintainer,Operator",
-                    default="Operator",
-                    label="User type"
-                )
-                result = assistant.run_dialog()
-                print("User type should be: ", result.user_type)
-        """
-        options, default = to_options(options, default)
-        radios: List[Control] = [
-            Radio(value=option, label=option) for option in options
-        ]
-        radio_group = RadioGroup(content=Column(radios), value=default)
-
-        self._client.results[name] = default
-        self._client.add_element(Text(value=label))
-        self._client.add_element(radio_group, name=str(name))
-
-    @keyword(tags=["input"])
-    def add_checkbox(
-        self,
-        name: str,
-        label: str,
-        default: bool = False,
-    ) -> None:
-        """Add a checkbox element
-
-        :param name:    Name of result field
-        :param label:   Label text for checkbox
-        :param default: Default checked state
-
-        Adds a checkbox that indicates a true or false value.
-        The selection will be available in the ``name`` field of the result,
-        and the ``label`` text will be shown next to the checkbox.
-
-        The boolean ``default`` value will define the initial checked
-        state of the element.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Select checkboxes
-                Add heading     Enable features
-                Add checkbox    name=vault        label=Enable vault       default=True
-                Add checkbox    name=triggers     label=Enable triggers    default=False
-                Add checkbox    name=assistants   label=Enable assistants  default=True
-                ${result}=      Run dialog
-                IF    $result.vault
-                    Enable vault
-                END
-
-        .. code-block:: python
-
-            def select_checkboxes():
-                assistant = Assistant()
-                assistant.add_heading("Enable features")
-                assistant.add_checkbox(name="vault", label="Enable vault", default=True)
-                assistant.add_checkbox(name="triggers", label="Enable triggers", default=False)
-                assistant.add_checkbox(name="assistants", label="Enable assistants", default=True)
-                result = assistant.run_dialog()
-                if(result.vault):
-                    enable_vault()
-
-        """  # noqa: E501
-        self._client.results[name] = default
-        self._client.add_element(
-            name=str(name), element=Checkbox(label=str(label), value=bool(default))
-        )
-
-    @keyword(tags=["input"])
-    def add_submit_buttons(
-        self, buttons: Options, default: Optional[str] = None
-    ) -> None:
-        """Add custom submit buttons
-
-        :param buttons: Submit button options
-        :param default: The primary button
-
-        The result field will always be called ``submit`` and will contain
-        the pressed button text as a value.
-
-        If one of the custom ``options`` should be the preferred option,
-        the ``default`` argument controls which one is highlighted with
-        an accent color.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Delete user warning
-                Add icon      Warning
-                Add heading   Delete user ${username}?
-                Add submit buttons    buttons=No,Yes    default=Yes
-                ${result}=    Run dialog
-                IF   $result.submit == "Yes"
-                    Delete user    ${username}
-                END
-
-        .. code-block:: python
-
-            def delete_user_warning():
-                assistant = Assistant()
-                username = "user_01"
-                assistant.add_icon("warning")
-                assistant.add_heading(f"Delete user {username}?")
-                assistant.add_submit_buttons(buttons="No, Yes", default="Yes")
-                result = assistant.run_dialog()
-                if result.submit == "Yes":
-                    delete_user(username)
-        """
-        button_labels, default = to_options(buttons, default)
-
-        button_elements = [
-            self._create_closing_button(button) for button in button_labels
-        ]
-        for button in button_elements:
-            self._client.add_to_disablelist(button)
-
-        button_row = Row(button_elements, alignment=MainAxisAlignment.END)
-        container = Container(button_row, alignment=alignment.bottom_right)
-        self._client.add_element(container)
-
-    @keyword(tags=["dialog"])
-    def run_dialog(
-        self,
-        timeout: int = 180,
-        title: str = "Assistant",
-        height: Union[int, Literal["AUTO"]] = "AUTO",
-        width: int = 480,
-        on_top: bool = False,
-        location: Union[WindowLocation, Tuple[int, int], None] = None,
-    ) -> Result:
-        """Create a dialog from all the defined elements and block
-        until the user has handled it.
-
-        :param timeout: Time to wait for dialog to complete, in seconds
-        :param title:  Title of dialog
-        :param height: Height of dialog (in pixels or 'AUTO')
-        :param width:  Width of dialog (in pixels)
-        :param on_top: Show dialog always on top of other windows
-        :param location: Where to place the dialog (options are Center, TopLeft, or a
-                         tuple of ints)
-
-        If the `location` argument is `None` it will let the operating system
-        place the window.
-
-        Returns a result object with all input values.
-
-        When the dialog closes elements are cleared.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Open dialog
-                Add heading     Please enter your username
-                Add text input  name=username
-                ${result}=      Run dialog
-                Log    The username is: ${result.username}
-
-        .. code-block:: python
-
-            def open_dialog():
-                assistant = Assistant()
-                assistant.add_heading("Please enter your username")
-                assistant.add_text_input("username")
-                result = assistant.run_dialog()
-                print("The username is: ", result.username)
-        """
-
-        # height has to be either AUTO or an int value
-        if not isinstance(height, int) and height != "AUTO":
-            height = int(height)
-
-        # if location is given as a string (Robot autoconversion doesn't work) parse it
-        # to enum manually
-        if isinstance(location, str):
-            location = WindowLocation[location]
-
-        self._client.display_flet_window(
-            title, height, width, on_top, location, timeout
-        )
-        results = self._get_results()
-        self._client.results.clear()
-
-        return results
-
-    def _get_results(self) -> DotDict:
-        results = self._client.results
-        for name, value in results.items():
-            if name in self._client.date_inputs and isinstance(value, str):
-                results[name] = date.fromisoformat(value)
-        return DotDict(**results)
-
-    @keyword(tags=["dialog"])
-    def ask_user(self, timeout: int = 180, **options: Any) -> Result:
-        """Same as ``Run Dialog`` it will create a dialog from all the defined
-        elements and block until the user has handled it. It will also add
-        by default a submit and close buttons.
-
-        :param timeout: Time to wait for dialog to complete, in seconds
-        :param options: Options for the dialog
-
-        Returns a result object with all input values.
-
-        For more information about possible options for opening the dialog,
-        see the documentation for the keyword ``Run Dialog``.
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Ask user dialog
-                Add heading     Please enter your username
-                Add text input  name=username
-                ${result}=      Ask User
-                Log    The username is: ${result.username}
-
-        .. code-block:: python
-
-            def ask_user_dialog():
-                assistant = Assistant()
-                assistant.add_heading("Please enter your username")
-                assistant.add_text_input("username")
-                result = assistant.ask_user()
-                print("The username is: ", result.username)
-        """
-
-        self.add_submit_buttons(["Submit", "Close"], "Submit")
-        return self.run_dialog(**options, timeout=timeout)
-
-    @keyword(tags=["dialog", "running"])
-    def refresh_dialog(self):
-        """Can be used to update UI elements when adding elements while dialog is
-        running
-        """
-        self._client.update_elements()
-
-    @keyword(tags=["dialog"])
-    def add_button(
-        self,
-        label: str,
-        function: Union[Callable, str],
-        *args,
-        location: VerticalLocation = VerticalLocation.Left,
-        **kwargs,
-    ) -> None:
-        """Create a button and execute the `function` as a callback when pressed.
-
-        :param label: Text for the button
-        :param function: Python function or Robot Keyword name, that will get ``*args``
-            and ``**kwargs`` passed into it
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            First View
-                Add Heading  Here is the first view of the app
-                Add Button  Change View  Second View
-
-            Second View
-                Add Heading  Let's build an infinite loop
-                Add Button  Change View  First View
-
-        .. code-block:: python
-
-            def first_view():
-                assistant = Assistant()
-                assistant.add_heading("Here is the first view of the app")
-                assistant.add_button("Change view", second_view)
-                assistant.run_dialog()
-
-            def second_view():
-                assistant = Assistant()
-                assistant.add_heading("Let's build an infinite loop")
-                assistant.add_button("Change view", first_view)
-                assistant.run_dialog()
-        """  # noqa: E501
-
-        def on_click(_: ControlEvent):
-            self._callbacks.queue_fn_or_kw(function, *args, **kwargs)
-
-        button = ElevatedButton(label, on_click=on_click)
-        container = Container(alignment=location.value, content=button)
-        self._client.add_element(container)
-        self._client.add_to_disablelist(button)
-
-    @keyword(tags=["dialog"])
-    def add_next_ui_button(self, label: str, function: Union[Callable, str]):
-        """Create a button that leads to the next UI page, calling the passed
-        keyword or function, and passing current form results as first positional
-        argument to it.
-
-        :param label: Text for the button
-        :param function: Python function or Robot Keyword name, that will take form
-            results as its first argument
-
-        Example:
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Retrieve User Data
-                # Retrieves advanced data that needs to be displayed
-
-            Main Form
-                Add Heading  Username input
-                Add Text Input  name=username_1  placeholder=username
-                Add Next Ui Button        Show customer details  Customer Details
-
-            Customer Details
-                [Arguments]  ${form}
-                ${user_data}=  Retrieve User Data  ${form}[username_1]
-                Add Heading  Retrieved Data
-                Add Text  ${user_data}[phone_number]
-                Add Text  ${user_data}[address]
-
-        .. code-block:: python
-
-            def main_form():
-                assistant = Assistant()
-                assistant.add_heading("Username input")
-                assistant.add_text_input("username_1", placeholder="username")
-                assistant.add_next_ui_button("Show customer details", customer_details)
-                assistant.run_dialog()
-
-            def customer_details(form):
-                assistant = Assistant()
-                user_data = retrieve_user_data(form.username_1)
-                assistant.add_heading("Retrieved Data")
-                assistant.add_text(user_data[phone_number])
-                assistant.add_text(user_data[address])
-                assistant.run_dialog()
-        """
-
-        def on_click(_: ControlEvent):
-            self._callbacks.queue_fn_or_kw(function, self._get_results())
-
-        button = ElevatedButton(label, on_click=on_click)
-        self._client.add_element(button)
-        self._client.add_to_disablelist(button)
-
-    @keyword(tags=["input"])
-    def add_slider(
-        self,
-        name: str,
-        slider_min: Union[int, float] = 0,
-        slider_max: Union[int, float] = 100,
-        thumb_text="{value}",
-        steps: Optional[int] = None,
-        default: Optional[Union[int, float]] = None,
-        decimals: Optional[int] = 1,
-    ):
-        """Add a slider input.
-
-        :param name:        Name of result field
-        :param slider_min:  Minimum value of the slider
-        :param slider_max:  Maximum value of the slider
-        :param thumb_label: Text to display when the slider is being slided. Use the
-                            placeholder {value} for the number. (thumb text `{value%}`
-                            will display values: `0%`, `100%`)
-        :param steps:       Amount of steps for the slider. If None, the slider will be
-                            continuous.
-                            For integer output, specify a steps value where all the
-                            steps will be integers, or implement rounding when
-                            retrieving the result.
-        :param default:     Default value for the slider. Must be between min and max.
-        :param decimals:    How many decimals should the value have and show.
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Create Percentage Slider
-                Add Text    Percentage slider
-                Add Slider  name=percentage  slider_min=0  slider_max=100
-                            thumb_text={value}%  steps=100  round=1
-
-        .. code-block:: python
-
-            def create_percentage_slider():
-                assistant = Assistant()
-                assistant.add_text("Percentage slider")
-                assistant.add_slider(
-                    name="percentage",
-                    slider_min=0,
-                    slider_max=100,
-                    thumb_text="{value}%",
-                    steps=100,
-                    decimals=1
-                )
-                assistant.run_dialog()
-        """
-        if default:
-            default = float(default)
-
-            # Is this even necessary?
-            if default.is_integer():
-                default = int(default)
-
-            if slider_min > default or slider_max < default:
-                raise ValueError(f"Slider {name} had an out of bounds default value.")
-            self._client.results[name] = default
-
-        slider = Slider(
-            min=slider_min,
-            max=slider_max,
-            divisions=steps,
-            label=thumb_text,
-            value=default,
-            round=decimals,
-        )
-        self._client.add_element(name=name, element=slider)
-
-    @keyword(tags=["dialog", "running"])
-    def add_loading_spinner(
-        self,
-        name: str,
-        width: int = 16,
-        height: int = 16,
-        stroke_width: int = 2,
-        color: Optional[str] = None,
-        tooltip: Optional[str] = None,
-        value: Optional[float] = None,
-    ):
-        """Add a loading spinner.
-
-        :param name:        Name of the element
-        :param width:       Width of the spinner
-        :param height:      Height of the spinner
-        :param stroke_width: Width of the spinner's stroke
-        :param color:       Color of the spinner's stroke.
-                            Allowed values are colors from
-                            [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
-                            or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
-        :param tooltip:     Tooltip to be displayed
-                            on mouse hover.
-        :param value:       Between 0.0 and 1.0 if you want to manually control it's completion.
-                            If `None` it will spin endlessy.
-        """  # noqa: E501
-        pr = flet.ProgressRing(
-            width=width,
-            height=height,
-            stroke_width=stroke_width,
-            color=color,
-            tooltip=tooltip,
-            value=value,
-        )
-        self._client.add_element(pr, name)
-        return pr
-
-    @keyword(tags=["dialog", "running"])
-    def add_loading_bar(
-        self,
-        name: str,
-        width: int = 16,
-        bar_height: int = 16,
-        color: Optional[str] = None,
-        tooltip: Optional[str] = None,
-        value: Optional[float] = None,
-    ):
-        """Add a loading bar.
-
-        :param name:        Name of the element
-        :param width:       Width of the bar
-        :param bar_height:  Height of the bar
-        :param color:       Color of the bar's stroke.
-                            Allowed values are colors from
-                            [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
-                            or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
-        :param tooltip:     Tooltip to be displayed on mouse hover.
-        :param value:       Between 0.0 and 1.0 if you want to manually control it's completion.
-                            Use `None` for indeterminate progress indicator.
-        """  # noqa: E501
-        pb = flet.ProgressBar(
-            width=width,
-            bar_height=bar_height,
-            color=color,
-            tooltip=tooltip,
-            value=value,
-        )
-        self._client.add_element(pb, name)
-        return pb
-
-    @keyword(tags=["dialog", "running"])
-    def set_title(self, title: str):
-        """Set dialog title when it is running."""
-        self._client.set_title(title)
-
-    def _close_layouting_element(self, layouting_element: str):
-        """Check if the last opened layout element matches what is being closed,
-        otherwise raise `ValueError`. If the check passes, close the layout element.
-        """
-        if not self._open_layouting:
-            raise LayoutError(f"Cannot close {layouting_element}, no open layout")
-
-        last_opened = self._open_layouting[-1]
-        if not last_opened == layouting_element:
-            raise LayoutError(
-                f"Cannot close {layouting_element}, last opened layout is {last_opened}"
-            )
-
-        self._client.close_layout()
-        self._open_layouting.pop()
-
-    @keyword(tags=["layout"])
-    def open_row(self):
-        """Open a row layout container. Following ``Add <element>`` calls will add
-        items into that row until ``Close Row`` is called.
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Side By Side Elements
-                Open Row
-                Add Text  First item on the row
-                Add Text  Second item on the row
-                Close Row
-
-        .. code-block:: python
-
-            def side_by_side_elements():
-                assistant = Assistant()
-                assistant.open_row()
-                assistant.add_text("First item on the row")
-                assistant.add_text("Second item on the row")
-                assistant.close_row()
-                assistant.run_dialog()
-        """
-        self._open_layouting.append("Row")
-        self._client.add_layout(Row())
-
-    @keyword(tags=["layout"])
-    def close_row(self):
-        """Close previously opened row.
-
-        Raises LayoutError if called with no Row open, or if another layout element was
-        opened more recently than a row.
-        """
-        self._close_layouting_element("Row")
-
-    @keyword(tags=["layout"])
-    def open_container(
-        self,
-        margin: Optional[int] = 5,
-        padding: Optional[int] = None,
-        width: Optional[int] = None,
-        height: Optional[int] = None,
-        background_color: Optional[str] = None,
-        location: Union[Location, Tuple[int, int], None] = None,
-    ):
-        """Open a single element container. The following ``Add <element>`` calls adds
-        an element inside the container. Can be used for styling elements.
-
-
-        :param margin: How much margin to add around the container. RPA.Assistant adds
-                       by default a container of margin 5 around all elements, to have
-                       a smaller margin use containers with smaller margin value for
-                       elements.
-        :param padding: How much padding to add around the content of the container.
-        :param width: Width of the container.
-        :param height: Height of the container.
-
-        :param bgcolor:   Background color for the container. Default depends on icon.
-                          Allowed values are colors from
-                          [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
-                          or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
-        :param location:  Where to place the container (A Location value or tuple of
-                          ints). Only works inside a Stack layout element.
-
-                          To use any Center___ or ___Center locations you must define
-                          width and height to the element.
-
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Padded Element With Background
-                Open Container  padding=20  background_color=blue500
-                Add Text        sample text
-                Close Container
-
-        .. code-block:: python
-
-            def padded_element_with_background():
-                assistant = Assistant()
-                assistant.open_container(padding=20, background_color="blue500")
-                assistant.add_text("Sample text")
-                assistant.close_container()
-                assistant.run_dialog()
-        """  # noqa: E501
-        self._open_layouting.append("Container")
-        if not location:
-            top, left, bottom, right = None, None, None, None
-        else:
-            parent_height, parent_width = self._client.get_layout_dimensions()
-            parsed_location = location_to_absolute(
-                location, parent_width, parent_height, width, height
-            )
-            top = parsed_location.get("top")
-            left = parsed_location.get("left")
-            right = parsed_location.get("right")
-            bottom = parsed_location.get("bottom")
-        self._client.add_layout(
-            Container(
-                margin=margin,
-                padding=padding,
-                width=width,
-                height=height,
-                bgcolor=background_color,
-                top=top,
-                left=left,
-                bottom=bottom,
-                right=right,
-            )
-        )
-
-    @keyword(tags=["layout"])
-    def close_container(self):
-        """Close previously opened container.
-
-        Raises LayoutError if called with no Row open, or if another layout element was
-        opened more recently than a row.
-        """
-        self._close_layouting_element("Container")
-
-    @keyword(tags=["layout"])
-    def open_navbar(self, title: Optional[str] = None):
-        """Create a Navigation Bar. Following ``Add <element>`` calls will add
-        items into the Navbar until ``Close Navbar`` is called.
-
-        Navbar doesn't clear when Clear Dialog is called.
-
-        Only one Navbar can be initialized at a time. Trying to make a second one will
-        raise a LayoutError.
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-                Go To Start Menu
-                    Add Heading  Start menu
-                    Add Text  Start menu content
-
-                Assistant Navbar
-                    Open Navbar  title=Assistant
-                    Add Button   menu  Go To Start Menu
-                    Close Navbar
-
-        .. code-block:: python
-
-            def go_to_start_menu():
-                assistant = Assistant()
-                assistant.add_heading("Start menu")
-                assistant.add_text("Start menu content")
-                assistant.run_dialog()
-
-            def assistant_navbar():
-                assistant = Assistant()
-                assistant.open_navbar(title="Assistant")
-                assistant.add_button("menu", go_to_start_menu)
-                assistant.close_navbar()
-                assistant.run_dialog()
-        """
-        self._open_layouting.append("AppBar")
-        self._client.set_appbar(AppBar(title=Text(title)))
-
-    @keyword(tags=["layout"])
-    def close_navbar(self):
-        """Close previously opened navbar.
-
-        Raises LayoutError if called with no Row open, or if another layout element was
-        opened more recently than a row."""
-        self._close_layouting_element("AppBar")
-
-    @keyword(tags=["layout"])
-    def open_stack(self, width: Optional[int] = None, height: Optional[int] = None):
-        """Create a "Stack" layout element. Stack can be used to position elements
-        absolutely and to have overlapping elements in your layout. Use Container's
-        `top` and `left` arguments to position the elements in a stack.
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Absolutely Positioned Elements
-                # Positioning containers with relative location values requires
-                # absolute size for the Stack
-                Open Stack  height=360  width=360
-
-                Open Container  width=64  height=64  location=Center
-                Add Text  center
-                Close Container
-
-                Open Container  width=64  height=64  location=TopRight
-                Add Text  top right
-                Close Container
-
-                Open Container  width=64  height=64  location=BottomRight
-                Add Text  bottom right
-                Close Container
-
-                Close Stack
-
-        .. code-block:: python
-
-            def absolutely_positioned_elements():
-                # Positioning containers with relative location values requires
-                # absolute size for the Stack
-                assistant = Assistant()
-                assistant.open_stack(height=360, width=360)
-
-                assistant.open_container(width=64, height=64, location=Center)
-                assistant.add_text("center")
-                assistant.close_container()
-
-                assistant.open_container(width=64, height=64, location=TopRight)
-                assistant.add_text("top right")
-                assistant.close_container()
-
-                assistant.open_container(width=64, height=64, location=BottomRight)
-                assistant.add_text("bottom right")
-                assistant.close_container()
-
-                assistant.close_stack()
-                assistant.run_dialog()
-
-        """
-        self._open_layouting.append("Stack")
-        self._client.add_layout(Stack(width=width, height=height))
-
-    @keyword(tags=["layout"])
-    def close_stack(self):
-        """Close previously opened Stack.
-
-        Raises LayoutError if called with no Stack open, or if another layout element
-        was opened more recently than a Stack.
-        """
-        self._close_layouting_element("Stack")
-
-    @keyword(tags=["layout"])
-    def open_column(self):
-        """Open a Column layout container. Following ``Add <element>`` calls will add
-        items into that Column until ``Close Column`` is called.
-
-        .. code-block:: robotframework
-
-            *** Keywords ***
-            Double Column Layout
-                Open Row
-                Open Column
-                Add Text      First item in the first column
-                Add Text      Second item on the first column
-                Close Column
-                Open Column
-                Add Text      First item on the second column
-                Close Column
-                Close Row
-
-        .. code-block:: python
-
-            def double_column_layout():
-                assistant = Assistant()
-                assistant.open_row()
-                assistant.open_column()
-                assistant.add_text("First item in the first column")
-                assistant.add_text("Second item on the first column")
-                assistant.close_column()
-
-                assistant.open_column()
-                assistant.add_text("First item on the second column")
-                assistant.close_column()
-                assistant.close_row()
-
-                assistant.run_dialog()
-        """
-        self._open_layouting.append("Column")
-        self._client.add_layout(Column())
-
-    @keyword(tags=["layout"])
-    def close_column(self):
-        """Closes previously opened Column.
-
-        Raises LayoutError if called with no Column open, or if another layout element
-        was opened more recently than a Column.
-        """
-
-        self._close_layouting_element("Column")
+import glob
+import logging
+import os
+import platform
+import subprocess
+from datetime import date
+from pathlib import Path
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+
+import flet
+from flet import (
+    AppBar,
+    Checkbox,
+    Column,
+    Container,
+    Control,
+    Dropdown,
+    ElevatedButton,
+    FilePicker,
+    FilePickerResultEvent,
+    Image,
+    MainAxisAlignment,
+    Markdown,
+    Radio,
+    RadioGroup,
+    Row,
+    Slider,
+    Text,
+    TextField,
+    alignment,
+    colors,
+    icons,
+)
+from flet_core import Stack
+from flet_core.control_event import ControlEvent
+from flet_core.dropdown import Option
+from robot.api.deco import keyword, library
+from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
+from robot.utils.dotdict import DotDict
+from typing_extensions import Literal
+from RPA.Assistant.callback_runner import CallbackRunner
+
+from RPA.Assistant.flet_client import FletClient
+from RPA.Assistant.types import (
+    Icon,
+    LayoutError,
+    Location,
+    Options,
+    Result,
+    Size,
+    VerticalLocation,
+    WindowLocation,
+)
+from RPA.Assistant.utils import location_to_absolute, optional_str, to_options
+
+
+@library(scope="GLOBAL", doc_format="REST", auto_keywords=False)
+class Assistant:
+    """The `Assistant` library provides a way to display information to a user
+    and request input while a robot is running. It allows building processes
+    that require human interaction. Also it offers capabilities of running
+    other robots inside the current one and determine what to display to the
+    user based on his previous responses.
+
+    It is not included in the `rpaframework` package, so in order to use it
+    you have to add `rpaframework-assistant` with the desired version in your
+    *conda.yaml* file
+
+    Some examples of use-cases could be the following:
+
+    - Displaying generated files after an execution is finished
+    - Displaying dynamic and user-friendly error messages
+    - Requesting passwords or other personal information
+    - Running Keywords based on user's actions
+    - Displaying dynamic content based on user's actions
+    - Automating based on files created by the user
+
+    **Workflow**
+
+    The library is used to create dialogs, i.e. windows, that can be composed
+    on-the-fly based on the current state of the execution.
+
+    The content of the dialog is defined by calling relevant keywords
+    such as ``Add text`` or ``Add file input``. When the dialog is opened
+    the content is generated based on the previous keywords.
+
+    Depending on the way the dialog is started, the execution will either
+    block or continue while the dialog is open. During this time the user
+    can freely edit any possible input fields or handle other tasks.
+
+    After the user has successfully submitted the dialog, any possible
+    entered input will be returned as a result. The user also has the option
+    to abort by closing the dialog window forcefully.
+
+    **Results**
+
+    Each input field has a required ``name`` argument that controls what
+    the value will be called in the result object. Each input name should be
+    unique, and must not be called ``submit`` as that is reserved for the submit
+    button value.
+
+    A result object is a Robot Framework DotDict, where each key
+    is the name of the input field and the value is what the user entered.
+    The data type of each field depends on the input. For instance,
+    a text input will have a string, a checkbox will have a boolean, and
+    a file input will have a list of paths.
+
+    If the user closed the window before submitting or there was an internal
+    error, the results object returned by Run Dialog or Ask User won't have a "submit"
+    key.
+
+    **Layouting**
+
+    By default elements are added to the assistant dialog from top to bottom, with a bit
+    of margin around each element to add spaciousness. This margin is added as a
+    ``Container`` you can manually use ``Open Container`` to override the default
+    container. You can use it to set smaller margins.
+
+    You can combine layouting elements with each other. Layouting elements need to be
+    closed with the corresponding ``Close`` keyword. (So ``Open Row`` and then
+    ``Close Row``.)
+
+    ``Open Row`` can be used to layout elements in the same row.
+
+    ``Open Column`` can be used to layout elements in columns.
+
+    ``Open Stack`` and multiple ``Open Container``'s inside it can be used to set
+    positions like Center, Topleft, BottomRight, or coordinate tuples likes (0, 0),
+    (100, 100) and such.
+
+    ``Open Container`` can bse used for absolute positioning inside a Stack, or anywhere
+    for setting background color or margins and paddings.
+
+    ``Open Navbar`` can be used to make a navigation bar that will stay at the top of
+    the dialog. Its contents won't be cleared when.
+
+
+    **Examples**
+
+    .. code-block:: robotframework
+
+        *** Keywords ***
+        Success dialog
+            Add icon      Success
+            Add heading   Your orders have been processed
+            Add files     *.txt
+            Run dialog    title=Success
+
+        Failure dialog
+            Add icon      Failure
+            Add heading   There was an error
+            Add text      The assistant failed to login to the Enterprise portal
+            Add link      https://robocorp.com/docs    label=Troubleshooting guide
+            Run dialog    title=Failure
+
+        Large dialog
+            Add heading    A real chonker   size=large
+            Add image      fat-cat.jpeg
+            Run dialog     title=Large    height=1024    width=1024
+
+        Confirmation dialog
+            Add icon      Warning
+            Add heading   Delete user ${username}?
+            Add submit buttons    buttons=No,Yes    default=Yes
+            ${result}=    Run dialog
+            IF   $result.submit == "Yes"
+                Delete user    ${username}
+            END
+
+        Input form dialog
+            Add heading       Send feedback
+            Add text input    email    label=E-mail address
+            Add text input    message
+            ...    label=Feedback
+            ...    placeholder=Enter feedback here
+            ...    maximum_rows=5
+            ${result}=    Run dialog
+            Send feedback message    ${result.email}  ${result.message}
+
+
+    .. code-block:: python
+
+        def success_dialog():
+            assistant = Assistant()
+            assistant.add_icon("success")
+            assistant.add_heading("Your orders have been processed")
+            assistant.add_files("*.txt")
+            assistant.run_dialog(title="Success")
+
+        def failure_dialog():
+            assistant = Assistant()
+            assistant.add_icon("failure")
+            assistant.add_heading("There was an error")
+            assistant.add_text("The assistant failed to login to the Enterprise portal")
+            assistant.add_link("https://robocorp.com/docs", label="Troubleshooting guide")
+            assistant.add_files("*.txt")
+            assistant.run_dialog(title="Failure")
+
+        def large_dialog():
+            assistant = Assistant()
+            assistant.add_heading("A real chonker", size="large")
+            assistant.add_image("fat-cat.jpeg")
+            assistant.run_dialog(title="Large", height=1024, width=1024)
+
+        def confirmation_dialog():
+            assistant = Assistant()
+            assistant.add_icon("warning")
+            assistant.add_heading("Delete user ${username}?")
+            assistant.add_submit_buttons(buttons="No, Yes", default="Yes")
+            result = assistant.run_dialog()
+            if result.submit == "Yes":
+                delete_user(username)
+
+        def input_from_dialog():
+            assistant = Assistant()
+            assistant.add_heading("Send feedback")
+            assistant.add_text_input("email", label="E-mail address")
+            assistant.add_text_input("message", label="Feedback", placeholder="Enter feedback here", maximum_rows=5)
+            assistant.add_submit_buttons("Submit", default="Submit")
+            result = assistant.run_dialog()
+            send_feedback_message(result.email, result.message)
+    """  # noqa: E501
+
+    def __init__(self) -> None:
+        self.logger = logging.getLogger(__name__)
+        os.environ["FLET_LOG_LEVEL"] = "warning"
+        self._client = FletClient()
+        self._callbacks = CallbackRunner(self._client)
+        self._required_fields: Set[str] = set()
+        self._open_layouting: List[str] = []
+
+        try:
+            # Prevent logging from keywords that return results
+            keywords = [
+                "Run dialog",
+                "Ask user",
+            ]
+            BuiltIn().import_library(
+                "RPA.core.logger.RobotLogListener", "WITH NAME", "RPA.RobotLogListener"
+            )
+            listener = BuiltIn().get_library_instance("RPA.RobotLogListener")
+            # useful to comment out when debugging
+            listener.register_protected_keywords(keywords)
+        except RobotNotRunningError:
+            pass
+
+    def _create_closing_button(self, label="Submit") -> Control:
+        def validate_and_close(*_):
+            # remove None's from the result dictionary
+            for field_name in list(self._client.results.keys()):
+                if self._client.results[field_name] is None:
+                    self._client.results.pop(field_name)
+
+            should_close = True
+
+            for field_name in self._required_fields:
+                value = self._client.results.get(field_name)
+                error_message = (
+                    None if value else f"Mandatory field {field_name} was not completed"
+                )
+                if error_message:
+                    should_close = False
+                    self._client.set_error(field_name, error_message)
+                    self._client.flet_update()
+
+            for field_name, error in self._callbacks.validation_errors.items():
+                if error is not None:
+                    should_close = False
+                    self._client.set_error(field_name, error)
+            self._client.flet_update()
+
+            if should_close:
+                self._client.results["submit"] = label
+                self._client.page.window_destroy()
+
+        return ElevatedButton(label, on_click=validate_and_close)
+
+    @keyword(tags=["dialog", "running"])
+    def clear_dialog(self) -> None:
+        """Clear dialog and results while it is running."""
+        self._client.results = {}
+        self._client.clear_elements()
+
+    @keyword
+    def add_heading(
+        self,
+        heading: str,
+        size: Size = Size.Medium,
+    ) -> None:
+        """Add a centered heading text element
+
+        :param heading: The text content for the heading
+        :param size:    The size of the heading
+
+        Supported ``size`` values are Small, Medium, and Large. By default uses
+        the value Medium.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Add dialog heading
+                Add heading     User information  size=Large
+                Add heading     Location          size=Small
+                Add text input  address           label=User address
+                Run dialog
+
+
+        .. code-block:: python
+
+            def add_dialog_heading():
+                assistant = Assistant()
+                assistant.add_heading("User information", size="large")
+                assistant.add_heading("Location", size="small")
+                assistant.add_text_input("address", label="User address")
+                assistant.run_dialog()
+        """
+        if not isinstance(size, Size):
+            size = Size(size)
+
+        size_dict = {
+            Size.Small: "headlineSmall",
+            Size.Medium: "headlineMedium",
+            Size.Large: "headlineLarge",
+        }
+
+        self._client.add_element(element=Text(heading, style=size_dict[size]))
+
+    @keyword
+    def add_text(
+        self,
+        text: str,
+        size: Size = Size.Medium,
+    ) -> None:
+        """Add a text paragraph element, for larger bodies of text
+
+        :param text: The text content for the paragraph
+        :param size: The size of the text
+
+        Supported ``size`` values are Small, Medium, and Large. By default uses
+        the value Medium.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Show error dialog
+                Add heading   An error occurred
+                Add text      There was an error while requesting user information
+                Add text      ${error}   size=Small
+                Run dialog
+
+        .. code-block:: python
+
+            def show_error_dialog():
+                error = "Your error message"
+                assistant = Assistant()
+                assistant.add_heading("An error occurred")
+                assistant.add_text("There was an error while requesting user information")
+                assistant.add_text(f"{error}", size="small")
+                assistant.run_dialog()
+        """  # noqa: E501
+        if not isinstance(size, Size):
+            size = Size(size)
+
+        if size == Size.Small:
+            self._client.add_element(element=Text(text, style="bodySmall"))
+        elif size == Size.Medium:
+            self._client.add_element(element=Text(text, style="bodyMedium"))
+        elif size == Size.Large:
+            self._client.add_element(element=Text(text, style="bodyLarge"))
+
+    @keyword
+    def add_link(
+        self,
+        url: str,
+        label: Optional[str] = None,
+    ) -> None:
+        """Add an external URL link element
+
+        :param url:   The URL for the link
+        :param label: A custom label text for the link
+
+        Adds a clickable link element, which opens the user's default
+        browser to the given ``url``. Optionally a ``label`` can be given
+        which is shown as the link text, instead of the raw URL.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Display troubleshoot link
+                Add heading    An error occurred
+                Add text       See link for documentation
+                Add link       https://robocorp.com/docs    label=Troubleshooting
+                Run dialog
+
+        .. code-block:: python
+
+            def add_troubleshoot_link():
+                assistant = Assistant()
+                assistant.add_heading("An error occurred")
+                assistant.add_text("See link for documentation")
+                assistant.add_link("https://robocorp.com/docs", label="Troubleshooting")
+                assistant.run_dialog()
+        """
+        if not label:
+            label = url
+        self._client.add_element(
+            Markdown(
+                f"[{label}]({url})",
+                on_tap_link=lambda e: self._client.page.launch_url(e.data),
+            )
+        )
+
+    @keyword
+    def add_image(
+        self,
+        url_or_path: str,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+    ) -> None:
+        """Add an image element, from a local file or remote URL
+
+        :param url_or_path: The location of the image
+        :param width:       The static width of the image, in pixels
+        :param height:      The static height of the image, in pixels
+
+        Adds an inline image to the dialog, which can either
+        point to a local file path on the executing machine or to
+        a remote URL. If it's a local file path it has to be absolute path.
+
+        By default the image is resized to fit the width of the dialog
+        window, but the width and/or height can be explicitly defined
+        to a custom value. If only one of the dimensions is given,
+        the other is automatically changed to maintain the correct aspect ratio.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Display image
+                Add image      C:\\Users\\me\\company-logo.png
+                Add heading    To start, please press the Continue button   size=Small
+                Add submit buttons    Continue
+                Run dialog
+
+        .. code-block:: python
+            def display_image():
+                assistant = Assistant()
+                assistant.add_image("C:\\Users\\me\\company-logo.png")
+                assistant.add_heading("To start, please press the Continue button", size="small")
+                assistant.add_submit_buttons("Continue")
+                assistant.run_dialog()
+        """  # noqa: E501
+
+        is_url = url_or_path.startswith(("http://", "https://"))
+        is_absolute_path = os.path.isabs(url_or_path)
+        is_absolute_and_file_exists = is_absolute_path and os.path.isfile(url_or_path)
+
+        if is_url or is_absolute_and_file_exists:
+            self._client.add_element(
+                Container(content=Image(src=url_or_path, width=width, height=height))
+            )
+        else:
+            self.logger.warning(
+                "The image path you specified should be a valid URL or absolute path "
+                + f" to an existing file. The value provided: {url_or_path}"
+            )
+
+    @keyword
+    def add_file(
+        self,
+        path: str,
+        label: Optional[str] = None,
+    ) -> None:
+        """Add a file element, which links to a local file
+
+        :param path:  The path to the file
+        :param label: A custom label text for the file
+
+        Adds a button which opens a local file with the corresponding
+        default application. Can be used for instance to display generated
+        files from the robot to the end-user.
+
+        Optionally a custom ``label`` can be given for the button text.
+        By default uses the filename of the linked file.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Open file button
+                ${path}=   Generate order files
+                Add heading    Current orders
+                Add file    ${path}    label=Current
+                Run dialog
+
+        .. code-block:: python
+
+            def open_file_button():
+                path = generate_order_files()
+                assistant = Assistant()
+                assistant.add_heading("Current orders")
+                assistant.add_file(path, label="Current")
+                assistant.run_dialog()
+        """
+        resolved = Path(path).resolve()
+        self.logger.info("Adding file: %s", resolved)
+
+        if not resolved.exists():
+            self.logger.warning("File does not exist: %s", resolved)
+
+        def open_file(*_):
+            if platform.system() == "Windows":
+                os.startfile(resolved)  # type: ignore # pylint: disable=no-member
+            elif platform.system() == "Darwin":
+                subprocess.call(["open", resolved])
+            else:
+                subprocess.call(["xdg-open", resolved])
+
+        self._client.add_element(
+            element=ElevatedButton(
+                text=(label or str(resolved)), icon=icons.FILE_OPEN, on_click=open_file
+            )
+        )
+
+    @keyword
+    def add_files(
+        self,
+        pattern: str,
+    ) -> None:
+        """Add multiple file elements according to the given file pattern
+
+        :param pattern: File matching pattern
+
+        See the keyword ``Add file`` for information about the inserted
+        element itself.
+
+        The keyword uses Unix-style glob patterns for finding matching files,
+        and the supported pattern expressions are as follow:
+
+        ========== ================================================
+        Pattern    Meaning
+        ========== ================================================
+        ``*``      Match everything
+        ``?``      Match any single character
+        ``[seq]``  Match any character in seq
+        ``[!seq]`` Match any character not in seq
+        ``**``     Match all files, directories, and subdirectories
+        ========== ================================================
+
+        If a filename has any of these special characters, they
+        can be escaped by wrapping them with square brackets.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Open multiple files buttons
+                # Add all excel files
+                Add files    *.xlsx
+
+                # Add all log files in any subdirectory
+                Add files    **/*.log
+
+                # Add all PDFs between order0 and order9
+                Add files    order[0-9].pdf
+
+        .. code-block:: python
+
+            def open_multiple_files_buttons():
+                assistant = Assistant()
+                # Add all excel files
+                assistant.add_file("*.xlsx")
+                # Add all log files in any subdirectory
+                assistant.add_file("**/*.log")
+                # Add all PDFs between order0 and order9
+                assistant.add_file("order[0-9].pdf")
+                assistant.run_dialog()
+        """
+        matches = glob.glob(pattern, recursive=True)
+        for match in sorted(matches):
+            self.add_file(match)
+
+    @keyword
+    def add_icon(self, variant: Icon, size: int = 48) -> None:
+        """Add an icon element from RPA.Assistant's short icon list.
+
+        :param variant: The icon type
+        :param size:    The size of the icon
+
+        Adds an icon which can be used to indicate status
+        or the type of dialog being presented.
+
+        The currently supported icon types are:
+
+        ======= ==========================
+        Name    Description
+        ======= ==========================
+        Success A green check mark
+        Warning An orange warning triangle
+        Failure A red cross or X mark
+        ======= ==========================
+
+        The ``size`` of the icon can also be changed,
+        to a given height/width of pixels.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Confirmation dialog
+                Add icon              Warning    size=64
+                Add heading           Do you want to delete this order?
+                Add submit buttons    buttons=No,Yes
+                ${result}=    Run dialog
+
+        .. code-block:: python
+
+            def confirmation_dialog():
+                assistant = Assistant()
+                assistant.add_icon("warning", size="64")
+                assistant.add_heading("Do you want to delete this order?")
+                assistant.add_submit_buttons(buttons="No, Yes")
+                result = assistant.run_dialog()
+        """
+        if not isinstance(variant, Icon):
+            variant = Icon(variant)
+
+        flet_icon_conversions: Dict[Icon, Tuple[str, str]] = {
+            Icon.Success: (icons.CHECK, colors.GREEN_500),
+            Icon.Warning: (icons.WARNING, colors.YELLOW_500),
+            Icon.Failure: (icons.CLOSE, colors.RED_500),
+        }
+        flet_icon, color = flet_icon_conversions[variant]
+
+        self._client.add_element(flet.Icon(name=flet_icon, color=color, size=size))
+
+    @keyword
+    def add_flet_icon(
+        self,
+        icon: str,
+        color: Optional[str] = None,
+        size: Optional[int] = 24,
+    ):
+        """Add an icon from a large gallery of icons.
+
+        :param icon:      Corresponding flet icon name. Check
+                          https://gallery.flet.dev/icons-browser/ for a list of icons.
+                          Write the name in ``lower_case``
+        :param color:     Color for the icon. Default depends on icon. Allowed values
+                          are colors from
+                          https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37
+                          or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).
+        :param size:      Integer size for the icon.
+
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Add custom icon
+                Add Heading    Check icon
+                Add Flet Icon  icon_name=check_circle_rounded  color=FF00FF  size=48
+                Run Dialog
+
+        .. code-block:: python
+
+            def add_custom_icon()
+                assistant = Assistant()
+                assistant.add_heading("Check icon")
+                assistant.add_flet_icon(icon="check_circle_rounded", color="FF00FF", size="48")
+                assistant.run_dialog()
+        """  # noqa: E501
+
+        self._client.add_element(flet.Icon(name=icon, color=color, size=size))
+
+    @keyword(tags=["input"])
+    def add_text_input(
+        self,
+        name: str,
+        label: Optional[str] = None,
+        placeholder: Optional[str] = None,
+        validation: Optional[Union[Callable, str]] = None,
+        default: Optional[str] = None,
+        required: bool = False,
+        minimum_rows: Optional[int] = None,
+        maximum_rows: Optional[int] = None,
+    ) -> None:
+        """Add a text input element
+
+        :param name:        Name of result field
+        :param label:       Label for field
+        :param placeholder: Placeholder text in input field
+        :param validation:   Validation function for the input field
+        :param default:     Default value if the field wasn't completed
+        :param required:    If true, will display an error if not completed
+        :param minimum_rows: Minimum number of rows to display for the input field
+        :param maximum_rows: Maximum number of rows to display for the input field, the
+                             input content can be longer but a scrollbar will appear
+
+        Adds a text field that can be filled by the user. The entered
+        content will be available in the ``name`` field of the result.
+
+        For customizing the look of the input, the ``label`` text can be given
+        to add a descriptive label and the ``placholder`` text can be given
+        to act as an example of the input value.
+
+        The `default` value will be assigned to the input field if the user
+        doesn't complete it. If provided, the placeholder won't be shown.
+        This is `None` by default. Also, if a default value is provided
+        and the user deletes it, `None` will be the corresponding value in
+        the results dictionary.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Send feedback
+                Add heading    Send feedback
+                Add text input    email    label=E-mail address
+                Add text input    message
+                ...    label=Feedback
+                ...    placeholder=Enter feedback here
+                ${result}=    Run dialog
+                Send feedback message    ${result.email}  ${result.message}
+
+        Validation example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Validate Email
+                [Arguments]    ${email}
+                # E-mail specification is complicated, this matches that the e-mail has
+                # at least one character before and after the @ sign, and at least one
+                # character after the dot.
+                ${regex}=    Set Variable    ^.+@.+\\..+
+                ${valid}=    Run Keyword And Return Status    Should Match Regexp  ${email}  ${regex}
+                IF  not $valid
+                    RETURN  Invalid email address
+                END
+
+            Open Dialog
+                Add heading    Send feedback
+                Add text input    email
+                ...    label=Email
+                ...    validation=Validate Email
+                ${result}=    Run dialog
+                Log  ${result.email}
+
+        .. code-block:: python
+
+            import re
+            def validate_email(email):
+                # E-mail specification is complicated, this matches that the e-mail has
+                # at least one character before and after the @ sign, and at least one
+                # character after the dot.
+                regex = r"^.+@.+\\..+"
+                valid = re.match(regex, email)
+                if not valid:
+                    return "Invalid email address"
+
+            def open_dialog():
+                assistant.add_heading("Send feedback")
+                assistant.add_text_input("email", label="Email", validation=validate_email)
+                result = run_dialog()
+                print(result.email)
+
+
+
+        """  # noqa: E501
+        validation_function = None
+        if validation:
+            if isinstance(validation, str):
+                validation_function = self._callbacks.robot_validation(name, validation)
+            elif isinstance(validation, Callable):
+                validation_function = self._callbacks.python_validation(
+                    name, validation
+                )
+            else:
+                raise ValueError("Invalid validation function.")
+
+        if required:
+            self._required_fields.add(name)
+
+        self._client.results[name] = default
+
+        def empty_string_to_none(e):
+            if e.control.value == "":
+                e.data = None
+
+        if minimum_rows or maximum_rows:
+            multiline = True
+        else:
+            multiline = None
+
+        self._client.add_element(
+            name=name,
+            element=TextField(
+                label=label,
+                hint_text=placeholder,
+                value=default,
+                min_lines=minimum_rows,
+                max_lines=maximum_rows,
+                multiline=multiline,
+            ),
+            extra_handler=empty_string_to_none,
+            validation_func=validation_function,
+        )
+
+    @keyword(tags=["input"])
+    def add_password_input(
+        self,
+        name: str,
+        label: Optional[str] = None,
+        placeholder: Optional[str] = None,
+    ) -> None:
+        """Add a password input element
+
+        :param name:        Name of result field
+        :param label:       Label for field
+        :param placeholder: Placeholder text in input field
+
+        Adds a text field that hides the user's input. The entered
+        content will be available in the ``name`` field of the result.
+
+        For customizing the look of the input, the ``label`` text can be given
+        to add a descriptive label and the ``placholder`` text can be given
+        to act as an example of the input value.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Change password
+                Add heading    Change password
+                Add text input        username    label=Current username
+                Add password input    password    label=New password
+                Add submit buttons    buttons=Submit
+                ${result}=    Run dialog
+                Change user password    ${result.username}  ${result.password}
+
+        .. code-block:: python
+
+            def change_password():
+                assistant = Assistant()
+                assistant.add_heading("Change password")
+                assistant.add_text_input("username", label="Current username")
+                assistant.add_password_input("password", label="New password")
+                assistant.add_submit_buttons(buttons="Submit")
+                result = assistant.run_dialog()
+                change_user_password(result.username, result.password)
+        """
+        self._client.add_element(
+            name=name, element=TextField(label=label, value=placeholder, password=True)
+        )
+
+    @keyword(tags=["input"])
+    def add_hidden_input(
+        self,
+        name: str,
+        value: str,
+    ) -> None:
+        """Add a hidden input element
+
+        :param name:  Name of result feild
+        :param value: Value for input
+
+        Adds a special hidden result field that is not visible
+        to the user and always contains the given static value.
+
+        Can be used to keep user input together with already known
+        values such as user IDs, or to ensure that dialogs with differing
+        elements all have the same fields in results.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Get user information
+                Add hidden input   user_id   ${USER_ID}
+                Add text input     username
+                ${result}=         Run dialog
+                Enter user information    ${result.user_id}    ${result.username}
+
+        .. code-block:: python
+
+            def get_user_information():
+                assistant = Assistant()
+                user_id = "Your user value"
+                assistant.add_hidden_input("user_id", user_id)
+                assistant.add_text_input("username")
+                result = assistant.run_dialog()
+                enter_user_information(result.user_id, result.username)
+        """
+        self._client.results[name] = value
+
+    @keyword(tags=["input"])
+    def add_file_input(
+        self,
+        name: str,
+        label: Optional[str] = None,
+        source: Optional[str] = None,
+        file_type: Optional[str] = None,
+        multiple: bool = False,
+    ) -> None:
+        """Add a file input element
+
+        :param name:        Name of result field
+        :param label:       Label for input field
+        :param source:      Default source directory
+        :param file_type:   Accepted file types
+        :param multiple:    Allow selecting multiple files
+
+        Adds a native file selection dialog for inputting one or more files.
+        The list of selected files will be available in the ``name`` field
+        of the result.
+
+        By default opens up in the user's home directory, but it can be
+        set to a custom path with the ``source`` argument.
+
+        The argument ``file_type`` restricts the possible file extensions
+        that the user can select. The format of the argument is as follows:
+        ``pdf,png,svg``. For instance, an argument
+        to limit options to Excel files could be: ``xls,xlsx``.
+
+        To allow selecting more than one file, the ``multiple`` argument
+        can be enabled.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Multiple file selections
+                # This can be any one file
+                Add file input    name=anything
+
+                # This can be multiple files
+                Add file input    name=multiple  multiple=True
+
+                # This opens the select dialog to a custom folder
+                Add file input    name=src       source=C:\\Temp\\Output\\
+
+                # This restricts files to certain types
+                Add file input    name=types     file_type=pdf
+
+                # Every file input result is a list of paths
+                ${result}=    Run dialog
+                FOR    ${path}    IN    @{result.multiple}
+                    Log    Selected file: ${path}
+                END
+
+        .. code-block:: python
+
+            def multiple_file_selections():
+                assistant = Assistant()
+                # This can be any one file
+                assistant.add_file_input(name="anything")
+
+                # This can be multiple files
+                assistant.add_file_input(name="multiple", multiple=True)
+
+                # This opens the select dialog to a custom folder
+                assistant.add_file_input(name="src", source="C:\\Temp\\Output")
+
+                # This restricts files to certain types
+                assistant.add_file_input(name="types", file_type="pdf")
+
+                # Every file input result is a list of paths
+                result = assistant.run_dialog()
+                for path in result.multiple:
+                    print("Selected file: ", path)
+        """
+
+        def on_pick_result(event: FilePickerResultEvent):
+            if event.files:
+                self._client.results[str(name)] = [f.path for f in event.files]
+                selected_files.value = (
+                    ", ".join(map(lambda f: f.name, event.files))
+                    if event.files
+                    else "Cancelled!"
+                )
+                selected_files.update()
+
+        file_picker = FilePicker(on_result=on_pick_result)
+        self._client.add_invisible_element(file_picker)
+        selected_files = Text()
+
+        options = {
+            "source": optional_str(source),
+            "file_type": optional_str(file_type),
+        }
+
+        if not options["source"]:
+            options["source"] = os.path.expanduser("~")
+
+        if options["file_type"]:
+            options["file_type"] = options["file_type"].split(",")
+
+        self._client.add_element(
+            Row(
+                [
+                    ElevatedButton(
+                        label or "Choose files...",
+                        on_click=lambda _: file_picker.pick_files(
+                            allow_multiple=bool(multiple),
+                            initial_directory=options["source"],
+                            allowed_extensions=options["file_type"],
+                        ),
+                    ),
+                    selected_files,
+                ]
+            )
+        )
+
+    @keyword("Add Drop-Down", tags=["input"])
+    def add_drop_down(
+        self,
+        name: str,
+        options: Options,
+        default: Optional[str] = None,
+        label: Optional[str] = None,
+    ) -> None:
+        """Add a drop-down element
+
+        :param name:    Name of result field
+        :param options: List of drop-down options
+        :param default: The default selection
+        :param label:   Label for input field
+
+        Creates a drop-down menu with the given ``options``. The selection
+        the user makes will be available in the ``name`` field of the result.
+
+        The ``default`` argument can be one of the defined options,
+        and the dialog automatically selects that option for the input.
+
+        A custom ``label`` text can also be added.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Select user type from drop down
+                Add heading     Select user type
+                Add drop-down
+                ...    name=user_type
+                ...    options=Admin,Maintainer,Operator
+                ...    default=Operator
+                ...    label=User type
+                ${result}=      Run dialog
+                Log    User type should be: ${result.user_type}
+
+        .. code-block:: python
+
+            def select_user_type_from_drop_down():
+                assistant = Assistant()
+                assistant.add_heading("Select user type")
+                assistant.add_drop_down(
+                    name="user_type",
+                    options="Admin,Maintainer,Operator",
+                    default="Operator",
+                    label="User type"
+                )
+                result = assistant.run_dialog()
+                print("User type should be: ", result.user_type)
+        """
+        options, default = to_options(options, default)
+        options: List[Control] = list(map(Option, options))
+        dropdown = Dropdown(options=options, value=default)
+
+        self._client.results[name] = default
+        self._client.add_element(Text(value=label))
+        self._client.add_element(dropdown, name=str(name))
+
+    @keyword(tags=["input"])
+    def add_date_input(
+        self,
+        name: str,
+        default: Optional[Union[date, str]] = None,
+        label: Optional[str] = None,
+    ) -> None:
+        """Add a date input element.
+
+        :param name:    Name of the result field
+        :param default: The default set date
+        :param label:   Label for the date input field
+
+        Displays a date input. The selection the user makes will be available
+        as a ``date`` object in the ``name`` field of the result.
+        The ``default`` argument can be a pre-set date as object or string in
+        "YYYY-MM-DD" format, otherwise the current date is used.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Select birthdate
+                Add heading       Enter your birthdate
+                Add Date Input    birthdate    default=1993-04-26
+                ${result} =       Run dialog
+                Log To Console    User birthdate year should be: ${result.birthdate.year}
+
+        .. code-block:: python
+
+            def select_birthdate():
+                assistant = Assistant()
+                assistant.add_heading("Enter your birthdate")
+                assistant.add_date_input("birthdate", default="1993-04-26")
+                result = assistant.run_dialog()
+                print("User birthdate year should be: ", result.birthdate.year)
+        """  # noqa: E501
+
+        def validate(date_text: str):
+            if not date_text:
+                return None
+            try:
+                date.fromisoformat(date_text)
+                return None
+            except ValueError:
+                return "Date should be in format YYYY-MM-DD"
+
+        if default:
+            if isinstance(default, str):
+                try:
+                    default = date.fromisoformat(default)
+                except ValueError as e:
+                    self.logger.error(
+                        f"Default date value {default} is not in a valid ISO format."
+                    )
+                    raise e
+            self._client.results[name] = default
+
+        self._client.date_inputs.append(name)
+        self._client.add_element(
+            name=name,
+            element=TextField(label=label, hint_text="YYYY-MM-DD", value=default),
+            validation_func=self._callbacks.python_validation(name, validate),
+        )
+
+    @keyword(tags=["input"])
+    def add_radio_buttons(
+        self,
+        name: str,
+        options: Options,
+        default: Optional[str] = None,
+        label: Optional[str] = None,
+    ) -> None:
+        """Add radio button elements
+
+        :param name:    Name of result field
+        :param options: List of drop-down options
+        :param default: The default selection
+        :param label:   Label for input field
+
+        Creates a set of radio buttons with the given ``options``. The selection
+        the user makes will be available in the ``name`` field of the result.
+
+        The ``default`` argument can be one of the defined options,
+        and the dialog automatically selects that option for the input.
+
+        A custom ``label`` text can also be added.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Select user type from radio buttons
+                Add heading     Select user type
+                Add radio buttons
+                ...    name=user_type
+                ...    options=Admin,Maintainer,Operator
+                ...    default=Operator
+                ...    label=User type
+                ${result}=      Run dialog
+                Log    User type should be: ${result.user_type}
+
+        .. code-block:: python
+
+            def select_user_type_from_radio_buttons():
+                assistant = Assistant()
+                assistant.add_heading("Select user type")
+                assistant.add_radio_buttons(
+                    name="user_type",
+                    options="Admin,Maintainer,Operator",
+                    default="Operator",
+                    label="User type"
+                )
+                result = assistant.run_dialog()
+                print("User type should be: ", result.user_type)
+        """
+        options, default = to_options(options, default)
+        radios: List[Control] = [
+            Radio(value=option, label=option) for option in options
+        ]
+        radio_group = RadioGroup(content=Column(radios), value=default)
+
+        self._client.results[name] = default
+        self._client.add_element(Text(value=label))
+        self._client.add_element(radio_group, name=str(name))
+
+    @keyword(tags=["input"])
+    def add_checkbox(
+        self,
+        name: str,
+        label: str,
+        default: bool = False,
+    ) -> None:
+        """Add a checkbox element
+
+        :param name:    Name of result field
+        :param label:   Label text for checkbox
+        :param default: Default checked state
+
+        Adds a checkbox that indicates a true or false value.
+        The selection will be available in the ``name`` field of the result,
+        and the ``label`` text will be shown next to the checkbox.
+
+        The boolean ``default`` value will define the initial checked
+        state of the element.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Select checkboxes
+                Add heading     Enable features
+                Add checkbox    name=vault        label=Enable vault       default=True
+                Add checkbox    name=triggers     label=Enable triggers    default=False
+                Add checkbox    name=assistants   label=Enable assistants  default=True
+                ${result}=      Run dialog
+                IF    $result.vault
+                    Enable vault
+                END
+
+        .. code-block:: python
+
+            def select_checkboxes():
+                assistant = Assistant()
+                assistant.add_heading("Enable features")
+                assistant.add_checkbox(name="vault", label="Enable vault", default=True)
+                assistant.add_checkbox(name="triggers", label="Enable triggers", default=False)
+                assistant.add_checkbox(name="assistants", label="Enable assistants", default=True)
+                result = assistant.run_dialog()
+                if(result.vault):
+                    enable_vault()
+
+        """  # noqa: E501
+        self._client.results[name] = default
+        self._client.add_element(
+            name=str(name), element=Checkbox(label=str(label), value=bool(default))
+        )
+
+    @keyword(tags=["input"])
+    def add_submit_buttons(
+        self, buttons: Options, default: Optional[str] = None
+    ) -> None:
+        """Add custom submit buttons
+
+        :param buttons: Submit button options
+        :param default: The primary button
+
+        The result field will always be called ``submit`` and will contain
+        the pressed button text as a value.
+
+        If one of the custom ``options`` should be the preferred option,
+        the ``default`` argument controls which one is highlighted with
+        an accent color.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Delete user warning
+                Add icon      Warning
+                Add heading   Delete user ${username}?
+                Add submit buttons    buttons=No,Yes    default=Yes
+                ${result}=    Run dialog
+                IF   $result.submit == "Yes"
+                    Delete user    ${username}
+                END
+
+        .. code-block:: python
+
+            def delete_user_warning():
+                assistant = Assistant()
+                username = "user_01"
+                assistant.add_icon("warning")
+                assistant.add_heading(f"Delete user {username}?")
+                assistant.add_submit_buttons(buttons="No, Yes", default="Yes")
+                result = assistant.run_dialog()
+                if result.submit == "Yes":
+                    delete_user(username)
+        """
+        button_labels, default = to_options(buttons, default)
+
+        button_elements = [
+            self._create_closing_button(button) for button in button_labels
+        ]
+        for button in button_elements:
+            self._client.add_to_disablelist(button)
+
+        button_row = Row(button_elements, alignment=MainAxisAlignment.END)
+        container = Container(button_row, alignment=alignment.bottom_right)
+        self._client.add_element(container)
+
+    @keyword(tags=["dialog"])
+    def run_dialog(
+        self,
+        timeout: int = 180,
+        title: str = "Assistant",
+        height: Union[int, Literal["AUTO"]] = "AUTO",
+        width: int = 480,
+        on_top: bool = False,
+        location: Union[WindowLocation, Tuple[int, int], None] = None,
+    ) -> Result:
+        """Create a dialog from all the defined elements and block
+        until the user has handled it.
+
+        :param timeout: Time to wait for dialog to complete, in seconds
+        :param title:  Title of dialog
+        :param height: Height of dialog (in pixels or 'AUTO')
+        :param width:  Width of dialog (in pixels)
+        :param on_top: Show dialog always on top of other windows
+        :param location: Where to place the dialog (options are Center, TopLeft, or a
+                         tuple of ints)
+
+        If the `location` argument is `None` it will let the operating system
+        place the window.
+
+        Returns a result object with all input values.
+
+        When the dialog closes elements are cleared.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Open dialog
+                Add heading     Please enter your username
+                Add text input  name=username
+                ${result}=      Run dialog
+                Log    The username is: ${result.username}
+
+        .. code-block:: python
+
+            def open_dialog():
+                assistant = Assistant()
+                assistant.add_heading("Please enter your username")
+                assistant.add_text_input("username")
+                result = assistant.run_dialog()
+                print("The username is: ", result.username)
+        """
+
+        # height has to be either AUTO or an int value
+        if not isinstance(height, int) and height != "AUTO":
+            height = int(height)
+
+        # if location is given as a string (Robot autoconversion doesn't work) parse it
+        # to enum manually
+        if isinstance(location, str):
+            location = WindowLocation[location]
+
+        self._client.display_flet_window(
+            title, height, width, on_top, location, timeout
+        )
+        results = self._get_results()
+        self._client.results.clear()
+
+        return results
+
+    def _get_results(self) -> DotDict:
+        results = self._client.results
+        for name, value in results.items():
+            if name in self._client.date_inputs and isinstance(value, str):
+                results[name] = date.fromisoformat(value)
+        return DotDict(**results)
+
+    @keyword(tags=["dialog"])
+    def ask_user(self, timeout: int = 180, **options: Any) -> Result:
+        """Same as ``Run Dialog`` it will create a dialog from all the defined
+        elements and block until the user has handled it. It will also add
+        by default a submit and close buttons.
+
+        :param timeout: Time to wait for dialog to complete, in seconds
+        :param options: Options for the dialog
+
+        Returns a result object with all input values.
+
+        For more information about possible options for opening the dialog,
+        see the documentation for the keyword ``Run Dialog``.
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Ask user dialog
+                Add heading     Please enter your username
+                Add text input  name=username
+                ${result}=      Ask User
+                Log    The username is: ${result.username}
+
+        .. code-block:: python
+
+            def ask_user_dialog():
+                assistant = Assistant()
+                assistant.add_heading("Please enter your username")
+                assistant.add_text_input("username")
+                result = assistant.ask_user()
+                print("The username is: ", result.username)
+        """
+
+        self.add_submit_buttons(["Submit", "Close"], "Submit")
+        return self.run_dialog(**options, timeout=timeout)
+
+    @keyword(tags=["dialog", "running"])
+    def refresh_dialog(self):
+        """Can be used to update UI elements when adding elements while dialog is
+        running
+        """
+        self._client.update_elements()
+
+    @keyword(tags=["dialog"])
+    def add_button(
+        self,
+        label: str,
+        function: Union[Callable, str],
+        *args,
+        location: VerticalLocation = VerticalLocation.Left,
+        **kwargs,
+    ) -> None:
+        """Create a button and execute the `function` as a callback when pressed.
+
+        :param label: Text for the button
+        :param function: Python function or Robot Keyword name, that will get ``*args``
+            and ``**kwargs`` passed into it
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            First View
+                Add Heading  Here is the first view of the app
+                Add Button  Change View  Second View
+
+            Second View
+                Add Heading  Let's build an infinite loop
+                Add Button  Change View  First View
+
+        .. code-block:: python
+
+            def first_view():
+                assistant = Assistant()
+                assistant.add_heading("Here is the first view of the app")
+                assistant.add_button("Change view", second_view)
+                assistant.run_dialog()
+
+            def second_view():
+                assistant = Assistant()
+                assistant.add_heading("Let's build an infinite loop")
+                assistant.add_button("Change view", first_view)
+                assistant.run_dialog()
+        """  # noqa: E501
+
+        def on_click(_: ControlEvent):
+            self._callbacks.queue_fn_or_kw(function, *args, **kwargs)
+
+        button = ElevatedButton(label, on_click=on_click)
+        container = Container(alignment=location.value, content=button)
+        self._client.add_element(container)
+        self._client.add_to_disablelist(button)
+
+    @keyword(tags=["dialog"])
+    def add_next_ui_button(self, label: str, function: Union[Callable, str]):
+        """Create a button that leads to the next UI page, calling the passed
+        keyword or function, and passing current form results as first positional
+        argument to it.
+
+        :param label: Text for the button
+        :param function: Python function or Robot Keyword name, that will take form
+            results as its first argument
+
+        Example:
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Retrieve User Data
+                # Retrieves advanced data that needs to be displayed
+
+            Main Form
+                Add Heading  Username input
+                Add Text Input  name=username_1  placeholder=username
+                Add Next Ui Button        Show customer details  Customer Details
+
+            Customer Details
+                [Arguments]  ${form}
+                ${user_data}=  Retrieve User Data  ${form}[username_1]
+                Add Heading  Retrieved Data
+                Add Text  ${user_data}[phone_number]
+                Add Text  ${user_data}[address]
+
+        .. code-block:: python
+
+            def main_form():
+                assistant = Assistant()
+                assistant.add_heading("Username input")
+                assistant.add_text_input("username_1", placeholder="username")
+                assistant.add_next_ui_button("Show customer details", customer_details)
+                assistant.run_dialog()
+
+            def customer_details(form):
+                assistant = Assistant()
+                user_data = retrieve_user_data(form.username_1)
+                assistant.add_heading("Retrieved Data")
+                assistant.add_text(user_data[phone_number])
+                assistant.add_text(user_data[address])
+                assistant.run_dialog()
+        """
+
+        def on_click(_: ControlEvent):
+            self._callbacks.queue_fn_or_kw(function, self._get_results())
+
+        button = ElevatedButton(label, on_click=on_click)
+        self._client.add_element(button)
+        self._client.add_to_disablelist(button)
+
+    @keyword(tags=["input"])
+    def add_slider(
+        self,
+        name: str,
+        slider_min: Union[int, float] = 0,
+        slider_max: Union[int, float] = 100,
+        thumb_text="{value}",
+        steps: Optional[int] = None,
+        default: Optional[Union[int, float]] = None,
+        decimals: Optional[int] = 1,
+    ):
+        """Add a slider input.
+
+        :param name:        Name of result field
+        :param slider_min:  Minimum value of the slider
+        :param slider_max:  Maximum value of the slider
+        :param thumb_label: Text to display when the slider is being slided. Use the
+                            placeholder {value} for the number. (thumb text `{value%}`
+                            will display values: `0%`, `100%`)
+        :param steps:       Amount of steps for the slider. If None, the slider will be
+                            continuous.
+                            For integer output, specify a steps value where all the
+                            steps will be integers, or implement rounding when
+                            retrieving the result.
+        :param default:     Default value for the slider. Must be between min and max.
+        :param decimals:    How many decimals should the value have and show.
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Create Percentage Slider
+                Add Text    Percentage slider
+                Add Slider  name=percentage  slider_min=0  slider_max=100
+                            thumb_text={value}%  steps=100  round=1
+
+        .. code-block:: python
+
+            def create_percentage_slider():
+                assistant = Assistant()
+                assistant.add_text("Percentage slider")
+                assistant.add_slider(
+                    name="percentage",
+                    slider_min=0,
+                    slider_max=100,
+                    thumb_text="{value}%",
+                    steps=100,
+                    decimals=1
+                )
+                assistant.run_dialog()
+        """
+        if default:
+            default = float(default)
+
+            # Is this even necessary?
+            if default.is_integer():
+                default = int(default)
+
+            if slider_min > default or slider_max < default:
+                raise ValueError(f"Slider {name} had an out of bounds default value.")
+            self._client.results[name] = default
+
+        slider = Slider(
+            min=slider_min,
+            max=slider_max,
+            divisions=steps,
+            label=thumb_text,
+            value=default,
+            round=decimals,
+        )
+        self._client.add_element(name=name, element=slider)
+
+    @keyword(tags=["dialog", "running"])
+    def add_loading_spinner(
+        self,
+        name: str,
+        width: int = 16,
+        height: int = 16,
+        stroke_width: int = 2,
+        color: Optional[str] = None,
+        tooltip: Optional[str] = None,
+        value: Optional[float] = None,
+    ):
+        """Add a loading spinner.
+
+        :param name:        Name of the element
+        :param width:       Width of the spinner
+        :param height:      Height of the spinner
+        :param stroke_width: Width of the spinner's stroke
+        :param color:       Color of the spinner's stroke.
+                            Allowed values are colors from
+                            [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
+                            or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
+        :param tooltip:     Tooltip to be displayed
+                            on mouse hover.
+        :param value:       Between 0.0 and 1.0 if you want to manually control it's completion.
+                            If `None` it will spin endlessy.
+        """  # noqa: E501
+        pr = flet.ProgressRing(
+            width=width,
+            height=height,
+            stroke_width=stroke_width,
+            color=color,
+            tooltip=tooltip,
+            value=value,
+        )
+        self._client.add_element(pr, name)
+        return pr
+
+    @keyword(tags=["dialog", "running"])
+    def add_loading_bar(
+        self,
+        name: str,
+        width: int = 16,
+        bar_height: int = 16,
+        color: Optional[str] = None,
+        tooltip: Optional[str] = None,
+        value: Optional[float] = None,
+    ):
+        """Add a loading bar.
+
+        :param name:        Name of the element
+        :param width:       Width of the bar
+        :param bar_height:  Height of the bar
+        :param color:       Color of the bar's stroke.
+                            Allowed values are colors from
+                            [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
+                            or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
+        :param tooltip:     Tooltip to be displayed on mouse hover.
+        :param value:       Between 0.0 and 1.0 if you want to manually control it's completion.
+                            Use `None` for indeterminate progress indicator.
+        """  # noqa: E501
+        pb = flet.ProgressBar(
+            width=width,
+            bar_height=bar_height,
+            color=color,
+            tooltip=tooltip,
+            value=value,
+        )
+        self._client.add_element(pb, name)
+        return pb
+
+    @keyword(tags=["dialog", "running"])
+    def set_title(self, title: str):
+        """Set dialog title when it is running."""
+        self._client.set_title(title)
+
+    def _close_layouting_element(self, layouting_element: str):
+        """Check if the last opened layout element matches what is being closed,
+        otherwise raise `ValueError`. If the check passes, close the layout element.
+        """
+        if not self._open_layouting:
+            raise LayoutError(f"Cannot close {layouting_element}, no open layout")
+
+        last_opened = self._open_layouting[-1]
+        if not last_opened == layouting_element:
+            raise LayoutError(
+                f"Cannot close {layouting_element}, last opened layout is {last_opened}"
+            )
+
+        self._client.close_layout()
+        self._open_layouting.pop()
+
+    @keyword(tags=["layout"])
+    def open_row(self):
+        """Open a row layout container. Following ``Add <element>`` calls will add
+        items into that row until ``Close Row`` is called.
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Side By Side Elements
+                Open Row
+                Add Text  First item on the row
+                Add Text  Second item on the row
+                Close Row
+
+        .. code-block:: python
+
+            def side_by_side_elements():
+                assistant = Assistant()
+                assistant.open_row()
+                assistant.add_text("First item on the row")
+                assistant.add_text("Second item on the row")
+                assistant.close_row()
+                assistant.run_dialog()
+        """
+        self._open_layouting.append("Row")
+        self._client.add_layout(Row())
+
+    @keyword(tags=["layout"])
+    def close_row(self):
+        """Close previously opened row.
+
+        Raises LayoutError if called with no Row open, or if another layout element was
+        opened more recently than a row.
+        """
+        self._close_layouting_element("Row")
+
+    @keyword(tags=["layout"])
+    def open_container(
+        self,
+        margin: Optional[int] = 5,
+        padding: Optional[int] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        background_color: Optional[str] = None,
+        location: Union[Location, Tuple[int, int], None] = None,
+    ):
+        """Open a single element container. The following ``Add <element>`` calls adds
+        an element inside the container. Can be used for styling elements.
+
+
+        :param margin: How much margin to add around the container. RPA.Assistant adds
+                       by default a container of margin 5 around all elements, to have
+                       a smaller margin use containers with smaller margin value for
+                       elements.
+        :param padding: How much padding to add around the content of the container.
+        :param width: Width of the container.
+        :param height: Height of the container.
+
+        :param bgcolor:   Background color for the container. Default depends on icon.
+                          Allowed values are colors from
+                          [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
+                          or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
+        :param location:  Where to place the container (A Location value or tuple of
+                          ints). Only works inside a Stack layout element.
+
+                          To use any Center___ or ___Center locations you must define
+                          width and height to the element.
+
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Padded Element With Background
+                Open Container  padding=20  background_color=blue500
+                Add Text        sample text
+                Close Container
+
+        .. code-block:: python
+
+            def padded_element_with_background():
+                assistant = Assistant()
+                assistant.open_container(padding=20, background_color="blue500")
+                assistant.add_text("Sample text")
+                assistant.close_container()
+                assistant.run_dialog()
+        """  # noqa: E501
+        self._open_layouting.append("Container")
+        if not location:
+            top, left, bottom, right = None, None, None, None
+        else:
+            parent_height, parent_width = self._client.get_layout_dimensions()
+            parsed_location = location_to_absolute(
+                location, parent_width, parent_height, width, height
+            )
+            top = parsed_location.get("top")
+            left = parsed_location.get("left")
+            right = parsed_location.get("right")
+            bottom = parsed_location.get("bottom")
+        self._client.add_layout(
+            Container(
+                margin=margin,
+                padding=padding,
+                width=width,
+                height=height,
+                bgcolor=background_color,
+                top=top,
+                left=left,
+                bottom=bottom,
+                right=right,
+            )
+        )
+
+    @keyword(tags=["layout"])
+    def close_container(self):
+        """Close previously opened container.
+
+        Raises LayoutError if called with no Row open, or if another layout element was
+        opened more recently than a row.
+        """
+        self._close_layouting_element("Container")
+
+    @keyword(tags=["layout"])
+    def open_navbar(self, title: Optional[str] = None):
+        """Create a Navigation Bar. Following ``Add <element>`` calls will add
+        items into the Navbar until ``Close Navbar`` is called.
+
+        Navbar doesn't clear when Clear Dialog is called.
+
+        Only one Navbar can be initialized at a time. Trying to make a second one will
+        raise a LayoutError.
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+                Go To Start Menu
+                    Add Heading  Start menu
+                    Add Text  Start menu content
+
+                Assistant Navbar
+                    Open Navbar  title=Assistant
+                    Add Button   menu  Go To Start Menu
+                    Close Navbar
+
+        .. code-block:: python
+
+            def go_to_start_menu():
+                assistant = Assistant()
+                assistant.add_heading("Start menu")
+                assistant.add_text("Start menu content")
+                assistant.run_dialog()
+
+            def assistant_navbar():
+                assistant = Assistant()
+                assistant.open_navbar(title="Assistant")
+                assistant.add_button("menu", go_to_start_menu)
+                assistant.close_navbar()
+                assistant.run_dialog()
+        """
+        self._open_layouting.append("AppBar")
+        self._client.set_appbar(AppBar(title=Text(title)))
+
+    @keyword(tags=["layout"])
+    def close_navbar(self):
+        """Close previously opened navbar.
+
+        Raises LayoutError if called with no Row open, or if another layout element was
+        opened more recently than a row."""
+        self._close_layouting_element("AppBar")
+
+    @keyword(tags=["layout"])
+    def open_stack(self, width: Optional[int] = None, height: Optional[int] = None):
+        """Create a "Stack" layout element. Stack can be used to position elements
+        absolutely and to have overlapping elements in your layout. Use Container's
+        `top` and `left` arguments to position the elements in a stack.
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Absolutely Positioned Elements
+                # Positioning containers with relative location values requires
+                # absolute size for the Stack
+                Open Stack  height=360  width=360
+
+                Open Container  width=64  height=64  location=Center
+                Add Text  center
+                Close Container
+
+                Open Container  width=64  height=64  location=TopRight
+                Add Text  top right
+                Close Container
+
+                Open Container  width=64  height=64  location=BottomRight
+                Add Text  bottom right
+                Close Container
+
+                Close Stack
+
+        .. code-block:: python
+
+            def absolutely_positioned_elements():
+                # Positioning containers with relative location values requires
+                # absolute size for the Stack
+                assistant = Assistant()
+                assistant.open_stack(height=360, width=360)
+
+                assistant.open_container(width=64, height=64, location=Center)
+                assistant.add_text("center")
+                assistant.close_container()
+
+                assistant.open_container(width=64, height=64, location=TopRight)
+                assistant.add_text("top right")
+                assistant.close_container()
+
+                assistant.open_container(width=64, height=64, location=BottomRight)
+                assistant.add_text("bottom right")
+                assistant.close_container()
+
+                assistant.close_stack()
+                assistant.run_dialog()
+
+        """
+        self._open_layouting.append("Stack")
+        self._client.add_layout(Stack(width=width, height=height))
+
+    @keyword(tags=["layout"])
+    def close_stack(self):
+        """Close previously opened Stack.
+
+        Raises LayoutError if called with no Stack open, or if another layout element
+        was opened more recently than a Stack.
+        """
+        self._close_layouting_element("Stack")
+
+    @keyword(tags=["layout"])
+    def open_column(self):
+        """Open a Column layout container. Following ``Add <element>`` calls will add
+        items into that Column until ``Close Column`` is called.
+
+        .. code-block:: robotframework
+
+            *** Keywords ***
+            Double Column Layout
+                Open Row
+                Open Column
+                Add Text      First item in the first column
+                Add Text      Second item on the first column
+                Close Column
+                Open Column
+                Add Text      First item on the second column
+                Close Column
+                Close Row
+
+        .. code-block:: python
+
+            def double_column_layout():
+                assistant = Assistant()
+                assistant.open_row()
+                assistant.open_column()
+                assistant.add_text("First item in the first column")
+                assistant.add_text("Second item on the first column")
+                assistant.close_column()
+
+                assistant.open_column()
+                assistant.add_text("First item on the second column")
+                assistant.close_column()
+                assistant.close_row()
+
+                assistant.run_dialog()
+        """
+        self._open_layouting.append("Column")
+        self._client.add_layout(Column())
+
+    @keyword(tags=["layout"])
+    def close_column(self):
+        """Closes previously opened Column.
+
+        Raises LayoutError if called with no Column open, or if another layout element
+        was opened more recently than a Column.
+        """
+
+        self._close_layouting_element("Column")
```

### Comparing `rpaframework_assistant-3.0.2/src/RPA/Assistant/types.py` & `rpaframework_assistant-3.0.3/src/RPA/Assistant/types.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from enum import Enum, auto
-from typing import Any, Dict, List, Union
-
-from flet_core import Column, Container, Row, Stack, alignment
-
-Element = Dict[str, Any]
-Options = Union[List[str], str]
-Result = Dict[str, Any]
-
-
-class Size(Enum):
-    """Element size options"""
-
-    Small = "small"
-    Medium = "medium"
-    Large = "large"
-
-
-class Icon(Enum):
-    """Icon variants"""
-
-    Success = "success"
-    Warning = "warning"
-    Failure = "failure"
-
-
-class WindowLocation(Enum):
-    """A relative location for placing elements or windows"""
-
-    Center = auto()
-    TopLeft = auto()
-
-
-class VerticalLocation(Enum):
-    """A vertical location"""
-
-    Left = alignment.center_left
-    Center = alignment.center
-    Right = alignment.center_right
-
-
-class Location(Enum):
-    """A relative location for placing elements or windows, that can go into any
-    location
-    """
-
-    TopLeft = alignment.top_left
-    TopCenter = alignment.top_center
-    TopRight = alignment.top_right
-    CenterLeft = alignment.center_left
-    Center = alignment.center
-    CenterRight = alignment.center_right
-    BottomLeft = alignment.bottom_left
-    BottomCenter = alignment.bottom_center
-    BottomRight = alignment.bottom_right
-
-
-SupportedFletLayout = Union[Row, Column, Container, Stack]
-
-
-class PageNotOpenError(RuntimeError):
-    """Raised when a method is called that requires the dialog to be open but dialog
-    was not yet open"""
-
-
-class LayoutError(ValueError):
-    """Raised when an invalid layout is made. Debug, and do not catch these."""
+from enum import Enum, auto
+from typing import Any, Dict, List, Union
+
+from flet_core import Column, Container, Row, Stack, alignment
+
+Element = Dict[str, Any]
+Options = Union[List[str], str]
+Result = Dict[str, Any]
+
+
+class Size(Enum):
+    """Element size options"""
+
+    Small = "small"
+    Medium = "medium"
+    Large = "large"
+
+
+class Icon(Enum):
+    """Icon variants"""
+
+    Success = "success"
+    Warning = "warning"
+    Failure = "failure"
+
+
+class WindowLocation(Enum):
+    """A relative location for placing elements or windows"""
+
+    Center = auto()
+    TopLeft = auto()
+
+
+class VerticalLocation(Enum):
+    """A vertical location"""
+
+    Left = alignment.center_left
+    Center = alignment.center
+    Right = alignment.center_right
+
+
+class Location(Enum):
+    """A relative location for placing elements or windows, that can go into any
+    location
+    """
+
+    TopLeft = alignment.top_left
+    TopCenter = alignment.top_center
+    TopRight = alignment.top_right
+    CenterLeft = alignment.center_left
+    Center = alignment.center
+    CenterRight = alignment.center_right
+    BottomLeft = alignment.bottom_left
+    BottomCenter = alignment.bottom_center
+    BottomRight = alignment.bottom_right
+
+
+SupportedFletLayout = Union[Row, Column, Container, Stack]
+
+
+class PageNotOpenError(RuntimeError):
+    """Raised when a method is called that requires the dialog to be open but dialog
+    was not yet open"""
+
+
+class LayoutError(ValueError):
+    """Raised when an invalid layout is made. Debug, and do not catch these."""
```

### Comparing `rpaframework_assistant-3.0.2/src/RPA/Assistant/utils.py` & `rpaframework_assistant-3.0.3/src/RPA/Assistant/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-from typing_extensions import Literal
-from RPA.core.types import is_list_like  # type: ignore
-
-from RPA.Assistant.types import Element, Location, Options
-
-
-def to_options(
-    opts: Options, default: Optional[str] = None
-) -> Tuple[List[str], Optional[str]]:
-    """Convert keyword argument for multiple options into
-    a list of strings.
-
-    Also handles default option validation.
-    """
-    if isinstance(opts, str):
-        opts = [opt.strip() for opt in opts.split(",")]
-    elif is_list_like(opts):
-        opts = [str(opt) for opt in opts]
-    else:
-        raise ValueError(f"Unsupported options type: {opts}")
-
-    if not opts:
-        return [], None
-
-    if default is None:
-        default = opts[0]
-
-    if default not in opts:
-        raise ValueError(f"Default '{default}' is not in available options")
-
-    return opts, default
-
-
-def optional_str(val: Any) -> Optional[str]:
-    """Convert value to string, but keep NoneType"""
-    return str(val) if val is not None else val
-
-
-def optional_int(val: Any) -> Optional[int]:
-    """Convert value to int, but keep NoneType"""
-    return int(val) if val is not None else val
-
-
-def int_or_auto(val: Any) -> Union[int, str]:
-    """Convert value to int or 'AUTO' literal"""
-    if isinstance(val, int):
-        return val
-
-    try:
-        return int(val)
-    except ValueError:
-        pass
-
-    height = str(val).strip().upper()
-    if height == "AUTO":
-        return height
-
-    raise ValueError("Value not integer or AUTO")
-
-
-def is_input(element: Element) -> bool:
-    """Check if an element is an input"""
-    return element["type"].startswith("input-")
-
-
-def is_submit(element: Element) -> bool:
-    """Check if an element is a submit button."""
-    return element["type"] == "submit"
-
-
-def location_to_absolute(
-    location: Union[Location, Tuple[int, int], None],
-    parent_width: float,
-    parent_height: float,
-    element_width: Optional[float],
-    element_height: Optional[float],
-) -> Dict[Literal["left", "top", "bottom", "right"], float]:
-    """Calculates and returns absolute version of elements relative position as left or
-    right and bottom or top keys in dictionary.
-    """
-    if isinstance(location, tuple):
-        return {"left": location[0], "top": location[1]}
-
-    if location in [
-        Location.TopCenter,
-        Location.BottomCenter,
-        Location.CenterLeft,
-        Location.CenterRight,
-        Location.Center,
-    ]:
-        if element_height is None or element_width is None:
-            raise ValueError(
-                "Cannot determine centered position without static width and height"
-            )
-        half_height = (parent_height / 2) - (element_height / 2)
-        half_width = (parent_width / 2) - (element_width / 2)
-    else:
-        half_height, half_width = -1, -1
-
-    coordinates: Dict[
-        Location, Dict[Literal["left", "top", "bottom", "right"], float]
-    ] = {
-        Location.TopLeft: {"left": 0, "top": 0},
-        Location.TopCenter: {"left": half_width, "top": 0},
-        Location.TopRight: {"right": 0, "top": 0},
-        Location.CenterLeft: {"left": 0, "top": half_height},
-        Location.Center: {"left": half_width, "top": half_height},
-        Location.CenterRight: {"right": 0, "top": half_width},
-        Location.BottomLeft: {"left": 0, "bottom": 0},
-        Location.BottomCenter: {"left": half_width, "bottom": 0},
-        Location.BottomRight: {"right": 0, "bottom": 0},
-    }
-
-    if isinstance(location, Location):
-        return coordinates[location]
-    else:
-        raise ValueError(f"Invalid location {location}")
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+from typing_extensions import Literal
+from RPA.core.types import is_list_like  # type: ignore
+
+from RPA.Assistant.types import Element, Location, Options
+
+
+def to_options(
+    opts: Options, default: Optional[str] = None
+) -> Tuple[List[str], Optional[str]]:
+    """Convert keyword argument for multiple options into
+    a list of strings.
+
+    Also handles default option validation.
+    """
+    if isinstance(opts, str):
+        opts = [opt.strip() for opt in opts.split(",")]
+    elif is_list_like(opts):
+        opts = [str(opt) for opt in opts]
+    else:
+        raise ValueError(f"Unsupported options type: {opts}")
+
+    if not opts:
+        return [], None
+
+    if default is None:
+        default = opts[0]
+
+    if default not in opts:
+        raise ValueError(f"Default '{default}' is not in available options")
+
+    return opts, default
+
+
+def optional_str(val: Any) -> Optional[str]:
+    """Convert value to string, but keep NoneType"""
+    return str(val) if val is not None else val
+
+
+def optional_int(val: Any) -> Optional[int]:
+    """Convert value to int, but keep NoneType"""
+    return int(val) if val is not None else val
+
+
+def int_or_auto(val: Any) -> Union[int, str]:
+    """Convert value to int or 'AUTO' literal"""
+    if isinstance(val, int):
+        return val
+
+    try:
+        return int(val)
+    except ValueError:
+        pass
+
+    height = str(val).strip().upper()
+    if height == "AUTO":
+        return height
+
+    raise ValueError("Value not integer or AUTO")
+
+
+def is_input(element: Element) -> bool:
+    """Check if an element is an input"""
+    return element["type"].startswith("input-")
+
+
+def is_submit(element: Element) -> bool:
+    """Check if an element is a submit button."""
+    return element["type"] == "submit"
+
+
+def location_to_absolute(
+    location: Union[Location, Tuple[int, int], None],
+    parent_width: float,
+    parent_height: float,
+    element_width: Optional[float],
+    element_height: Optional[float],
+) -> Dict[Literal["left", "top", "bottom", "right"], float]:
+    """Calculates and returns absolute version of elements relative position as left or
+    right and bottom or top keys in dictionary.
+    """
+    if isinstance(location, tuple):
+        return {"left": location[0], "top": location[1]}
+
+    if location in [
+        Location.TopCenter,
+        Location.BottomCenter,
+        Location.CenterLeft,
+        Location.CenterRight,
+        Location.Center,
+    ]:
+        if element_height is None or element_width is None:
+            raise ValueError(
+                "Cannot determine centered position without static width and height"
+            )
+        half_height = (parent_height / 2) - (element_height / 2)
+        half_width = (parent_width / 2) - (element_width / 2)
+    else:
+        half_height, half_width = -1, -1
+
+    coordinates: Dict[
+        Location, Dict[Literal["left", "top", "bottom", "right"], float]
+    ] = {
+        Location.TopLeft: {"left": 0, "top": 0},
+        Location.TopCenter: {"left": half_width, "top": 0},
+        Location.TopRight: {"right": 0, "top": 0},
+        Location.CenterLeft: {"left": 0, "top": half_height},
+        Location.Center: {"left": half_width, "top": half_height},
+        Location.CenterRight: {"right": 0, "top": half_width},
+        Location.BottomLeft: {"left": 0, "bottom": 0},
+        Location.BottomCenter: {"left": half_width, "bottom": 0},
+        Location.BottomRight: {"right": 0, "bottom": 0},
+    }
+
+    if isinstance(location, Location):
+        return coordinates[location]
+    else:
+        raise ValueError(f"Invalid location {location}")
```

### Comparing `rpaframework_assistant-3.0.2/PKG-INFO` & `rpaframework_assistant-3.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-assistant
-Version: 3.0.2
+Version: 3.0.3
 Summary: Interactive UI library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,dialogs,assistant
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8,<4.0
@@ -15,19 +15,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: flet (==0.4.2)
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,!=6.1.0,<7.0.0)
-Requires-Dist: rpaframework-core (>=11.0.0,<12.0.0)
+Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-assistant
 ======================
```

