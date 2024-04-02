# Comparing `tmp/vtx-common-0.1.8.tar.gz` & `tmp/vtx-common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vtx-common-0.1.8.tar", last modified: Wed Aug 11 12:41:45 2021, max compression
+gzip compressed data, was "dist/vtx-common-0.1.9.tar", last modified: Mon Aug 23 14:17:13 2021, max compression
```

## Comparing `vtx-common-0.1.8.tar` & `vtx-common-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:45.000000 vtx-common-0.1.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2866 2021-08-11 12:41:45.000000 vtx-common-0.1.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1882 2021-08-11 12:41:28.000000 vtx-common-0.1.8/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      360 2021-08-11 12:41:45.000000 vtx-common-0.1.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2067 2021-08-11 12:41:28.000000 vtx-common-0.1.8/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tests/common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6442 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tests/test_github_release.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tests/test_utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common/tools/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tools/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7149 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tools/github_release.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      804 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tools/pep8_staged_files.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1649 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/tools/pre_commit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-08-11 12:41:28.000000 vtx-common-0.1.8/vtx_common/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2866 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2021-08-11 12:41:45.000000 vtx-common-0.1.8/vtx_common.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:17:13.000000 vtx-common-0.1.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2866 2021-08-23 14:17:13.000000 vtx-common-0.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1882 2021-08-23 14:16:52.000000 vtx-common-0.1.9/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      360 2021-08-23 14:17:13.000000 vtx-common-0.1.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2095 2021-08-23 14:16:52.000000 vtx-common-0.1.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1535 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tests/common.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      970 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tests/test_get_pkg_syn_minver.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6442 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tests/test_github_release.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tests/test_utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common/tools/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tools/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1447 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tools/get_pkg_syn_minver.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10058 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tools/github_release.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      804 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tools/pep8_staged_files.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1649 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/tools/pre_commit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-08-23 14:16:52.000000 vtx-common-0.1.9/vtx_common/version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2866 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      175 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2021-08-23 14:17:13.000000 vtx-common-0.1.9/vtx_common.egg-info/top_level.txt
```

### Comparing `vtx-common-0.1.8/PKG-INFO` & `vtx-common-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtx-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: Vertex project tools to assist with packaging.
 Home-page: https://github.com/vertexproject/common-tools
 Author: The Vertex Project LLC
 Author-email: epiphyte+tools@vertex.link
 License: Apache License 2.0
 Description: ===================
         Vertex Common Tools
```

### Comparing `vtx-common-0.1.8/README.rst` & `vtx-common-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `vtx-common-0.1.8/setup.py` & `vtx-common-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
 
     def run(self):
         tag = os.getenv('CIRCLE_TAG', '')
@@ -45,14 +45,15 @@
     packages=find_packages(exclude=['scripts',
                                     ]),
 
     include_package_data=True,
 
     install_requires=[
         'PyGithub==1.53',
+        'PyYAML>=5.4,<6.0',
         'bump2version==1.0.1',
         'pytest>=5.0.0,<6.0.0',
         'autopep8>=1.5.3,<2.0.0',
         'pytest-cov>=2.9.0,<3.0.0',
         'pycodestyle>=2.6.0,<3.0.0',
         'pytest-xdist>=1.32.0,<2.0.0',
     ],
```

### Comparing `vtx-common-0.1.8/vtx_common/tests/test_github_release.py` & `vtx-common-0.1.9/vtx_common/tests/test_github_release.py`

 * *Files identical despite different names*

### Comparing `vtx-common-0.1.8/vtx_common/tests/test_utils.py` & `vtx-common-0.1.9/vtx_common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vtx-common-0.1.8/vtx_common/tools/github_release.py` & `vtx-common-0.1.9/vtx_common/tools/github_release.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,34 @@
 import collections
 import configparser
 
 from typing import List, AnyStr
 
 import github
 
