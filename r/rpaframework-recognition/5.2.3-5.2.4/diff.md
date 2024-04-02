# Comparing `tmp/rpaframework_recognition-5.2.3.tar.gz` & `tmp/rpaframework_recognition-5.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_recognition-5.2.3.tar", max compression
+gzip compressed data, was "rpaframework_recognition-5.2.4.tar", max compression
```

## Comparing `rpaframework_recognition-5.2.3.tar` & `rpaframework_recognition-5.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11358 2021-09-09 09:55:26.470399 rpaframework_recognition-5.2.3/LICENSE
--rw-r--r--   0        0        0      213 2021-09-09 09:55:26.470493 rpaframework_recognition-5.2.3/README.rst
--rw-r--r--   0        0        0     1733 2023-10-10 16:48:33.620709 rpaframework_recognition-5.2.3/pyproject.toml
--rw-r--r--   0        0        0       96 2021-09-09 09:55:26.470821 rpaframework_recognition-5.2.3/src/RPA/recognition/__init__.py
--rw-r--r--   0        0        0     4565 2023-03-08 07:24:21.299506 rpaframework_recognition-5.2.3/src/RPA/recognition/ocr.py
--rw-r--r--   0        0        0     4482 2022-09-09 11:28:10.272313 rpaframework_recognition-5.2.3/src/RPA/recognition/templates.py
--rw-r--r--   0        0        0     1234 2021-09-09 09:55:26.471024 rpaframework_recognition-5.2.3/src/RPA/recognition/utils.py
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 rpaframework_recognition-5.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11560 2022-09-28 13:20:32.822375 rpaframework_recognition-5.2.4/LICENSE
+-rw-r--r--   0        0        0     1794 2024-04-02 10:19:38.016584 rpaframework_recognition-5.2.4/pyproject.toml
+-rw-r--r--   0        0        0      220 2022-09-28 13:20:32.823374 rpaframework_recognition-5.2.4/README.rst
+-rw-r--r--   0        0        0       99 2022-09-28 13:20:32.824375 rpaframework_recognition-5.2.4/src/RPA/recognition/__init__.py
+-rw-r--r--   0        0        0     4712 2023-12-05 08:21:31.490823 rpaframework_recognition-5.2.4/src/RPA/recognition/ocr.py
+-rw-r--r--   0        0        0     4614 2023-12-05 08:21:31.490823 rpaframework_recognition-5.2.4/src/RPA/recognition/templates.py
+-rw-r--r--   0        0        0     1278 2022-09-28 13:20:32.825374 rpaframework_recognition-5.2.4/src/RPA/recognition/utils.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 rpaframework_recognition-5.2.4/PKG-INFO
```

### Comparing `rpaframework_recognition-5.2.3/LICENSE` & `rpaframework_recognition-5.2.4/LICENSE`

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

### Comparing `rpaframework_recognition-5.2.3/pyproject.toml` & `rpaframework_recognition-5.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-[tool.poetry]
-name = "rpaframework-recognition"
-version = "5.2.3"
-description = "OCR capabilities used by RPA Framework"
-authors = ["RPA Framework <rpafw@robocorp.com>"]
-license = "Apache-2.0"
-readme = "README.rst"
-
-homepage = "https://rpaframework.org/"
-documentation = "https://rpaframework.org/"
-repository = "https://github.com/robocorp/rpaframework"
-
-keywords = ["robotframework", "rpa", "automation", "recognition", "cv", "ocr"]
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
-packages = [{ include = "RPA", from = "src" }]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-rpaframework-core = "^11.2.1"
-pillow = "^10.0.1"
-opencv-python-headless = "^4.8.1, <4.9.0"
-numpy = "^1.19.3"
-pytesseract = "^0.3.6"
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-flake8 = "^3.7.9"
-pylint = "^2.4.4, <2.13"
-pytest = "^7.2.0"
-mock = "^5.0.0"
-pytest-cov = "^4.0.0"
-toml = "^0.10.2"
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
+name = "rpaframework-recognition"
+version = "5.2.4"
+description = "OCR capabilities used by RPA Framework"
+authors = ["RPA Framework <rpafw@robocorp.com>"]
+license = "Apache-2.0"
+readme = "README.rst"
+
+homepage = "https://rpaframework.org/"
+documentation = "https://rpaframework.org/"
+repository = "https://github.com/robocorp/rpaframework"
+
+keywords = ["robotframework", "rpa", "automation", "recognition", "cv", "ocr"]
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
+packages = [{ include = "RPA", from = "src" }]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+rpaframework-core = "^11.3.1"
+pillow = "^10.2.0"
+opencv-python-headless = "^4.8.1, <4.9.0"
+numpy = "^1.19.3"
+pytesseract = "^0.3.6"
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.3.0"
+flake8 = "^3.7.9"
+pylint = "^2.4.4, <2.13"
+pytest = "^7.2.0"
+mock = "^5.0.0"
+pytest-cov = "^4.0.0"
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

