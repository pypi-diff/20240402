# Comparing `tmp/guarddog-1.5.5.tar.gz` & `tmp/guarddog-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.5.5.tar", max compression
+gzip compressed data, was "guarddog-1.5.6.tar", max compression
```

## Comparing `guarddog-1.5.5.tar` & `guarddog-1.5.6.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0    11377 2024-02-14 14:17:15.376340 guarddog-1.5.5/LICENSE
--rw-r--r--   0        0        0      314 2024-02-14 14:17:15.376340 guarddog-1.5.5/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      154 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9680 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0      609 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0      951 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0     2449 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/direct_url_dependency.py
--rw-r--r--   0        0        0      793 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     4215 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
--rw-r--r--   0        0        0     1260 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0     4153 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      976 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      723 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1873 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11635 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      438 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2024-02-14 14:17:15.380340 guarddog-1.5.5/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2024-02-14 14:17:15.384340 guarddog-1.5.5/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5619 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0      889 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      524 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/clipboard-access.yml
--rw-r--r--   0        0        0      682 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4599 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     1806 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2324 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1786 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0      716 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0      835 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0     1415 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    13158 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/cli.py
--rw-r--r--   0        0        0      315 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6189 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2512 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5491 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11104 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2024-02-14 14:17:15.388340 guarddog-1.5.5/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2024-02-14 14:17:15.388340 guarddog-1.5.5/pypi.rst
--rw-r--r--   0        0        0     1334 2024-02-14 14:17:28.184412 guarddog-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 guarddog-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11377 2024-04-02 20:03:33.960460 guarddog-1.5.6/LICENSE
+-rw-r--r--   0        0        0      314 2024-04-02 20:03:33.960460 guarddog-1.5.6/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      140 2024-04-02 20:03:33.960460 guarddog-1.5.6/NOTICE
+-rw-r--r--   0        0        0      154 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9680 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0      609 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0      951 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/direct_url_dependency.py
+-rw-r--r--   0        0        0      793 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     4215 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
+-rw-r--r--   0        0        0     1260 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0     4153 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      976 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1873 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11635 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      438 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2024-04-02 20:03:33.964460 guarddog-1.5.6/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2024-04-02 20:03:33.968459 guarddog-1.5.6/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5619 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0      889 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/clipboard-access.yml
+-rw-r--r--   0        0        0      682 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4599 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     1806 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2324 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1815 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0     1067 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0      835 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0     1415 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    13182 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2512 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5491 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11170 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2024-04-02 20:03:33.972460 guarddog-1.5.6/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2024-04-02 20:03:33.972460 guarddog-1.5.6/pypi.rst
+-rw-r--r--   0        0        0     1334 2024-04-02 20:03:45.008539 guarddog-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 guarddog-1.5.6/PKG-INFO
```

### Comparing `guarddog-1.5.5/LICENSE` & `guarddog-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/analyzer.py` & `guarddog-1.5.6/guarddog/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/detector.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/direct_url_dependency.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/direct_url_dependency.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.5.6/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.5.6/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.5.6/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/clipboard-access.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/clipboard-access.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     pattern-sources:
       - pattern: os.environ.items()
       - pattern: '[... for ... in os.environ.items()]'
       - pattern: socket.gethostname()
       - pattern: getpass.getuser()
       - pattern: platform.node()
       - pattern: browser_cookie3.$BROWSER(...)
+      - pattern: os.getcwd()
       - patterns:
           - pattern-either:
               - pattern: open($FILE)
               - pattern: open(... + $FILE)
           - metavariable-regex:
               metavariable: $FILE
               regex: ([\"\'].*(.aws/credentials|.docker/config.json)[\"\'])
```

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.5.6/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/cli.py` & `guarddog-1.5.6/guarddog/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         elif ecosystem == ECOSYSTEM.PYPI:
             all_rules |= set(get_metadata_detectors(ECOSYSTEM.PYPI).keys())
 
         rule_param = all_rules - set(exclude_rules)
 
         if len(rules) > 0:
             print("--rules and --exclude-rules cannot be used together")
-            exit(1)
+            sys.exit(1)
 
     return rule_param
 
 
 def _verify(path, rules, exclude_rules, output_format, exit_non_zero_on_finding, ecosystem):
     """Verify a requirements.txt file
 
@@ -188,32 +188,31 @@
         rules (list[str]): specific rules to run, defaults to all
     """
 
     rule_param = _get_rule_param(rules, exclude_rules, ecosystem)
     scanner = cast(Optional[PackageScanner], get_scanner(ecosystem, False))
     if scanner is None:
         sys.stderr.write(f"Command scan is not supported for ecosystem {ecosystem}")
-        exit(1)
+        sys.exit(1)
     results = []
     if is_local_target(identifier):
         log.debug(f"Considering that '{identifier}' is a local target, scanning filesystem")
         if os.path.isdir(identifier):
             log.debug(f"Considering that '{identifier}' as a local directory")
             for package in os.listdir(identifier):
                 results.append({'package': package} | scanner.scan_local(f"{identifier}/{package}", rule_param))
         else:
             results.append({'package': identifier} | scanner.scan_local(identifier, rule_param))
     else:
         log.debug(f"Considering that '{identifier}' is a remote target")
         try:
             results.append({'package': identifier} | scanner.scan_remote(identifier, version, rule_param))
         except Exception as e:
-            sys.stderr.write("\n")
-            sys.stderr.write(str(e))
-            sys.exit()
+            sys.stderr.write(f"\nError '{e}' occurred while scanning remote package.")
+            sys.exit(1)
 
     if output_format == "json":
         import json as js
         if len(results) == 1:
             # return only a json like {}
             print(js.dumps(results[0]))
         else:
```

### Comparing `guarddog-1.5.5/guarddog/reporters/sarif.py` & `guarddog-1.5.6/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/scanners/__init__.py` & `guarddog-1.5.6/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.5.6/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.5.6/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.5.6/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.5.6/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/scanners/scanner.py` & `guarddog-1.5.6/guarddog/scanners/scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,16 @@
             package_info, file_path = self.download_and_get_package_info(directory, name, version)
         except Exception as e:
             log.debug("Unable to download package, ignoring: " + str(e))
             return {'issues': 0, 'errors': {'download-package': str(e)}}
 
         results = self.analyzer.analyze(file_path, package_info, rules, name, version)
         if write_package_info:
-            suffix = f"{name}-{version}" if version is not None else name
+            package_name = name.replace("/", "-")
+            suffix = f"{package_name}-{version}" if version is not None else package_name
             with open(os.path.join(results["path"], f'package_info-{suffix}.json'), "w") as file:
                 file.write(json.dumps(package_info))
 
         return results
 
     def scan_remote(self, name, version=None, rules=None, base_dir=None, write_package_info=False):
         """
```

### Comparing `guarddog-1.5.5/guarddog/utils/archives.py` & `guarddog-1.5.6/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/guarddog/utils/package_info.py` & `guarddog-1.5.6/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.5/pyproject.toml` & `guarddog-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "guarddog"
 description = "GuardDog is a CLI tool to Identify malicious PyPI packages"
 authors = ["Ellen Wang", "Christophe Tafani-Dereeper"]
 license = "Apache-2.0"
 readme = "pypi.rst"
 repository = "https://github.com/DataDog/guarddog"
-version = "v1.5.5"
+version = "v1.5.6"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 # NOTE: Before https://github.com/returntocorp/semgrep/issues/6631 is addressed, we can't seem to upgrade past 0.112.1
```

### Comparing `guarddog-1.5.5/PKG-INFO` & `guarddog-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.5.5
+Version: 1.5.6
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