+import vtx_common.tools.get_pkg_syn_minver as v_gpsm
+
+
 HEADER_RE = r'v[0-9]+\.[0-9]+\.[0-9]+((a|b|rc)[0-9]*)?\s-\s20[0-9]{2}-[0-9]{2}-[0-9]{2}'
 PASSLINE = r'^=.*$'
 SEMVER_RE = r'v[0-9]+\.[0-9]+\.[0-9]+(?P<pre>((a|b|rc)[0-9]*)?)'
 URL_RE = r'\s+\(`#\d+\s<http'
 logger = logging.getLogger(__name__)
 
 CFG_HEADER = 'vtx_common:github_release'
 
-RELEASE_NAME = 'release_name'
-REMOVE_URLS = 'remove_urls'
 DRYRUN = 'dryrun'
 CHANGELOG = 'changelog'
+CHANGELOG_PKGNAME = 'changelog_pkgname'
+REMOVE_URLS = 'remove_urls'
+RELEASE_NAME = 'release_name'
+STORM_PKG_FILE = 'storm_pkg_file'
+STORM_PKG_TYPE = 'storm_pkg_type'
+STORM_PKG_FILE_PKGNAME = 'storm_pkg_file_pkgname'
+
 CFG_OPTS = {
     'release-name': {
         'type': 'str',
         'key': RELEASE_NAME,
     },
     'extra-lines': {
         'type': 'str',
@@ -36,39 +44,64 @@
         'type': 'bool',
         'key': REMOVE_URLS,
     },
     'dry-run': {
         'type': 'bool',
         'key': DRYRUN,
     },
+    'storm-pkg-file': {
+        'type': 'str',
+        'key': STORM_PKG_FILE,
+    },
+    'storm-pkg-file-pkgname': {
+        'type': 'bool',
+        'key': STORM_PKG_FILE_PKGNAME,
+    },
+    'storm-pkg-type': {
+        'type': 'str',
+        'key': STORM_PKG_TYPE,
+    },
     'changelog': {
         'type': 'str',
         'key': CHANGELOG,
-    }
+    },
+    'changelog-pkgname': {
+        'type': 'bool',
+        'key': CHANGELOG_PKGNAME,
+    },
 }
 
 def get_parser():
     pars = argparse.ArgumentParser()
     pars.add_argument('-g', '--github-token', dest='gittokenvar', default='GITHUB_TOKEN', type=str,
                       help='Environment variable to pull the github token from.')
     pars.add_argument('-u', '--github-user', dest='gituservar', default='CIRCLE_PROJECT_USERNAME', type=str,
                       help='Environment variable to pull the github user from')
     pars.add_argument('-r', '--github-repo', dest='gitrepovar', default='CIRCLE_PROJECT_REPONAME', type=str,
                       help='Environment variable to pull the github repo from')
     pars.add_argument('-t', '--tagvar', dest='tagvar', default='CIRCLE_TAG', type=str,
                       help='Environment variable to pull the tag from.')
     pars.add_argument('-c', '--changelog', dest=CHANGELOG, default='./CHANGELOG.rst',
                       help='Path to changelog file to process')
+    pars.add_argument('--changelog-pkgname', dest=CHANGELOG_PKGNAME, default=False, action='store_true',
+                      help='inject package name derived from a tag into the changelog path.')
     pars.add_argument('--remove-urls', dest=REMOVE_URLS, default=False, action='store_true',
                       help='Remove lines starting with RST formated links.')
     pars.add_argument('-d', '--dry-run', dest=DRYRUN, default=False, action='store_true',
                       help='Do not do an actual Github release action. Does not require github variables to be set.'
                            'Does require the tag variable to be set. This will print the changlog found to stderr.')
     pars.add_argument('--release-name', dest=RELEASE_NAME, default=None, type=str,
                       help='Release name to prefix the tag with for the github release.')
