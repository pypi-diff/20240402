# Comparing `tmp/rpaframework_pdf-7.3.1.tar.gz` & `tmp/rpaframework_pdf-7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_pdf-7.3.1.tar", max compression
+gzip compressed data, was "rpaframework_pdf-7.3.2.tar", max compression
```

## Comparing `rpaframework_pdf-7.3.1.tar` & `rpaframework_pdf-7.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11358 2021-09-09 09:55:26.451320 rpaframework_pdf-7.3.1/LICENSE
--rw-r--r--   0        0        0      187 2021-09-09 09:55:26.451408 rpaframework_pdf-7.3.1/README.rst
--rw-r--r--   0        0        0    66540 2023-10-10 16:50:11.235091 rpaframework_pdf-7.3.1/RPA_PDF.libspec
--rw-r--r--   0        0        0     1948 2023-10-10 16:48:33.619978 rpaframework_pdf-7.3.1/pyproject.toml
--rw-r--r--   0        0        0     4047 2023-03-31 12:08:05.029080 rpaframework_pdf-7.3.1/src/RPA/PDF/__init__.py
--rw-r--r--   0        0        0   316100 2022-09-09 11:28:10.260100 rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-Bold.ttf
--rw-r--r--   0        0        0   265920 2022-09-09 11:28:10.261375 rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-BoldItalic.ttf
--rw-r--r--   0        0        0   263548 2022-09-09 11:28:10.263934 rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-Italic.ttf
--rw-r--r--   0        0        0   309828 2022-09-09 11:28:10.265438 rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-Regular.ttf
--rw-r--r--   0        0        0      258 2023-02-03 14:24:02.149967 rpaframework_pdf-7.3.1/src/RPA/PDF/keywords/__init__.py
--rw-r--r--   0        0        0      789 2022-09-09 11:28:10.265897 rpaframework_pdf-7.3.1/src/RPA/PDF/keywords/context.py
--rw-r--r--   0        0        0    47046 2023-10-03 07:53:58.877154 rpaframework_pdf-7.3.1/src/RPA/PDF/keywords/document.py
--rw-r--r--   0        0        0    16873 2023-02-03 14:24:02.150961 rpaframework_pdf-7.3.1/src/RPA/PDF/keywords/finder.py
--rw-r--r--   0        0        0    28419 2023-08-11 08:51:22.188058 rpaframework_pdf-7.3.1/src/RPA/PDF/keywords/model.py
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 rpaframework_pdf-7.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.443221 rpaframework_pdf-7.3.2/LICENSE
+-rw-r--r--   0        0        0     1889 2024-04-02 12:08:08.568585 rpaframework_pdf-7.3.2/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-12-05 08:21:31.443221 rpaframework_pdf-7.3.2/README.rst
+-rw-r--r--   0        0        0    68462 2024-04-02 12:09:28.501443 rpaframework_pdf-7.3.2/RPA_PDF.libspec
+-rw-r--r--   0        0        0     4165 2023-12-05 08:21:31.444223 rpaframework_pdf-7.3.2/src/RPA/PDF/__init__.py
+-rw-r--r--   0        0        0   316100 2023-12-05 08:21:31.447248 rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-Bold.ttf
+-rw-r--r--   0        0        0   265920 2023-12-05 08:21:31.450758 rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-BoldItalic.ttf
+-rw-r--r--   0        0        0   263548 2023-12-05 08:21:31.452793 rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-Italic.ttf
+-rw-r--r--   0        0        0   309828 2023-12-05 08:21:31.455788 rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-Regular.ttf
+-rw-r--r--   0        0        0      269 2023-12-05 08:21:31.455788 rpaframework_pdf-7.3.2/src/RPA/PDF/keywords/__init__.py
+-rw-r--r--   0        0        0      822 2023-12-05 08:21:31.456768 rpaframework_pdf-7.3.2/src/RPA/PDF/keywords/context.py
+-rw-r--r--   0        0        0    48476 2023-12-05 08:21:31.456768 rpaframework_pdf-7.3.2/src/RPA/PDF/keywords/document.py
+-rw-r--r--   0        0        0    17353 2023-12-05 08:21:31.457768 rpaframework_pdf-7.3.2/src/RPA/PDF/keywords/finder.py
+-rw-r--r--   0        0        0    29282 2023-12-05 08:21:31.457768 rpaframework_pdf-7.3.2/src/RPA/PDF/keywords/model.py
+-rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 rpaframework_pdf-7.3.2/PKG-INFO
```

### Comparing `rpaframework_pdf-7.3.1/LICENSE` & `rpaframework_pdf-7.3.2/LICENSE`

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

### Comparing `rpaframework_pdf-7.3.1/RPA_PDF.libspec` & `rpaframework_pdf-7.3.2/RPA_PDF.libspec`

 * *Files 24% similar despite different names*

#### Comparing `rpaframework_pdf-7.3.1/RPA_PDF.libspec` & `rpaframework_pdf-7.3.2/RPA_PDF.libspec`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.PDF" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-10-10T16:50:11+00:00" specversion="5" source="./RPA/PDF/__init__.py" lineno="11">
+<keywordspec name="RPA.PDF" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-04-02T12:09:28+00:00" specversion="5" source="./RPA/PDF/__init__.py" lineno="11">
   <version/>
   <doc>`PDF` is a library for managing PDF documents.
 
 It can be used to extract text from PDFs, add watermarks to pages, and
 decrypt/encrypt documents.
 
 Merging and splitting PDFs is supported by ``Add Files To PDF`` keyword. Read
```