### Comparing `rpaframework_recognition-5.2.3/src/RPA/recognition/ocr.py` & `rpaframework_recognition-5.2.4/src/RPA/recognition/ocr.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import logging
-from collections import defaultdict
-from difflib import SequenceMatcher
-from pathlib import Path
-from typing import Union, Dict, List, Generator, Optional
-
-import pytesseract
-from pytesseract import TesseractNotFoundError
-from PIL import Image
-
-from RPA.core import geometry
-from RPA.core.geometry import Region
-from RPA.recognition.utils import to_image, clamp
-
-LOGGER = logging.getLogger(__name__)
-
-# TODO: refer to conda package when created?
-INSTALL_PROMPT = (
-    "tesseract is not installed or not in PATH, "
-    "see library documentation for installation instructions"
-)
-
-DEFAULT_CONFIDENCE = 80.0
-
-
-def read(image: Union[Image.Image, Path]):
-    """Scan image for text and return it as one string.
-
-    :param image: Path to image or Image object
-    """
-    image = to_image(image)
-
-    try:
-        return pytesseract.image_to_string(image).strip()
-    except TesseractNotFoundError as err:
-        raise EnvironmentError(INSTALL_PROMPT) from err
-
-
-def find(
-    image: Union[Image.Image, Path],
-    text: str,
-    confidence: float = DEFAULT_CONFIDENCE,
-    region: Optional[Region] = None,
-    language: Optional[str] = None,
-):
-    """Scan image for text and return a list of regions
-    that contain it (or something close to it).
-
-    :param image: Path to image or Image object
-    :param text: Text to find in image
-    :param confidence: Minimum confidence for text similaritys
-    :param region: Limit the region of the screen where to look for the text
-    :param language: 3-character ISO 639-2 language code of the text.
-     This is passed directly to the pytesseract lib in the lang parameter.
-     See https://tesseract-ocr.github.io/tessdoc/Command-Line-Usage.html#using-one-language
-    """  # noqa: E501
-    image = to_image(image)
-    confidence = clamp(1, float(confidence), 100)
-
-    text = str(text).strip()
-    if not text:
-        raise ValueError("Empty search string")
-
-    if region is not None:
-        region = geometry.to_region(region)
-        image = image.crop(region.as_tuple())
-
-    try:
-        data = pytesseract.image_to_data(
-            image, lang=language, output_type=pytesseract.Output.DICT
-        )
-    except TesseractNotFoundError as err:
-        raise EnvironmentError(INSTALL_PROMPT) from err
-
-    lines = _dict_lines(data)
-    matches = _match_lines(lines, text, confidence)
-
-    if region is not None:
-        for match in matches:
-            match["region"] = match["region"].move(region.left, region.top)
-
-    return matches
-
-
-def _dict_lines(data: Dict) -> List:
-    lines = defaultdict(list)
-    for word in _iter_rows(data):
-        if word["level"] != 5:
-            continue
-
-        if not word["text"].strip():
-            continue
-
-        key = "{:d}-{:d}-{:d}".format(
-            word["block_num"], word["par_num"], word["line_num"]
-        )
-        region = Region.from_size(
-            word["left"], word["top"], word["width"], word["height"]
-        )
-
-        # NOTE: Currently ignoring confidence in tesseract results
-        lines[key].append({"text": word["text"], "region": region})
-        assert len(lines[key]) == word["word_num"]
-
-    return list(lines.values())
-
-
-def _iter_rows(data: Dict) -> Generator:
-    """Iterate dictionary of columns by row."""
-    return (dict(zip(data.keys(), values)) for values in zip(*data.values()))
-
-
-def _match_lines(lines: List[Dict], text: str, confidence: float) -> List[Dict]:
-    """Find best matches between lines of text and target text,
-    and return resulting bounding boxes and confidences.
-
-    A line of N words will be matched to the given text in all 1 to N
-    length sections, in every sequential position.
-    """
-    matches = []
-    for line in lines:
-        match = {}
-
-        for window in range(1, len(line) + 1):
-            for index in range(len(line) - window + 1):
-                words = line[index : index + window]
-                regions = [word["region"] for word in words]
-
-                sentence = " ".join(word["text"] for word in words)
-                ratio = SequenceMatcher(None, sentence, text).ratio() * 100.0
-
-                if ratio < confidence:
-                    continue
-
-                if match and match["confidence"] >= ratio:
-                    continue
-
-                match = {
-                    "text": sentence,
-                    "region": Region.merge(regions),
-                    "confidence": ratio,
-                }
-
-        if match:
-            matches.append(match)
-
-    return sorted(matches, key=lambda match: match["confidence"], reverse=True)
+import logging
+from collections import defaultdict
+from difflib import SequenceMatcher
+from pathlib import Path
+from typing import Union, Dict, List, Generator, Optional
+
+import pytesseract
+from pytesseract import TesseractNotFoundError
+from PIL import Image
+
+from RPA.core import geometry
+from RPA.core.geometry import Region
+from RPA.recognition.utils import to_image, clamp
+
+LOGGER = logging.getLogger(__name__)
+
+# TODO: refer to conda package when created?
+INSTALL_PROMPT = (
+    "tesseract is not installed or not in PATH, "
+    "see library documentation for installation instructions"
+)
+
+DEFAULT_CONFIDENCE = 80.0
+
+
+def read(image: Union[Image.Image, Path]):
+    """Scan image for text and return it as one string.
+
+    :param image: Path to image or Image object
+    """
+    image = to_image(image)
+
+    try:
+        return pytesseract.image_to_string(image).strip()
+    except TesseractNotFoundError as err:
+        raise EnvironmentError(INSTALL_PROMPT) from err
+
+
+def find(
+    image: Union[Image.Image, Path],
+    text: str,
+    confidence: float = DEFAULT_CONFIDENCE,
+    region: Optional[Region] = None,
+    language: Optional[str] = None,
+):
+    """Scan image for text and return a list of regions
+    that contain it (or something close to it).
+
+    :param image: Path to image or Image object
+    :param text: Text to find in image
+    :param confidence: Minimum confidence for text similaritys
+    :param region: Limit the region of the screen where to look for the text
+    :param language: 3-character ISO 639-2 language code of the text.
+     This is passed directly to the pytesseract lib in the lang parameter.
+     See https://tesseract-ocr.github.io/tessdoc/Command-Line-Usage.html#using-one-language
+    """  # noqa: E501
+    image = to_image(image)
+    confidence = clamp(1, float(confidence), 100)
+
+    text = str(text).strip()
+    if not text:
+        raise ValueError("Empty search string")
+
+    if region is not None:
+        region = geometry.to_region(region)
+        image = image.crop(region.as_tuple())
+
+    try:
+        data = pytesseract.image_to_data(
+            image, lang=language, output_type=pytesseract.Output.DICT
+        )
+    except TesseractNotFoundError as err:
+        raise EnvironmentError(INSTALL_PROMPT) from err
+
+    lines = _dict_lines(data)
+    matches = _match_lines(lines, text, confidence)
+
+    if region is not None:
+        for match in matches:
+            match["region"] = match["region"].move(region.left, region.top)
+
+    return matches
+
+
+def _dict_lines(data: Dict) -> List:
+    lines = defaultdict(list)
+    for word in _iter_rows(data):
+        if word["level"] != 5:
+            continue
+
+        if not word["text"].strip():
+            continue
+
+        key = "{:d}-{:d}-{:d}".format(
+            word["block_num"], word["par_num"], word["line_num"]
+        )
+        region = Region.from_size(
+            word["left"], word["top"], word["width"], word["height"]
+        )
+
+        # NOTE: Currently ignoring confidence in tesseract results
+        lines[key].append({"text": word["text"], "region": region})
+        assert len(lines[key]) == word["word_num"]
+
+    return list(lines.values())
+
+
+def _iter_rows(data: Dict) -> Generator:
+    """Iterate dictionary of columns by row."""
+    return (dict(zip(data.keys(), values)) for values in zip(*data.values()))
+
+
+def _match_lines(lines: List[Dict], text: str, confidence: float) -> List[Dict]:
+    """Find best matches between lines of text and target text,
+    and return resulting bounding boxes and confidences.
+
+    A line of N words will be matched to the given text in all 1 to N
+    length sections, in every sequential position.
+    """
+    matches = []
+    for line in lines:
+        match = {}
+
+        for window in range(1, len(line) + 1):
+            for index in range(len(line) - window + 1):
+                words = line[index : index + window]
+                regions = [word["region"] for word in words]
+
+                sentence = " ".join(word["text"] for word in words)
+                ratio = SequenceMatcher(None, sentence, text).ratio() * 100.0
+
+                if ratio < confidence:
+                    continue
+
+                if match and match["confidence"] >= ratio:
+                    continue
+
+                match = {
+                    "text": sentence,
+                    "region": Region.merge(regions),
+                    "confidence": ratio,
+                }
+
+        if match:
+            matches.append(match)
+
+    return sorted(matches, key=lambda match: match["confidence"], reverse=True)
```

### Comparing `rpaframework_recognition-5.2.3/src/RPA/recognition/templates.py` & `rpaframework_recognition-5.2.4/src/RPA/recognition/templates.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import logging
-from pathlib import Path
-from typing import Iterator, List, Optional, Union
-
-import cv2
-import numpy
-from PIL import Image
-
-from RPA.core import geometry
-from RPA.core.geometry import Region
-from RPA.recognition.utils import to_image, clamp, log2lin
-
-
-DEFAULT_CONFIDENCE = 80.0
-LIMIT_FAILSAFE = 256
-
-LOGGER = logging.getLogger(__name__)
-
-
-class ImageNotFoundError(Exception):
-    """Raised when template matching fails."""
-
-
-def find(
-    image: Union[Image.Image, Path],
-    template: Union[Image.Image, Path],
-    region: Optional[Region] = None,
-    limit: Optional[int] = None,
-    confidence: float = DEFAULT_CONFIDENCE,
-) -> List[Region]:
-    """Attempt to find the template from the given image.
-
-    :param image:       Path to image or Image instance, used to search from
-    :param template:    Path to image or Image instance, used to search with
-    :param limit:       Limit returned results to maximum of `limit`.
-    :param region:      Area to search from. Can speed up search significantly.
-    :param confidence:  Confidence for matching, value between 1 and 100
-    :return:            List of matching regions
-    :raises ImageNotFoundError: No match was found
-    """
-    # Ensure images are in Pillow format
-    image = to_image(image)
-    template = to_image(template)
-
-    # Convert confidence value to tolerance
-    tolerance = _to_tolerance(confidence)
-
-    # Crop image if requested
-    if region is not None:
-        region = geometry.to_region(region)
-        image = image.crop(region.as_tuple())
-
-    # Verify template still fits in image
-    if template.size[0] > image.size[0] or template.size[1] > image.size[1]:
-        raise ValueError("Template is larger than search region")
-
-    # Do the actual search
-    matches: List[Region] = []
-    for match in _match_template(image, template, tolerance):
-        matches.append(match)
-        if limit is not None and len(matches) >= int(limit):
-            break
-        elif len(matches) >= LIMIT_FAILSAFE:
-            LOGGER.warning("Reached maximum of %d matches", LIMIT_FAILSAFE)
-            break
-
-    if not matches:
-        raise ImageNotFoundError("No matches for given template")
-
-    # Convert region coördinates back to full-size coördinates
-    if region is not None:
-        matches = [match.move(region.left, region.top) for match in matches]
-
-    return matches
-
-
-def _to_tolerance(confidence):
-    """Convert confidence value to tolerance.
-
-    Confidence is a logarithmic scale from 1 to 100,
-    tolerance is a linear scale from 0.01 to 1.00.
-    """
-    value = float(confidence)
-    value = clamp(1, value, 100)
-    value = log2lin(1, value, 100)
-    value = value / 100.0
-    return value
-
-
-def _match_template(
-    image: Image.Image, template: Image.Image, tolerance: float
-) -> Iterator[Region]:
-    """Use opencv's matchTemplate() to slide the `template` over
-    `image` to calculate correlation coefficients, and then
-    filter with a tolerance to find all relevant global maximums.
-    """
-    template_width, template_height = template.size
-
-    if image.mode == "RGBA":
-        image = image.convert("RGB")
-    if template.mode == "RGBA":
-        template = template.convert("RGB")
-
-    image = numpy.array(image)
-    template = numpy.array(template)
-
-    # pylint: disable=no-member
-    image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
-    template = cv2.cvtColor(template, cv2.COLOR_RGB2BGR)
-
-    # Template matching result is a single channel array of shape:
-    # Width:  Image width  - template width  + 1
-    # Height: Image height - template height + 1
-    coefficients = cv2.matchTemplate(image, template, cv2.TM_CCOEFF_NORMED)
-    coeff_height, coeff_width = coefficients.shape
-
-    while True:
-        # The point (match_x, match_y) is the top-left of the best match
-        _, match_coeff, _, (match_x, match_y) = cv2.minMaxLoc(coefficients)
-        if match_coeff < tolerance:
-            break
-
-        # Zero out values for a template-sized region around the best match
-        # to prevent duplicate matches for the same element.
-        left = clamp(0, match_x - template_width // 2, coeff_width)
-        top = clamp(0, match_y - template_height // 2, coeff_height)
-        right = clamp(0, match_x + template_width // 2, coeff_width)
-        bottom = clamp(0, match_y + template_height // 2, coeff_height)
-
-        coefficients[top:bottom, left:right] = 0
-
-        yield Region.from_size(match_x, match_y, template_width, template_height)
+import logging
+from pathlib import Path
+from typing import Iterator, List, Optional, Union
+
+import cv2
+import numpy
+from PIL import Image
+
+from RPA.core import geometry
+from RPA.core.geometry import Region
+from RPA.recognition.utils import to_image, clamp, log2lin
+
+
+DEFAULT_CONFIDENCE = 80.0
+LIMIT_FAILSAFE = 256
+
+LOGGER = logging.getLogger(__name__)
+
+
+class ImageNotFoundError(Exception):
+    """Raised when template matching fails."""
+
+
+def find(
+    image: Union[Image.Image, Path],
+    template: Union[Image.Image, Path],
+    region: Optional[Region] = None,
+    limit: Optional[int] = None,
+    confidence: float = DEFAULT_CONFIDENCE,
+) -> List[Region]:
+    """Attempt to find the template from the given image.
+
+    :param image:       Path to image or Image instance, used to search from
+    :param template:    Path to image or Image instance, used to search with
+    :param limit:       Limit returned results to maximum of `limit`.
+    :param region:      Area to search from. Can speed up search significantly.
+    :param confidence:  Confidence for matching, value between 1 and 100
+    :return:            List of matching regions
+    :raises ImageNotFoundError: No match was found
+    """
+    # Ensure images are in Pillow format
+    image = to_image(image)
+    template = to_image(template)
+
+    # Convert confidence value to tolerance
+    tolerance = _to_tolerance(confidence)
+
+    # Crop image if requested
+    if region is not None:
+        region = geometry.to_region(region)
+        image = image.crop(region.as_tuple())
+
+    # Verify template still fits in image
+    if template.size[0] > image.size[0] or template.size[1] > image.size[1]:
+        raise ValueError("Template is larger than search region")
+
+    # Do the actual search
+    matches: List[Region] = []
+    for match in _match_template(image, template, tolerance):
+        matches.append(match)
+        if limit is not None and len(matches) >= int(limit):
+            break
+        elif len(matches) >= LIMIT_FAILSAFE:
+            LOGGER.warning("Reached maximum of %d matches", LIMIT_FAILSAFE)
+            break
+
+    if not matches:
+        raise ImageNotFoundError("No matches for given template")
+
+    # Convert region coördinates back to full-size coördinates
+    if region is not None:
+        matches = [match.move(region.left, region.top) for match in matches]
+
+    return matches
+
+
+def _to_tolerance(confidence):
+    """Convert confidence value to tolerance.
+
+    Confidence is a logarithmic scale from 1 to 100,
+    tolerance is a linear scale from 0.01 to 1.00.
+    """
+    value = float(confidence)
+    value = clamp(1, value, 100)
+    value = log2lin(1, value, 100)
+    value = value / 100.0
+    return value
+
+
+def _match_template(
+    image: Image.Image, template: Image.Image, tolerance: float
+) -> Iterator[Region]:
+    """Use opencv's matchTemplate() to slide the `template` over
+    `image` to calculate correlation coefficients, and then
+    filter with a tolerance to find all relevant global maximums.
+    """
+    template_width, template_height = template.size
+
+    if image.mode == "RGBA":
+        image = image.convert("RGB")
+    if template.mode == "RGBA":
+        template = template.convert("RGB")
+
+    image = numpy.array(image)
+    template = numpy.array(template)
+
+    # pylint: disable=no-member
+    image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+    template = cv2.cvtColor(template, cv2.COLOR_RGB2BGR)
+
+    # Template matching result is a single channel array of shape:
+    # Width:  Image width  - template width  + 1
+    # Height: Image height - template height + 1
+    coefficients = cv2.matchTemplate(image, template, cv2.TM_CCOEFF_NORMED)
+    coeff_height, coeff_width = coefficients.shape
+
+    while True:
+        # The point (match_x, match_y) is the top-left of the best match
+        _, match_coeff, _, (match_x, match_y) = cv2.minMaxLoc(coefficients)
+        if match_coeff < tolerance:
+            break
+
+        # Zero out values for a template-sized region around the best match
+        # to prevent duplicate matches for the same element.
+        left = clamp(0, match_x - template_width // 2, coeff_width)
+        top = clamp(0, match_y - template_height // 2, coeff_height)
+        right = clamp(0, match_x + template_width // 2, coeff_width)
+        bottom = clamp(0, match_y + template_height // 2, coeff_height)
+
+        coefficients[top:bottom, left:right] = 0
+
+        yield Region.from_size(match_x, match_y, template_width, template_height)
```

### Comparing `rpaframework_recognition-5.2.3/src/RPA/recognition/utils.py` & `rpaframework_recognition-5.2.4/src/RPA/recognition/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import base64
-import io
-import math
-from typing import Any
-
-from PIL import Image
-
-
-def to_image(obj: Any) -> Image.Image:
-    """Convert `obj` to instance of Pillow's Image class."""
-    if obj is None or isinstance(obj, Image.Image):
-        return obj
-    return Image.open(obj)
-
-
-def image_to_base64(image: Image.Image) -> str:
-    """Convert Image object to base64 string."""
-    stream = io.BytesIO()
-    image.save(stream)
-    data = stream.getvalue()
-    text = base64.b64encode(data).decode()
-    return text
-
-
-def base64_to_image(text: str) -> Image.Image:
-    """Convert image in base64 string to Image object."""
-    data = base64.b64decode(text)
-    stream = io.BytesIO(data)
-    image = Image.open(stream)
-    return image
-
-
-def clamp(minimum: float, value: float, maximum: float) -> float:
-    """Clamp value between given minimum and maximum."""
-    return max(minimum, min(value, maximum))
-
-
-def log2lin(minimum: float, value: float, maximum: float) -> float:
-    """Maps logarithmic scale to linear scale of same range."""
-    assert value >= minimum
-    assert value <= maximum
-    return (maximum - minimum) * (math.log(value) - math.log(minimum)) / (
-        math.log(maximum) - math.log(minimum)
-    ) + minimum
+import base64
+import io
+import math
+from typing import Any
+
+from PIL import Image
+
+
+def to_image(obj: Any) -> Image.Image:
+    """Convert `obj` to instance of Pillow's Image class."""
+    if obj is None or isinstance(obj, Image.Image):
+        return obj
+    return Image.open(obj)
+
+
+def image_to_base64(image: Image.Image) -> str:
+    """Convert Image object to base64 string."""
+    stream = io.BytesIO()
+    image.save(stream)
+    data = stream.getvalue()
+    text = base64.b64encode(data).decode()
+    return text
+
+
+def base64_to_image(text: str) -> Image.Image:
+    """Convert image in base64 string to Image object."""
+    data = base64.b64decode(text)
+    stream = io.BytesIO(data)
+    image = Image.open(stream)
+    return image
+
+
+def clamp(minimum: float, value: float, maximum: float) -> float:
+    """Clamp value between given minimum and maximum."""
+    return max(minimum, min(value, maximum))
+
+
+def log2lin(minimum: float, value: float, maximum: float) -> float:
+    """Maps logarithmic scale to linear scale of same range."""
+    assert value >= minimum
+    assert value <= maximum
+    return (maximum - minimum) * (math.log(value) - math.log(minimum)) / (
+        math.log(maximum) - math.log(minimum)
+    ) + minimum
```

### Comparing `rpaframework_recognition-5.2.3/PKG-INFO` & `rpaframework_recognition-5.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-recognition
-Version: 5.2.3
+Version: 5.2.4
 Summary: OCR capabilities used by RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,recognition,cv,ocr
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8,<4.0
@@ -15,21 +15,22 @@
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
 Requires-Dist: numpy (>=1.19.3,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.8.1,<4.9.0)
-Requires-Dist: pillow (>=10.0.1,<11.0.0)
+Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pytesseract (>=0.3.6,<0.4.0)
-Requires-Dist: rpaframework-core (>=11.2.1,<12.0.0)
+Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-recognition
 ========================
```