+    pars.add_argument('--pkg-file', dest=STORM_PKG_FILE, default=None, type=str,
+                      help='Storm package file to get minimum storm service from.')
+    pars.add_argument('--pkg-file', dest=STORM_PKG_FILE_PKGNAME, default=False, action='store_true',
+                      help='inject pkgname derived from a tag into the pkgapath path')
+    pars.add_argument('--pkg-type', dest=STORM_PKG_TYPE, default=None, type=str, choices=['Storm Service', 'Power-Up'],
+                      help='Storm package file to get minimum storm service from.')
+
     return pars
 
 def parse_changelog(s: str) -> dict:
     curv = None
     ret = collections.defaultdict(list)
     for line in s.split('\n'):
         if re.match(HEADER_RE, line):
@@ -96,27 +129,27 @@
         logger.debug('Config file [{}] does not exist.')
         return
 
     config = configparser.RawConfigParser()
     config.read(fn)
 
     if not config.has_section(CFG_HEADER):
-        return
+        logger.info(f'No {CFG_HEADER} header found')
 
     for opt, info in CFG_OPTS.items():
         typ = info.get('type')
         defval = info.get('defval')
         try:
             if typ == 'bool':
                 valu = config.getboolean(CFG_HEADER, opt)
             elif typ == 'int':
                 valu = config.getint(CFG_HEADER, opt)
             else:
                 valu = config.get(CFG_HEADER, opt,)
-        except configparser.NoOptionError:
+        except (configparser.NoOptionError, configparser.NoSectionError):
             if defval is None:
                 continue
             valu = defval
 
         setattr(opts, info.get('key'), valu)
 
     logger.info(f'Parsed {opts} from setup.cfg')
@@ -133,17 +166,23 @@
 
     tag = os.getenv(opts.tagvar, '')
     if not tag:
         logger.error(f'No tag found for {opts.tagvar}')
         return 1
 
     logger.info(f'envar {opts.tagvar} resolved to {tag}')
-    m = re.search(SEMVER_RE, tag)
+    nicetag = tag
+    pkgname = None
+    if '@' in tag:
+        logger.info('@ delimited tag, splitting into name and tag part')
+        pkgname, nicetag = tag.split('@')
+        logger.info(f'Got pkgname={pkgname} @ nicetag={nicetag}')
+    m = re.search(SEMVER_RE, nicetag)
     if not m:
-        logger.error('tag does not match semver regex')
+        logger.error(f'nicetag={nicetag} does not match semver regex')
         return 1
     is_prerelease = False
     if m.groupdict().get('pre'):
         is_prerelease = True
 
     defvalu = ''
     if opts.dryrun:
@@ -158,28 +197,56 @@
         logger.error('No github user found')
         return 1
     gh_repo = os.getenv(opts.gitrepovar, defvalu)
     if not gh_repo:
         logger.error('No github repo found')
         return 1
 
+    extra_parts = []
+
+    pfile = opts.storm_pkg_file
+    mtyp = opts.storm_pkg_type
+    if pfile and mtyp:
+
+        if opts.storm_pkg_file_pkgname:
+            assert pkgname is not None
+            logger.info('Injecting pkgname to pkg path')
+            pfile = pfile.format(pkgname=pkgname)
+
+        logger.info(f'Getting storm package from {pfile}')
+        pkg = v_gpsm.yamlload(pfile)
+        minv_message = v_gpsm.getMessageFromPkg(pkg, mtyp)
+        logger.info(f'Got message: {minv_message}')
+        extra_parts.append(minv_message)
+
     extra_lines = opts.extra_lines
     if extra_lines:
         logger.info(f'Extra lines found: {extra_lines}')
+        extra_parts.append(extra_lines)
+
+    # Join extra lines together
+    extra_lines = '\n'.join(extra_parts)
 
-    raw_changelog = open(opts.changelog, 'rb').read().decode()
+    changelog_fp = opts.changelog
+    if opts.changelog_pkgname:
+        assert pkgname is not None
+        logger.info('Injecting pkgname to changelog path')
+        changelog_fp = changelog_fp.format(pkgname=pkgname)
+
+    assert os.path.isfile(changelog_fp)
+    raw_changelog = open(changelog_fp, 'rb').read().decode()
     parsed_logs = parse_changelog(raw_changelog)
 
