# Comparing `tmp/git_changelog-2.4.1.tar.gz` & `tmp/git_changelog-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_changelog-2.4.1.tar", last modified: Thu Mar 14 13:35:36 2024, max compression
+gzip compressed data, was "git_changelog-2.5.0.tar", last modified: Mon Apr  1 22:31:20 2024, max compression
```

## Comparing `git_changelog-2.4.1.tar` & `git_changelog-2.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      754 2024-03-14 13:21:38.029424 git_changelog-2.4.1/LICENSE
--rw-r--r--   0        0        0     4356 2024-03-14 13:21:38.029424 git_changelog-2.4.1/README.md
--rw-r--r--   0        0        0     1830 2024-03-14 13:35:36.360043 git_changelog-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      278 2024-03-14 13:21:38.029424 git_changelog-2.4.1/src/git_changelog/__init__.py
--rw-r--r--   0        0        0      387 2024-03-14 13:21:38.029424 git_changelog-2.4.1/src/git_changelog/__main__.py
--rw-r--r--   0        0        0    19442 2024-03-14 13:18:19.165573 git_changelog-2.4.1/src/git_changelog/build.py
--rw-r--r--   0        0        0    24717 2024-03-14 13:21:38.029424 git_changelog-2.4.1/src/git_changelog/cli.py
--rw-r--r--   0        0        0    13517 2024-03-14 13:18:19.212216 git_changelog-2.4.1/src/git_changelog/commit.py
--rw-r--r--   0        0        0     2710 2024-03-14 13:21:35.667272 git_changelog-2.4.1/src/git_changelog/debug.py
--rw-r--r--   0        0        0    13417 2023-08-21 08:53:30.539869 git_changelog-2.4.1/src/git_changelog/providers.py
--rw-r--r--   0        0        0        0 2024-03-14 13:21:35.670603 git_changelog-2.4.1/src/git_changelog/py.typed
--rw-r--r--   0        0        0     1122 2023-02-03 19:05:40.815432 git_changelog-2.4.1/src/git_changelog/templates/__init__.py
--rw-r--r--   0        0        0     1588 2023-02-04 13:50:13.931438 git_changelog-2.4.1/src/git_changelog/templates/angular.md.jinja
--rw-r--r--   0        0        0     2213 2023-02-04 13:49:16.982323 git_changelog-2.4.1/src/git_changelog/templates/keepachangelog.md.jinja
--rw-r--r--   0        0        0      166 2024-03-14 13:21:35.680599 git_changelog-2.4.1/tests/__init__.py
--rw-r--r--   0        0        0      850 2024-03-14 13:21:38.029424 git_changelog-2.4.1/tests/conftest.py
--rw-r--r--   0        0        0     2839 2024-03-14 13:18:19.212216 git_changelog-2.4.1/tests/helpers.py
--rw-r--r--   0        0        0     2361 2023-08-21 08:53:30.539869 git_changelog-2.4.1/tests/test_angular_style.py
--rw-r--r--   0        0        0     2308 2023-08-21 08:53:30.539869 git_changelog-2.4.1/tests/test_basic_style.py
--rw-r--r--   0        0        0     5849 2024-03-14 13:18:19.228875 git_changelog-2.4.1/tests/test_build.py
--rw-r--r--   0        0        0     6573 2024-03-14 13:21:38.029424 git_changelog-2.4.1/tests/test_cli.py
--rw-r--r--   0        0        0     1079 2023-11-04 15:32:33.005418 git_changelog-2.4.1/tests/test_commit.py
--rw-r--r--   0        0        0     5483 2023-08-21 08:53:30.539869 git_changelog-2.4.1/tests/test_conventional_commit_style.py
--rw-r--r--   0        0        0     6527 2024-03-07 18:44:41.163788 git_changelog-2.4.1/tests/test_end_to_end.py
--rw-r--r--   0        0        0     1505 2023-08-21 08:53:30.539869 git_changelog-2.4.1/tests/test_providers.py
--rw-r--r--   0        0        0      897 2023-08-21 08:53:30.543202 git_changelog-2.4.1/tests/test_release_notes.py
--rw-r--r--   0        0        0     3091 2023-11-04 18:19:55.207904 git_changelog-2.4.1/tests/test_version.py
--rw-r--r--   0        0        0     5988 1970-01-01 00:00:00.000000 git_changelog-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-31 19:47:09.968170 git_changelog-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3702 2024-03-31 19:47:09.968170 git_changelog-2.5.0/README.md
+-rw-r--r--   0        0        0     1830 2024-04-01 22:31:20.311422 git_changelog-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      278 2024-03-31 19:47:09.968170 git_changelog-2.5.0/src/git_changelog/__init__.py
+-rw-r--r--   0        0        0      387 2024-03-31 19:47:09.968170 git_changelog-2.5.0/src/git_changelog/__main__.py
+-rw-r--r--   0        0        0    20209 2024-04-01 11:49:17.580819 git_changelog-2.5.0/src/git_changelog/build.py
+-rw-r--r--   0        0        0    27496 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/cli.py
+-rw-r--r--   0        0        0    14008 2024-04-01 11:45:41.037014 git_changelog-2.5.0/src/git_changelog/commit.py
+-rw-r--r--   0        0        0     2840 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/debug.py
+-rw-r--r--   0        0        0    13417 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/providers.py
+-rw-r--r--   0        0        0        0 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/py.typed
+-rw-r--r--   0        0        0     1122 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/templates/__init__.py
+-rw-r--r--   0        0        0     1588 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/templates/angular.md.jinja
+-rw-r--r--   0        0        0     2213 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/templates/keepachangelog.md.jinja
+-rw-r--r--   0        0        0    27786 2024-03-31 19:47:09.971503 git_changelog-2.5.0/src/git_changelog/versioning.py
+-rw-r--r--   0        0        0      166 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      850 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     3243 2024-03-31 19:52:40.640087 git_changelog-2.5.0/tests/helpers.py
+-rw-r--r--   0        0        0     2361 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_angular_style.py
+-rw-r--r--   0        0        0     2308 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_basic_style.py
+-rw-r--r--   0        0        0     8744 2024-04-01 11:46:08.991345 git_changelog-2.5.0/tests/test_build.py
+-rw-r--r--   0        0        0     8550 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1079 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_commit.py
+-rw-r--r--   0        0        0     5483 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_conventional_commit_style.py
+-rw-r--r--   0        0        0     6546 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_end_to_end.py
+-rw-r--r--   0        0        0     1505 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_providers.py
+-rw-r--r--   0        0        0      897 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_release_notes.py
+-rw-r--r--   0        0        0    11631 2024-03-31 19:47:09.971503 git_changelog-2.5.0/tests/test_versioning.py
+-rw-r--r--   0        0        0     5334 1970-01-01 00:00:00.000000 git_changelog-2.5.0/PKG-INFO
```

### Comparing `git_changelog-2.4.1/LICENSE` & `git_changelog-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/README.md` & `git_changelog-2.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,45 +15,41 @@
   Built-in [Keep a Changelog][keep-a-changelog] and [Angular][angular] templates
   (also see [Conventional Changelog][conventional-changelog]).
 - Commit styles/conventions parsing.
   Built-in [Angular][angular-convention], [Conventional Commit][conventional-commit] and basic conventions.
 - Git service/provider agnostic,
   plus references parsing (issues, commits, etc.).
   Built-in [GitHub][github-refs], [Gitlab][gitlab-refs] and [Bitbucket][bitbucket-refs] support.