### Comparing `rpaframework_pdf-7.3.1/pyproject.toml` & `rpaframework_pdf-7.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,66 @@
-[tool.poetry]
-name = "rpaframework-pdf"
-version = "7.3.1"
-description = "PDF library of RPA Framework"
-authors = ["RPA Framework <rpafw@robocorp.com>"]
-license = "Apache-2.0"
-readme = "README.rst"
-
-homepage = "https://rpaframework.org/"
-documentation = "https://rpaframework.org/"
-repository = "https://github.com/robocorp/rpaframework"
-
-keywords = ["robotframework", "rpa", "automation", "pdf"]
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
-python = "^3.8.1"
-rpaframework-core = "^11.2.1"
-robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
-robotframework-pythonlibcore = "^4.2.0"
-"pdfminer.six" = "20221105"
-pypdf = "^3.16.2"
-fpdf2 = "^2.7.5"
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-flake8 = "^3.7.9"
-pylint = "^2.4.4, <2.13"
-pytest = "^7.2.0"
-mock = "^5.0.0"
-pytest-cov = "^4.0.0"
-invoke = "^2.2.0"
-sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.1.1"
-toml = "^0.10.2"
-sphinx-markdown-builder = "^0.5.4"
-robotframework-docgen = "^0.16.0"
-sphinx-issues = "^3.0.1"
-docutils = "0.16"
-colorama = "^0.4.5"
-keyring = "^24.2.0"
-PyYAML = ">=5.4.1,<7.0.0"
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
+[tool.poetry]
+name = "rpaframework-pdf"
+version = "7.3.2"
+description = "PDF library of RPA Framework"
+authors = ["RPA Framework <rpafw@robocorp.com>"]
+license = "Apache-2.0"
+readme = "README.rst"
+
+homepage = "https://rpaframework.org/"
+documentation = "https://rpaframework.org/"
+repository = "https://github.com/robocorp/rpaframework"
+
+keywords = ["robotframework", "rpa", "automation", "pdf"]
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
+python = "^3.8.1"
+rpaframework-core = "^11.3.1"
+robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
+robotframework-pythonlibcore = "^4.2.0"
+"pdfminer.six" = "20221105"
+pypdf = "^3.16.2"
+fpdf2 = "2.7.5"
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.3.0"
+flake8 = "^3.7.9"
+pylint = "^2.4.4, <2.13"
+pytest = "^7.2.0"
+mock = "^5.0.0"
+pytest-cov = "^4.0.0"
+invoke = "^2.2.0"
+robotframework-docgen = "^0.16.0"
+toml = "^0.10.2"
+colorama = "^0.4.5"
+keyring = "^24.2.0"
+PyYAML = ">=5.4.1,<7.0.0"
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
```

### Comparing `rpaframework_pdf-7.3.1/src/RPA/PDF/__init__.py` & `rpaframework_pdf-7.3.2/src/RPA/PDF/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import logging
-from typing import Dict
-
-from robotlibcore import DynamicCore
-from RPA.core.logger import RobotLogListener
-
-from RPA.PDF.keywords import DocumentKeywords, FinderKeywords, ModelKeywords
-from RPA.PDF.keywords.model import Document
-
-
-class PDF(DynamicCore):
-    """`PDF` is a library for managing PDF documents.
-
-    It can be used to extract text from PDFs, add watermarks to pages, and
-    decrypt/encrypt documents.
-
-    Merging and splitting PDFs is supported by ``Add Files To PDF`` keyword. Read
-    the keyword documentation for examples.
-
-    There is also limited support for updating form field values. (check
-    ``Set Field Value`` and ``Save Field Values`` for more info)
-
-    The input PDF file can be passed as an argument to the keywords, or it can be
-    omitted if you first call ``Open PDF``. A reference to the current active PDF will
-    be stored in the library instance and can be changed by using the ``Switch To PDF``
-    keyword with another PDF file path, therefore you can asynchronously work with
-    multiple PDFs.
-
-    .. Attention::
-        Keep in mind that this library works with text-based PDFs, and it **can't
-        extract information from an image-based (scan)** PDF file. For accurate
-        results, you have to use specialized external services wrapped by the
-        ``RPA.DocumentAI`` library.
-
-    Portal example with video recording demo for parsing PDF invoices:
-    https://github.com/robocorp/example-parse-pdf-invoice
-
-    **Examples**
-
-    **Robot Framework**
-
-    .. code-block:: robotframework
-
-        *** Settings ***
-        Library    RPA.PDF
-        Library    String
-
-        *** Tasks ***
-        Extract Data From First Page
-            ${text} =    Get Text From PDF    report.pdf
-            ${lines} =     Get Lines Matching Regexp    ${text}[${1}]    .+pain.+
-            Log    ${lines}
-
-        Get Invoice Number
-            Open Pdf    invoice.pdf
-            ${matches} =  Find Text    Invoice Number
-            Log List      ${matches}
-
-        Fill Form Fields
-            Switch To Pdf    form.pdf
-            ${fields} =     Get Input Fields   encoding=utf-16
-            Log Dictionary    ${fields}
-            Set Field Value    Given Name Text Box    Mark
-            Save Field Values    output_path=${OUTPUT_DIR}${/}completed-form.pdf
-            ...                  use_appearances_writer=${True}
-
-    .. code-block:: python
-
-        from RPA.PDF import PDF
-        from robot.libraries.String import String
-
-        pdf = PDF()
-        string = String()
-
-        def extract_data_from_first_page():
-            text = pdf.get_text_from_pdf("report.pdf")
-            lines = string.get_lines_matching_regexp(text[1], ".+pain.+")
-            print(lines)
-
-        def get_invoice_number():
-            pdf.open_pdf("invoice.pdf")
-            matches = pdf.find_text("Invoice Number")
-            for match in matches:
-                print(match)
-
-        def fill_form_fields():
-            pdf.switch_to_pdf("form.pdf")
-            fields = pdf.get_input_fields(encoding="utf-16")
-            for key, value in fields.items():
-                print(f"{key}: {value}")
-            pdf.set_field_value("Given Name Text Box", "Mark")
-            pdf.save_field_values(
-                output_path="completed-form.pdf",
-                use_appearances_writer=True
-            )
-    """
-
-    ROBOT_LIBRARY_SCOPE = "GLOBAL"
-    ROBOT_LIBRARY_DOC_FORMAT = "REST"
-
-    def __init__(self):
-        self.logger = logging.getLogger(__name__)
-        self.documents: Dict[str, Document] = {}
-        self.active_pdf_document = None
-        self.convert_settings = {}
-
-        # Register keyword libraries to LibCore
-        libraries = [
-            DocumentKeywords(self),
-            FinderKeywords(self),
-            ModelKeywords(self),
-        ]
-        super().__init__(libraries)
-
-        listener = RobotLogListener()
-        listener.register_protected_keywords(["RPA.PDF.Decrypt PDF"])
-
-        logging.getLogger("pdfminer").setLevel(logging.WARNING)
+import logging
+from typing import Dict
+
+from robotlibcore import DynamicCore
+from RPA.core.logger import RobotLogListener
+
+from RPA.PDF.keywords import DocumentKeywords, FinderKeywords, ModelKeywords
+from RPA.PDF.keywords.model import Document
+
+
+class PDF(DynamicCore):
+    """`PDF` is a library for managing PDF documents.
+
+    It can be used to extract text from PDFs, add watermarks to pages, and
+    decrypt/encrypt documents.
+
+    Merging and splitting PDFs is supported by ``Add Files To PDF`` keyword. Read
+    the keyword documentation for examples.
+
+    There is also limited support for updating form field values. (check
+    ``Set Field Value`` and ``Save Field Values`` for more info)
+
+    The input PDF file can be passed as an argument to the keywords, or it can be
+    omitted if you first call ``Open PDF``. A reference to the current active PDF will
+    be stored in the library instance and can be changed by using the ``Switch To PDF``
+    keyword with another PDF file path, therefore you can asynchronously work with
+    multiple PDFs.
+
+    .. Attention::
+        Keep in mind that this library works with text-based PDFs, and it **can't
+        extract information from an image-based (scan)** PDF file. For accurate
+        results, you have to use specialized external services wrapped by the
+        ``RPA.DocumentAI`` library.
+
+    Portal example with video recording demo for parsing PDF invoices:
+    https://github.com/robocorp/example-parse-pdf-invoice
+
+    **Examples**
+
+    **Robot Framework**
+
+    .. code-block:: robotframework
+
+        *** Settings ***
+        Library    RPA.PDF
+        Library    String
+
+        *** Tasks ***
+        Extract Data From First Page
+            ${text} =    Get Text From PDF    report.pdf
+            ${lines} =     Get Lines Matching Regexp    ${text}[${1}]    .+pain.+
+            Log    ${lines}
+
+        Get Invoice Number
+            Open Pdf    invoice.pdf
+            ${matches} =  Find Text    Invoice Number
+            Log List      ${matches}
+
+        Fill Form Fields
+            Switch To Pdf    form.pdf
+            ${fields} =     Get Input Fields   encoding=utf-16
+            Log Dictionary    ${fields}
+            Set Field Value    Given Name Text Box    Mark
+            Save Field Values    output_path=${OUTPUT_DIR}${/}completed-form.pdf
+            ...                  use_appearances_writer=${True}
+
+    .. code-block:: python
+
+        from RPA.PDF import PDF
+        from robot.libraries.String import String
+
+        pdf = PDF()
+        string = String()
+
+        def extract_data_from_first_page():
+            text = pdf.get_text_from_pdf("report.pdf")
+            lines = string.get_lines_matching_regexp(text[1], ".+pain.+")
+            print(lines)
+
+        def get_invoice_number():
+            pdf.open_pdf("invoice.pdf")
+            matches = pdf.find_text("Invoice Number")
+            for match in matches:
+                print(match)
+
+        def fill_form_fields():
+            pdf.switch_to_pdf("form.pdf")
+            fields = pdf.get_input_fields(encoding="utf-16")
+            for key, value in fields.items():
+                print(f"{key}: {value}")
+            pdf.set_field_value("Given Name Text Box", "Mark")
+            pdf.save_field_values(
+                output_path="completed-form.pdf",
+                use_appearances_writer=True
+            )
+    """
+
+    ROBOT_LIBRARY_SCOPE = "GLOBAL"
+    ROBOT_LIBRARY_DOC_FORMAT = "REST"
+
+    def __init__(self):
+        self.logger = logging.getLogger(__name__)
+        self.documents: Dict[str, Document] = {}
+        self.active_pdf_document = None
+        self.convert_settings = {}
+
+        # Register keyword libraries to LibCore
+        libraries = [
+            DocumentKeywords(self),
+            FinderKeywords(self),
+            ModelKeywords(self),
+        ]
+        super().__init__(libraries)
+
+        listener = RobotLogListener()
+        listener.register_protected_keywords(["RPA.PDF.Decrypt PDF"])
+
+        logging.getLogger("pdfminer").setLevel(logging.WARNING)
```

### Comparing `rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-Bold.ttf` & `rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-BoldItalic.ttf` & `rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-Italic.ttf` & `rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rpaframework_pdf-7.3.1/src/RPA/PDF/assets/Inter-Regular.ttf` & `rpaframework_pdf-7.3.2/src/RPA/PDF/assets/Inter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rpaframework_pdf-7.3.1/src/RPA/PDF/keywords/finder.py` & `rpaframework_pdf-7.3.2/src/RPA/PDF/keywords/finder.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,480 +1,480 @@
-import functools
-import math
-import re
-from dataclasses import dataclass
-
-try:
-    # Python >=3.7
-    from re import Pattern
-except ImportError:
-    # Python =3.6
-    from re import _pattern_type as Pattern
-
-from typing import Callable, Dict, List, Optional, Union
-
-from RPA.PDF.keywords import LibraryContext, keyword
-from RPA.PDF.keywords.model import BaseElement, TextBox
-
-
-class TargetObject(BaseElement):
-    """Container for Target text boxes with coordinates."""
-
-    # Class level constants.
-    boxid: int = -1
-    text: str = ""
-
-
-Element = Union[TextBox, TargetObject]
-
-
-@dataclass
-class Match:
-    """Match object returned by the `Find Text` keyword.
-
-    It contains the anchor point and its relative found elements in text format.
-    """
-
-    anchor: str
-    direction: str
-    neighbours: List[str]
-
-
-class FinderKeywords(LibraryContext):
-    """Keywords for locating elements."""
-
-    RE_FLAGS = re.MULTILINE | re.DOTALL  # default regexp flags
-
-    def __init__(self, ctx):
-        super().__init__(ctx)
-
-        # Text locator might lead to multiple valid found anchors.
-        self._anchors: List[Element] = []
-        # The others usually have just one. (if multiple are found, set to it the
-        #   first one)
-        self.anchor_element = None
-
-    def _get_candidate_search_function(
-        self, direction: str, regexp: Optional[Pattern], strict: bool
-    ) -> Callable[[TextBox], bool]:
-        if direction in ["left", "right"]:
-            return functools.partial(
-                self._is_match_on_horizontal,
-                direction=direction,
-                regexp=regexp,
-                strict=strict,
-            )
-        if direction in ["top", "bottom", "up", "down"]:
-            return functools.partial(
-                self._is_match_on_vertical,
-                direction=direction,
-                regexp=regexp,
-                strict=strict,
-            )
-        if direction == "box":
-            return self._is_match_in_box
-
-        raise ValueError(f"Not recognized direction search {direction!r}")
-
-    def _log_element(self, elem: Element, prefix: str = ""):
-        template = f"{prefix} box %d | bbox %s | text %r"
-        self.logger.debug(template, elem.boxid, elem.bbox, elem.text)
-
-    @classmethod
-    def _re_flags(cls, ignore_case: bool) -> int:
-        flags = cls.RE_FLAGS
-        if ignore_case:
-            flags |= re.IGNORECASE
-        return flags
-
-    @keyword
-    def find_text(
-        self,
-        locator: str,
-        pagenum: Union[int, str] = 1,
-        direction: str = "right",
-        closest_neighbours: Optional[Union[int, str]] = 1,
-        strict: bool = False,
-        regexp: Optional[str] = None,
-        trim: bool = True,
-        ignore_case: bool = False,
-    ) -> List[Match]:
-        """Find the closest text elements near the set anchor(s) through `locator`.
-
-        The PDF will be parsed automatically before elements can be searched.
-
-        :param locator: Element to set anchor to. This can be prefixed with either
-            "text:", "subtext:", "regex:" or "coords:" to find the anchor by text or
-            coordinates. The "text" strategy is assumed if no such prefix is specified.
-            (text search is case-sensitive; use `ignore_case` param for controlling it)
-        :param pagenum: Page number where search is performed on, defaults to 1 (first
-            page).
-        :param direction: In which direction to search for text elements. This can be
-            any of 'top'/'up', 'bottom'/'down', 'left' or 'right'. (defaults to
-            'right')
-        :param closest_neighbours: How many neighbours to return at most, sorted by the
-            distance from the current anchor.
-        :param strict: If element's margins should be used for matching those which are
-            aligned to the anchor. (turned off by default)
-        :param regexp: Expected format of the searched text value. By default all the
-            candidates in range are considered valid neighbours.
-        :param trim: Automatically trim leading/trailing whitespace from the text
-            elements. (switched on by default)
-        :param ignore_case: Do a case-insensitive search when set to `True`. (affects
-            the passed `locator` and `regexp` filtering)
-        :returns: A list of `Match` objects where every match has the following
-            attributes: `.anchor` - the matched text with the locator; `.neighbours` -
-            a list of adjacent texts found on the specified direction
-
-        .. Attention::
-            Keep in mind that this keyword works with text-based PDFs, and it **can't
-            extract information from an image-based (scan)** PDF file. For accurate
-            results, you have to use specialized external services wrapped by the
-            ``RPA.DocumentAI`` library.
-
-        Portal example with video recording demo for parsing PDF invoices:
-        https://github.com/robocorp/example-parse-pdf-invoice
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            PDF Invoice Parsing
-                Open Pdf    invoice.pdf
-                ${matches} =  Find Text    Invoice Number
-                Log List      ${matches}
-
-        .. code-block::
-
-            List has one item:
-            Match(anchor='Invoice Number', direction='right', neighbours=['INV-3337'])
-
-        **Python**
-
-        .. code-block:: python
-
-            from RPA.PDF import PDF
-
-            pdf = PDF()
-
-            def pdf_invoice_parsing():
-                pdf.open_pdf("invoice.pdf")
-                matches = pdf.find_text("Invoice Number")
-                for match in matches:
-                    print(match)
-
-            pdf_invoice_parsing()
-
-        .. code-block::
-
-            Match(anchor='Invoice Number', direction='right', neighbours=['INV-3337'])
-        """
-        pagenum = int(pagenum)
-        if closest_neighbours is not None:
-            closest_neighbours = int(closest_neighbours)
-        self.logger.info(
-            "Searching for %s neighbour(s) to the %s of %r on page %d using regular "
-            "expression: %s (case %s)",
-            f"closest {closest_neighbours}"
-            if closest_neighbours is not None
-            else "all",
-            direction,
-            locator,
-            pagenum,
-            regexp,
-            "insensitive" if ignore_case else "sensitive",
-        )
-        self.set_anchor_to_element(
-            locator, trim=trim, pagenum=pagenum, ignore_case=ignore_case
-        )
-        if not self.anchor_element:
-            self.logger.warning("No anchor(s) set for locator: %s", locator)
-            return []
-
-        regexp_compiled = None
-        if regexp:
-            regexp_compiled = re.compile(regexp, flags=self._re_flags(ignore_case))
-        search_for_candidate = self._get_candidate_search_function(
-            direction, regexp_compiled, strict
-        )
-
-        candidates_dict: Dict[int, List[Element]] = {}
-        anchors_map: Dict[int, Element] = {}
-        for anchor in self._anchors:
-            candidates_dict[anchor.boxid] = []
-            anchors_map[anchor.boxid] = anchor
-
-        for candidate in self._get_textboxes_on_page(pagenum):
-            self._log_element(candidate, prefix="Current candidate:")
-            for anchor in self._anchors:
-                self._log_element(anchor, prefix="Current anchor:")
-                # Skip anchor element itself from matching and check if the candidate
-                # matches the search criteria.
-                if candidate.boxid != anchor.boxid and search_for_candidate(
-                    candidate, anchor=anchor
-                ):
-                    candidates_dict[anchor.boxid].append(candidate)
-
-        matches = []
-        for anchor_id, candidates in candidates_dict.items():
-            anchor = anchors_map[anchor_id]
-            self._sort_candidates_by_anchor(candidates, anchor=anchor)
-            if closest_neighbours is not None:
-                # Keep the first N closest neighbours from the entire set of candidates.
-                candidates[closest_neighbours:] = []
-            match = Match(
-                anchor=anchor.text,
-                direction=direction,
-                neighbours=[candidate.text for candidate in candidates],
-            )
-            matches.append(match)
-
-        return matches
-
-    @keyword
-    def set_anchor_to_element(
-        self,
-        locator: str,
-        trim: bool = True,
-        pagenum: Union[int, str] = 1,
-        ignore_case: bool = False,
-    ) -> bool:
-        """Sets main anchor point in the document for further searches.
-
-        This is used internally in the library and can work with multiple anchors at
-        the same time if such are found.
-
-        :param locator: Element to set anchor to. This can be prefixed with either
-            "text:", "subtext:", "regex:" or "coords:" to find the anchor by text or
-            coordinates. The "text" strategy is assumed if no such prefix is specified.
-            (text search is case-sensitive; use `ignore_case` param for controlling it)
-        :param trim: Automatically trim leading/trailing whitespace from the text
-            elements. (switched on by default)
-        :param pagenum: Page number where search is performed on, defaults to 1 (first
-            page).
-        :param ignore_case: Do a case-insensitive search when set to `True`.
-        :returns: True if at least one anchor was found.
-
-        **Examples**
-
-        **Robot Framework**
-
-        .. code-block:: robotframework
-
-            Example Keyword
-                 ${success} =  Set Anchor To Element    Invoice Number
-
-        **Python**
-
-        .. code-block:: python
-
-            from RPA.PDF import PDF
-
-            pdf = PDF()
-
-            def example_keyword():
-                success = pdf.set_anchor_to_element("Invoice Number")
-        """
-        pagenum = int(pagenum)
-        self.logger.info(
-            "Trying to set anchor on page %d using locator: %r (case %s)",
-            pagenum,
-            locator,
-            "insensitive" if ignore_case else "sensitive",
-        )
-        self.ctx.convert(trim=trim, pagenum=pagenum)
-        self._anchors.clear()
-        self.anchor_element = None
-
-        pure_locator = locator
-        criteria = "text"
-        parts = locator.split(":", 1)
-        if len(parts) == 2 and parts[0] in ("coords", "text", "regex", "subtext"):
-            criteria = parts[0]
-            pure_locator = parts[1]
-
-        if criteria == "coords":
-            coords = pure_locator.split(",")
-            if len(coords) == 2:
-                left, bottom = coords
-                top = bottom
-                right = left
-            elif len(coords) == 4:
-                left, bottom, right, top = coords
-            else:
-                raise ValueError("Give 2 coordinates for point, or 4 for area")
-
-            bbox = (
-                int(left),
-                int(bottom),
-                int(right),
-                int(top),
-            )
-            anchor = TargetObject(bbox=bbox)
-            self._anchors.append(anchor)
-        else:  # text-based search
-            if criteria == "regex":
-                pure_locator = re.compile(
-                    pure_locator, flags=self._re_flags(ignore_case)
-                )
-            anchors = self._find_matching_textboxes(
-                pure_locator,
-                pagenum=pagenum,
-                is_subtext=criteria == "subtext",
-                ignore_case=ignore_case,
-            )
-            self._anchors.extend(anchors)
-
-        if self._anchors:
-            self.anchor_element = self._anchors[0]
-            return True
-
-        return False
-
-    def _get_textboxes_on_page(self, pagenum: int) -> List[TextBox]:
-        page = self.active_pdf_document.get_page(pagenum)
-        return list(page.textboxes.values())
-
-    def _find_matching_textboxes(
-        self,
-        locator: Union[str, Pattern],
-        *,
-        pagenum: int,
-        is_subtext: bool = False,
-        ignore_case: bool = False,
-    ) -> List[TextBox]:
-        self.logger.info("Searching for matching text boxes with: %r", locator)
-
-        if isinstance(locator, str):
-            get_text = lambda string: (  # noqa: E731
-                string.lower() if ignore_case else string
-            )
-            if is_subtext:
-                matches_anchor = lambda _anchor: (  # noqa: E731
-                    get_text(locator) in get_text(_anchor.text)
-                )
-            else:
-                matches_anchor = lambda _anchor: (  # noqa: E731
-                    get_text(_anchor.text) == get_text(locator)
-                )
-        else:
-            matches_anchor = lambda _anchor: locator.match(_anchor.text)  # noqa: E731
-
-        anchors = []
-        for anchor in self._get_textboxes_on_page(pagenum):
-            if matches_anchor(anchor):
-                anchors.append(anchor)
-        if anchors:
-            self.logger.info("Found %d matches with locator %r", len(anchors), locator)
-            for anchor in anchors:
-                self._log_element(anchor)
-        else:
-            self.logger.warning("Did not find any matches with locator %r", locator)
-
-        return anchors
-
-    def _check_text_match(self, candidate: TextBox, regexp: Optional[Pattern]) -> bool:
-        if regexp and regexp.match(candidate.text):
-            self._log_element(candidate, prefix="Exact match:")
-            return True
-        if regexp is None:
-            self._log_element(candidate, prefix="Potential match:")
-            return True
-
-        return False
-
-    def _is_match_on_horizontal(
-        self,
-        candidate: TextBox,
-        *,
-        direction: str,
-        regexp: Optional[Pattern],
-        strict: bool,
-        anchor: TextBox,
-    ) -> bool:
-        (left, bottom, right, top) = anchor.bbox
-        direction_left = direction == "left"
-        direction_right = direction == "right"
-
-        if not any(
-            [
-                direction_left and candidate.right <= left,
-                direction_right and candidate.left >= right,
-            ]
-        ):
-            return False  # not in the seeked direction
-
-        non_strict_match = not strict and (
-            bottom <= candidate.bottom <= top
-            or bottom <= candidate.top <= top
-            or candidate.bottom <= bottom <= candidate.top
-            or candidate.bottom <= top <= candidate.top
-        )
-        strict_match = strict and (candidate.bottom == bottom or candidate.top == top)
-        if not any([non_strict_match, strict_match]):
-            return False  # candidate not in boundaries
-
-        return self._check_text_match(candidate, regexp)
-
-    def _is_match_on_vertical(
-        self,
-        candidate: TextBox,
-        *,
-        direction: str,
-        regexp: Optional[Pattern],
-        strict: bool,
-        anchor: TextBox,
-    ) -> bool:
-        (left, bottom, right, top) = anchor.bbox
-        direction_down = direction in ["bottom", "down"]
-        direction_up = direction in ["top", "up"]
-
-        if not any(
-            [
-                direction_down and candidate.top <= bottom,
-                direction_up and candidate.bottom >= top,
-            ]
-        ):
-            return False  # not in the seeked direction
-
-        non_strict_match = not strict and (
-            left <= candidate.left <= right
-            or left <= candidate.right <= right
-            or candidate.left <= left <= candidate.right
-            or candidate.left <= right <= candidate.right
-        )
-        strict_match = strict and (candidate.left == left or candidate.right == right)
-        if not any([non_strict_match, strict_match]):
-            return False  # candidate not in boundaries
-
-        return self._check_text_match(candidate, regexp)
-
-    def _is_match_in_box(self, candidate: TextBox, *, anchor: TextBox) -> bool:
-        (left, bottom, right, top) = anchor.bbox
-        return (
-            left <= candidate.left
-            and right >= candidate.right
-            and bottom <= candidate.bottom
-            and top >= candidate.top
-        )
-
-    @staticmethod
-    def _sort_candidates_by_anchor(
-        candidates: List[TextBox], *, anchor: TextBox
-    ) -> None:
-        get_center = lambda item: (  # noqa: E731
-            (item.left + item.right) / 2,
-            (item.bottom + item.top) / 2,
-        )
-        anchor_center = get_center(anchor)
-
-        def get_distance(candidate):
-            candidate_center = get_center(candidate)
-            anchor_to_candidate_distance = math.sqrt(
-                math.pow((candidate_center[0] - anchor_center[0]), 2)
-                + math.pow((candidate_center[1] - anchor_center[1]), 2)
-            )
-            return anchor_to_candidate_distance
-
-        candidates.sort(key=get_distance)
+import functools
+import math
+import re
+from dataclasses import dataclass
+
+try:
+    # Python >=3.7
+    from re import Pattern
+except ImportError:
+    # Python =3.6
+    from re import _pattern_type as Pattern
+
+from typing import Callable, Dict, List, Optional, Union
+
+from RPA.PDF.keywords import LibraryContext, keyword
+from RPA.PDF.keywords.model import BaseElement, TextBox
+
+
+class TargetObject(BaseElement):
+    """Container for Target text boxes with coordinates."""
+
+    # Class level constants.
+    boxid: int = -1
+    text: str = ""
+
+
+Element = Union[TextBox, TargetObject]
+
+
+@dataclass
+class Match:
+    """Match object returned by the `Find Text` keyword.
+
+    It contains the anchor point and its relative found elements in text format.
+    """
+
+    anchor: str
+    direction: str
+    neighbours: List[str]
+
+
+class FinderKeywords(LibraryContext):
+    """Keywords for locating elements."""
+
+    RE_FLAGS = re.MULTILINE | re.DOTALL  # default regexp flags
+
+    def __init__(self, ctx):
+        super().__init__(ctx)
+
+        # Text locator might lead to multiple valid found anchors.
+        self._anchors: List[Element] = []
+        # The others usually have just one. (if multiple are found, set to it the
+        #   first one)
+        self.anchor_element = None
+
+    def _get_candidate_search_function(
+        self, direction: str, regexp: Optional[Pattern], strict: bool
+    ) -> Callable[[TextBox], bool]:
+        if direction in ["left", "right"]:
+            return functools.partial(
+                self._is_match_on_horizontal,
+                direction=direction,
+                regexp=regexp,
+                strict=strict,
+            )
+        if direction in ["top", "bottom", "up", "down"]:
+            return functools.partial(
+                self._is_match_on_vertical,
+                direction=direction,
+                regexp=regexp,
+                strict=strict,
+            )
+        if direction == "box":
+            return self._is_match_in_box
+
+        raise ValueError(f"Not recognized direction search {direction!r}")
+
+    def _log_element(self, elem: Element, prefix: str = ""):
+        template = f"{prefix} box %d | bbox %s | text %r"
+        self.logger.debug(template, elem.boxid, elem.bbox, elem.text)
+
+    @classmethod
+    def _re_flags(cls, ignore_case: bool) -> int:
+        flags = cls.RE_FLAGS
+        if ignore_case:
+            flags |= re.IGNORECASE
+        return flags
+
+    @keyword
+    def find_text(
+        self,
+        locator: str,
+        pagenum: Union[int, str] = 1,
+        direction: str = "right",
+        closest_neighbours: Optional[Union[int, str]] = 1,
+        strict: bool = False,
+        regexp: Optional[str] = None,
+        trim: bool = True,
+        ignore_case: bool = False,
+    ) -> List[Match]:
+        """Find the closest text elements near the set anchor(s) through `locator`.
+
+        The PDF will be parsed automatically before elements can be searched.
+
+        :param locator: Element to set anchor to. This can be prefixed with either
+            "text:", "subtext:", "regex:" or "coords:" to find the anchor by text or
+            coordinates. The "text" strategy is assumed if no such prefix is specified.
+            (text search is case-sensitive; use `ignore_case` param for controlling it)
+        :param pagenum: Page number where search is performed on, defaults to 1 (first
+            page).
+        :param direction: In which direction to search for text elements. This can be
+            any of 'top'/'up', 'bottom'/'down', 'left' or 'right'. (defaults to
+            'right')
+        :param closest_neighbours: How many neighbours to return at most, sorted by the
+            distance from the current anchor.
+        :param strict: If element's margins should be used for matching those which are
+            aligned to the anchor. (turned off by default)
+        :param regexp: Expected format of the searched text value. By default all the
+            candidates in range are considered valid neighbours.
+        :param trim: Automatically trim leading/trailing whitespace from the text
+            elements. (switched on by default)
+        :param ignore_case: Do a case-insensitive search when set to `True`. (affects
+            the passed `locator` and `regexp` filtering)
+        :returns: A list of `Match` objects where every match has the following
+            attributes: `.anchor` - the matched text with the locator; `.neighbours` -
+            a list of adjacent texts found on the specified direction
+
+        .. Attention::
+            Keep in mind that this keyword works with text-based PDFs, and it **can't
+            extract information from an image-based (scan)** PDF file. For accurate
+            results, you have to use specialized external services wrapped by the
+            ``RPA.DocumentAI`` library.
+
+        Portal example with video recording demo for parsing PDF invoices:
+        https://github.com/robocorp/example-parse-pdf-invoice
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            PDF Invoice Parsing
+                Open Pdf    invoice.pdf
+                ${matches} =  Find Text    Invoice Number
+                Log List      ${matches}
+
+        .. code-block::
+
+            List has one item:
+            Match(anchor='Invoice Number', direction='right', neighbours=['INV-3337'])
+
+        **Python**
+
+        .. code-block:: python
+
+            from RPA.PDF import PDF
+
+            pdf = PDF()
+
+            def pdf_invoice_parsing():
+                pdf.open_pdf("invoice.pdf")
+                matches = pdf.find_text("Invoice Number")
+                for match in matches:
+                    print(match)
+
+            pdf_invoice_parsing()
+
+        .. code-block::
+
+            Match(anchor='Invoice Number', direction='right', neighbours=['INV-3337'])
+        """
+        pagenum = int(pagenum)
+        if closest_neighbours is not None:
+            closest_neighbours = int(closest_neighbours)
+        self.logger.info(
+            "Searching for %s neighbour(s) to the %s of %r on page %d using regular "
+            "expression: %s (case %s)",
+            f"closest {closest_neighbours}"
+            if closest_neighbours is not None
+            else "all",
+            direction,
+            locator,
+            pagenum,
+            regexp,
+            "insensitive" if ignore_case else "sensitive",
+        )
+        self.set_anchor_to_element(
+            locator, trim=trim, pagenum=pagenum, ignore_case=ignore_case
+        )
+        if not self.anchor_element:
+            self.logger.warning("No anchor(s) set for locator: %s", locator)
+            return []
+
+        regexp_compiled = None
+        if regexp:
+            regexp_compiled = re.compile(regexp, flags=self._re_flags(ignore_case))
+        search_for_candidate = self._get_candidate_search_function(
+            direction, regexp_compiled, strict
+        )
+
+        candidates_dict: Dict[int, List[Element]] = {}
+        anchors_map: Dict[int, Element] = {}
+        for anchor in self._anchors:
+            candidates_dict[anchor.boxid] = []
+            anchors_map[anchor.boxid] = anchor
+
+        for candidate in self._get_textboxes_on_page(pagenum):
+            self._log_element(candidate, prefix="Current candidate:")
+            for anchor in self._anchors:
+                self._log_element(anchor, prefix="Current anchor:")
+                # Skip anchor element itself from matching and check if the candidate
+                # matches the search criteria.
+                if candidate.boxid != anchor.boxid and search_for_candidate(
+                    candidate, anchor=anchor
+                ):
+                    candidates_dict[anchor.boxid].append(candidate)
+
+        matches = []
+        for anchor_id, candidates in candidates_dict.items():
+            anchor = anchors_map[anchor_id]
+            self._sort_candidates_by_anchor(candidates, anchor=anchor)
+            if closest_neighbours is not None:
+                # Keep the first N closest neighbours from the entire set of candidates.
+                candidates[closest_neighbours:] = []
+            match = Match(
+                anchor=anchor.text,
+                direction=direction,
+                neighbours=[candidate.text for candidate in candidates],
+            )
+            matches.append(match)
+
+        return matches
+
+    @keyword
+    def set_anchor_to_element(
+        self,
+        locator: str,
+        trim: bool = True,
+        pagenum: Union[int, str] = 1,
+        ignore_case: bool = False,
+    ) -> bool:
+        """Sets main anchor point in the document for further searches.
+
+        This is used internally in the library and can work with multiple anchors at
+        the same time if such are found.
+
+        :param locator: Element to set anchor to. This can be prefixed with either
+            "text:", "subtext:", "regex:" or "coords:" to find the anchor by text or
+            coordinates. The "text" strategy is assumed if no such prefix is specified.
+            (text search is case-sensitive; use `ignore_case` param for controlling it)
+        :param trim: Automatically trim leading/trailing whitespace from the text
+            elements. (switched on by default)
+        :param pagenum: Page number where search is performed on, defaults to 1 (first
+            page).
+        :param ignore_case: Do a case-insensitive search when set to `True`.
+        :returns: True if at least one anchor was found.
+
+        **Examples**
+
+        **Robot Framework**
+
+        .. code-block:: robotframework
+
+            Example Keyword
+                 ${success} =  Set Anchor To Element    Invoice Number
+
+        **Python**
+
+        .. code-block:: python
+
+            from RPA.PDF import PDF
+
+            pdf = PDF()
+
+            def example_keyword():
+                success = pdf.set_anchor_to_element("Invoice Number")
+        """
+        pagenum = int(pagenum)
+        self.logger.info(
+            "Trying to set anchor on page %d using locator: %r (case %s)",
+            pagenum,
+            locator,
+            "insensitive" if ignore_case else "sensitive",
+        )
+        self.ctx.convert(trim=trim, pagenum=pagenum)
+        self._anchors.clear()
+        self.anchor_element = None
+
+        pure_locator = locator
+        criteria = "text"
+        parts = locator.split(":", 1)
+        if len(parts) == 2 and parts[0] in ("coords", "text", "regex", "subtext"):
+            criteria = parts[0]
+            pure_locator = parts[1]
+
+        if criteria == "coords":
+            coords = pure_locator.split(",")
+            if len(coords) == 2:
+                left, bottom = coords
+                top = bottom
+                right = left
+            elif len(coords) == 4:
+                left, bottom, right, top = coords
+            else:
+                raise ValueError("Give 2 coordinates for point, or 4 for area")
+
+            bbox = (
+                int(left),
+                int(bottom),
+                int(right),
+                int(top),
+            )
+            anchor = TargetObject(bbox=bbox)
+            self._anchors.append(anchor)
+        else:  # text-based search
+            if criteria == "regex":
+                pure_locator = re.compile(
+                    pure_locator, flags=self._re_flags(ignore_case)
+                )
+            anchors = self._find_matching_textboxes(
+                pure_locator,
+                pagenum=pagenum,
+                is_subtext=criteria == "subtext",
+                ignore_case=ignore_case,
+            )
+            self._anchors.extend(anchors)
+
+        if self._anchors:
+            self.anchor_element = self._anchors[0]
+            return True
+
+        return False
+
+    def _get_textboxes_on_page(self, pagenum: int) -> List[TextBox]:
+        page = self.active_pdf_document.get_page(pagenum)
+        return list(page.textboxes.values())
+
+    def _find_matching_textboxes(
+        self,
+        locator: Union[str, Pattern],
+        *,
+        pagenum: int,
+        is_subtext: bool = False,
+        ignore_case: bool = False,
+    ) -> List[TextBox]:
+        self.logger.info("Searching for matching text boxes with: %r", locator)
+
+        if isinstance(locator, str):
+            get_text = lambda string: (  # noqa: E731
+                string.lower() if ignore_case else string
+            )
+            if is_subtext:
+                matches_anchor = lambda _anchor: (  # noqa: E731
+                    get_text(locator) in get_text(_anchor.text)
+                )
+            else:
+                matches_anchor = lambda _anchor: (  # noqa: E731
+                    get_text(_anchor.text) == get_text(locator)
+                )
+        else:
+            matches_anchor = lambda _anchor: locator.match(_anchor.text)  # noqa: E731
+
+        anchors = []
+        for anchor in self._get_textboxes_on_page(pagenum):
+            if matches_anchor(anchor):
+                anchors.append(anchor)
+        if anchors:
+            self.logger.info("Found %d matches with locator %r", len(anchors), locator)
+            for anchor in anchors:
+                self._log_element(anchor)
+        else:
+            self.logger.warning("Did not find any matches with locator %r", locator)
+
+        return anchors
+
+    def _check_text_match(self, candidate: TextBox, regexp: Optional[Pattern]) -> bool:
+        if regexp and regexp.match(candidate.text):
+            self._log_element(candidate, prefix="Exact match:")
+            return True
+        if regexp is None:
+            self._log_element(candidate, prefix="Potential match:")
+            return True
+
+        return False
+
+    def _is_match_on_horizontal(
+        self,
+        candidate: TextBox,
+        *,
+        direction: str,
+        regexp: Optional[Pattern],
+        strict: bool,
+        anchor: TextBox,
+    ) -> bool:
+        (left, bottom, right, top) = anchor.bbox
+        direction_left = direction == "left"
+        direction_right = direction == "right"
+
+        if not any(
+            [
+                direction_left and candidate.right <= left,
+                direction_right and candidate.left >= right,
+            ]
+        ):
+            return False  # not in the seeked direction
+
+        non_strict_match = not strict and (
+            bottom <= candidate.bottom <= top
+            or bottom <= candidate.top <= top
+            or candidate.bottom <= bottom <= candidate.top
+            or candidate.bottom <= top <= candidate.top
+        )
+        strict_match = strict and (candidate.bottom == bottom or candidate.top == top)
+        if not any([non_strict_match, strict_match]):
+            return False  # candidate not in boundaries
+
+        return self._check_text_match(candidate, regexp)
+
+    def _is_match_on_vertical(
+        self,
+        candidate: TextBox,
+        *,
+        direction: str,
+        regexp: Optional[Pattern],
+        strict: bool,
+        anchor: TextBox,
+    ) -> bool:
+        (left, bottom, right, top) = anchor.bbox
+        direction_down = direction in ["bottom", "down"]
+        direction_up = direction in ["top", "up"]
+
+        if not any(
+            [
+                direction_down and candidate.top <= bottom,
+                direction_up and candidate.bottom >= top,
+            ]
+        ):
+            return False  # not in the seeked direction
+
+        non_strict_match = not strict and (
+            left <= candidate.left <= right
+            or left <= candidate.right <= right
+            or candidate.left <= left <= candidate.right
+            or candidate.left <= right <= candidate.right
+        )
+        strict_match = strict and (candidate.left == left or candidate.right == right)
+        if not any([non_strict_match, strict_match]):
+            return False  # candidate not in boundaries
+
+        return self._check_text_match(candidate, regexp)
+
+    def _is_match_in_box(self, candidate: TextBox, *, anchor: TextBox) -> bool:
+        (left, bottom, right, top) = anchor.bbox
+        return (
+            left <= candidate.left
+            and right >= candidate.right
+            and bottom <= candidate.bottom
+            and top >= candidate.top
+        )
+
+    @staticmethod
+    def _sort_candidates_by_anchor(
+        candidates: List[TextBox], *, anchor: TextBox
+    ) -> None:
+        get_center = lambda item: (  # noqa: E731
+            (item.left + item.right) / 2,
+            (item.bottom + item.top) / 2,
+        )
+        anchor_center = get_center(anchor)
+
+        def get_distance(candidate):
+            candidate_center = get_center(candidate)
+            anchor_to_candidate_distance = math.sqrt(
+                math.pow((candidate_center[0] - anchor_center[0]), 2)
+                + math.pow((candidate_center[1] - anchor_center[1]), 2)
+            )
+            return anchor_to_candidate_distance
+
+        candidates.sort(key=get_distance)
```

### Comparing `rpaframework_pdf-7.3.1/PKG-INFO` & `rpaframework_pdf-7.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-pdf
-Version: 7.3.1
+Version: 7.3.2
 Summary: PDF library of RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,pdf
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -14,23 +14,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: fpdf2 (>=2.7.5,<3.0.0)
+Requires-Dist: fpdf2 (==2.7.5)
 Requires-Dist: pdfminer.six (==20221105)
 Requires-Dist: pypdf (>=3.16.2,<4.0.0)
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,!=6.1.0,<7.0.0)
 Requires-Dist: robotframework-pythonlibcore (>=4.2.0,<5.0.0)
-Requires-Dist: rpaframework-core (>=11.2.1,<12.0.0)
+Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-pdf
 ================
```