-    target_log = parsed_logs.get(tag)
+    target_log = parsed_logs.get(nicetag)
     if not target_log:
-        logger.error(f'Unable to find logs for tag [{tag}]')
+        logger.error(f'Unable to find logs for tag [{nicetag}]')
         # It's possible for pre-release tags to end up without a changelog.
         # This condition should not end up failing a CI pipeline.
         return 0
-    logger.info(f'Found changelogs for [{tag}]')
+    logger.info(f'Found changelogs for [{nicetag}] in [{opts.changelog}]')
 
     if opts.remove_urls:
         logger.info('Removing URLs')
         target_log = remove_urls(target_log)
 
     # join logs together and strip them
     target_log = '\n'.join(target_log)
@@ -196,22 +263,28 @@
         logger.debug(line)
 
     name = tag
     if opts.release_name:
         name = f'{opts.release_name} {tag}'
 
     logger.info(f'Release Name: [{name}]')
+    gh_repo_path = f'{gh_username}/{gh_repo}'
 
     if opts.dryrun:
         logger.info('Dry-run mode enabled. Not performing a Github release action.')
+        logger.info('Would have made release with the following information:')
+        logger.info(f'gh_repo_path={gh_repo_path}')
+        logger.info(f'tag={tag}')
+        logger.info(f'name={name}')
+        logger.info(f'prerelease={is_prerelease}')
+        logger.info(f'message={target_log}')
         return 0
 
     gh = github.Github(gh_token)
 
-    gh_repo_path = f'{gh_username}/{gh_repo}'
     logger.info(f'Getting github repo for {gh_repo_path}')
     repo = gh.get_repo(gh_repo_path)
 
     logger.info('Making github release')
     release = repo.create_git_release(tag=tag,
                                       name=name,
                                       draft=False,
```

### Comparing `vtx-common-0.1.8/vtx_common/tools/pep8_staged_files.py` & `vtx-common-0.1.9/vtx_common/tools/pep8_staged_files.py`

 * *Files identical despite different names*

### Comparing `vtx-common-0.1.8/vtx_common/tools/pre_commit.py` & `vtx-common-0.1.9/vtx_common/tools/pre_commit.py`

 * *Files identical despite different names*

### Comparing `vtx-common-0.1.8/vtx_common/utils.py` & `vtx-common-0.1.9/vtx_common/utils.py`

 * *Files identical despite different names*

### Comparing `vtx-common-0.1.8/vtx_common.egg-info/PKG-INFO` & `vtx-common-0.1.9/vtx_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtx-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: Vertex project tools to assist with packaging.
 Home-page: https://github.com/vertexproject/common-tools
 Author: The Vertex Project LLC
 Author-email: epiphyte+tools@vertex.link
 License: Apache License 2.0
 Description: ===================
         Vertex Common Tools
```

### Comparing `vtx-common-0.1.8/vtx_common.egg-info/SOURCES.txt` & `vtx-common-0.1.9/vtx_common.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,13 +7,15 @@
 vtx_common.egg-info/PKG-INFO
 vtx_common.egg-info/SOURCES.txt
 vtx_common.egg-info/dependency_links.txt
 vtx_common.egg-info/requires.txt
 vtx_common.egg-info/top_level.txt
 vtx_common/tests/__init__.py
 vtx_common/tests/common.py
+vtx_common/tests/test_get_pkg_syn_minver.py
 vtx_common/tests/test_github_release.py
 vtx_common/tests/test_utils.py
 vtx_common/tools/__init__.py
+vtx_common/tools/get_pkg_syn_minver.py
 vtx_common/tools/github_release.py
 vtx_common/tools/pep8_staged_files.py
 vtx_common/tools/pre_commit.py
```