-- Understands [Semantic Versioning][semantic-versioning]:
-  major/minor/patch for versions and commits.
+- Understands [SemVer][semver] and [PEP 440][pep-440] versioning schemes.
   Guesses next version based on last commits.
 - Parses [Git trailers][git-trailers], allowing to reference
   issues, PRs, etc., in your commit messages
   in a clean, provider-agnostic way.
+- Template context injection,
+  to furthermore customize how your changelog will be rendered.
 
 - Todo:
     - [Plugin architecture][issue-19],
       to support more commit conventions and git services.
-    - [Template context injection][issue-17],
-      to furthermore customize how your changelog will be rendered.
     - [Easy access to "Breaking Changes"][issue-14] in the templates.
-    - [Commits/dates/versions range limitation ability][issue-16].
 
 [jinja2]:                 http://jinja.pocoo.org/
 [keep-a-changelog]:       http://keepachangelog.com/en/1.0.0/
 [angular]:                https://github.com/angular/angular/blob/master/CHANGELOG.md
 [conventional-changelog]: https://github.com/conventional-changelog/conventional-changelog
-[semantic-versioning]:    http://semver.org/spec/v2.0.0.html
+[semver]:                 http://semver.org/spec/v2.0.0.html
 [angular-convention]:     https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
 [conventional-commit]:    https://www.conventionalcommits.org/en/v1.0.0/
 [github-refs]:            https://help.github.com/articles/autolinked-references-and-urls/
 [gitlab-refs]:            https://docs.gitlab.com/ce/user/markdown.html#special-gitlab-references
 [bitbucket-refs]:         https://support.atlassian.com/bitbucket-cloud/docs/markup-comments
 [git-trailers]:           https://git-scm.com/docs/git-interpret-trailers
+[pep-440]:                https://peps.python.org/pep-0440/
 
 [issue-14]: https://github.com/pawamoy/git-changelog/issues/14
-[issue-15]: https://github.com/pawamoy/git-changelog/issues/15
-[issue-16]: https://github.com/pawamoy/git-changelog/issues/16
-[issue-17]: https://github.com/pawamoy/git-changelog/issues/17
 [issue-19]: https://github.com/pawamoy/git-changelog/issues/19
 
 ## Installation
 
 With `pip`:
 
 ```bash
@@ -65,24 +61,14 @@
 ```bash
 python3.8 -m pip install --user pipx
 pipx install git-changelog
 ```
 
 ## Usage
 
-```
-git-changelog [--config-file [PATH ...]] [-b] [-B VERSION] [-h] [-i]
-              [-g VERSION_REGEX] [-m MARKER_LINE] [-o OUTPUT]
-              [-p {github,gitlab,bitbucket}] [-r] [-R] [-I INPUT]
-              [-c {angular,conventional,basic}] [-s SECTIONS]
-              [-t {angular,keepachangelog}] [-T] [-E] [-Z] [-F FILTER_COMMITS]
-              [-V] [--debug-info]
-              [REPOSITORY]
-```
-
 Simply run `git-changelog` in your repository to output a changelog on standard output.
 To show the different options and their descriptions, use `git-changelog -h`.
 
 - See [Quick usage](http://pawamoy.github.io/git-changelog/usage/#quick-usage)
   for some command line examples.
 - See [Configuration](https://pawamoy.github.io/git-changelog/usage/#configuration-files)
   to learn how to configure *git-changelog* for your project.
```

### Comparing `git_changelog-2.4.1/pyproject.toml` & `git_changelog-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ]
 dependencies = [
     "appdirs>=1.4",
     "Jinja2>=2.10",
     "semver>=2.13",
     "tomli>=2.0; python_version < '3.11'",
 ]
-version = "2.4.1"
+version = "2.5.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/git-changelog"
 Documentation = "https://pawamoy.github.io/git-changelog"
```

### Comparing `git_changelog-2.4.1/src/git_changelog/build.py` & `git_changelog-2.5.0/src/git_changelog/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,68 +6,69 @@
 import os
 import sys
 import warnings
 from subprocess import CalledProcessError, check_output
 from typing import TYPE_CHECKING, ClassVar, Literal, Type, Union
 from urllib.parse import urlsplit, urlunsplit
 
-from semver import Version as SemverVersion
-from semver import VersionInfo
-
 from git_changelog.commit import (
     AngularConvention,
     BasicConvention,
     Commit,
     CommitConvention,
     ConventionalCommitConvention,
 )
 from git_changelog.providers import Bitbucket, GitHub, GitLab, ProviderRefParser
+from git_changelog.versioning import ParsedVersion, bump_pep440, bump_semver, parse_pep440, parse_semver
 
 if TYPE_CHECKING:
     from pathlib import Path
 
+    from git_changelog.versioning import SemVerVersion
+
 ConventionType = Union[str, CommitConvention, Type[CommitConvention]]
 
 
+# TODO: Remove at some point.
 def bump(version: str, part: Literal["major", "minor", "patch"] = "patch", *, zerover: bool = True) -> str:
-    """Bump a version.
+    """Bump a version. Deprecated, use [`bump_semver`][git_changelog.versioning.bump_semver] instead.
 
     Arguments:
         version: The version to bump.
         part: The part of the version to bump (major, minor, or patch).
         zerover: Keep major version at zero, even for breaking changes.
 
     Returns:
         The bumped version.
     """
-    semver_version, prefix = parse_version(version)
-    if part == "major" and (semver_version.major != 0 or not zerover):
-        semver_version = semver_version.bump_major()
-    elif part == "minor" or (part == "major" and semver_version.major == 0):
-        semver_version = semver_version.bump_minor()
-    elif part == "patch" and not semver_version.prerelease:
-        semver_version = semver_version.bump_patch()
-    return prefix + str(semver_version)
+    warnings.warn(
+        "This function is deprecated in favor of `git_changelog.versioning.bump_semver`",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return bump_semver(version, part, zerover=zerover)
 
 
-def parse_version(version: str) -> tuple[SemverVersion, str]:
-    """Parse a version.
+# TODO: Remove at some point.
+def parse_version(version: str) -> tuple[SemVerVersion, str]:
+    """Parse a version. Deprecated, use [`bump_semver`][git_changelog.versioning.parse_semver] instead.
 
     Arguments:
         version: The version to parse.
 
     Returns:
         semver_version: The semantic version.
         prefix: The version prefix.
     """
-    prefix = ""
-    if version[0] == "v":
-        prefix = "v"
-        version = version[1:]
-    return VersionInfo.parse(version), prefix
+    warnings.warn(
+        "This function is deprecated in favor of `git_changelog.versioning.parse_semver`",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    return parse_semver(version)
 
 
 class Section:
     """A list of commits grouped by section_type."""
 
     def __init__(self, section_type: str = "", commits: list[Commit] | None = None):
         """Initialization method.
@@ -153,15 +154,15 @@
     def add_commit(self, commit: Commit) -> None:
         """Register the given commit and add it to the relevant section based on its message convention.
 
         Arguments:
             commit: The git commit.
         """
         self.commits.append(commit)
-        commit.version = self.tag
+        commit.version = self.tag or "HEAD"
         if commit_type := commit.convention.get("type"):
             if commit_type not in self.sections_dict:
                 section = Section(section_type=commit_type)
                 self.sections_list.append(section)
                 self.sections_dict[commit_type] = section
             self.sections_dict[commit_type].commits.append(commit)
 
@@ -198,14 +199,15 @@
         parse_provider_refs: bool = False,
         parse_trailers: bool = False,
         sections: list[str] | None = None,
         bump_latest: bool = False,
         bump: str | None = None,
         zerover: bool = True,
         filter_commits: str | None = None,
+        versioning: Literal["semver", "pep440"] = "semver",
     ):
         """Initialization method.
 
         Arguments:
             repository: The repository (directory) for which to build the changelog.
             provider: The provider to use (github.com, gitlab.com, etc.).
             convention: The commit convention to use (angular, etc.).
@@ -260,25 +262,30 @@
 
         # set sections
         sections = (
             [self.convention.TYPES[section] for section in sections] if sections else self.convention.DEFAULT_RENDER
         )
         self.sections = sections
 
+        # get version parser based on selected versioning scheme
+        self.version_parser, self.version_bumper = {
+            "semver": (parse_semver, bump_semver),
+            "pep440": (parse_pep440, bump_pep440),
+        }[versioning]
+
         # get git log and parse it into list of commits
         self.raw_log: str = self.get_log()
         self.commits: list[Commit] = self.parse_commits()
         self.tag_commits: list[Commit] = [commit for commit in self.commits[1:] if commit.tag]
         self.tag_commits.insert(0, self.commits[0])
 
         # apply dates to commits and group them by version
         v_list, v_dict = self._group_commits_by_version()
         self.versions_list = v_list
         self.versions_dict = v_dict
-        self._assign_previous_versions()
 
         # TODO: remove at some point
         if bump_latest:
             warnings.warn(
                 "`bump_latest=True` is deprecated in favor of `bump='auto'`",
                 DeprecationWarning,
                 stacklevel=1,
@@ -305,15 +312,15 @@
     def get_remote_url(self) -> str:
         """Get the git remote URL for the repository.
 
         Returns:
             The origin remote URL.
         """
         remote = "remote." + os.environ.get("GIT_CHANGELOG_REMOTE", "origin") + ".url"
-        git_url = self.run_git("config", "--get", remote).rstrip("\n")
+        git_url = self.run_git("config", "--default", "", "--get", remote).rstrip("\n")
         if git_url.startswith("git@"):
             git_url = git_url.replace(":", "/", 1).replace("git@", "https://", 1)
         if git_url.endswith(".git"):
             git_url = git_url[:-4]
 
         # Remove credentials from the URL.
         if git_url.startswith(("http://", "https://")):
@@ -375,14 +382,15 @@
                 committer_date=lines[pos + 6],
                 refs=lines[pos + 7],
                 parent_hashes=lines[pos + 8],
                 commits_map=commits_map,
                 subject=lines[pos + 9],
                 body=body,
                 parse_trailers=self.parse_trailers,
+                version_parser=self.version_parser,
             )
 
             pos += nbl_index + 1
 
             # Expand commit object with provider parsing.
             if self.provider:
                 commit.update_with_provider(self.provider, parse_refs=self.parse_provider_refs)
@@ -407,97 +415,97 @@
 
         Returns:
             versions_list: The list of versions order descending by timestamp.
             versions_dict: A dictionary of versions with the tag name as keys.
         """
         versions_dict: dict[str, Version] = {}
         versions_list: list[Version] = []
+        previous_versions: dict[str, str] = {}
 
         # Iterate in reversed order (oldest to newest tag) to assign commits to the first version they were released with.
         for tag_commit in reversed(self.tag_commits):
             # Create new version object.
             version = self._create_version(tag_commit)
             versions_dict[tag_commit.version] = version
             versions_list.insert(0, version)
 
             # Find all commits for this version by following the commit graph.
             version.add_commit(tag_commit)
+            previous_parsed_version: ParsedVersion | None = None
             next_commits = tag_commit.parent_commits  # Always new: we can mutate it.
             while next_commits:
                 next_commit = next_commits.pop(0)
-                if not next_commit.tag and not next_commit.version:
+                if next_commit.tag:
+                    parsed_version, _ = self.version_parser(next_commit.tag)
+                    if not previous_parsed_version or parsed_version > previous_parsed_version:
+                        previous_parsed_version = parsed_version
+                        previous_versions[version.tag] = next_commit.tag
+                elif not next_commit.version:
                     version.add_commit(next_commit)
                     next_commits.extend(next_commit.parent_commits)
 
+        self._assign_previous_versions(versions_dict, previous_versions)
         return versions_list, versions_dict
 
     def _create_version(self, commit: Commit) -> Version:
         date = commit.committer_date.date() if commit.version else datetime.date.today()  # noqa: DTZ011
         version = Version(tag=commit.version, date=date)
         if self.provider:
             version.url = self.provider.get_tag_url(tag=commit.version)
         return version
 
-    def _assign_previous_versions(self) -> None:
+    def _assign_previous_versions(self, versions_dict: dict[str, Version], previous_versions: dict[str, str]) -> None:
         """Assign each version its previous version and create the compare URL.
 
         The previous version is defined as the version with the highest semantic version,
         that is found by following the commit graph.
 
         If no previous version is found, either because it is the first commit or
         due to the commit filter excluding it, the compare URL is created with the
         first commit (oldest).
-        """
-        for version in self.versions_list:
-            next_commits = version.commits[0].parent_commits  # Always new: we can mutate it.
-            previous_semver: SemverVersion | None = None
-            previous_version = ""
-            while next_commits:
-                next_commit = next_commits.pop(0)
-                if next_commit.tag:
-                    semver, _ = parse_version(next_commit.tag)
-                    if not previous_semver or semver.compare(previous_semver) > 0:
-                        previous_semver = semver
-                        previous_version = next_commit.tag
-                else:
-                    next_commits.extend(next_commit.parent_commits)
 
-            if not previous_version:
-                previous_version = version.commits[-1].hash
-
-            version.previous_version = self.versions_dict.get(previous_version)
+        Arguments:
+            versions_dict: A dictionary of versions with the tag name as keys.
+            previous_versions: A dictonary with version and previous version.
+        """
+        for version in versions_dict.values():
+            previous_version = previous_versions.get(version.tag, version.commits[-1].hash)
+            version.previous_version = versions_dict.get(previous_version)
             if version.previous_version:
                 version.previous_version.next_version = version
             if self.provider:
                 version.compare_url = self.provider.get_compare_url(
                     base=previous_version,
                     target=version.tag or "HEAD",
                 )
 
     def _bump(self, version: str) -> None:
         last_version = self.versions_list[0]
         if not last_version.tag and last_version.previous_version:
             last_tag = last_version.previous_version.tag
+            version, *plus = version.split("+")
             if version == "auto":
                 # guess the next version number based on last version and recent commits
                 version = "patch"
                 for commit in last_version.commits:
                     if commit.convention["is_major"]:
                         version = "major"
                         break
                     if commit.convention["is_minor"]:
                         version = "minor"
-            if version in {"major", "minor", "patch"}:
-                # bump version (don't fail on non-semver versions)
-                try:
-                    last_version.planned_tag = bump(last_tag, version, zerover=self.zerover)  # type: ignore[arg-type]
-                except ValueError:
-                    return
+            version = "+".join((version, *plus))
+            if version in self.version_bumper.strategies:
+                # bump version
+                last_version.planned_tag = self.version_bumper(last_tag, version, zerover=self.zerover)
             else:
                 # user specified version
+                try:
+                    self.version_bumper(version)
+                except ValueError as error:
+                    raise ValueError(f"{error}; typo in bumping strategy? Check the CLI help and our docs") from error
                 last_version.planned_tag = version
             # update URLs
             if self.provider:
                 last_version.url = self.provider.get_tag_url(tag=last_version.planned_tag)
                 last_version.compare_url = self.provider.get_compare_url(
                     base=last_version.previous_version.tag,
                     target=last_version.planned_tag,
```

### Comparing `git_changelog-2.4.1/src/git_changelog/cli.py` & `git_changelog-2.5.0/src/git_changelog/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,49 +15,51 @@
 
 import argparse
 import re
 import sys
 import warnings
 from importlib import metadata
 from pathlib import Path
-from typing import Any, Pattern, Sequence, TextIO
+from typing import Any, Literal, Pattern, Sequence, TextIO
 
 from appdirs import user_config_dir
 from jinja2.exceptions import TemplateNotFound
 
 from git_changelog import debug, templates
 from git_changelog.build import Changelog, Version
 from git_changelog.commit import (
     AngularConvention,
     BasicConvention,
     CommitConvention,
     ConventionalCommitConvention,
 )
 from git_changelog.providers import Bitbucket, GitHub, GitLab, ProviderRefParser
+from git_changelog.versioning import bump_pep440, bump_semver
 
 # TODO: Remove once support for Python 3.10 is dropped.
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
+DEFAULT_VERSIONING = "semver"
 DEFAULT_VERSION_REGEX = r"^## \[(?P<version>v?[^\]]+)"
 DEFAULT_MARKER_LINE = "<!-- insertion marker -->"
 DEFAULT_CHANGELOG_FILE = "CHANGELOG.md"
 CONVENTIONS = ("angular", "conventional", "basic")
 DEFAULT_CONFIG_FILES = [
     "pyproject.toml",
     ".git-changelog.toml",
     "config/git-changelog.toml",
     ".config/git-changelog.toml",
     str(Path(user_config_dir()) / "git-changelog.toml"),
 ]
 """Default configuration files read by git-changelog."""
 
-DEFAULT_SETTINGS = {
+DEFAULT_SETTINGS: dict[str, Any] = {
     "bump": None,
     "bump_latest": None,
     "convention": "basic",
     "filter_commits": None,
     "in_place": False,
     "input": DEFAULT_CHANGELOG_FILE,
     "marker_line": DEFAULT_MARKER_LINE,
@@ -66,15 +68,17 @@
     "parse_refs": False,
     "parse_trailers": False,
     "provider": None,
     "release_notes": False,
     "repository": ".",
     "sections": None,
     "template": "keepachangelog",
+    "jinja_context": {},
     "version_regex": DEFAULT_VERSION_REGEX,
+    "versioning": DEFAULT_VERSIONING,
     "zerover": True,
 }
 
 
 class Templates(tuple):  # (subclassing tuple)
     """Helper to pick a template on the command line."""
 
@@ -96,14 +100,30 @@
         return "0.0.0"
 
 
 def _comma_separated_list(value: str) -> list[str]:
     return value.split(",")
 
 
+class _ParseDictAction(argparse.Action):
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,  # noqa: ARG002
+        namespace: argparse.Namespace,
+        values: str | Sequence[Any] | None,
+        option_string: str | Sequence[Any] | None = None,  # noqa: ARG002
+    ):
+        attribute = getattr(namespace, self.dest)
+        if not isinstance(attribute, dict):
+            setattr(namespace, self.dest, {})
+        if isinstance(values, str):
+            key, value = values.split("=", 1)
+            getattr(namespace, self.dest)[key] = value
+
+
 providers: dict[str, type[ProviderRefParser]] = {
     "github": GitHub,
     "gitlab": GitLab,
     "bitbucket": Bitbucket,
 }
 
 
@@ -178,20 +198,38 @@
     parser.add_argument(
         "-B",
         "--bump",
         action="store",
         dest="bump",
         metavar="VERSION",
         help="Specify the bump from latest version for the set of unreleased commits. "
-        "Can be one of `auto`, `major`, `minor`, `patch` or a valid semver version (eg. 1.2.3). "
-        "With `auto`, if a commit contains breaking changes, bump the major number (or the minor number for 0.x versions), "
-        "else if there are new features, bump the minor number, else just bump the patch number. "
+        "Can be one of `auto`, `major`, `minor`, `patch` or a valid SemVer version (eg. 1.2.3). "
+        "For both SemVer and PEP 440 versioning schemes (see -n), `auto` will bump the major number "
+        "if a commit contains breaking changes (or the minor number for 0.x versions, see -Z), "
+        "else the minor number if there are new features, else the patch number. "
         "Default: unset (false).",
     )
     parser.add_argument(
+        "-n",
+        "--versioning",
+        action="store",
+        dest="versioning",
+        metavar="SCHEME",
+        help="Versioning scheme to use when bumping and comparing versions. "
+        "The selected scheme will impact the values accepted by the `--bump` option. "
+        "Supported: `pep440`, `semver`. PEP 440 provides the following bump strategies: `auto`, "
+        f"`{'`, `'.join(part for part in bump_pep440.strategies if '+' not in part)}`. "
+        "Values `auto`, `major`, `minor`, `micro` can be suffixed with one of `+alpha`, `+beta`, `+candidate`, "
+        "and/or `+dev`. Values `alpha`, `beta` and `candidate` can be suffixed with `+dev`. "
+        "Examples: `auto+alpha`, `major+beta+dev`, `micro+dev`, `candidate+dev`, etc.. "
+        "SemVer provides the following bump strategies: `auto`, "
+        f"`{'`, `'.join(bump_semver.strategies)}`. "
+        "See the docs for more information. Default: unset (`semver`).",
+    )
+    parser.add_argument(
         "-h",
         "--help",
         action="help",
         default=argparse.SUPPRESS,
         help="Show this help message and exit.",
     )
     parser.add_argument(
@@ -330,14 +368,23 @@
         "--filter-commits",
         action="store",
         metavar="RANGE",
         dest="filter_commits",
         help="The Git revision-range filter to use (e.g. `v1.2.0..`). Default: no filter.",
     )
     parser.add_argument(
+        "-j",
+        "--jinja-context",
+        action=_ParseDictAction,
+        metavar="KEY=VALUE",
+        dest="jinja_context",
+        help="Pass additional key/value pairs to the template. Option can be used multiple times. "
+        "The key/value pairs are accessible as 'jinja_context' in the template.",
+    )
+    parser.add_argument(
         "-V",
         "--version",
         action="version",
         version=f"%(prog)s {debug.get_version()}",
         help="Show the current version of the program and exit.",
     )
     parser.add_argument("--debug-info", action=_DebugInfo, help="Print debug information.")
@@ -454,19 +501,24 @@
 
     config_file = explicit_opts_dict.pop("config_file", DEFAULT_CONFIG_FILES)
     if str(config_file).strip().lower() in ("no", "none", "off", "false", "0", ""):
         config_file = None
     elif str(config_file).strip().lower() in ("yes", "default", "on", "true", "1"):
         config_file = DEFAULT_CONFIG_FILES
 
+    jinja_context = explicit_opts_dict.pop("jinja_context", {})
+
     settings = read_config(config_file)
 
     # CLI arguments override the config file settings
     settings.update(explicit_opts_dict)
 
+    # Merge jinja context, CLI values override config file values.
+    settings["jinja_context"].update(jinja_context)
+
     # TODO: remove at some point
     if "bump_latest" in explicit_opts_dict:
         warnings.warn("`--bump-latest` is deprecated in favor of `--bump=auto`", FutureWarning, stacklevel=1)
 
     return settings
 
 
@@ -483,14 +535,16 @@
     marker_line: str = DEFAULT_MARKER_LINE,
     bump_latest: bool = False,  # noqa: FBT001,FBT002
     omit_empty_versions: bool = False,  # noqa: FBT001,FBT002
     provider: str | None = None,
     bump: str | None = None,
     zerover: bool = True,  # noqa: FBT001,FBT002
     filter_commits: str | None = None,
+    jinja_context: dict[str, Any] | None = None,
+    versioning: Literal["pep440", "semver"] = "semver",
 ) -> tuple[Changelog, str]:
     """Build a changelog and render it.
 
     This function returns the changelog instance and the rendered contents,
     but also updates the specified output file (side-effect) or writes to stdout.
 
     Parameters:
@@ -507,14 +561,16 @@
         bump_latest: Deprecated, use --bump=auto instead.
             Whether to try and bump the latest version to guess the new one.
         omit_empty_versions: Whether to omit empty versions from the output.
         provider: Provider class used by this repository.
         bump: Whether to try and bump to a given version.
         zerover: Keep major version at zero, even for breaking changes.
         filter_commits: The Git revision-range used to filter commits in git-log.
+        jinja_context: Key/value pairs passed to the Jinja template.
+        versioning: Versioning scheme to use when grouping commits and bumping versions.
 
     Raises:
         ValueError: When some arguments are incompatible or missing.
 
     Returns:
         The built changelog and the rendered contents.
     """
@@ -551,14 +607,15 @@
         convention=convention,
         parse_provider_refs=parse_refs,
         parse_trailers=parse_trailers,
         sections=sections,
         bump=bump,
         zerover=zerover,
         filter_commits=filter_commits,
+        versioning=versioning,
     )
 
     # remove empty versions from changelog data
     if omit_empty_versions:
         section_set = set(changelog.sections)
         empty_versions = [
             version for version in changelog.versions_list if section_set.isdisjoint(version.sections_dict.keys())
@@ -589,15 +646,22 @@
                 raise ValueError(f"Version {last_released} already in changelog")
             changelog.versions_list = _unreleased(
                 changelog.versions_list,
                 last_released,
             )
 
         # render new entries
-        rendered = jinja_template.render(changelog=changelog, in_place=True).rstrip("\n") + "\n"
+        rendered = (
+            jinja_template.render(
+                changelog=changelog,
+                jinja_context=jinja_context,
+                in_place=True,
+            ).rstrip("\n")
+            + "\n"
+        )
 
         # find marker line(s) in current changelog
         marker = lines.index(marker_line)
         try:
             marker2 = lines[marker + 1 :].index(marker_line)
         except ValueError:
             # apply new entries at marker line
@@ -608,15 +672,15 @@
 
         # write back updated changelog lines
         with open(output, "w") as changelog_file:  # type: ignore[arg-type]
             changelog_file.write("\n".join(lines).rstrip("\n") + "\n")
 
     # overwrite output file
     else:
-        rendered = jinja_template.render(changelog=changelog)
+        rendered = jinja_template.render(changelog=changelog, jinja_context=jinja_context)
 
         # write result in specified output
         if output is sys.stdout:
             sys.stdout.write(rendered)
         else:
             with open(output, "w") as stream:  # type: ignore[arg-type]
                 stream.write(rendered)
```

### Comparing `git_changelog-2.4.1/src/git_changelog/commit.py` & `git_changelog-2.5.0/src/git_changelog/commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,37 @@
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import suppress
 from datetime import datetime, timezone
-from typing import TYPE_CHECKING, Any, ClassVar, Pattern
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Pattern
 
 if TYPE_CHECKING:
     from git_changelog.providers import ProviderRefParser, Ref
+    from git_changelog.versioning import ParsedVersion
 
 
 def _clean_body(lines: list[str]) -> list[str]:
     while lines and not lines[0].strip():
         lines.pop(0)
     while lines and not lines[-1].strip():
         lines.pop()
     return lines
 
 
+def _is_valid_version(version: str, version_parser: Callable[[str], tuple[ParsedVersion, str]]) -> bool:
+    try:
+        version_parser(version)
+    except ValueError:
+        return False
+    return True
+
+
 class Commit:
     """A class to represent a commit."""
 
     def __init__(
         self,
         commit_hash: str,
         author_name: str = "",
@@ -37,14 +46,15 @@
         subject: str = "",
         body: list[str] | None = None,
         url: str = "",
         *,
         parse_trailers: bool = False,
         parent_hashes: str | list[str] = "",
         commits_map: dict[str, Commit] | None = None,
+        version_parser: Callable[[str], tuple[ParsedVersion, str]] | None = None,
     ):
         """Initialization method.
 
         Arguments:
             commit_hash: The commit hash.
             author_name: The author name.
             author_email: The author email.
@@ -78,16 +88,18 @@
         self.body: list[str] = _clean_body(body) if body else []
         self.url: str = url
 
         tag = ""
         for ref in refs.split(","):
             ref = ref.strip()  # noqa: PLW2901
             if ref.startswith("tag: "):
-                tag = ref.replace("tag: ", "")
-                break
+                ref = ref.replace("tag: ", "")  # noqa: PLW2901
+                if version_parser is None or _is_valid_version(ref, version_parser):
+                    tag = ref
+                    break
         self.tag: str = tag
         self.version: str = tag
 
         if isinstance(parent_hashes, str):
             parent_hashes = parent_hashes.split()
         self.parent_hashes = parent_hashes
         self._commits_map = commits_map
```

### Comparing `git_changelog-2.4.1/src/git_changelog/debug.py` & `git_changelog-2.5.0/src/git_changelog/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 class Environment:
     """Dataclass to store environment information."""
 
     interpreter_name: str
     """Python interpreter name."""
     interpreter_version: str
     """Python interpreter version."""
+    interpreter_path: str
+    """Path to Python executable."""
     platform: str
     """Operating System."""
     packages: list[Package]
     """Installed packages."""
     variables: list[Variable]
     """Environment variables."""
 
@@ -79,25 +81,26 @@
     """
     py_name, py_version = _interpreter_name_version()
     packages = ["git-changelog"]
     variables = ["PYTHONPATH", *[var for var in os.environ if var.startswith("GIT_CHANGELOG")]]
     return Environment(
         interpreter_name=py_name,
         interpreter_version=py_version,
+        interpreter_path=sys.executable,
         platform=platform.platform(),
         variables=[Variable(var, val) for var in variables if (val := os.getenv(var))],
         packages=[Package(pkg, get_version(pkg)) for pkg in packages],
     )
 
 
 def print_debug_info() -> None:
     """Print debug/environment information."""
     info = get_debug_info()
     print(f"- __System__: {info.platform}")
-    print(f"- __Python__: {info.interpreter_name} {info.interpreter_version}")
+    print(f"- __Python__: {info.interpreter_name} {info.interpreter_version} ({info.interpreter_path})")
     print("- __Environment variables__:")
     for var in info.variables:
         print(f"  - `{var.name}`: `{var.value}`")
     print("- __Installed packages__:")
     for pkg in info.packages:
         print(f"  - `{pkg.name}` v{pkg.version}")
```

### Comparing `git_changelog-2.4.1/src/git_changelog/providers.py` & `git_changelog-2.5.0/src/git_changelog/providers.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/src/git_changelog/templates/__init__.py` & `git_changelog-2.5.0/src/git_changelog/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/src/git_changelog/templates/angular.md.jinja` & `git_changelog-2.5.0/src/git_changelog/templates/angular.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/src/git_changelog/templates/keepachangelog.md.jinja` & `git_changelog-2.5.0/src/git_changelog/templates/keepachangelog.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/conftest.py` & `git_changelog-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/test_angular_style.py` & `git_changelog-2.5.0/tests/test_angular_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/test_basic_style.py` & `git_changelog-2.5.0/tests/test_basic_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/test_build.py` & `git_changelog-2.5.0/tests/test_build.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @pytest.mark.parametrize(
     ("bump", "expected"),
     [("auto", "0.1.0"), ("major", "0.1.0"), ("minor", "0.1.0"), ("1.1.1", "1.1.1")],
 )
 def test_bump_with_semver_on_new_repo(repo: GitRepo, bump: str, expected: str) -> None:
-    """Bump to user specified version (semver) on new git repo.
+    """Bump to user specified version (SemVer) on new git repo.
 
     Parameters:
         repo: GitRepo to a temporary repository.
         bump: The bump parameter value.
         expected: Expected version for the new changelog entry.
     """
     changelog = Changelog(repo.path, convention=AngularConvention, bump=bump)
@@ -193,7 +193,115 @@
     if expected_prev_tag:
         assert version.previous_version is not None, f"Expected previous version '{expected_prev_tag}', but was None"
         assert version.previous_version.tag == expected_prev_tag
     else:
         assert version.previous_version is None
     hashes = [commit.hash for commit in version.commits]
     assert hashes == expected_commits
+
+
+def test_no_remote_url(repo: GitRepo) -> None:
+    """Test parsing and grouping commits to versions without a git remote.
+
+    Parameters:
+        repo: GitRepo to a temporary repository.
+    """
+    repo.git("remote", "remove", "origin")
+    commit_a = repo.first_hash
+    repo.tag("1.0.0")
+
+    changelog = Changelog(repo.path, convention=AngularConvention)
+
+    assert len(changelog.versions_list) == 1
+    _assert_version(
+        changelog.versions_list[0],
+        expected_tag="1.0.0",
+        expected_prev_tag=None,
+        expected_commits=[commit_a],
+    )
+
+
+def test_merge_into_unreleased(repo: GitRepo) -> None:
+    r"""Test parsing and grouping commits to versions.
+
+    Commit graph:
+    main       A---C---E
+                \ / \ /
+    feat         B   D
+
+    Expected:
+    - Unreleased: E D C B A
+
+    Parameters:
+        repo: GitRepo to a temporary repository.
+    """
+    commit_a = repo.first_hash
+    repo.branch("feat/1")
+    repo.checkout("feat/1")
+    commit_b = repo.commit("feat: B")
+    repo.checkout("main")
+    commit_c = repo.merge("feat/1")
+    repo.branch("feat/2")
+    repo.checkout("feat/2")
+    commit_d = repo.commit("feat: D")
+    repo.checkout("main")
+    commit_e = repo.merge("feat/2")
+
+    changelog = Changelog(repo.path, convention=AngularConvention)
+
+    assert len(changelog.versions_list) == 1
+    version = changelog.versions_list[0]
+    _assert_version(
+        version,
+        expected_tag="0.1.0",
+        expected_prev_tag=None,
+        expected_commits=[commit_e, commit_c, commit_d, commit_a, commit_b],
+    )
+
+
+def test_build_changelog_with_pep440_versions(repo: GitRepo) -> None:
+    """Test parsing and grouping commits to PEP440 versions.
+
+    Parameters:
+        repo: GitRepo to a temporary repository.
+    """
+    repo.commit("feat: Feature")
+    repo.tag("1.0.0")
+    repo.commit("fix: Fix")
+    repo.tag("1.0.0.post0")
+    repo.commit("feat: Feat")
+    changelog = Changelog(repo.path, convention=AngularConvention, versioning="pep440")
+    assert len(changelog.versions_list) == 3
+    assert changelog.versions_list[1].tag == "1.0.0.post0"
+
+
+def test_ignore_nonsemver_tag(repo: GitRepo) -> None:
+    """Test parsing and grouping commits to versions.
+
+    Commit graph:
+                 1.0.0
+                   |
+    main       A-B-C
+                 |
+               dummy
+
+    Expected:
+    - 1.0.0: C B A
+
+    Parameters:
+        repo: GitRepo to a temporary repository.
+    """
+    commit_a = repo.first_hash
+    commit_b = repo.commit("fix: B")
+    repo.tag("dummy")
+    commit_c = repo.commit("feat: C")
+    repo.tag("1.0.0")
+
+    changelog = Changelog(repo.path, convention=AngularConvention)
+
+    assert len(changelog.versions_list) == 1
+    _assert_version(
+        changelog.versions_list[0],
+        expected_tag="1.0.0",
+        expected_prev_tag=None,
+        expected_commits=[commit_c, commit_b, commit_a],
+    )
```

### Comparing `git_changelog-2.4.1/tests/test_cli.py` & `git_changelog-2.5.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 # it will use its own config file and possibly modify
 # the CHANGELOG!
 
 from __future__ import annotations
 
 import os
 import sys
+from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Iterator
 
 import pytest
 import tomli_w
 
 from git_changelog import cli, debug
 
 if TYPE_CHECKING:
     from pathlib import Path
 
+    from tests.helpers import GitRepo
+
 
 if sys.version_info >= (3, 11):
     from contextlib import chdir
 else:
     # TODO: remove once support for Python 3.10 is dropped
     from contextlib import contextmanager
 
@@ -208,7 +211,70 @@
     with pytest.raises(SystemExit):
         cli.main(["--debug-info"])
     captured = capsys.readouterr().out.lower()
     assert "python" in captured
     assert "system" in captured
     assert "environment" in captured
     assert "packages" in captured
+
+
+# IMPORTANT: See top module comment.
+def test_jinja_context(repo: GitRepo) -> None:
+    """Render template with custom template variables.
+
+    Parameters:
+        repo: Temporary Git repository (fixture).
+    """
+    repo.path.joinpath("conf.toml").write_text(
+        dedent(
+            """
+            [jinja_context]
+            k1 = "ignored"
+            k2 = "v2"
+            k3 = "v3"
+            """,
+        ),
+    )
+
+    template = repo.path.joinpath(".custom_template.md.jinja")
+    template.write_text("{% for key, val in jinja_context.items() %}{{ key }} = {{ val }}\n{% endfor %}")
+
+    exit_code = cli.main(
+        [
+            "--config-file",
+            str(repo.path / "conf.toml"),
+            "-o",
+            str(repo.path / "CHANGELOG.md"),
+            "-t",
+            f"path:{template}",
+            "--jinja-context",
+            "k1=v1",
+            "-j",
+            "k3=v3",
+            str(repo.path),
+        ],
+    )
+
+    assert exit_code == 0
+
+    contents = repo.path.joinpath("CHANGELOG.md").read_text()
+    assert contents == "k1 = v1\nk2 = v2\nk3 = v3\n"
+
+
+# IMPORTANT: See top module comment.
+def test_versioning(repo: GitRepo) -> None:
+    """Use a specific versioning scheme.
+
+    Parameters:
+        repo: Temporary Git repository (fixture).
+    """
+    repo.commit("feat: Feature")
+    repo.tag("1.0.0")
+    repo.commit("fix: Fix")
+    with repo.enter():
+        assert cli.main(["-cconventional", "-nsemver", "-Bauto"]) == 0
+        assert cli.main(["-cconventional", "-npep440", "-Bauto"]) == 0
+        assert cli.main(["-cconventional", "-nsemver", "-B1.1.0"]) == 0
+        assert cli.main(["-cconventional", "-npep440", "-B1.1.0"]) == 0
+        assert cli.main(["-cconventional", "-nsemver", "-Bunknown"]) == 1
+        assert cli.main(["-cconventional", "-npep440", "-Bunknown"]) == 1
+        assert cli.main(["-cconventional", "-npep440", "-Balpha"]) == 1
```

### Comparing `git_changelog-2.4.1/tests/test_commit.py` & `git_changelog-2.5.0/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/test_conventional_commit_style.py` & `git_changelog-2.5.0/tests/test_conventional_commit_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/test_end_to_end.py` & `git_changelog-2.5.0/tests/test_end_to_end.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import re
 from typing import TYPE_CHECKING
 from urllib.parse import urlsplit, urlunsplit
 
 import pytest
 
 from git_changelog import Changelog
-from git_changelog.build import bump
 from git_changelog.cli import build_and_render
 from git_changelog.commit import AngularConvention
 from git_changelog.templates import get_template
+from git_changelog.versioning import bump_semver
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from tests.helpers import GitRepo
 
 VERSIONS = ("0.1.0", "0.2.0", "0.2.1", "1.0.0", "1.1.0", "")
@@ -30,15 +30,15 @@
 
     Parameters:
         repo: Temporary Git repository (fixture).
     """
     changelog = Changelog(repo.path, convention=AngularConvention, bump="auto")
     # features, no breaking changes: minor bumped
     assert changelog.versions_list[0].planned_tag is not None
-    assert changelog.versions_list[0].planned_tag.lstrip("v") == bump(
+    assert changelog.versions_list[0].planned_tag.lstrip("v") == bump_semver(
         VERSIONS[-2],
         "minor",
     )
     rendered = KEEP_A_CHANGELOG.render(changelog=changelog)
     assert "Unreleased" not in rendered
```

### Comparing `git_changelog-2.4.1/tests/test_providers.py` & `git_changelog-2.5.0/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/tests/test_release_notes.py` & `git_changelog-2.5.0/tests/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.4.1/PKG-INFO` & `git_changelog-2.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-changelog
-Version: 2.4.1
+Version: 2.5.0
 Summary: Automatic Changelog generator using Jinja2 templates.
 Keywords: git changelog changelog-generator commit-style commit-convention
 Author-Email: Timothée Mazzucotelli <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -51,45 +51,41 @@
   Built-in [Keep a Changelog][keep-a-changelog] and [Angular][angular] templates
   (also see [Conventional Changelog][conventional-changelog]).
 - Commit styles/conventions parsing.
   Built-in [Angular][angular-convention], [Conventional Commit][conventional-commit] and basic conventions.
 - Git service/provider agnostic,
   plus references parsing (issues, commits, etc.).
   Built-in [GitHub][github-refs], [Gitlab][gitlab-refs] and [Bitbucket][bitbucket-refs] support.
-- Understands [Semantic Versioning][semantic-versioning]:
-  major/minor/patch for versions and commits.
+- Understands [SemVer][semver] and [PEP 440][pep-440] versioning schemes.
   Guesses next version based on last commits.
 - Parses [Git trailers][git-trailers], allowing to reference
   issues, PRs, etc., in your commit messages
   in a clean, provider-agnostic way.
+- Template context injection,
+  to furthermore customize how your changelog will be rendered.
 
 - Todo:
     - [Plugin architecture][issue-19],
       to support more commit conventions and git services.
-    - [Template context injection][issue-17],
-      to furthermore customize how your changelog will be rendered.
     - [Easy access to "Breaking Changes"][issue-14] in the templates.
-    - [Commits/dates/versions range limitation ability][issue-16].
 
 [jinja2]:                 http://jinja.pocoo.org/
 [keep-a-changelog]:       http://keepachangelog.com/en/1.0.0/
 [angular]:                https://github.com/angular/angular/blob/master/CHANGELOG.md
 [conventional-changelog]: https://github.com/conventional-changelog/conventional-changelog
-[semantic-versioning]:    http://semver.org/spec/v2.0.0.html
+[semver]:                 http://semver.org/spec/v2.0.0.html
 [angular-convention]:     https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
 [conventional-commit]:    https://www.conventionalcommits.org/en/v1.0.0/
 [github-refs]:            https://help.github.com/articles/autolinked-references-and-urls/
 [gitlab-refs]:            https://docs.gitlab.com/ce/user/markdown.html#special-gitlab-references
 [bitbucket-refs]:         https://support.atlassian.com/bitbucket-cloud/docs/markup-comments
 [git-trailers]:           https://git-scm.com/docs/git-interpret-trailers
+[pep-440]:                https://peps.python.org/pep-0440/
 
 [issue-14]: https://github.com/pawamoy/git-changelog/issues/14
-[issue-15]: https://github.com/pawamoy/git-changelog/issues/15
-[issue-16]: https://github.com/pawamoy/git-changelog/issues/16
-[issue-17]: https://github.com/pawamoy/git-changelog/issues/17
 [issue-19]: https://github.com/pawamoy/git-changelog/issues/19
 
 ## Installation
 
 With `pip`:
 
 ```bash
@@ -101,24 +97,14 @@
 ```bash
 python3.8 -m pip install --user pipx
 pipx install git-changelog
 ```
 
 ## Usage
 
-```
-git-changelog [--config-file [PATH ...]] [-b] [-B VERSION] [-h] [-i]
-              [-g VERSION_REGEX] [-m MARKER_LINE] [-o OUTPUT]
-              [-p {github,gitlab,bitbucket}] [-r] [-R] [-I INPUT]
-              [-c {angular,conventional,basic}] [-s SECTIONS]
-              [-t {angular,keepachangelog}] [-T] [-E] [-Z] [-F FILTER_COMMITS]
-              [-V] [--debug-info]
-              [REPOSITORY]
-```
-
 Simply run `git-changelog` in your repository to output a changelog on standard output.
 To show the different options and their descriptions, use `git-changelog -h`.
 
 - See [Quick usage](http://pawamoy.github.io/git-changelog/usage/#quick-usage)
   for some command line examples.
 - See [Configuration](https://pawamoy.github.io/git-changelog/usage/#configuration-files)
   to learn how to configure *git-changelog* for your project.
```

